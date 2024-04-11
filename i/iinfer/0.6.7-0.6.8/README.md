# Comparing `tmp/iinfer-0.6.7.tar.gz` & `tmp/iinfer-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.6.7.tar", last modified: Sun Mar 31 14:39:33 2024, max compression
+gzip compressed data, was "iinfer-0.6.8.tar", last modified: Thu Apr 11 14:35:47 2024, max compression
```

## Comparing `iinfer-0.6.7.tar` & `iinfer-0.6.8.tar`

### file list

```diff
@@ -1,175 +1,181 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.926842 iinfer-0.6.7/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.6.7/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-03-31 14:39:33.925842 iinfer-0.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.6.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.263843 iinfer-0.6.7/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.358843 iinfer-0.6.7/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.6.7/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    40575 2024-03-30 02:52:07.000000 iinfer-0.6.7/iinfer/app/app.py
--rw-rw-rw-   0        0        0    26784 2024-03-31 14:29:35.000000 iinfer-0.6.7/iinfer/app/client.py
--rw-rw-rw-   0        0        0    11057 2024-03-20 10:59:26.000000 iinfer-0.6.7/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.372844 iinfer-0.6.7/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.6.7/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.6.7/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0    45788 2024-03-31 14:25:45.000000 iinfer-0.6.7/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     4967 2024-02-25 04:42:39.000000 iinfer-0.6.7/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.395843 iinfer-0.6.7/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2953 2024-02-26 12:49:27.000000 iinfer-0.6.7/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     4295 2024-02-28 14:16:12.000000 iinfer-0.6.7/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     5911 2024-03-17 13:06:29.000000 iinfer-0.6.7/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     3463 2024-02-26 12:49:54.000000 iinfer-0.6.7/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     5521 2024-03-23 13:47:09.000000 iinfer-0.6.7/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.6.7/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.6.7/iinfer/app/install.py
--rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.6.7/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.423845 iinfer-0.6.7/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     4184 2024-03-17 02:48:02.000000 iinfer-0.6.7/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.6.7/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.6.7/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     6463 2024-03-16 15:20:39.000000 iinfer-0.6.7/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     8325 2024-03-17 11:26:01.000000 iinfer-0.6.7/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     4635 2024-02-26 12:51:56.000000 iinfer-0.6.7/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.6.7/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.467844 iinfer-0.6.7/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.6.7/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.6.7/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.6.7/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.6.7/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.6.7/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.6.7/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5476 2024-03-30 02:49:51.000000 iinfer-0.6.7/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.6.7/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.6.7/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.6.7/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    40369 2024-03-31 14:26:00.000000 iinfer-0.6.7/iinfer/app/server.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.475841 iinfer-0.6.7/iinfer/datasets/
--rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/datasets/label_coco.txt
--rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/datasets/label_voc.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.489843 iinfer-0.6.7/iinfer/docker/
--rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.6.7/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.192840 iinfer-0.6.7/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.526842 iinfer-0.6.7/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0        2 2024-02-24 14:47:49.000000 iinfer-0.6.7/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      107 2024-02-25 04:46:38.000000 iinfer-0.6.7/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      239 2024-02-25 08:52:44.000000 iinfer-0.6.7/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.6.7/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0       80 2024-03-23 03:50:35.000000 iinfer-0.6.7/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.6.7/iinfer/extensions/injection/before_gray_injection.json
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.745845 iinfer-0.6.7/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.6.7/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0     1010 2024-03-31 14:39:24.000000 iinfer-0.6.7/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.747841 iinfer-0.6.7/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.201842 iinfer-0.6.7/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.774841 iinfer-0.6.7/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.779842 iinfer-0.6.7/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.789842 iinfer-0.6.7/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.809845 iinfer-0.6.7/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.832841 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.200849 iinfer-0.6.7/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.838843 iinfer-0.6.7/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.887842 iinfer-0.6.7/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.900847 iinfer-0.6.7/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.204844 iinfer-0.6.7/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.907842 iinfer-0.6.7/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.920843 iinfer-0.6.7/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.923843 iinfer-0.6.7/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.6.7/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    72109 2024-03-31 14:12:02.000000 iinfer-0.6.7/iinfer/web/main.html
-drwxrwxrwx   0        0        0        0 2024-03-31 14:39:33.289842 iinfer-0.6.7/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6577 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-31 14:39:33.000000 iinfer-0.6.7/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 14:39:33.927844 iinfer-0.6.7/setup.cfg
--rw-rw-rw-   0        0        0     2169 2024-03-10 09:36:19.000000 iinfer-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.974518 iinfer-0.6.8/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.6.8/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-04-11 14:35:47.973520 iinfer-0.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.6.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.440513 iinfer-0.6.8/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.618517 iinfer-0.6.8/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.6.8/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    42217 2024-04-11 12:15:10.000000 iinfer-0.6.8/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    26784 2024-03-31 14:29:35.000000 iinfer-0.6.8/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    12275 2024-04-07 04:28:16.000000 iinfer-0.6.8/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.625515 iinfer-0.6.8/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.6.8/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.6.8/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0    48856 2024-04-11 14:07:45.000000 iinfer-0.6.8/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.6.8/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.649519 iinfer-0.6.8/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.6.8/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.6.8/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.6.8/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.6.8/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.6.8/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.6.8/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.6.8/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.6.8/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.6.8/iinfer/app/install.py
+-rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.6.8/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.675518 iinfer-0.6.8/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.6.8/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.6.8/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.6.8/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.6.8/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.6.8/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.712516 iinfer-0.6.8/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.6.8/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.6.8/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    40369 2024-03-31 14:26:00.000000 iinfer-0.6.8/iinfer/app/server.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.719521 iinfer-0.6.8/iinfer/datasets/
+-rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/datasets/label_coco.txt
+-rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/datasets/label_voc.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.727518 iinfer-0.6.8/iinfer/docker/
+-rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.6.8/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.393645 iinfer-0.6.8/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.751519 iinfer-0.6.8/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.8/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.6.8/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.6.8/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.8/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.6.8/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.6.8/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.6.8/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.6.8/iinfer/extensions/injection/before_gray_injection.json
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.872519 iinfer-0.6.8/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0     1010 2024-04-11 14:17:29.000000 iinfer-0.6.8/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.875520 iinfer-0.6.8/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.404514 iinfer-0.6.8/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.888521 iinfer-0.6.8/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.891521 iinfer-0.6.8/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.893518 iinfer-0.6.8/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.914519 iinfer-0.6.8/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.930519 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.403514 iinfer-0.6.8/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.939518 iinfer-0.6.8/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.953522 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.956519 iinfer-0.6.8/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.405512 iinfer-0.6.8/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.958519 iinfer-0.6.8/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.969523 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.972520 iinfer-0.6.8/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    72259 2024-04-11 12:58:28.000000 iinfer-0.6.8/iinfer/web/main.html
+drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.558516 iinfer-0.6.8/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6875 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:35:47.975520 iinfer-0.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.6.8/setup.py
```

### Comparing `iinfer-0.6.7/LICENSE` & `iinfer-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/PKG-INFO` & `iinfer-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.7
+Version: 0.6.8
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.7/README.md` & `iinfer-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/app.py` & `iinfer-0.6.8/iinfer/app/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from iinfer import version
 from iinfer.app import common, client, gui, install, postprocess, redis, server
-from iinfer.app.postprocesses import csv, det_clip, det_face_store, det_filter, det_jadge, cls_jadge, httpreq
+from iinfer.app.postprocesses import cls_jadge, csv, det_clip, det_face_store, det_filter, det_jadge, httpreq, seg_bbox, seg_filter
 from pathlib import Path
 import argparse
 import argcomplete
 import cv2
 import os
 import sys
 import time
@@ -32,15 +32,15 @@
     parser.add_argument('--timeout', help='Setting the cmd timeout.', type=int, default=60)
     parser.add_argument('-c', '--cmd', help='Setting the cmd type.',
                         choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', # install mode
                                  'docker_run', 'docker_stop', # redis mode
                                  'start', 'stop', # server or client or gui mode
                                  'list' , # server mode
                                  'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
-                                 'det_filter', 'det_jadge', 'det_clip', 'det_face_store', 'cls_jadge', 'csv', 'httpreq', # postprocess mode
+                                 'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
                                 ])
     parser.add_argument('-T','--use_track', help='Setting the multi object tracking enable for Object Detection.', action='store_true')
     parser.add_argument('--model_img_width', help='Setting the cmd deploy model_img_width.', type=int)
     parser.add_argument('--model_img_height', help='Setting the cmd deploy model_img_height.', type=int)
     parser.add_argument('--model_file', help='Setting the cmd deploy model_file file.')
     parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file.', action='append')
     parser.add_argument('--predict_type', help='Setting the cmd deploy predict_type. If Custom, custom_predict_py must be specified.',
@@ -100,14 +100,20 @@
     parser.add_argument('--ng_classes', help='Setting the postprocess ng_classes.', type=int, action='append')
     parser.add_argument('--ng_labels', help='Setting the postprocess ng_labels.', type=str, action='append')
     parser.add_argument('--ext_score_th', help='Setting the postprocess ext_score_th.', type=float, default=None)
     parser.add_argument('--ext_classes', help='Setting the postprocess ext_classes.', type=int, action='append')
     parser.add_argument('--ext_labels', help='Setting the postprocess ext_labels.', type=str, action='append')
     parser.add_argument('--face_threshold', help='Setting the postprocess face_threshold.', type=float, default=0.0)
 
+    parser.add_argument('--del_segments', help='Setting the postprocess del_segments.', action='store_true')
+    parser.add_argument('--nodraw_bbox', help='Setting the postprocess nodraw_bbox.', action='store_true')
+    parser.add_argument('--nodraw_rbbox', help='Setting the postprocess nodraw_rbbox.', action='store_true')
+    parser.add_argument('--logits_th', help='Setting the postprocess logits_th.', type=float, default=0.0)
+    parser.add_argument('--del_logits', help='Setting the postprocess del_logits.', action='store_true')
+
     parser.add_argument('--install_iinfer', help='Setting the install server install_iinfer.', type=str, default='iinfer')
     parser.add_argument('--install_onnx', help='Setting the install server install_onnx.', action='store_true')
     parser.add_argument('--install_mmdet', help='Setting the install server install_mmdet.', action='store_true')
     parser.add_argument('--install_mmseg', help='Setting the install server install_mmseg.', action='store_true')
     parser.add_argument('--install_mmcls', help='Setting the install server install_mmcls.', action='store_true')
     parser.add_argument('--install_mmpretrain', help='Setting the install server install_mmpretrain.', action='store_true')
     parser.add_argument('--install_insightface', help='Setting the install server install_insightface.', action='store_true')
@@ -192,14 +198,20 @@
     ng_classes = common.getopt(opt, 'ng_classes', preval=args_dict, withset=True)
     ng_labels = common.getopt(opt, 'ng_labels', preval=args_dict, withset=True)
     ext_score_th = common.getopt(opt, 'ext_score_th', preval=args_dict, withset=True)
     ext_classes = common.getopt(opt, 'ext_classes', preval=args_dict, withset=True)
     ext_labels = common.getopt(opt, 'ext_labels', preval=args_dict, withset=True)
     face_threshold = common.getopt(opt, 'face_threshold', preval=args_dict, withset=True)
 
+    del_segments = common.getopt(opt, 'del_segments', preval=args_dict, withset=True)
+    nodraw_bbox = common.getopt(opt, 'nodraw_bbox', preval=args_dict, withset=True)
+    nodraw_rbbox = common.getopt(opt, 'nodraw_rbbox', preval=args_dict, withset=True)
+    logits_th = common.getopt(opt, 'logits_th', preval=args_dict, withset=True)
+    del_logits = common.getopt(opt, 'del_logits', preval=args_dict, withset=True)
+
     install_iinfer = common.getopt(opt, 'install_iinfer', preval=args_dict, withset=True)
     install_onnx = common.getopt(opt, 'install_onnx', preval=args_dict, withset=True)
     install_mmdet = common.getopt(opt, 'install_mmdet', preval=args_dict, withset=True)
     install_mmseg = common.getopt(opt, 'install_mmseg', preval=args_dict, withset=True)
     install_mmcls = common.getopt(opt, 'install_mmcls', preval=args_dict, withset=True)
     install_mmpretrain = common.getopt(opt, 'install_mmpretrain', preval=args_dict, withset=True)
     install_insightface = common.getopt(opt, 'install_insightface', preval=args_dict, withset=True)
@@ -419,108 +431,123 @@
                 return ret
             finally:
                 try:
                     cv2.destroyWindow('preview')
                 except:
                     pass
 
-        if cmd == 'det_filter':
-            proc = det_filter.DetFilter(logger, score_th=score_th, width_th=width_th, height_th=height_th, classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
+        def _exec_proc(input_file, stdin, proc:postprocess.Postprocess, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, output_json, output_json_append, output_csv=None):
             if input_file is not None:
                 with open(input_file, 'r', encoding="UTF-8") as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
             elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append, output_csv=output_csv)
             else:
                 msg = {"warn":f"Image file or stdin is empty."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
+            return 0, ret
 
-        elif cmd == 'det_jadge':
+        if cmd == 'cls_jadge':
             try:
-                proc = det_jadge.DetJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
+                proc = cls_jadge.ClaJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
                                         ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
                                         ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
                                         nodraw=nodraw, output_preview=output_preview)
             except Exception as e:
-                msg = {"warn":f"Invalid options. {e}"}
-                common.print_format(msg, format, tm, output_json, output_json_append)
-                return 1, msg
-            if input_file is not None:
-                with open(input_file, 'r', encoding="UTF-8") as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
 
-        elif cmd == 'cls_jadge':
-            proc = cls_jadge.ClaJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
-                                      ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
-                                      ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
-                                      nodraw=nodraw, output_preview=output_preview)
-            if input_file is not None:
-                with open(input_file, 'r', encoding="UTF-8") as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
+        elif cmd == 'csv':
+            try:
+                proc = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+            if code != 0:
+                return code, ret
 
         elif cmd == 'det_clip':
-            proc = det_clip.DetClip(logger, image_type=image_type, clip_margin=clip_margin)
-            if input_file is not None:
-                with open(input_file, 'r') as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, None, False)
+            try:
+                proc = det_clip.DetClip(logger, image_type=image_type, clip_margin=clip_margin)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
+            if code != 0:
+                return code, ret
 
         elif cmd == 'det_face_store':
-            proc = det_face_store.DetFaceStore(logger, face_threshold=face_threshold, image_type=image_type, clip_margin=clip_margin)
-            if input_file is not None:
-                with open(input_file, 'r') as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, None, False)
+            try:
+                proc = det_face_store.DetFaceStore(logger, face_threshold=face_threshold, image_type=image_type, clip_margin=clip_margin)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
 
-        elif cmd == 'csv':
-            proc = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
-            if input_file is not None:
-                with open(input_file, 'r') as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, None, timeout, False, tm, None, False, output_csv=output_csv)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, None, False)
+        elif cmd == 'det_filter':
+            try:
+                proc = det_filter.DetFilter(logger, score_th=score_th, width_th=width_th, height_th=height_th, classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
+
+        elif cmd == 'det_jadge':
+            try:
+                proc = det_jadge.DetJadge(logger, ok_score_th=ok_score_th, ok_classes=ok_classes, ok_labels=ok_labels,
+                                        ng_score_th=ng_score_th, ng_classes=ng_classes, ng_labels=ng_labels,
+                                        ext_score_th=ext_score_th, ext_classes=ext_classes, ext_labels=ext_labels,
+                                        nodraw=nodraw, output_preview=output_preview)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
 
         elif cmd == 'httpreq':
-            proc = httpreq.Httpreq(logger, fileup_name=fileup_name)
-            if input_file is not None:
-                with open(input_file, 'r') as f:
-                    ret = _to_proc(f.readlines(), proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
-            elif stdin:
-                ret = _to_proc(sys.stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
-            else:
-                msg = {"warn":f"Image file or stdin is empty."}
-                common.print_format(msg, format, tm, output_json, output_json_append)
+            try:
+                proc = httpreq.Httpreq(logger, fileup_name=fileup_name)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, text_connectstr, timeout, format, tm, None, False)
+            if code != 0:
+                return code, ret
+
+        elif cmd == 'seg_bbox':
+            try:
+                proc = seg_bbox.SegBBox(logger, del_segments=del_segments, nodraw=nodraw, nodraw_bbox=nodraw_bbox, nodraw_rbbox=nodraw_rbbox,
+                                        output_preview=output_preview)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
+                return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
+
+        elif cmd == 'seg_filter':
+            try:
+                proc = seg_filter.SegFilter(logger, logits_th=logits_th, classes=classes, labels=labels, nodraw=nodraw, del_logits=del_logits)
+            except Exception as e:
+                common.print_format({"warn":f"Invalid options. {e}"}, format, tm, output_json, output_json_append)
                 return 1, msg
+            code, ret = _exec_proc(input_file, stdin, proc, json_connectstr, img_connectstr, None, timeout, format, tm, output_json, output_json_append)
+            if code != 0:
+                return code, ret
+
         else:
             msg = {"warn":f"Unkown command."}
             common.print_format(msg, format, tm, output_json, output_json_append)
             return 1, msg
 
     elif mode == 'redis':
         logger, _ = common.load_config(mode)
```

### Comparing `iinfer-0.6.7/iinfer/app/client.py` & `iinfer-0.6.8/iinfer/app/client.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/common.py` & `iinfer-0.6.8/iinfer/app/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from pathlib import Path
 from PIL import Image, ImageDraw
 from pkg_resources import resource_string
 from tabulate import tabulate
 from typing import List, Tuple, Dict, Any
-import json
-import os
+import cv2
 import logging
 import logging.config
+import json
 import numpy as np
+import os
 import platform
 import random
 import shutil
 import string
 import requests
 import subprocess
 import time
@@ -250,14 +251,42 @@
                 logger.debug(f"output:{output}")
                 break
             except UnicodeDecodeError:
                 pass
 
     return proc.returncode, output
 
+def draw_segment(img_npy:np.ndarray, segment:np.ndarray, colors:List[Tuple[int]], nodraw:bool=False) -> np.ndarray:
+    """
+    画像にマスクを描画します。
+
+    Args:
+        img_npy (np.ndarray): 元画像
+        segment (np.ndarray): セグメンテーションのクラスマップ
+        colors (List[Tuple[int]]): クラスごとの色のリスト
+        nodraw (bool, optional): 描画しない場合はTrue. Defaults to False.
+
+    Returns:
+        Image: マスクが描画された画像
+    """
+    img_npy = cv2.cvtColor(img_npy, cv2.COLOR_RGB2BGR)
+    masked_image = np.zeros_like(img_npy)
+
+    for c in np.unique(segment):
+        color = colors[int(c)] if colors is not None else make_color(str(int(c)))
+        m = segment == c
+        r = np.where(m, color[0], 0).astype(np.uint8)
+        g = np.where(m, color[1], 0).astype(np.uint8)
+        b = np.where(m, color[2], 0).astype(np.uint8)
+        mask = cv2.merge([r, g, b])
+        masked_image = cv2.addWeighted(masked_image, 1, mask[0], 1, 0)
+    img_npy = cv2.addWeighted(img_npy, 0.5, masked_image, 0.5, 0)
+    img_npy = cv2.cvtColor(img_npy, cv2.COLOR_BGR2RGB)
+    return img_npy
+
 def draw_boxes(image:Image.Image, boxes:List[List[float]], scores:List[float], classes:List[int], ids:List[str]=None, labels:List[str]=None, colors:List[Tuple[int]]=None,
                nodraw:bool=False, nolookup:bool=False) -> Tuple[Image.Image, List[str]]:
     """
     画像にバウンディングボックスを描画します。
 
     Args:
         image (Image.Image): 描画する画像
@@ -281,18 +310,18 @@
         y1, x1, y2, x2 = box
         x1 = max(0, np.floor(x1 + 0.5).astype(int))
         y1 = max(0, np.floor(y1 + 0.5).astype(int))
         x2 = min(image.width, np.floor(x2 + 0.5).astype(int))
         y2 = min(image.height, np.floor(y2 + 0.5).astype(int))
         if not nolookup:
             color = colors[int(cl)] if colors is not None and len(colors) > cl else make_color(str(int(cl)))
-            label = labels[int(cl)] if labels is not None else str(id) if id is not None else None
+            label = str(labels[int(cl)]) if labels is not None else str(id) if id is not None else None
         else:
             color = colors[i] if colors is not None and len(colors) > i else make_color(str(int(cl)))
-            label = labels[i] if labels is not None and len(labels) > i else None
+            label = str(labels[i]) if labels is not None and len(labels) > i else None
         if not nodraw:
             if x2 - x1 > 0 and y2 - y1 > 0:
                 draw.rectangle(((x1, y1), (x2, y2)), outline=color)
                 if label is not None:
                     draw.rectangle(((x1, y1), (x2, y1+10)), outline=color, fill=color)
                     draw.text((x1, y1), label, tuple([int(255-c) for c in color]))
         output_labels.append(label)
```

### Comparing `iinfer-0.6.7/iinfer/app/commons/convert.py` & `iinfer-0.6.8/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/commons/module.py` & `iinfer-0.6.8/iinfer/app/commons/module.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/gui.py` & `iinfer-0.6.8/iinfer/app/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         @eel.expose
         def get_cmd_opt(mode):
             if mode == "client":
                 return ['', 'deploy', 'start', 'stop', 'predict', 'deploy_list', 'undeploy', 'predict_type_list', 'capture']
             elif mode == "server":
                 return ['', 'start', 'stop', 'list']
             elif mode == "postprocess":
-                return ['', 'det_filter', 'det_jadge', 'det_clip', 'det_face_store', 'cls_jadge', 'csv', 'httpreq']
+                return ['', 'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter']
             elif mode == "redis":
                 return ['', 'docker_run', 'docker_stop']
             elif mode == "install":
                 return ['', 'redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain']
             else:
                 return ['Please select mode.']
 
@@ -195,30 +195,15 @@
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                         dict(opt="stdout_log", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False])
                     ]
                 return []
             elif mode == "postprocess":
-                if cmd == "det_filter":
-                    return [
-                        dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
-                        dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="score_th", type="float", default="0.0", required=False, multi=False, hide=False, choise=None),
-                        dict(opt="width_th", type="int", default="0", required=False, multi=False, hide=False, choise=None),
-                        dict(opt="height_th", type="int", default="0", required=False, multi=False, hide=False, choise=None),
-                        dict(opt="classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
-                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
-                    ]
-                elif cmd == "det_jadge":
+                if cmd == "cls_jadge":
                     return [
                         dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="ok_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
                         dict(opt="ok_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
                         dict(opt="ok_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                         dict(opt="ng_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
@@ -229,31 +214,21 @@
                         dict(opt="ext_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
                         dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
-                elif cmd == "cls_jadge":
+                elif cmd == "csv":
                     return [
                         dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="ok_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
-                        dict(opt="ok_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="ok_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="ng_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
-                        dict(opt="ng_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="ng_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="ext_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
-                        dict(opt="ext_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="ext_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
-                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="out_headers", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="noheader", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_csv", type="file", default="", required=False, multi=False, hide=True, choise=None),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
                 elif cmd == "det_clip":
                     return [
                         dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="image_type", type="str", default="capture", required=False, multi=False, hide=False, choise=['bmp', 'png', 'jpeg', 'capture']),
@@ -268,32 +243,84 @@
                         dict(opt="image_type", type="str", default="capture", required=False, multi=False, hide=False, choise=['bmp', 'png', 'jpeg', 'capture']),
                         dict(opt="face_threshold", type="float", default=0.0, required=False, multi=False, hide=False, choise=None),
                         dict(opt="clip_margin", type="int", default=0, required=False, multi=False, hide=False, choise=None),
                         dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
-                elif cmd == "csv":
+                elif cmd == "det_filter":
                     return [
                         dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="out_headers", type="str", default="", required=False, multi=True, hide=False, choise=None),
-                        dict(opt="noheader", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
-                        dict(opt="output_csv", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="score_th", type="float", default="0.0", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="width_th", type="int", default="0", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="height_th", type="int", default="0", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "det_jadge":
+                    return [
+                        dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="ok_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
+                        dict(opt="ok_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="ok_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="ng_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
+                        dict(opt="ng_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="ng_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="ext_score_th", type="float", default=None, required=False, multi=False, hide=False, choise=None),
+                        dict(opt="ext_classes", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="ext_labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
                 elif cmd == "httpreq":
                     return [
                         dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="json_connectstr", type="str", default="", required=True, multi=False, hide=False, choise=None),
                         dict(opt="img_connectstr", type="str", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="fileup_name", type="str", default="file", required=True, multi=False, hide=False, choise=None),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
+                elif cmd == "seg_bbox":
+                    return [
+                        dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="del_segments", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="nodraw_bbox", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="nodraw_rbbox", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "seg_filter":
+                    return [
+                        dict(opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="stdin", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="logits_th", type="float", default="-100.0", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="classes", type="int", default="", required=False, multi=True, hide=True, choise=None),
+                        dict(opt="labels", type="str", default="", required=False, multi=True, hide=False, choise=None),
+                        dict(opt="nodraw", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="del_logits", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
                 return []
             elif mode == "redis":
                 if cmd == "docker_run":
                     return [
                         dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
                         dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
                         dict(opt="wsl_name", type="str", default="", required=False, multi=False, hide=True, choise=None),
```

### Comparing `iinfer-0.6.7/iinfer/app/injection.py` & `iinfer-0.6.8/iinfer/app/injection.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,25 @@
         設定を取得します。
         Args:
             key (str): キー
             default (Any): デフォルト値
         Returns:
             Any: 設定値
         """
-        return self.config.get(key, default)
+        ret = self.config.get(key, default)
+        return ret if ret is not None else default
+
+    def _set_config(self, key:str, val:Any=None) -> Any:
+        """
+        設定を設定します。
+        Args:
+            key (str): キー
+            val (Any): 値
+        """
+        self.config[key] = val
 
 class BeforeInjection(Injection):
     """
     サーバーサイドで実行する前処理を実装するためのクラスです。
     """
 
     def action(self, reskey:str, name:str, image:Image.Image, session:Dict[str, Any]) -> Image.Image:
```

### Comparing `iinfer-0.6.7/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.6.8/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,13 @@
-from iinfer.app import injection
-from iinfer.app.postprocesses import csv
+from iinfer.app.injections import after_det_jadge_injection
 from PIL import Image
 from typing import Tuple, Dict, Any
-import logging
 
 
-class AfterCSVInjection(injection.AfterInjection):
-    """
-    このクラスは推論実行後の後処理のインジェクションクラスです。
-    """
-    def __init__(self, config:Dict[str,Any], logger:logging.Logger):
-        """
-        このクラスのインスタンスを初期化します。
-        継承時は、このコンストラクタを呼び出すようにしてください。
-            super().__init__(logger)
-        Args:
-            config (Dict[str,Any]): 設定
-            logger (logging.Logger): ロガー
-        """
-        super().__init__(config, logger)
-        out_headers = self.get_config("out_headers", default=None)
-        noheader = self.get_config("noheader", default=True)
-        self.csv = csv.Csv(logger, out_headers=out_headers, noheader=noheader)
-        self.csv_session = self.csv.create_session(None, None, None)
+class AfterClsJadgeInjection(after_det_jadge_injection.AfterDetJadgeInjection):
 
     def action(self, reskey:str, name:str, outputs:Dict[str, Any], output_image:Image.Image, session:Dict[str, Any]) -> Tuple[Dict[str, Any], Image.Image]:
         """
         このメソッドは推論を実行した後の処理を実行します。
         Args:
             reskey (str): レスポンスキー
             name (str): モデル名
@@ -44,10 +25,8 @@
                 ・predict_obj: app.predict.Predict インスタンス
                 ・labels: クラスラベルのリスト
                 ・colors: ボックスの色のリスト
                 ・tracker: use_trackがTrueの場合、トラッカーのインスタンス
         Returns:
             Tuple[Dict[str, Any], Image.Image]: 後処理後の推論結果と画像データのタプル
         """
-        csv_str = self.csv.post_json(self.csv_session, outputs, output_image)
-        self.add_success(outputs, csv_str)
-        return outputs, output_image
+        return super().action(reskey, name, outputs, output_image, session)
```

### Comparing `iinfer-0.6.7/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.6.8/iinfer/app/injections/after_det_filter_injection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from iinfer.app import injection
+from iinfer.app import common, injection
 from PIL import Image
 from typing import Tuple, Dict, Any
 
 
 class AfterDetFilterInjection(injection.AfterInjection):
 
     def action(self, reskey:str, name:str, outputs:Dict[str, Any], output_image:Image.Image, session:Dict[str, Any]) -> Tuple[Dict[str, Any], Image.Image]:
@@ -25,27 +25,63 @@
                 ・predict_obj: app.predict.Predict インスタンス
                 ・labels: クラスラベルのリスト
                 ・colors: ボックスの色のリスト
                 ・tracker: use_trackがTrueの場合、トラッカーのインスタンス
         Returns:
             Tuple[Dict[str, Any], Image.Image]: 後処理後の推論結果と画像データのタプル
         """
+        nodraw = self.get_config('nodraw', False)
+
+        try:
+            outputs = self.post_json(outputs)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
+            return outputs, output_image
+
+        try:
+            if not nodraw:
+                output_image = self.post_img(outputs, output_image)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
+            return outputs, output_image
+
+        self.add_success(outputs, "filterd")
+
+        return outputs, output_image
+
+    def post_json(self, outputs:Dict[str, Any]) -> Dict[str, Any]:
+        """
+        outputsに対して後処理を行う関数です。
+        outputsは、以下のような構造を持つDict[str, Any]です。
+        {
+            'success': {
+                'output_ids': List[int],
+                'output_scores': List[float],
+                'output_classes': List[int],
+                'output_labels': List[str],
+                'output_boxes': List[List[int]],
+                'output_tracks': List[int]
+            }
+        }
+        Args:
+            outputs (Dict[str, Any]): 推論結果。
+        Returns:
+            Dict[str, Any]: 後処理後の推論結果
+        """
         score_th = self.get_config('score_th', 0.0)
         width_th = self.get_config('width_th', 0)
         height_th = self.get_config('height_th', 0)
         classes = self.get_config('classes', [])
         labels = self.get_config('labels', [])
 
         if 'success' not in outputs or type(outputs['success']) != dict:
-            self.add_warning(outputs, 'Invalid outputs. outputs[\'success\'] must be dict.')
-            return outputs, output_image
+            raise Exception('Invalid outputs. outputs[\'success\'] must be dict.')
         data = outputs['success']
         if 'output_scores' not in data or 'output_classes' not in data:
-            self.add_warning(outputs, 'Invalid outputs. outputs[\'success\'][\'output_scores\'] and outputs[\'success\'][\'output_classes\'] must be set.')
-            return outputs, output_image
+            raise Exception('Invalid outputs. outputs[\'success\'][\'output_scores\'] and outputs[\'success\'][\'output_classes\'] must be set.')
         output_boxes = []
         output_scores = []
         output_classes = []
         output_labels = []
         output_tracks = []
         for i, score in enumerate(data['output_scores']):
             if score < score_th:
@@ -71,10 +107,30 @@
         data['output_scores'] = output_scores
         data['output_classes'] = output_classes
         if 'output_labels' in data:
             data['output_labels'] = output_labels
         if 'output_tracks' in data:
             data['output_tracks'] = output_tracks
 
-        self.add_success(outputs, "filterd")
+        return outputs
 
-        return outputs, output_image
+    def post_img(self, outputs:Dict[str, Any], output_image:Image.Image) -> Image.Image:
+        """
+        output_imageに対して後処理を行う関数です。
+        Args:
+            outputs (Dict[str, Any]): 後処理結果
+            output_image (Image.Image): 推論後の画像データ
+        Returns:
+            Image.Image: 後処理後の画像データ
+        """
+        if 'success' not in outputs or type(outputs['success']) != dict:
+            raise Exception(outputs, 'Invalid outputs. outputs[\'success\'] must be dict.')
+
+        nodraw = self.get_config('nodraw', False)
+
+        data = outputs['success']
+        output_labels = data["output_labels"] if "output_labels" in data else None
+        output_tracks = data["output_tracks"] if "output_tracks" in data else None
+        image, output_labels = common.draw_boxes(output_image, data["output_boxes"], data["output_scores"], data["output_classes"],
+                                                 ids=output_labels, labels=output_tracks, nodraw=nodraw, nolookup=True)
+
+        return image
```

### Comparing `iinfer-0.6.7/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.6.8/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,42 +25,81 @@
                 ・predict_obj: app.predict.Predict インスタンス
                 ・labels: クラスラベルのリスト
                 ・colors: ボックスの色のリスト
                 ・tracker: use_trackがTrueの場合、トラッカーのインスタンス
         Returns:
             Tuple[Dict[str, Any], Image.Image]: 後処理後の推論結果と画像データのタプル
         """
+        nodraw = self.get_config('nodraw', False)
+
+        try:
+            outputs = self.post_json(outputs)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
+            return outputs, output_image
+
+        try:
+            if not nodraw:
+                output_image = self.post_img(outputs, output_image)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
+            return outputs, output_image
+
+        self.add_success(outputs, outputs['success']['output_jadge'])
+
+        return outputs, output_image
+
+    def post_json(self, outputs:Dict[str, Any]) -> Dict[str, Any]:
+        """
+        outputsに対して後処理を行う関数です。
+        outputsは、以下のような構造を持つDict[str, Any]です。
+        {
+            'success': {
+                'output_ids': List[int],
+                'output_scores': List[float],
+                'output_classes': List[int],
+                'output_labels': List[str],
+                'output_boxes': List[List[int]],
+                'output_tracks': List[int]
+            }
+        }
+        Args:
+            outputs (Dict[str, Any]): 推論結果
+        Returns:
+            Dict[str, Any]: 後処理後の推論結果
+        """
         ok_score_th = self.get_config('ok_score_th', None)
         ok_classes = self.get_config('ok_classes', [])
         ok_labels = self.get_config('ok_labels', [])
         ng_score_th = self.get_config('ng_score_th', None)
         ng_classes = self.get_config('ng_classes', [])
         ng_labels = self.get_config('ng_labels', [])
         ext_score_th = self.get_config('ext_score_th', None)
         ext_classes = self.get_config('ext_classes', [])
         ext_labels = self.get_config('ext_labels', [])
-        nodraw = self.get_config('nodraw', False)
 
+        if ok_score_th is not None and ((ok_classes is None or len(ok_classes)<=0) and (ok_labels is None or len(ok_labels)<=0)):
+            raise Exception('If ok_score_th is specified, ok_classes or ok_labels must be set.')
+        if ng_score_th is not None and ((ng_classes is None or len(ng_classes)<=0) and (ng_labels is None or len(ng_labels)<=0)):
+            raise Exception('If ng_score_th is specified, ng_classes or ng_labels must be set.')
+        if ext_score_th is not None and ((ext_classes is None or len(ext_classes)<=0) and (ext_labels is None or len(ext_labels)<=0)):
+            raise Exception('If ext_score_th is specified, ext_classes or ext_labels must be set.')
+        """
         if ok_score_th is not None and (not(ok_classes is not None and len(ok_classes)>0) or (ok_labels is not None and len(ok_labels)>0)):
-            self.add_warning(outputs, 'If ok_score_th is specified, ok_classes or ok_labels must be set.')
-            return outputs, output_image
+            raise Exception('If ok_score_th is specified, ok_classes or ok_labels must be set.')
         if ng_score_th is not None and (not(ng_classes is not None and len(ng_classes)>0) or (ng_labels is not None and len(ng_labels)>0)):
-            self.add_warning(outputs, 'If ng_score_th is specified, ng_classes or ng_labels must be set.')
-            return outputs, output_image
+            raise Exception(outputs, 'If ng_score_th is specified, ng_classes or ng_labels must be set.')
         if ext_score_th is not None and (not(ext_classes is not None and len(ext_classes)>0) or (ext_labels is not None and len(ext_labels)>0)):
-            self.add_warning(outputs, 'If ext_score_th is specified, ext_classes or ext_labels must be set.')
-            return outputs, output_image
-
+            raise Exception(outputs, 'If ext_score_th is specified, ext_classes or ext_labels must be set.')
+        """
         if 'success' not in outputs or type(outputs['success']) != dict:
-            self.add_warning(outputs, 'Invalid outputs. outputs[\'success\'] must be dict.')
-            return outputs, output_image
+            raise Exception('Invalid outputs. outputs[\'success\'] must be dict.')
         data = outputs['success']
         if 'output_scores' not in data or 'output_classes' not in data:
-            self.add_warning(outputs, 'Invalid outputs. outputs[\'success\'][\'output_scores\'] and outputs[\'success\'][\'output_classes\'] must be set.')
-            return outputs, output_image
+            raise Exception('Invalid outputs. outputs[\'success\'][\'output_scores\'] and outputs[\'success\'][\'output_classes\'] must be set.')
 
         output_jadge_score = [0.0, 0.0, 0.0] # ok, ng, ext
         for i, cls in enumerate(data['output_classes']):
             label = data['output_labels'][i] if 'output_labels' in data else None
             if ext_classes is not None and cls in ext_classes or ext_labels is not None and label in ext_labels:
                 output_jadge_score[2] = max(output_jadge_score[2], data['output_scores'][i])
             elif ng_classes is not None and cls in ng_classes or ng_labels is not None and label in ng_labels:
@@ -78,17 +117,37 @@
             output_jadge = 'ng'
         elif ok_score_th is not None and output_jadge_score[0] >= ok_score_th:
             output_jadge = 'ok'
 
         data['output_jadge_score'] = output_jadge_score
         data['output_jadge_label'] = output_jadge_label
         data['output_jadge'] = output_jadge
-        self.add_success(outputs, output_jadge)
+
+        return outputs
+
+    def post_img(self, outputs:Dict[str, Any], output_image:Image.Image) -> Image.Image:
+        """
+        output_imageに対して後処理を行う関数です。
+        Args:
+            outputs (Dict[str, Any]): 後処理結果
+            output_image (Image.Image): 推論後の画像データ
+        Returns:    
+            Image: 後処理結果
+        """
+        if 'success' not in outputs or type(outputs['success']) != dict:
+            raise Exception('Invalid outputs. outputs[\'success\'] must be dict.')
+        data = outputs['success']
+        if 'output_jadge_score' not in data:
+            raise Exception('Invalid outputs. outputs[\'success\'][\'output_jadge_score\'] must be set.')
+        if 'output_jadge' not in data:
+            raise Exception('Invalid outputs. outputs[\'success\'][\'output_jadge\'] must be set.')
+        output_jadge_score = data['output_jadge_score']
+        output_jadge = data['output_jadge']
 
         jadge_score = output_jadge_score[output_jadge_score.index(max(output_jadge_score))]
         draw = ImageDraw.Draw(output_image)
-        if not nodraw:
-            color = common.make_color(str(jadge_score*1000))
-            draw.rectangle(((0, 0), (output_image.width, 10)), outline=color, fill=color)
-            draw.text((0, 0), f"{output_jadge}:{jadge_score}", tuple([int(255-c) for c in color]))
 
-        return outputs, output_image
+        color = common.make_color(str(jadge_score*1000))
+        draw.rectangle(((0, 0), (output_image.width, 10)), outline=color, fill=color)
+        draw.text((0, 0), f"{output_jadge}:{jadge_score}", tuple([int(255-c) for c in color]))
+
+        return output_image
```

### Comparing `iinfer-0.6.7/iinfer/app/injections/after_http_injection.py` & `iinfer-0.6.8/iinfer/app/injections/after_http_injection.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,34 +28,69 @@
                 ・predict_obj: app.predict.Predict インスタンス
                 ・labels: クラスラベルのリスト
                 ・colors: ボックスの色のリスト
                 ・tracker: use_trackがTrueの場合、トラッカーのインスタンス
         Returns:
             Tuple[Dict[str, Any], Image.Image]: 後処理後の推論結果と画像データのタプル
         """
-        outputs_url = self.get_config('outputs_url', None)
-        if outputs_url is not None:
-            resp = requests.post(outputs_url, json=outputs)
-            if resp.status_code != 200:
-                self.add_warning(outputs, f"HTTP POST request failed with status code {resp.status_code}. {outputs_url}")
+        req_session = requests.Session()
+        try:
+            url = self.get_config('outputs_url', None)
+            if url is None:
+                self.add_warning(outputs, "No outputs_url in config")
             else:
-                self.add_success(outputs, resp.text)
-        else:
-            self.add_warning(outputs, f"No outputs_url in config")
-
-        output_image_url = self.get_config('output_image_url', None)
-        if output_image_url is not None:
-            ext = self.get_config('output_image_ext', 'jpeg')
-            prefix = self.get_config('output_image_prefix', 'output_')
-            img_bytes = convert.img2byte(output_image, format=ext)
-            finename = f'{prefix}{datetime.datetime.now().strftime("%Y%m%d%H%M%S")}.{ext}'
-            finename = finename if 'output_image_name' not in outputs else outputs['output_image_name']
-            file = {'file': (finename, io.BytesIO(img_bytes))}
-            resp = requests.post(output_image_url, files=file)
-            if resp.status_code != 200:
-                self.add_warning(outputs, f"HTTP POST request failed with status code {resp.status_code}. {output_image_url}")
+                result = self.post_json(url, req_session, outputs)
+                self.add_success(outputs, result)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
+
+        try:
+            url = self.get_config('output_image_url', None)
+            if url is None:
+                self.add_warning(outputs, "No output_image_url in config")
             else:
-                self.add_success(outputs, resp.text)
-        else:
-            self.add_warning(outputs, "No output_image_url in config")
+                result = self.post_img(req_session, outputs, output_image)
+                self.add_success(outputs, result)
+        except Exception as e:
+            self.add_warning(outputs, str(e))
 
         return outputs, output_image
+
+    def post_text(self, url, req_session:requests.Session, res_str:str):
+        res = req_session.post(url, data=res_str, verify=False)
+        if res.status_code != 200:
+            raise Exception(f"HTTP POST request failed. status_code={res.status_code} res.reason={res.reason} res.text={res.text} url={url}")
+        try:
+            result = res.json()
+        except:
+            result = dict(success=res.text)
+        return result
+
+    def post_json(self, url, req_session:requests.Session, outputs:Dict[str, Any]):
+        res = req_session.post(url, json=outputs, verify=False)
+        if res.status_code != 200:
+            raise Exception(f"HTTP POST request failed. status_code={res.status_code} res.reason={res.reason} res.text={res.text} url={url}")
+        try:
+            result = res.json()
+        except:
+            result = dict(success=res.text)
+        return result
+
+    def post_img(self, url, req_session:requests.Session, outputs:Dict[str, Any], output_image:Image.Image):
+        finename = self.get_config('fileup_name', None)
+        ext = self.get_config('output_image_ext', 'jpeg')
+        if finename is None:
+            prefix = self.get_config('output_image_prefix', 'output_')
+            finename = f'{prefix}{datetime.datetime.now().strftime("%Y%m%d%H%M%S")}.{ext}'
+
+        finename = finename if 'output_image_name' not in outputs else outputs['output_image_name']
+        img_bytes = convert.img2byte(output_image, format=ext)
+        file = {'file': (finename, io.BytesIO(img_bytes))}
+
+        res = req_session.post(url, files=file, verify=False)
+        if res.status_code != 200:
+            raise Exception(f"HTTP POST request failed. status_code={res.status_code} res.reason={res.reason} res.text={res.text} url={url}")
+        try:
+            result = res.json()
+        except:
+            result = dict(success=res.text)
+        return result
```

### Comparing `iinfer-0.6.7/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.6.8/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/install.py` & `iinfer-0.6.8/iinfer/app/install.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/postprocess.py` & `iinfer-0.6.8/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.6.8/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/postprocesses/csv.py` & `iinfer-0.6.8/iinfer/app/injections/after_csv_injection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,95 @@
-from iinfer.app import postprocess
+from iinfer.app import injection
 from PIL import Image
-from typing import Dict, List, Any
+from typing import Tuple, Dict, Any
 import csv
 import io
-import logging
 
-class Csv(postprocess.Postprocess):
-    def __init__(self, logger:logging.Logger, out_headers:List[str]=None, noheader:bool=False):
-        """
-        JSONをCSVに変換する後処理クラスです。
-        
-        Args:
-            logger (logging.Logger): ロガー
-            out_headers (List[str], optional): 出力させるヘッダー. Defaults to None.
-            noheader (bool, optional): ヘッダーを出力しない. Defaults to False.
-        """
-        super().__init__(logger)
-        self.out_headers = out_headers
-        self.noheader = noheader
 
-    def create_session(self, json_connectstr:str, img_connectstr:str, text_connectstr:str):
-        """
-        後処理のセッションを作成する関数です。
-        ここで後処理準備を完了するようにしてください。
-        戻り値の後処理セッションの型は問いません。
+class AfterCSVInjection(injection.AfterInjection):
+    """
+    このクラスは推論実行後の後処理のインジェクションクラスです。
+    """
 
-        Args:
-            json_connectstr (str): 推論結果後処理のセッション確立に必要な接続文字列
-            img_connectstr (str): 可視化画像後処理のセッション確立に必要な接続文字列
-            text_connectstr (str): テキストデータ処理のセッション確立に必要な接続文字列
-
-        Returns:
-            推論結果後処理のセッション
-            可視化画像後処理のセッション
-            テキストデータ処理のセッション
+    def action(self, reskey:str, name:str, outputs:Dict[str, Any], output_image:Image.Image, session:Dict[str, Any]) -> Tuple[Dict[str, Any], Image.Image]:
         """
-        return 'json_connectstr', None, None
-
-    def post_json(self, json_session, outputs:Dict[str, Any], output_image:Image.Image):
-        """
-        outputsに対して後処理を行う関数です。
-
+        このメソッドは推論を実行した後の処理を実行します。
         Args:
-            json_session (任意): JSONセッション
-            outputs (Dict[str, Any]): 推論結果
-            output_image (Image.Image): 入力画像（RGB配列であること）
-
+            reskey (str): レスポンスキー
+            name (str): モデル名
+            outputs (Dict[str, Any]): 推論結果。次の項目が含まれます。
+                ・success or warn: 推論成功か警告のキーに対して、その内容が格納されます。
+                ・output_image: 推論後の画像データをbase64エンコードした文字列
+                ・output_image_shape: 推論後の画像データの形状（base46でコードするときに必要）
+                ・output_image_name: クライアントから指定されてきた推論後の画像データの名前
+
+            output_image (Image.Image): 推論後の画像データ
+            session (Dict[str, Any]): 推論セッション。次の項目が含まれます。
+                ・session: app.predict.Predict#create_session() で作成されたセッション
+                ・model_img_width: モデルの入力画像の幅
+                ・model_img_height: モデルの入力画像の高さ
+                ・predict_obj: app.predict.Predict インスタンス
+                ・labels: クラスラベルのリスト
+                ・colors: ボックスの色のリスト
+                ・tracker: use_trackがTrueの場合、トラッカーのインスタンス
         Returns:
-            Dict[str, Any]: 後処理結果
+            Tuple[Dict[str, Any], Image.Image]: 後処理後の推論結果と画像データのタプル
         """
-        def _to_csv(data, buffer, i):
-            if type(data) == dict:
-                data_keys = data.keys()
-                notfound = [] if self.out_headers is None else [h for h in self.out_headers if h not in data_keys]
-                if len(notfound) > 0:
-                    raise Exception(f"notfound headers: {notfound}")
-                headers = self.out_headers if self.out_headers is not None else list(data_keys)
-                row = {k:v for k, v in data.items() if k in headers}
-                w = csv.DictWriter(buffer, fieldnames=headers)
-                if not self.noheader and i<=0:
-                    w.writeheader()
-                w.writerow(row)
-            elif type(data) == list:
-                csv.writer(buffer).writerow(data)
-            else:
-                buffer.write(str(data))
-                buffer.write("\n")
-
+        out_headers = self.get_config("out_headers", default=None)
+        noheader = self.get_config("noheader", default=True)
+        result = self.write_csv(outputs, out_headers, noheader)
+        self.add_success(outputs, result)
+        return outputs, output_image
+    
+    def write_csv(self, outputs, out_headers, noheader):
         result = ''
         if 'success' in outputs and type(outputs['success']) == list:
             buffer = io.StringIO()
             for i, data in enumerate(outputs['success']):
-                _to_csv(data, buffer, i)
+                self._to_csv(data, buffer, i, out_headers, noheader)
             result = buffer.getvalue().strip()
             buffer.close()
 
         elif 'success' in outputs and type(outputs['success']) == dict:
             buffer = io.StringIO()
-            _to_csv(outputs['success'], buffer, 0)
+            self._to_csv(outputs['success'], buffer, 0, out_headers, noheader)
             result = buffer.getvalue().strip()
             buffer.close()
 
         elif type(outputs) == list:
             buffer = io.StringIO()
             for i, data in enumerate(outputs):
-                _to_csv(data, buffer, i)
+                self._to_csv(data, buffer, i, out_headers, noheader)
             result = buffer.getvalue().strip()
             buffer.close()
 
         elif type(outputs) == dict:
             buffer = io.StringIO()
-            _to_csv(outputs, buffer, 0)
+            self._to_csv(outputs, buffer, 0, out_headers, noheader)
             result = buffer.getvalue().strip()
             buffer.close()
 
         else:
             buffer = io.StringIO()
-            _to_csv(outputs, buffer, 0)
+            self._to_csv(outputs, buffer, 0, out_headers, noheader)
             result = buffer.getvalue().strip()
             buffer.close()
-
-        self.noheader = True
+        
         return result
+
+    def _to_csv(self, data, buffer, i, out_headers, noheader):
+        if type(data) == dict:
+            data_keys = data.keys()
+            notfound = [] if out_headers is None else [h for h in out_headers if h not in data_keys]
+            if len(notfound) > 0:
+                raise Exception(f"notfound headers: {notfound}")
+            headers = out_headers if out_headers is not None else list(data_keys)
+            row = {k:v for k, v in data.items() if k in headers}
+            w = csv.DictWriter(buffer, fieldnames=headers)
+            if not noheader and i<=0:
+                w.writeheader()
+            w.writerow(row)
+        elif type(data) == list:
+            csv.writer(buffer).writerow(data)
+        else:
+            buffer.write(str(data))
+            buffer.write("\n")
```

### Comparing `iinfer-0.6.7/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.6.8/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.6.8/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.6.8/iinfer/app/postprocesses/det_filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from iinfer.app import postprocess
 from iinfer.app.commons import convert
+from iinfer.app.injections import after_det_filter_injection
 from PIL import Image
-from typing import Dict, Any
+from typing import Dict, Any, List
+import cv2
 import logging
-import requests
 
-class Httpreq(postprocess.Postprocess):
-    def __init__(self, logger:logging.Logger, fileup_name:str='file'):
+class DetFilter(postprocess.Postprocess):
+    def __init__(self, logger:logging.Logger, score_th:float=0.0, width_th:int=0, height_th:int=0, classes:List[int]=None, labels:List[str]=None, nodraw:bool=False, output_preview:bool=False):
         """
-        HTTP Requestを行う後処理クラスです。
+        Object Detectionの推論結果をフィルタリングする後処理クラスです。
+        閾値に満たない推論結果を除外します。
         
         Args:
             logger (logging.Logger): ロガー
+            score_th (float): スコアの閾値
+            width_th (int): ボックスの幅の閾値
+            height_th (int): ボックスの高さの閾値
+            classes (List[int]): クラスのリスト
+            labels (List[str]): ラベルのリスト
+            nodraw (bool): 描画しない
+            output_preview (bool): プレビューを出力する
         """
         super().__init__(logger)
-        self.fileup_name = fileup_name
-        import urllib3
-        from urllib3.exceptions import InsecureRequestWarning
-        urllib3.disable_warnings(InsecureRequestWarning)
+        self.config = dict(score_th=score_th, width_th=width_th, height_th=height_th,
+                           classes=classes, labels=labels, nodraw=nodraw, output_preview=output_preview)
+        self.injection = after_det_filter_injection.AfterDetFilterInjection(self.config, self.logger)
 
     def create_session(self, json_connectstr:str, img_connectstr:str, text_connectstr:str):
         """
         後処理のセッションを作成する関数です。
         ここで後処理準備を完了するようにしてください。
         戻り値の後処理セッションの型は問いません。
 
@@ -31,81 +39,62 @@
             text_connectstr (str): テキストデータ処理のセッション確立に必要な接続文字列
 
         Returns:
             推論結果後処理のセッション
             可視化画像後処理のセッション
             テキストデータ処理のセッション
         """
-        json_session = (requests.Session(), json_connectstr)
-        img_session = (requests.Session(), img_connectstr)
-        text_session = (requests.Session(), text_connectstr)
-        return json_session, img_session, text_session
-
-    def post_text(self, text_session, res_str:str):
-        """
-        res_strに対して後処理を行う関数です。
-
-        Args:
-            text_session (任意): テキストセッション
-            res_str (text): 入力テキスト
-
-        Returns:
-            str: 後処理結果
-        """
-        if text_session is None or text_session[1] == "":
-            return res_str
-        res = text_session[0].post(text_session[1], data=res_str, verify=False)
-        if res.status_code != 200:
-            raise Exception(f"Failed to postprocess. status_code={res.status_code}. res.reason={res.reason} res.text={res.text}")
-        try:
-            outputs = res.json()
-        except:
-            outputs = dict(success=res.text)
-        return outputs
+        return 'json_connectstr', 'img_connectstr', None
 
     def post_json(self, json_session, outputs:Dict[str, Any], output_image:Image.Image):
         """
         outputsに対して後処理を行う関数です。
+        outputsは、以下のような構造を持つDict[str, Any]です。
+        {
+            'success': {
+                'output_ids': List[int],
+                'output_scores': List[float],
+                'output_classes': List[int],
+                'output_labels': List[str],
+                'output_boxes': List[List[int]],
+                'output_tracks': List[int]
+            }
+        }
 
         Args:
             json_session (任意): JSONセッション
             outputs (Dict[str, Any]): 推論結果
             output_image (Image.Image): 入力画像（RGB配列であること）
 
         Returns:
             Dict[str, Any]: 後処理結果
         """
-        if json_session is None or json_session[1] == "":
-            return outputs
-        res = json_session[0].post(json_session[1], json=outputs, verify=False)
-        if res.status_code != 200:
-            raise Exception(f"Failed to postprocess. status_code={res.status_code}. res.reason={res.reason} res.text={res.text}")
-        try:
-            outputs = res.json()
-        except:
-            outputs = dict(success=res.text)
-        return outputs
+        outputs = self.injection.post_json(outputs)
+        data = outputs['success']
+        return data
 
     def post_img(self, img_session, result:Dict[str, Any], output_image:Image.Image):
         """
         output_imageに対して後処理を行う関数です。
         引数のimageはRGBですので、戻り値の出力画像もRGBにしてください。
 
         Args:
             img_session (任意): 画像セッション
             result (Dict[str, Any]): 後処理結果
             output_image (Image.Image): 入力画像（RGB配列であること）
 
         Returns:
             Image: 後処理結果
         """
-        if img_session is None or img_session[1] == "":
-            return output_image
-        if self.fileup_name is None:
-            raise Exception(f"fileup_name is empty.")
-        files = {self.fileup_name: convert.img2byte(output_image, "JPEG")}
-        res = img_session[0].post(img_session[1], files=files, verify=False)
-        if res.status_code != 200:
-            raise Exception(f"Failed to postprocess. status_code={res.status_code}. res.reason={res.reason} res.text={res.text}")
-        output_image = convert.imgbytes2npy(res.content)
-        return output_image
+        output_image = self.injection.post_img(dict(success=result), output_image)
 
+        output_preview = self.injection.get_config('output_preview', False)
+        if output_preview:
+            # RGB画像をBGR画像に変換
+            img_npy = convert.img2npy(output_image).copy()
+            img_npy = convert.bgr2rgb(img_npy)
+            try:
+                cv2.imshow('preview', img_npy)
+                cv2.waitKey(1)
+            except KeyboardInterrupt:
+                pass
+        return output_image
```

### Comparing `iinfer-0.6.7/iinfer/app/predict.py` & `iinfer-0.6.8/iinfer/app/predict.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/insightface_det.py` & `iinfer-0.6.8/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.6.8/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from PIL import Image
 from iinfer.app import common, predict
 from iinfer.app.commons import convert
 from typing import List, Tuple
 import logging
+import numpy as np
 
 
 SITE = 'https://github.com/open-mmlab/mmsegmentation/tree/main/configs/pspnet'
 IMAGE_WIDTH = 1024
 IMAGE_HEIGHT = 512
 REQUIREd_MODEL_CONF = True
 REQUIREd_MODEL_WEIGHT = False
@@ -69,33 +70,37 @@
 
         result:SegDataSample = inference_model(model, img_npy)
         if hasattr(model, 'module'):
             model = model.module
         
         segment = result.pred_sem_seg.numpy()
         logits = result.seg_logits.numpy()
-        output_labels = model.dataset_meta['classes']
-        output_classes = [i for i in range(len(output_labels))]
+        output_catalog = model.dataset_meta['classes']
+        output_palette = model.dataset_meta['palette']
+        output_classes = np.unique(segment.data)
+        output_labels = [output_catalog[i] for i in output_classes]
         output_sem_seg = convert.npy2b64str(segment.data)
         output_sem_seg_shape = segment.data.shape
         output_sem_seg_dtype = str(segment.data.dtype)
         output_seg_logits = convert.npy2b64str(logits.data)
         output_seg_logits_shape = logits.data.shape
         output_seg_logits_dtype = str(logits.data.dtype)
 
         if not nodraw:
             img = self.draw_mask(img_npy, result,
-                                 labels if labels is not None else output_labels,
+                                 labels if labels is not None else output_catalog,
                                  colors if colors is not None else model.dataset_meta['palette'])
             output_image = convert.npy2img(img)
 
         else:
             output_image = image
 
-        return dict(output_classes=output_classes,
+        return dict(output_catalog=output_catalog,
+                    output_palette=output_palette,
+                    output_classes=output_classes,
                     output_labels=output_labels,
                     output_sem_seg=output_sem_seg,
                     output_sem_seg_shape=output_sem_seg_shape,
                     output_sem_seg_dtype=output_sem_seg_dtype,
                     output_seg_logits=output_seg_logits,
                     output_seg_logits_shape=output_seg_logits_shape,
                     output_seg_logits_dtype=output_seg_logits_dtype), output_image
```

### Comparing `iinfer-0.6.7/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.6.8/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.6.8/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/redis.py` & `iinfer-0.6.8/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/app/server.py` & `iinfer-0.6.8/iinfer/app/server.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/datasets/label_coco.txt` & `iinfer-0.6.8/iinfer/datasets/label_coco.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/docker/Dockerfile` & `iinfer-0.6.8/iinfer/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.6.8/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/licenses/files.txt` & `iinfer-0.6.8/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_client.yml` & `iinfer-0.6.8/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_gui.yml` & `iinfer-0.6.8/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_install.yml` & `iinfer-0.6.8/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_postprocess.yml` & `iinfer-0.6.8/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_redis.yml` & `iinfer-0.6.8/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/logconf_server.yml` & `iinfer-0.6.8/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/version.py` & `iinfer-0.6.8/iinfer/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 3, 31)
+dt_now = datetime.datetime(2024, 4, 11)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.6.7'
+__version__ = '0.6.8'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.6.8/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.6.8/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.6.8/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.6.8/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.6.8/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.6.8/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.6.8/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.7/iinfer/web/main.html` & `iinfer-0.6.8/iinfer/web/main.html`

 * *Files 1% similar despite different names*

```diff
@@ -706,16 +706,18 @@
                 } else {
                     $(elem).removeClass(`is-invalid`);
                     $(elem).addClass(`is-valid`);
                 }
                 if(data_multi==`true`){
                     if(!opt[data_name]) opt[data_name] = [];
                     if(data_val && data_val!=``) opt[data_name].push(data_val);
+                    else if(data_val==false) opt[data_name].push(data_val);
                 } else {
                     if(data_val && data_val!=``) opt[data_name] = data_val;
+                    else if(data_val==false) opt[data_name] = data_val;
                 }
             });
             return [title, opt];
         }
         // コマンドファイルの保存
         $(`#cmd_save`).off(`click`).on('click', async () => {
             cmd_modal = $(`#cmd_modal`);
```

### Comparing `iinfer-0.6.7/iinfer.egg-info/PKG-INFO` & `iinfer-0.6.8/iinfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.7
+Version: 0.6.8
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.7/iinfer.egg-info/SOURCES.txt` & `iinfer-0.6.8/iinfer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,31 @@
 iinfer/app/install.py
 iinfer/app/postprocess.py
 iinfer/app/predict.py
 iinfer/app/redis.py
 iinfer/app/server.py
 iinfer/app/commons/convert.py
 iinfer/app/commons/module.py
+iinfer/app/injections/after_cls_jadge_injection.py
 iinfer/app/injections/after_csv_injection.py
 iinfer/app/injections/after_det_filter_injection.py
 iinfer/app/injections/after_det_jadge_injection.py
 iinfer/app/injections/after_http_injection.py
 iinfer/app/injections/after_seg_bbox_injection.py
+iinfer/app/injections/after_seg_filter_injection.py
 iinfer/app/injections/before_grayimg_injection.py
 iinfer/app/postprocesses/cls_jadge.py
 iinfer/app/postprocesses/csv.py
 iinfer/app/postprocesses/det_clip.py
 iinfer/app/postprocesses/det_face_store.py
 iinfer/app/postprocesses/det_filter.py
 iinfer/app/postprocesses/det_jadge.py
 iinfer/app/postprocesses/httpreq.py
+iinfer/app/postprocesses/seg_bbox.py
+iinfer/app/postprocesses/seg_filter.py
 iinfer/app/predicts/__init__.py
 iinfer/app/predicts/insightface_det.py
 iinfer/app/predicts/mmdet_det_YoloX.py
 iinfer/app/predicts/mmdet_det_YoloX_Lite.py
 iinfer/app/predicts/mmpretrain_cls_swin.py
 iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
 iinfer/app/predicts/mmrotate_det_ReDet.py
@@ -59,19 +63,21 @@
 iinfer/app/predicts/onnx_det_YoloX_Lite.py
 iinfer/datasets/label_coco.txt
 iinfer/datasets/label_voc.txt
 iinfer/docker/Dockerfile
 iinfer/docker/__init__.py
 iinfer/docker/build.sh
 iinfer/docker/docker-compose.yml
+iinfer/extensions/injection/after_cls_jadge_injection.json
 iinfer/extensions/injection/after_csv_injection.json
 iinfer/extensions/injection/after_det_filter_injection.json
 iinfer/extensions/injection/after_det_jadge_injection.json
 iinfer/extensions/injection/after_http_injection.json
 iinfer/extensions/injection/after_seg_bbox_injection.json
+iinfer/extensions/injection/after_seg_filter_injection.json
 iinfer/extensions/injection/before_gray_injection.json
 iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
 iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
 iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
 iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
 iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
 iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
```

### Comparing `iinfer-0.6.7/setup.py` & `iinfer-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'motpy',
     'opencv-python',
     'Pillow',
     'pyyaml',
     'redis',
     'requests',
     'tabulate',
+    'urllib3',
     'wheel'
 ]
 PACKAGES = [
     'iinfer',
     'iinfer.app',
     'iinfer.app.commons',
     'iinfer.app.injections',
```

