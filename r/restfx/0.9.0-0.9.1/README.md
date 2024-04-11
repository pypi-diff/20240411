# Comparing `tmp/restfx-0.9.0.tar.gz` & `tmp/restfx-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\restfx-0.9.0.tar", last modified: Tue Mar  9 03:14:33 2021, max compression
+gzip compressed data, was "dist\restfx-0.9.1.tar", last modified: Wed Mar 10 08:17:13 2021, max compression
```

## Comparing `restfx-0.9.0.tar` & `restfx-0.9.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/
--rw-rw-rw-   0        0        0     1094 2020-04-13 02:28:12.000000 restfx-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     1503 2021-01-07 02:22:17.000000 restfx-0.9.0/LICENSE.WERKZEUG.rst
--rw-rw-rw-   0        0        0       68 2021-02-24 06:12:14.000000 restfx-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6350 2021-03-09 03:14:33.000000 restfx-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4142 2021-03-09 02:18:10.000000 restfx-0.9.0/README.md
--rw-rw-rw-   0        0        0     1260 2021-03-09 03:14:33.000000 restfx-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      291 2020-12-21 01:39:03.000000 restfx-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/
--rw-rw-rw-   0        0        0    10768 2021-03-09 02:37:57.000000 restfx-0.9.0/src/restfx/app.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/commands/
--rw-rw-rw-   0        0        0     2658 2021-02-24 06:11:37.000000 restfx-0.9.0/src/restfx/commands/commands.py
--rw-rw-rw-   0        0        0      648 2021-01-29 01:16:16.000000 restfx-0.9.0/src/restfx/commands/__init__.py
--rw-rw-rw-   0        0        0     2508 2021-03-09 03:09:10.000000 restfx-0.9.0/src/restfx/context.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/http/
--rw-rw-rw-   0        0        0     1041 2021-02-02 08:42:18.000000 restfx-0.9.0/src/restfx/http/request.py
--rw-rw-rw-   0        0        0     1962 2021-02-24 12:25:27.000000 restfx-0.9.0/src/restfx/http/response.py
--rw-rw-rw-   0        0        0      415 2021-02-21 09:27:03.000000 restfx-0.9.0/src/restfx/http/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/sample/
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/sample/bar/
--rw-rw-rw-   0        0        0      378 2021-02-02 09:27:00.000000 restfx-0.9.0/src/restfx/internal_assets/sample/bar/foobar.py
--rw-rw-rw-   0        0        0        0 2021-01-06 08:17:42.000000 restfx-0.9.0/src/restfx/internal_assets/sample/bar/__init__.py
--rw-rw-rw-   0        0        0     1316 2021-03-04 01:31:09.000000 restfx-0.9.0/src/restfx/internal_assets/sample/main.py
--rw-rw-rw-   0        0        0      625 2021-02-24 12:18:38.000000 restfx-0.9.0/src/restfx/internal_assets/sample/settings.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/sample/static/
--rw-rw-rw-   0        0        0      164 2021-01-06 08:14:59.000000 restfx-0.9.0/src/restfx/internal_assets/sample/static/index.html
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/
--rw-rw-rw-   0        0        0     2555 2021-01-28 08:28:58.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/index.js
--rw-rw-rw-   0        0        0     1100 2021-01-28 06:19:47.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/options.js
--rw-rw-rw-   0        0        0      774 2021-01-28 06:24:07.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/panel.js
--rw-rw-rw-   0        0        0     9650 2021-03-04 01:44:13.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/renderers.js
--rw-rw-rw-   0        0        0     8309 2021-02-23 07:48:03.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/test.js
--rw-rw-rw-   0        0        0     1591 2021-01-29 07:58:08.000000 restfx-0.9.0/src/restfx/internal_assets/scripts/xhr.js
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/styles/
--rw-rw-rw-   0        0        0    11476 2021-02-04 07:55:09.000000 restfx-0.9.0/src/restfx/internal_assets/styles/index.css
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/internal_assets/templates/
--rw-rw-rw-   0        0        0     5410 2021-02-24 06:12:02.000000 restfx-0.9.0/src/restfx/internal_assets/templates/api_list.html
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/middleware/
--rw-rw-rw-   0        0        0     2518 2021-02-01 07:13:49.000000 restfx-0.9.0/src/restfx/middleware/interface.py
--rw-rw-rw-   0        0        0     2304 2021-02-02 08:52:40.000000 restfx-0.9.0/src/restfx/middleware/manager.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/middleware/middlewares/
--rw-rw-rw-   0        0        0      822 2020-12-23 11:46:38.000000 restfx-0.9.0/src/restfx/middleware/middlewares/auth.py
--rw-rw-rw-   0        0        0     5438 2021-02-04 09:09:23.000000 restfx-0.9.0/src/restfx/middleware/middlewares/session.py
--rw-rw-rw-   0        0        0     1510 2021-01-06 05:42:36.000000 restfx-0.9.0/src/restfx/middleware/middlewares/timetick.py
--rw-rw-rw-   0        0        0       78 2020-12-29 06:36:19.000000 restfx-0.9.0/src/restfx/middleware/middlewares/__init__.py
--rw-rw-rw-   0        0        0       79 2020-12-23 12:18:31.000000 restfx-0.9.0/src/restfx/middleware/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/routes/
--rw-rw-rw-   0        0        0    10860 2021-03-09 02:19:38.000000 restfx-0.9.0/src/restfx/routes/collector.py
--rw-rw-rw-   0        0        0    13657 2021-02-02 09:10:44.000000 restfx-0.9.0/src/restfx/routes/decorator.py
--rw-rw-rw-   0        0        0     1581 2021-02-01 08:32:20.000000 restfx-0.9.0/src/restfx/routes/meta.py
--rw-rw-rw-   0        0        0     4443 2021-03-09 03:00:15.000000 restfx-0.9.0/src/restfx/routes/router.py
--rw-rw-rw-   0        0        0     5683 2021-03-08 09:30:51.000000 restfx-0.9.0/src/restfx/routes/route_resolver.py
--rw-rw-rw-   0        0        0       29 2020-11-16 02:21:02.000000 restfx-0.9.0/src/restfx/routes/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/session/
--rw-rw-rw-   0        0        0     4058 2020-12-24 01:14:35.000000 restfx-0.9.0/src/restfx/session/interfaces.py
--rw-rw-rw-   0        0        0     7421 2021-02-23 07:34:19.000000 restfx-0.9.0/src/restfx/session/providers.py
--rw-rw-rw-   0        0        0     2993 2020-11-16 01:09:01.000000 restfx-0.9.0/src/restfx/session/session.py
--rw-rw-rw-   0        0        0       34 2020-11-16 01:08:24.000000 restfx-0.9.0/src/restfx/session/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx/util/
--rw-rw-rw-   0        0        0      487 2020-11-12 07:40:46.000000 restfx-0.9.0/src/restfx/util/b64.py
--rw-rw-rw-   0        0        0     8495 2021-02-02 08:38:00.000000 restfx-0.9.0/src/restfx/util/func_util.py
--rw-rw-rw-   0        0        0      673 2021-02-21 08:56:03.000000 restfx-0.9.0/src/restfx/util/helper.py
--rw-rw-rw-   0        0        0     1754 2021-03-04 01:30:08.000000 restfx-0.9.0/src/restfx/util/logger.py
--rw-rw-rw-   0        0        0      315 2020-11-12 07:42:17.000000 restfx-0.9.0/src/restfx/util/md5.py
--rw-rw-rw-   0        0        0      317 2020-11-12 07:42:01.000000 restfx-0.9.0/src/restfx/util/sha1.py
--rw-rw-rw-   0        0        0      852 2021-03-08 09:21:09.000000 restfx-0.9.0/src/restfx/util/utils.py
--rw-rw-rw-   0        0        0        0 2020-04-22 00:57:38.000000 restfx-0.9.0/src/restfx/util/__init__.py
--rw-rw-rw-   0        0        0       59 2020-12-18 08:48:24.000000 restfx-0.9.0/src/restfx/__init__.py
--rw-rw-rw-   0        0        0       83 2021-03-09 03:13:26.000000 restfx-0.9.0/src/restfx/__meta__.py
-drwxrwxrwx   0        0        0        0 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx.egg-info/
--rw-rw-rw-   0        0        0        1 2021-03-09 03:14:32.000000 restfx-0.9.0/src/restfx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-03-09 03:14:32.000000 restfx-0.9.0/src/restfx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     6350 2021-03-09 03:14:32.000000 restfx-0.9.0/src/restfx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       16 2021-03-09 03:14:32.000000 restfx-0.9.0/src/restfx.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1901 2021-03-09 03:14:33.000000 restfx-0.9.0/src/restfx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2021-03-09 03:14:32.000000 restfx-0.9.0/src/restfx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/
+-rw-rw-rw-   0        0        0     1094 2020-04-13 02:28:12.000000 restfx-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1503 2021-01-07 02:22:17.000000 restfx-0.9.1/LICENSE.WERKZEUG.rst
+-rw-rw-rw-   0        0        0       68 2021-02-24 06:12:14.000000 restfx-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6261 2021-03-10 08:17:13.000000 restfx-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4077 2021-03-10 08:05:19.000000 restfx-0.9.1/README.md
+-rw-rw-rw-   0        0        0     1260 2021-03-10 08:17:13.000000 restfx-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      291 2020-12-21 01:39:03.000000 restfx-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/
+-rw-rw-rw-   0        0        0    10852 2021-03-10 08:10:20.000000 restfx-0.9.1/src/restfx/app.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/commands/
+-rw-rw-rw-   0        0        0     2658 2021-02-24 06:11:37.000000 restfx-0.9.1/src/restfx/commands/commands.py
+-rw-rw-rw-   0        0        0      648 2021-01-29 01:16:16.000000 restfx-0.9.1/src/restfx/commands/__init__.py
+-rw-rw-rw-   0        0        0     2493 2021-03-10 08:07:07.000000 restfx-0.9.1/src/restfx/context.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/http/
+-rw-rw-rw-   0        0        0     1041 2021-02-02 08:42:18.000000 restfx-0.9.1/src/restfx/http/request.py
+-rw-rw-rw-   0        0        0     1962 2021-02-24 12:25:27.000000 restfx-0.9.1/src/restfx/http/response.py
+-rw-rw-rw-   0        0        0      415 2021-02-21 09:27:03.000000 restfx-0.9.1/src/restfx/http/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/sample/
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/sample/bar/
+-rw-rw-rw-   0        0        0      378 2021-02-02 09:27:00.000000 restfx-0.9.1/src/restfx/internal_assets/sample/bar/foobar.py
+-rw-rw-rw-   0        0        0        0 2021-01-06 08:17:42.000000 restfx-0.9.1/src/restfx/internal_assets/sample/bar/__init__.py
+-rw-rw-rw-   0        0        0     1298 2021-03-10 08:05:19.000000 restfx-0.9.1/src/restfx/internal_assets/sample/main.py
+-rw-rw-rw-   0        0        0      625 2021-02-24 12:18:38.000000 restfx-0.9.1/src/restfx/internal_assets/sample/settings.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/sample/static/
+-rw-rw-rw-   0        0        0      164 2021-01-06 08:14:59.000000 restfx-0.9.1/src/restfx/internal_assets/sample/static/index.html
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/
+-rw-rw-rw-   0        0        0     2555 2021-01-28 08:28:58.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/index.js
+-rw-rw-rw-   0        0        0     1100 2021-01-28 06:19:47.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/options.js
+-rw-rw-rw-   0        0        0      774 2021-01-28 06:24:07.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/panel.js
+-rw-rw-rw-   0        0        0     9650 2021-03-04 01:44:13.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/renderers.js
+-rw-rw-rw-   0        0        0     8309 2021-02-23 07:48:03.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/test.js
+-rw-rw-rw-   0        0        0     1591 2021-01-29 07:58:08.000000 restfx-0.9.1/src/restfx/internal_assets/scripts/xhr.js
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/styles/
+-rw-rw-rw-   0        0        0    11476 2021-02-04 07:55:09.000000 restfx-0.9.1/src/restfx/internal_assets/styles/index.css
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/internal_assets/templates/
+-rw-rw-rw-   0        0        0     5410 2021-02-24 06:12:02.000000 restfx-0.9.1/src/restfx/internal_assets/templates/api_list.html
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/middleware/
+-rw-rw-rw-   0        0        0     2518 2021-02-01 07:13:49.000000 restfx-0.9.1/src/restfx/middleware/interface.py
+-rw-rw-rw-   0        0        0     2304 2021-02-02 08:52:40.000000 restfx-0.9.1/src/restfx/middleware/manager.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/middleware/middlewares/
+-rw-rw-rw-   0        0        0      822 2020-12-23 11:46:38.000000 restfx-0.9.1/src/restfx/middleware/middlewares/auth.py
+-rw-rw-rw-   0        0        0     5438 2021-02-04 09:09:23.000000 restfx-0.9.1/src/restfx/middleware/middlewares/session.py
+-rw-rw-rw-   0        0        0     1510 2021-01-06 05:42:36.000000 restfx-0.9.1/src/restfx/middleware/middlewares/timetick.py
+-rw-rw-rw-   0        0        0       78 2020-12-29 06:36:19.000000 restfx-0.9.1/src/restfx/middleware/middlewares/__init__.py
+-rw-rw-rw-   0        0        0       79 2020-12-23 12:18:31.000000 restfx-0.9.1/src/restfx/middleware/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/routes/
+-rw-rw-rw-   0        0        0    10860 2021-03-09 02:19:38.000000 restfx-0.9.1/src/restfx/routes/collector.py
+-rw-rw-rw-   0        0        0    13657 2021-03-10 08:06:25.000000 restfx-0.9.1/src/restfx/routes/decorator.py
+-rw-rw-rw-   0        0        0     1581 2021-02-01 08:32:20.000000 restfx-0.9.1/src/restfx/routes/meta.py
+-rw-rw-rw-   0        0        0     4443 2021-03-10 08:06:25.000000 restfx-0.9.1/src/restfx/routes/router.py
+-rw-rw-rw-   0        0        0     5683 2021-03-08 09:30:51.000000 restfx-0.9.1/src/restfx/routes/route_resolver.py
+-rw-rw-rw-   0        0        0       29 2020-11-16 02:21:02.000000 restfx-0.9.1/src/restfx/routes/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/session/
+-rw-rw-rw-   0        0        0     4058 2020-12-24 01:14:35.000000 restfx-0.9.1/src/restfx/session/interfaces.py
+-rw-rw-rw-   0        0        0     7421 2021-02-23 07:34:19.000000 restfx-0.9.1/src/restfx/session/providers.py
+-rw-rw-rw-   0        0        0     2993 2020-11-16 01:09:01.000000 restfx-0.9.1/src/restfx/session/session.py
+-rw-rw-rw-   0        0        0       34 2020-11-16 01:08:24.000000 restfx-0.9.1/src/restfx/session/__init__.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx/util/
+-rw-rw-rw-   0        0        0      487 2020-11-12 07:40:46.000000 restfx-0.9.1/src/restfx/util/b64.py
+-rw-rw-rw-   0        0        0     8495 2021-02-02 08:38:00.000000 restfx-0.9.1/src/restfx/util/func_util.py
+-rw-rw-rw-   0        0        0      673 2021-02-21 08:56:03.000000 restfx-0.9.1/src/restfx/util/helper.py
+-rw-rw-rw-   0        0        0     1749 2021-03-10 08:14:40.000000 restfx-0.9.1/src/restfx/util/logger.py
+-rw-rw-rw-   0        0        0      315 2020-11-12 07:42:17.000000 restfx-0.9.1/src/restfx/util/md5.py
+-rw-rw-rw-   0        0        0      317 2020-11-12 07:42:01.000000 restfx-0.9.1/src/restfx/util/sha1.py
+-rw-rw-rw-   0        0        0      852 2021-03-08 09:21:09.000000 restfx-0.9.1/src/restfx/util/utils.py
+-rw-rw-rw-   0        0        0        0 2020-04-22 00:57:38.000000 restfx-0.9.1/src/restfx/util/__init__.py
+-rw-rw-rw-   0        0        0       59 2020-12-18 08:48:24.000000 restfx-0.9.1/src/restfx/__init__.py
+-rw-rw-rw-   0        0        0       83 2021-03-10 08:17:10.000000 restfx-0.9.1/src/restfx/__meta__.py
+drwxrwxrwx   0        0        0        0 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     6261 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1901 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2021-03-10 08:17:13.000000 restfx-0.9.1/src/restfx.egg-info/top_level.txt
```

### Comparing `restfx-0.9.0/LICENSE` & `restfx-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/LICENSE.WERKZEUG.rst` & `restfx-0.9.1/LICENSE.WERKZEUG.rst`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/PKG-INFO` & `restfx-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: restfx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Auto RESTful framework for Python3.
 Home-page: https://gitee.com/hyjiacan/restfx
 Author: hyjiacan
 Author-email: hyjiacan@163.com
 Maintainer: hyjiacan
 Maintainer-email: hyjiacan@163.com
 License: UNKNOWN
 Project-URL: Issue tracker, https://gitee.com/hyjiacan/restfx/issues
-Project-URL: Documention, https://gitee.com/hyjiacan/restfx/wikis
 Project-URL: Code, https://gitee.com/hyjiacan/restfx
+Project-URL: Documention, https://gitee.com/hyjiacan/restfx/wikis
 Description: # restfx
         
         Python3 的 restful 多应用自动路由框架。
         
         > 底层基于 [werkzeug](https://werkzeug.palletsprojects.com/)
         
         ## 为什么要使用此框架
@@ -63,15 +63,15 @@
         ```python
         import os
         
         import restfx
         
         if __name__ == '__main__':
             root = os.path.dirname(__file__)
-            app = restfx.App('app_id', root, api_prefix='any/prefix', debug_mode=True)
+            app = restfx.App(root, api_prefix='any/prefix', debug=True)
             app.map_routes({
                 'x': 'test'
             })
             app.map_static(static_map={})
             app.startup(host='127.0.0.1', port=9127)
         ```
         
@@ -143,17 +143,14 @@
         
         [1]: https://gitee.com/hyjiacan/restfx/wikis
         [2]: https://gitee.com/hyjiacan/restfx/wikis/0B.%20%E8%B7%AF%E7%94%B1%E6%B3%A8%E5%85%A5?sort_id=3519061
         [3]: https://gitee.com/hyjiacan/restfx#%E6%88%AA%E5%9B%BE
         [11]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/__init__.py
         [12]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/demo.py
         
-        ## TODO LIST
-        
-        - [ ] 移除 `api_prefix` 参数
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `restfx-0.9.0/README.md` & `restfx-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 ```python
 import os
 
 import restfx
 
 if __name__ == '__main__':
     root = os.path.dirname(__file__)
-    app = restfx.App('app_id', root, api_prefix='any/prefix', debug_mode=True)
+    app = restfx.App(root, api_prefix='any/prefix', debug=True)
     app.map_routes({
         'x': 'test'
     })
     app.map_static(static_map={})
     app.startup(host='127.0.0.1', port=9127)
 ```
 
@@ -129,11 +129,7 @@
 
 
 [1]: https://gitee.com/hyjiacan/restfx/wikis
 [2]: https://gitee.com/hyjiacan/restfx/wikis/0B.%20%E8%B7%AF%E7%94%B1%E6%B3%A8%E5%85%A5?sort_id=3519061
 [3]: https://gitee.com/hyjiacan/restfx#%E6%88%AA%E5%9B%BE
 [11]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/__init__.py
 [12]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/demo.py
-
-## TODO LIST
-
-- [ ] 移除 `api_prefix` 参数
```

### Comparing `restfx-0.9.0/setup.cfg` & `restfx-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/app.py` & `restfx-0.9.1/src/restfx/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import uuid
 from types import FunctionType
 
 from werkzeug.exceptions import NotFound
 from werkzeug.routing import Map, Rule
 
 from .context import AppContext
 from .http import HttpServerError, HttpNotFound, HttpRequest
@@ -11,42 +12,45 @@
 
 # APP 实例集合
 _APPS = {}
 
 
 class App:
     def __init__(self,
-                 app_id: str,
                  app_root: str,
+                 app_id: str = None,
                  api_prefix='api',
-                 debug_mode=False,
+                 debug=True,
                  append_slash=False,
                  strict_mode=False,
                  api_page_enabled=None,
                  api_page_name: str = None,
                  api_page_expanded=False,
                  api_page_cache=True,
                  api_page_addition=None
                  ):
         """
 
-        :param app_id: 全局的唯一 id, 用于标识一个APP。可以通过 AppContext.get(id) 获取应用的 Context
         :param app_root: 应用的根目录
+        :param app_id: 全局的唯一 id, 用于标识一个APP。可以通过 AppContext.get(id) 获取应用的 Context，若不指定，则自动生成一个 uuid
         :param api_prefix: API接口URL前缀
-        :param debug_mode: 是否启用调试模式
+        :param debug: 是否启用调试模式
         :param append_slash: 是否在URL末尾使用 / 符号
         :param strict_mode: 是否启用严格模式。在严格模式下，不允许在请求时携带未声明的参数
         :param api_page_enabled: 只否启用接口页面
         :param api_page_name: 接口页面名称
         :param api_page_expanded: 是否展示接口列表
         :param api_page_cache: 是否缓存接口数据
         :param api_page_addition: 接口页面上要展示的接口的附加信息函数，其接收一个 dict 类型的参数 route_info
         """
-        self.id = app_id
-        self.context = AppContext(self.id, app_root, debug_mode, append_slash,
+        self.id = app_id or str(uuid.uuid4())
+
+        _APPS[self.id] = self
+
+        self.context = AppContext(self.id, app_root, debug, append_slash,
                                   strict_mode, api_page_enabled, api_page_name,
                                   api_page_expanded, api_page_cache, api_page_addition)
 
         self.api_prefix = api_prefix
         self.router = Router(self.context)
 
         self.custom_url_map = {}
@@ -80,15 +84,15 @@
             elif endpoint in self.custom_url_map:
                 response = self.custom_url_map[endpoint](request, **values)
             else:
                 response = HttpNotFound()
         except Exception as e:
             if isinstance(e, NotFound):
                 response = HttpNotFound()
-            elif self.context.DEBUG:
+            elif self.context.debug:
                 raise e
             else:
                 response = HttpServerError()
 
             msg = repr(e)
             if request:
                 msg += ':' + request.path
@@ -118,17 +122,17 @@
         :param threaded:
         :param kwargs: 适用于 werkzueg 的 run_simple 函数的其它参数
         :return:
         """
         from restfx.util import helper
         from werkzeug.serving import run_simple
 
-        debug_mode = self.context.DEBUG
+        debug = self.context.debug
 
-        if debug_mode:
+        if debug:
             helper.print_meta('dev-server *DEBUG MODE*')
         else:
             helper.print_meta('dev-server')
 
         # 检查启动参数
         argv = sys.argv
         if len(argv) > 1:
@@ -149,15 +153,15 @@
             port = int(env_port)
 
         if self.context.api_page_enabled:
             print(' * Table of APIs: http://%s:%s/%s%s' % (
                 host, port, self.api_prefix, '/' if self.context.append_slash else ''
             ))
 
-        run_simple(host, port, self, use_debugger=debug_mode, use_reloader=debug_mode, threaded=threaded, **kwargs)
+        run_simple(host, port, self, use_debugger=debug, use_reloader=debug, threaded=threaded, **kwargs)
 
     def collect(self):
         """
         收集路由
         :return:
         """
         return self.context.collector.collect(self.context.routes_map)
```

### Comparing `restfx-0.9.0/src/restfx/commands/commands.py` & `restfx-0.9.1/src/restfx/commands/commands.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/commands/__init__.py` & `restfx-0.9.1/src/restfx/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/context.py` & `restfx-0.9.1/src/restfx/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 class AppContext:
     """
     应用的上下文环境
     """
 
     def __init__(self, app_id: str,
                  app_root: str,
-                 debug_mode: bool,
+                 debug: bool,
                  append_slash: bool,
                  strict_mode: bool,
                  api_page_enabled: bool,
                  api_page_name: str,
                  api_page_expanded: bool,
                  api_page_cache: bool,
                  api_page_addition):
         """
 
         """
         _CONTEXTS[app_id] = self
         self.app_id = app_id
         # 是否启用DEBUG模式
-        self.DEBUG = debug_mode
+        self.debug = debug
         # 是否启用 API 页面
-        self.api_page_enabled = debug_mode if api_page_enabled is None else api_page_enabled
+        self.api_page_enabled = debug if api_page_enabled is None else api_page_enabled
         # 工作目录
         self.ROOT = app_root
         self.append_slash = append_slash
         self.strict_mode = strict_mode
         # 注册的中间件实例集合
         self.middlewares = []
         """
@@ -52,26 +52,26 @@
         self.static_map = {}
 
         # 注入数据/函数集合
         # 其中存放将被注入到路由函数参数列表上的数据/函数
         self.injections = {}
 
         self.api_page_options = {
-            'api_page_name': api_page_name or 'An awesome %s project' % __meta__.name,
+            'api_page_name': api_page_name or 'Another awesome %s project' % __meta__.name,
             'api_page_expanded': api_page_expanded,
             # 是否缓存API页面的 html 文件 和 接口数据
             'api_page_cache': api_page_cache,
             'api_page_addition': api_page_addition
         }
 
         if self.api_page_enabled:
             self.static_map['/internal_assets'] = os.path.join(os.path.dirname(__file__), 'internal_assets')
 
         self.collector = Collector(app_root, append_slash)
-        self.logger = Logger(debug_mode)
+        self.logger = Logger(debug)
 
     def __del__(self):
         if self.app_id in _CONTEXTS:
             del _CONTEXTS[self.app_id]
         del self.middlewares
 
     @staticmethod
```

### Comparing `restfx-0.9.0/src/restfx/http/request.py` & `restfx-0.9.1/src/restfx/http/request.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/http/response.py` & `restfx-0.9.1/src/restfx/http/response.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/sample/main.py` & `restfx-0.9.1/src/restfx/internal_assets/sample/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 import settings
 from restfx import App
 from restfx.middleware.middlewares import SessionMiddleware
 from restfx.session.providers import MemorySessionProvider
 
 # 访问 http://127.0.0.1:9127/api 查看接口页面
-app = App(settings.APP_ID,
-          settings.ROOT,
+app = App(settings.ROOT,
+          app_id=settings.APP_ID,
           api_prefix=settings.API_PREFIX,
-          debug_mode=settings.DEBUG,
+          debug=settings.DEBUG,
           strict_mode=settings.STRICT_MODE,
-          api_page_name='An awesome restfx project'
+          api_page_name='Another awesome restfx project'
           )
 
 app.map_routes(settings.ROUTES_MAP)
 app.map_static(settings.STATIC_MAP)
 
 app.register_middleware(
     SessionMiddleware(MemorySessionProvider(20)),
@@ -43,12 +43,12 @@
     return True
 
 
 if __name__ == '__main__':
     # 提供对 python main.py persist 命令的支持
     if command_persist():
         exit(0)
-    else:
-        if not settings.DEBUG:
-            load_routes_map()
-        # 启动内置服务器
-        app.startup(host=settings.HOST, port=settings.PORT)
+
+    if not settings.DEBUG:
+        load_routes_map()
+    # 启动内置服务器
+    app.startup(host=settings.HOST, port=settings.PORT)
```

### Comparing `restfx-0.9.0/src/restfx/internal_assets/sample/settings.py` & `restfx-0.9.1/src/restfx/internal_assets/sample/settings.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/index.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/options.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/options.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/panel.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/panel.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/renderers.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/renderers.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/test.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/test.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/scripts/xhr.js` & `restfx-0.9.1/src/restfx/internal_assets/scripts/xhr.js`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/styles/index.css` & `restfx-0.9.1/src/restfx/internal_assets/styles/index.css`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/internal_assets/templates/api_list.html` & `restfx-0.9.1/src/restfx/internal_assets/templates/api_list.html`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/middleware/interface.py` & `restfx-0.9.1/src/restfx/middleware/interface.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/middleware/manager.py` & `restfx-0.9.1/src/restfx/middleware/manager.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/middleware/middlewares/auth.py` & `restfx-0.9.1/src/restfx/middleware/middlewares/auth.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/middleware/middlewares/session.py` & `restfx-0.9.1/src/restfx/middleware/middlewares/session.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/middleware/middlewares/timetick.py` & `restfx-0.9.1/src/restfx/middleware/middlewares/timetick.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/routes/collector.py` & `restfx-0.9.1/src/restfx/routes/collector.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/routes/decorator.py` & `restfx-0.9.1/src/restfx/routes/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         if use_default is None:
             msg = '%s\n\tMissing required argument "%s", Parameters: (%s)' % (
                 get_func_info(func),
                 arg_name,
                 _get_parameter_str(args)
             )
             context.logger.warning(msg)
-            if not context.DEBUG:
+            if not context.debug:
                 msg = 'Missing required argument'
             return HttpBadRequest(msg)
 
         # 使用默认值
         if use_default is True:
             actual_args[arg_name] = arg_value
             used_args.append(arg_name)
@@ -302,15 +302,15 @@
                     continue
             actual_args[arg_name] = arg_spec.annotation(arg_value)
             used_args.append(arg_name)
         except Exception:
             msg = 'Argument type of "%s" mismatch, expect type "%s" but got "%s", Parameters: (%s)' \
                   % (arg_name, arg_spec.annotation.__name__, type(arg_value).__name__, _get_parameter_str(args))
             context.logger.warning(msg)
-            if not context.DEBUG:
+            if not context.debug:
                 msg = 'Argument type mismatch'
             return HttpBadRequest(msg)
 
     # 填充注入参数
     for arg_name in injection_args:
         # 注入名称不包含前缀 _
         # 所以要 [1:]
@@ -318,15 +318,15 @@
         if injection_name in request.injections:
             actual_args[arg_name] = request.injections[injection_name]
         elif injection_name in context.injections:
             actual_args[arg_name] = context.injections[injection_name]
         else:
             msg = 'Injection name "%s" not found' % injection_name
             context.logger.warning(msg)
-            return HttpServerError(msg) if context.DEBUG else HttpServerError()
+            return HttpServerError(msg) if context.debug else HttpServerError()
 
     # 填充可变参数
     variable_args = {}
     for item in arg_source:
         if item in used_args:
             continue
         variable_args[item] = arg_source[item]
@@ -356,15 +356,15 @@
         return actual_args
 
     # 启用了严格模式
     # 返回 400 响应
     msg = 'Unknown argument(s) found: "%s", Parameters: (%s)' \
           % (','.join(variable_arg_keys), _get_parameter_str(args))
     context.logger.warning(msg)
-    if not context.DEBUG:
+    if not context.debug:
         msg = 'Unknown argument(s)'
     return HttpBadRequest(msg)
 
 
 def _wrap_http_response(mgr, data):
     """
     将数据包装成 HttpResponse 返回
```

### Comparing `restfx-0.9.0/src/restfx/routes/meta.py` & `restfx-0.9.1/src/restfx/routes/meta.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/routes/router.py` & `restfx-0.9.1/src/restfx/routes/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         :param entry: 入口地址
         :return:
         """
         if self.intercepter is not None:
             # noinspection PyCallingNonCallable
             entry = self.intercepter(request, entry)
 
-        if not self.context.DEBUG:
+        if not self.context.debug:
             return self.route_for_production(request, '/' + entry)
 
         resolver = RouteResolver(self.context,
                                  self.routes_cache,
                                  self.entry_cache,
                                  request.method, entry)
```

### Comparing `restfx-0.9.0/src/restfx/routes/route_resolver.py` & `restfx-0.9.1/src/restfx/routes/route_resolver.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/session/interfaces.py` & `restfx-0.9.1/src/restfx/session/interfaces.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/session/providers.py` & `restfx-0.9.1/src/restfx/session/providers.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/session/session.py` & `restfx-0.9.1/src/restfx/session/session.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/util/func_util.py` & `restfx-0.9.1/src/restfx/util/func_util.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/util/helper.py` & `restfx-0.9.1/src/restfx/util/helper.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx/util/logger.py` & `restfx-0.9.1/src/restfx/util/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def warning(self, message):
         self.log('warning', message)
 
     def error(self, message, e=None, _raise=True):
         temp = message if e is None else '%s\n\t%s' % (message, repr(e))
 
         # 非开发模式时，始终不会输出堆栈信息
-        if not self.debug_mode:
+        if not self.debug:
             self.log('ERROR', temp, e)
             return
 
         # print('\033[1;31;47m {0} \033[0m'.format(temp))
         # if e is not None:
         #     print(repr(e.__traceback__.tb_frame))
```

### Comparing `restfx-0.9.0/src/restfx/util/utils.py` & `restfx-0.9.1/src/restfx/util/utils.py`

 * *Files identical despite different names*

### Comparing `restfx-0.9.0/src/restfx.egg-info/PKG-INFO` & `restfx-0.9.1/src/restfx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: restfx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Auto RESTful framework for Python3.
 Home-page: https://gitee.com/hyjiacan/restfx
 Author: hyjiacan
 Author-email: hyjiacan@163.com
 Maintainer: hyjiacan
 Maintainer-email: hyjiacan@163.com
 License: UNKNOWN
 Project-URL: Issue tracker, https://gitee.com/hyjiacan/restfx/issues
-Project-URL: Documention, https://gitee.com/hyjiacan/restfx/wikis
 Project-URL: Code, https://gitee.com/hyjiacan/restfx
+Project-URL: Documention, https://gitee.com/hyjiacan/restfx/wikis
 Description: # restfx
         
         Python3 的 restful 多应用自动路由框架。
         
         > 底层基于 [werkzeug](https://werkzeug.palletsprojects.com/)
         
         ## 为什么要使用此框架
@@ -63,15 +63,15 @@
         ```python
         import os
         
         import restfx
         
         if __name__ == '__main__':
             root = os.path.dirname(__file__)
-            app = restfx.App('app_id', root, api_prefix='any/prefix', debug_mode=True)
+            app = restfx.App(root, api_prefix='any/prefix', debug=True)
             app.map_routes({
                 'x': 'test'
             })
             app.map_static(static_map={})
             app.startup(host='127.0.0.1', port=9127)
         ```
         
@@ -143,17 +143,14 @@
         
         [1]: https://gitee.com/hyjiacan/restfx/wikis
         [2]: https://gitee.com/hyjiacan/restfx/wikis/0B.%20%E8%B7%AF%E7%94%B1%E6%B3%A8%E5%85%A5?sort_id=3519061
         [3]: https://gitee.com/hyjiacan/restfx#%E6%88%AA%E5%9B%BE
         [11]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/__init__.py
         [12]: https://gitee.com/hyjiacan/restfx/blob/master/test/test/api/demo.py
         
-        ## TODO LIST
-        
-        - [ ] 移除 `api_prefix` 参数
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `restfx-0.9.0/src/restfx.egg-info/SOURCES.txt` & `restfx-0.9.1/src/restfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

