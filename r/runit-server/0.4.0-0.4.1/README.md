# Comparing `tmp/runit-server-0.4.0.tar.gz` & `tmp/runit-server-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit-server-0.4.0.tar", last modified: Mon Jan  1 16:19:45 2024, max compression
+gzip compressed data, was "runit-server-0.4.1.tar", last modified: Thu Apr 11 19:13:09 2024, max compression
```

## Comparing `runit-server-0.4.0.tar` & `runit-server-0.4.1.tar`

### file list

```diff
@@ -1,169 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.194187 runit-server-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-01-01 16:19:36.000000 runit-server-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-01 16:19:36.000000 runit-server-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-01 16:19:45.194187 runit-server-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-01-01 16:19:36.000000 runit-server-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.166187 runit-server-0.4.0/runit_server/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.170188 runit-server-0.4.0/runit_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/common/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/common/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/dockerize.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/kubernetes-1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/kubernetes-2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.170188 runit-server-0.4.0/runit_server/models/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.170188 runit-server-0.4.0/runit_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/modules/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.170188 runit-server-0.4.0/runit_server/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.174188 runit-server-0.4.0/runit_server/routers/api/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/api/public.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/routers/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.162187 runit-server-0.4.0/runit_server/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.174188 runit-server-0.4.0/runit_server/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232948 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589161 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.174188 runit-server-0.4.0/runit_server/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/dark-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40957 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.178187 runit-server-0.4.0/runit_server/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/html5.svg
--rw-r--r--   0 runner    (1001) docker     (127)    46753 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/nodejs.png
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/nodejs.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/php.svg
--rw-r--r--   0 runner    (1001) docker     (127)   150090 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/python.png
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/python.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/python1.svg
--rw-r--r--   0 runner    (1001) docker     (127)   587840 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/images/terminal.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.178187 runit-server-0.4.0/runit_server/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80663 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   331886 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/databases.js
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/github.js
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/profile.js
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/projects.js
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/js/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.186188 runit-server-0.4.0/runit_server/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   133034 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   715890 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    89824 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76612 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34390 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144322 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   202902 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   897426 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   202616 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   103300 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    79444 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.186188 runit-server-0.4.0/runit_server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.186188 runit-server-0.4.0/runit_server/templates/account/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/account/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/account/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.186188 runit-server-0.4.0/runit_server/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.186188 runit-server-0.4.0/runit_server/templates/admin/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/admin/databases/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/modals/database.html
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/databases/modals/document.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/admin/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/projects/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/projects/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/projects/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/projects/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/projects/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/admin/users/
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/users/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/users/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/users/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/users/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/admin/users/modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/databases/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/databases/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/databases/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/databases/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/databases/modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/docker/bun.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/docker/node.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/docker/php.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/docker/python.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/exposed.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.190188 runit-server-0.4.0/runit_server/templates/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/functions/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.194187 runit-server-0.4.0/runit_server/templates/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/modals/confirm.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/modals/create_database.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.194187 runit-server-0.4.0/runit_server/templates/projects/
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/projects/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/projects/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/projects/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/projects/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/projects/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.194187 runit-server-0.4.0/runit_server/templates/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/setup/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/templates/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-01 16:19:36.000000 runit-server-0.4.0/runit_server/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 16:19:45.194187 runit-server-0.4.0/runit_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-01 16:19:45.000000 runit-server-0.4.0/runit_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 16:19:45.194187 runit-server-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-01-01 16:19:36.000000 runit-server-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.803169 runit-server-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-11 19:13:05.000000 runit-server-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 19:13:05.000000 runit-server-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 19:13:09.799169 runit-server-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-11 19:13:05.000000 runit-server-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.775169 runit-server-0.4.1/runit_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.775169 runit-server-0.4.1/runit_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/dockerize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/kubernetes-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/kubernetes-2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/modules/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/routers/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.771169 runit-server-0.4.1/runit_server/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232948 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589161 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/dark-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40957 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    46753 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/nodejs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/nodejs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/php.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   150090 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   587840 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/terminal.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.787169 runit-server-0.4.1/runit_server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80663 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   331886 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/databases.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/profile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/projects.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.791169 runit-server-0.4.1/runit_server/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   133034 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   715890 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    89824 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76612 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34390 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144322 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   202902 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   897426 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   202616 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   103300 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    79444 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/databases/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/modals/database.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/modals/document.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/admin/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/bun.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/node.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/php.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/python.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/exposed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/functions/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/modals/confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/modals/create_database.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/setup/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:13:09.803169 runit-server-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-11 19:13:05.000000 runit-server-0.4.1/setup.py
```

### Comparing `runit-server-0.4.0/LICENSE` & `runit-server-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/PKG-INFO` & `runit-server-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit-server-0.4.0/README.md` & `runit-server-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/Request.py` & `runit-server-0.4.1/runit_server/Request.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/app.py` & `runit-server-0.4.1/runit_server/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 from pathlib import Path
 from sys import platform
 from datetime import timedelta
 
 
-from fastapi import FastAPI, Request, status
+from fastapi import FastAPI, Request, status, Depends
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse
 from starlette.middleware import Middleware
 from starlette.middleware.sessions import SessionMiddleware
 
 from dotenv import load_dotenv
 
@@ -25,27 +25,28 @@
 from .routers import public
 from .routers import setup
 
 from .routers.api import api_router
 
 load_dotenv()
 
-app = FastAPI(lifespan=lifespan)
+app = FastAPI(dependencies=[Depends(lifespan)], force_https=True)
 app.add_middleware(
     SessionMiddleware,
     secret_key=SESSION_SECRET_KEY,
     max_age=3600,
     https_only=True
 )
 
 static = Path(__file__).resolve().parent / "static"
 uploads = Path(RUNIT_WORKDIR, 'accounts')
 app.mount('/static', StaticFiles(directory=static, html=True),  name='static')
-if not Path(RUNIT_WORKDIR).resolve().exists():
-    Path(RUNIT_WORKDIR).resolve().mkdir()
+
+if not Path(RUNIT_WORKDIR).exists():
+    Path(RUNIT_WORKDIR).mkdir()
     
 if not Path(uploads).resolve().exists():
     Path(uploads).resolve().mkdir()
     
 
 app.mount('/uploads', StaticFiles(directory=uploads, html=True),  name='uploads')
 
@@ -65,8 +66,8 @@
 
 @app.exception_handler(UnauthorizedAdminException)
 async def redirect_to_admin_login(request: Request, exception: Optional[str]):
     return RedirectResponse(request.url_for('admin_login_page'))
 
 @app.exception_handler(status.HTTP_404_NOT_FOUND)
 async def not_found_page(request: Request, exception: Optional[str]):
-    return templates.TemplateResponse('404.html', {'request': request})
+    return templates.TemplateResponse('404.html', {'request': request})
```

### Comparing `runit-server-0.4.0/runit_server/auth.py` & `runit-server-0.4.1/runit_server/auth.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/cli.py` & `runit-server-0.4.1/runit_server/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         print('[#] Complete Setup configuration first.\n')
         setup_runit(args)
         print('')
 
     RunIt.DOCKER = args.docker
     RunIt.KUBERNETES = args.kubernetes
 
-    uvicorn.run(app, host=args.host, port=args.port, log_level='info', proxy_headers=True)
+    uvicorn.run(app, host=args.host, port=args.port, log_level='info', proxy_headers=True, forwarded_allow_ips="*")
 
 def get_arguments():
     global parser
     global VERSION
     
     subparsers = parser.add_subparsers()
```

### Comparing `runit-server-0.4.0/runit_server/common/fast_api.py` & `runit-server-0.4.1/runit_server/common/fast_api.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/common/security.py` & `runit-server-0.4.1/runit_server/common/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Function for authenticating user
 
     @param email Email Address
     @param password Password
     @return User Instance or None
     '''
     user = User.get_by_email(email)
+    
     if user and Utils.check_hashed_password(password, user.password):
         return user
     return None
 
 def create_access_token(data: dict, expires_delta: Optional[timedelta] = None):
     to_encode = data.copy()
     if expires_delta:
```

### Comparing `runit-server-0.4.0/runit_server/common/utils.py` & `runit-server-0.4.1/runit_server/common/utils.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/constants.py` & `runit-server-0.4.1/runit_server/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from enum import Enum
 from typing import Literal
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = os.path.realpath(os.curdir)
@@ -19,18 +19,16 @@
 API_VERSION = 'v1'
 SUBSCRIPTION_EVENTS = Literal['all', 'create', 'update', 'delete']
 
 RUNIT_HOMEDIR = os.getenv(
     'RUNIT_HOMEDIR',
     os.path.dirname(os.path.realpath(__file__))
 )
-RUNIT_WORKDIR = os.getenv(
-    'RUNIT_WORKDIR',
-    os.path.join(os.path.expanduser('~'), 'RUNIT_WORKDIR')
-)
+
+RUNIT_WORKDIR = os.path.join(os.path.expanduser('~'), 'RUNIT_WORKDIR')
 
 GITHUB_APP_CLIENT_ID = os.getenv('GITHUB_APP_CLIENT_ID','')
 GITHUB_APP_CLIENT_SECRET = os.getenv('GITHUB_APP_CLIENT_SECRET','')
 
 PROJECTS_DIR = os.path.join(RUNIT_WORKDIR, 'projects')
 TEMPLATES_PATH = os.path.join(RUNIT_HOMEDIR, 'templates')
 DOCKER_TEMPLATES = os.path.join(TEMPLATES_PATH, 'docker')
```

### Comparing `runit-server-0.4.0/runit_server/core.py` & `runit-server-0.4.1/runit_server/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,48 +5,59 @@
 from pathlib import Path
 from contextlib import asynccontextmanager
 
 from odbms import DBMS
 from dotenv import dotenv_values, find_dotenv
 from fastapi import FastAPI, WebSocket, Request
 from fastapi.templating import Jinja2Templates
-
+from fastapi.responses import RedirectResponse
 
 from .constants import RUNIT_WORKDIR, SUBSCRIPTION_EVENTS
 
+app_initialized = False
+
 def flash(request: Request, message: str, category: str = "primary") -> None:
    if "_messages" not in request.session:
        request.session["_messages"] = []
        request.session["_messages"].append((category, message))
        
 def get_flashed_messages(request: Request):
    return request.session.pop("_messages") if "_messages" in request.session else []
 
 templates_path = Path(__file__).resolve().parent / 'templates'
 templates = Jinja2Templates(templates_path)
 templates.env.globals['get_flashed_messages'] = get_flashed_messages
 
-@asynccontextmanager
-async def lifespan(app: FastAPI):
+async def lifespan(request: Request):
+    global app_initialized
+    
     if not Path(RUNIT_WORKDIR).resolve().exists():
         Path(RUNIT_WORKDIR).resolve().mkdir()
     
     if not Path(RUNIT_WORKDIR, 'accounts').resolve().exists():
         Path(RUNIT_WORKDIR, 'account').resolve().mkdir()
         
     if not Path(RUNIT_WORKDIR, 'projects').resolve().exists():
         Path(RUNIT_WORKDIR, 'projects').resolve().mkdir()
 
     settings = dotenv_values(find_dotenv())
-
-    if 'SETUP' in settings.keys() and settings['SETUP'] == 'completed':
-        DBMS.initialize(settings['DBMS'], settings['DATABASE_HOST'], settings['DATABASE_PORT'], # type: ignore
-                    settings['DATABASE_USERNAME'], settings['DATABASE_PASSWORD'],  # type: ignore
-                    settings['DATABASE_NAME']) # type: ignore
-    yield
+    setup = os.getenv('SETUP') or settings['SETUP']
+    DB_DBMS = os.getenv('DBMS') or settings['DBMS']
+    DB_HOST = os.getenv('DATABASE_HOST') or settings['DATABASE_HOST']
+    DB_PORT = os.getenv('DATABASE_PORT') or settings['DATABASE_PORT']
+    DB_USERNAME = os.getenv('DATABASE_USERNAME') or settings['DATABASE_USERNAME']
+    DB_PASSWORD = os.getenv('DATABASE_PASSWORD') or settings['DATABASE_PASSWORD']
+    DB_DATABASE = os.getenv('DATABASE_NAME') or settings['DATABASE_NAME']
+    
+    if not app_initialized and setup and setup == 'completed':
+        DBMS.initialize(DB_DBMS, DB_HOST, DB_PORT, DB_USERNAME, DB_PASSWORD,DB_DATABASE) # type: ignore
+        app_initialized = True
+    else:
+        return RedirectResponse(request.url_for('setup_index'))
+    return True
 
 async def jsonify(data):
     """
     Converts a string containing a dictionary to a Python dictionary.
 
     Args:
         data: The string containing a dictionary.
```

### Comparing `runit-server-0.4.0/runit_server/dockerize.py` & `runit-server-0.4.1/runit_server/dockerize.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/favicon.ico` & `runit-server-0.4.1/runit_server/favicon.ico`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/kubernetes-1.py` & `runit-server-0.4.1/runit_server/kubernetes-1.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/kubernetes-2.py` & `runit-server-0.4.1/runit_server/kubernetes-2.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/admin.py` & `runit-server-0.4.1/runit_server/models/admin.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/collection.py` & `runit-server-0.4.1/runit_server/models/collection.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/database.py` & `runit-server-0.4.1/runit_server/models/database.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/function.py` & `runit-server-0.4.1/runit_server/models/function.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/permission.py` & `runit-server-0.4.1/runit_server/models/permission.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/project.py` & `runit-server-0.4.1/runit_server/models/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         '''
         Instance Method for retrieving User of Project instance
         
         @params None
         @return User Instance
         '''
 
-        return Model.normalise(DBMS.Database.find_one('users', Model.normalise({'id': self.user_id}, 'params')))
+        return Model.normalise(DBMS.Database.find_one('users', Model.normalise({'id': self.user_id}, 'params'))) # type: ignore
     
     def functions(self):
         '''
         Instance Method for retrieving Functions of Project Instance
 
         @params None
         @return List of Function Instances
@@ -60,15 +60,15 @@
         '''
         Instance Method for counting function in Project
 
         @params None
         @return Count of functions
         '''
 
-        return DBMS.Database.count('functions', Model.normalise({'project_id': self.id}, 'params'))
+        return DBMS.Database.count('functions', Model.normalise({'project_id': self.id}, 'params')) # type: ignore
     
     def json(self)-> dict:
         '''
         Instance Method for converting instance to Dict
 
         @paramas None
         @return Dict() format of Project instance
@@ -87,9 +87,9 @@
 
         @param user_id:str _id of the user
         @return List of Project instances
         '''
         
         projects = DBMS.Database.find(Project.TABLE_NAME, Model.normalise({'user_id': user_id}, 'params'))
         
-        return [cls(**Model.normalise(elem)) for elem in projects]
+        return [cls(**Model.normalise(elem)) for elem in projects] # type: ignore
```

### Comparing `runit-server-0.4.0/runit_server/models/role.py` & `runit-server-0.4.1/runit_server/models/role.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/models/user.py` & `runit-server-0.4.1/runit_server/models/user.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/modules/account.py` & `runit-server-0.4.1/runit_server/modules/account.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/account.py` & `runit-server-0.4.1/runit_server/routers/account.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/admin.py` & `runit-server-0.4.1/runit_server/routers/admin.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/api/account.py` & `runit-server-0.4.1/runit_server/routers/api/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,20 @@
     
     return JSONResponse(json_projects)
 
  
 @account_api.get('/profile')
 async def api_user_profile(user: Annotated[User, Depends(get_current_user)]):
     user = User.get(str(user.id)) # type: ignore
+    user_json = user.json()
+    del user_json['password']
+    del user_json['gat']
+    del user_json['grt']
     
-    return JSONResponse(user.json())
+    return JSONResponse(user_json)
 
 @account_api.post('/profile')
 async def api_update_user_profile(
     user: Annotated[User, Depends(get_current_user)],
     account: AccountData
 ):
     user = User.get(str(user.id)) # type: ignore
```

### Comparing `runit-server-0.4.0/runit_server/routers/api/database.py` & `runit-server-0.4.1/runit_server/routers/api/database.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/api/project.py` & `runit-server-0.4.1/runit_server/routers/api/project.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/api/public.py` & `runit-server-0.4.1/runit_server/routers/api/public.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/database.py` & `runit-server-0.4.1/runit_server/routers/database.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/functions.py` & `runit-server-0.4.1/runit_server/routers/functions.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/github.py` & `runit-server-0.4.1/runit_server/routers/github.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/project.py` & `runit-server-0.4.1/runit_server/routers/project.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/routers/public.py` & `runit-server-0.4.1/runit_server/routers/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 import logging
 from pathlib import Path
+import time
 from typing import Annotated, Optional
 
 from fastapi.responses import RedirectResponse, JSONResponse
 from fastapi.security import OAuth2PasswordRequestForm
 from fastapi import APIRouter, Form, Request, WebSocket, WebSocketDisconnect, Depends, status
 
 from ..core import WSConnectionManager, flash, templates, jsonify
@@ -20,16 +21,14 @@
 from dotenv import load_dotenv, find_dotenv, dotenv_values
 
 from ..constants import (
     RUNIT_HOMEDIR,
     PROJECTS_DIR
 )
 
-load_dotenv()
-
 REGISTER_HTML_TEMPLATE = 'register.html'
 HOME_PAGE = 'index'
 
 wsmanager = WSConnectionManager()
 
 public = APIRouter(
     tags=["public"]
@@ -78,16 +77,17 @@
     else:
         return templates.TemplateResponse('404.html', context={'request': request})
 
 @public.get('/')
 @public.get('/login')
 async def index(request: Request):
     settings = dotenv_values(find_dotenv())
+    setup = os.getenv('SETUP') or settings['SETUP']
     
-    if settings is None or settings['SETUP'] != 'completed':
+    if setup != 'completed':
         return RedirectResponse(request.url_for('setup_index'))
     if 'user_id' in request.session.keys():
         return RedirectResponse(request.url_for('user_home'))
     return templates.TemplateResponse('login.html', context={'request': request})
 
 @public.get('/register')
 async def registration_page(request: Request):
@@ -120,15 +120,15 @@
         logging.exception(e)
         flash(request, 'Error during registration', 'danger')
         return RedirectResponse(request.url_for('registration_page'), status_code=status.HTTP_303_SEE_OTHER)
 
 @public.post('/login')
 async def login(request: Request, form_data: OAuth2PasswordRequestForm = Depends()):
     user = authenticate(form_data.username, form_data.password)
-
+    
     if not user:
         flash(request, 'Invalid Login Credentials', 'danger')
         return templates.TemplateResponse('login.html', context={'request': request})
     access_token = create_access_token(user.json())
     request.session['user_id'] = user.id
     request.session['user_name'] = user.name
     request.session['user_email'] = user.email
@@ -162,24 +162,28 @@
     if 'user_id' in request.session.keys():
         return RedirectResponse(request.url_for('user_home'))
     return templates.TemplateResponse('login.html', context={'request': request})
 
 @public.get('/{project_id}')
 @public.get('/{project_id}/{function}')
 async def run_project(request: Request, project_id: str, function: Optional[str] = None):
+    t0 = time.perf_counter()
     excluded = ['favicon.ico']
     if project_id in excluded:
         return None
     project = Project.get(project_id)
     if not project:
         return RunIt.notfound()
     
     current_project_dir = Path(PROJECTS_DIR, project.id).resolve()
     function = function if function else 'index'
     if current_project_dir.is_dir():
         if not RunIt.is_private(project_id, str(current_project_dir)):
             result = RunIt.start(project_id, function, str(current_project_dir), request.query_params._dict)
             os.chdir(RUNIT_HOMEDIR)
             response = await jsonify(result)
-            return JSONResponse(response) if type(response) is dict else response
-
+        t1 = time.perf_counter() # Record the stop time
+        elapsed_time = t1 - t0 # Calculate elapsed time
+        print(f'Time taken: {elapsed_time:.8f} seconds')
+        return JSONResponse(response) if type(response) is dict else response
+    
     return RunIt.notfound()
```

### Comparing `runit-server-0.4.0/runit_server/routers/setup.py` & `runit-server-0.4.1/runit_server/routers/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,16 +41,28 @@
         'request': request
     })
 
 @setup.post('/')
 async def initsetup(request: Request):
     env_file = find_dotenv()
     settings = dotenv_values(env_file)
-
-    settings.update(request.form().__dict__)
+    data = await request.form()
+    
+    settings.update(data._dict)
 
     for key, value in settings.items():
          set_key(env_file, key, value) # type: ignore
     set_key(env_file, 'SETUP', 'completed')
     
     flash(request,'Setup completed', category='success')
     return RedirectResponse(request.url_for('complete_setup'))
+
+@setup.get('/complete')
+async def complete_setup():
+    settings = dotenv_values(find_dotenv())
+
+    if 'SETUP' in settings.keys() and settings['SETUP'] == 'completed':
+        DBMS.initialize(settings['DBMS'], settings['DATABASE_HOST'], settings['DATABASE_PORT'], # type: ignore
+                    settings['DATABASE_USERNAME'], settings['DATABASE_PASSWORD'],  # type: ignore
+                    settings['DATABASE_NAME']) # type: ignore
+
+    return RedirectResponse(request.url_for('index'))
```

### Comparing `runit-server-0.4.0/runit_server/static/css/all.min.css` & `runit-server-0.4.1/runit_server/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/css/bootstrap.min.css` & `runit-server-0.4.1/runit_server/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/css/bootstrap.min.css.map` & `runit-server-0.4.1/runit_server/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/css/styles.css` & `runit-server-0.4.1/runit_server/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/loading.gif` & `runit-server-0.4.1/runit_server/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/html5.svg` & `runit-server-0.4.1/runit_server/static/images/logos/html5.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/nodejs.png` & `runit-server-0.4.1/runit_server/static/images/logos/nodejs.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/nodejs.svg` & `runit-server-0.4.1/runit_server/static/images/logos/nodejs.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/php.svg` & `runit-server-0.4.1/runit_server/static/images/logos/php.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/python.png` & `runit-server-0.4.1/runit_server/static/images/logos/python.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/python.svg` & `runit-server-0.4.1/runit_server/static/images/logos/python.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/python1.svg` & `runit-server-0.4.1/runit_server/static/images/logos/python1.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png` & `runit-server-0.4.1/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/images/terminal.svg` & `runit-server-0.4.1/runit_server/static/images/terminal.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/bootstrap.bundle.min.js` & `runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/bootstrap.bundle.min.js.map` & `runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/databases.js` & `runit-server-0.4.1/runit_server/static/js/databases.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/github.js` & `runit-server-0.4.1/runit_server/static/js/github.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/main.js` & `runit-server-0.4.1/runit_server/static/js/main.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/profile.js` & `runit-server-0.4.1/runit_server/static/js/profile.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/js/projects.js` & `runit-server-0.4.1/runit_server/static/js/projects.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -113,50 +113,57 @@
         let result = await response.json()
 
         return new Project(result)
     }
 
     static async create(form) {
         if (!form.reportValidity()) return null
-
         setLoading(true)
-        let data = Object.fromEntries(new FormData(form))
-        let access_token = document.getElementById('accessToken').innerText.trim()
-        let modalCloseBtn = document.querySelector('.btn-close')
-
-        let url = '/projects/'
-
-        let response = await fetch(url, {
-            headers: {
-                'Content-Type': 'application/json',
-                Authorization: `Bearer ${access_token}`
-            },
-            method: 'POST',
-            mode: 'same-origin',
-            body: JSON.stringify(data)
-        })
-
-        let result = await response.json()
 
-        setLoading(false)
-
-        const {
-            status,
-            message,
-            project
-        } = result
-
-        if (status === 'success') {
-            console.log(message)
-            console.log(project)
-            modalCloseBtn.click()
-            return new Project(project)
+        try {
+            let data = Object.fromEntries(new FormData(form))
+            let access_token = document.getElementById('accessToken').innerText.trim()
+            let modalCloseBtn = document.querySelector('.btn-close')
+
+            let url = '/projects/'
+
+            let response = await fetch(url, {
+                headers: {
+                    'Content-Type': 'application/json',
+                    Authorization: `Bearer ${access_token}`
+                },
+                method: 'POST',
+                mode: 'same-origin',
+                body: JSON.stringify(data)
+            })
+
+            let result = await response.json()
+
+            setLoading(false)
+
+            const {
+                status,
+                message,
+                project
+            } = result
+
+            if (status === 'success') {
+                console.log(message)
+                console.log(project)
+                modalCloseBtn.click()
+                return new Project(project)
+            }
+            console.error(message)
+            return null
+
+        } catch (error) {
+            setLoading(false)
+            console.log(error)
         }
-        console.error(message)
-        return null
+
 
 
     }
 
     static setRepos(repos = []) {
 
     }
```

### Comparing `runit-server-0.4.0/runit_server/static/js/setup.js` & `runit-server-0.4.1/runit_server/static/js/setup.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.eot` & `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.svg` & `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.ttf` & `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.woff` & `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-brands-400.woff2` & `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.eot` & `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.svg` & `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.ttf` & `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.woff` & `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-regular-400.woff2` & `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.eot` & `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.svg` & `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.ttf` & `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.woff` & `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/static/webfonts/fa-solid-900.woff2` & `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/404.html` & `runit-server-0.4.1/runit_server/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/account/home.html` & `runit-server-0.4.1/runit_server/templates/account/home.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/account/layout.html` & `runit-server-0.4.1/runit_server/templates/account/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
     <meta name="description" content="">
     <meta name="keywords" content="">
 
     <link href="/static/css/bootstrap.min.css" rel="stylesheet">
     <link href="/static/css/all.min.css" rel="stylesheet">
 
-    <link rel='icon' href="{{url_for('static', path='images/dark-terminal.svg')}}">
+    <link rel='icon' href="/static/images/dark-terminal.svg">
 
     <meta name="msapplication-TileColor" content="#ffff00">
     
     <meta name="theme-color" content="#ffff00">
 </head>
 
 <body class="bg-light bg-gradient">
@@ -119,11 +119,11 @@
             </nav>
             {% endif %}
             {% block content %}
             {% endblock %}
         </div>
     </main>
     {% block scripts %}
-    <script src="{{url_for('static', path='js/bootstrap.bundle.min.js')}}"></script>
+    <script src="/static/js/bootstrap.bundle.min.js"></script>
     {% endblock %}
 </body>
 </html>
```

### Comparing `runit-server-0.4.0/runit_server/templates/account/profile.html` & `runit-server-0.4.1/runit_server/templates/account/profile.html`

 * *Files 4% similar despite different names*

```diff
@@ -94,9 +94,9 @@
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
-<script src="{{url_for('static', path='js/profile.js')}}"></script>
+<script src="/static/js/profile.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/details.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/details.html`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,16 @@
 
 {% block scripts %} 
 <!-- <script>
 let db = JSON.parse({{ database | tojson }})
 document.getElementById("database").textContent = JSON.stringify(db, null, 4);
 </script> -->
 {{super()}}
-<script src="{{url_for('static', path='js/databases.js')}}"></script>
-<script src="{{url_for('static', path='js/ace/ace.js')}}" type="text/javascript" charset="utf-8"></script>
+<script src="/static/js/databases.js"></script>
+<script src="/static/js/ace/ace.js" type="text/javascript" charset="utf-8"></script>
 <script>
     const editor = ace.edit("database");
     editor.setTheme("ace/theme/chaos")
     editor.setReadOnly(true)
     editor.session.setMode(`ace/mode/javascript`)
     let db = {{ collections | tojson }}
     editor.session.setValue(JSON.stringify(db, null, 4))
```

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/grid.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/index.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/list.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/modals/database.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/modals/database.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/databases/modals/document.html` & `runit-server-0.4.1/runit_server/templates/admin/databases/modals/document.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/index.html` & `runit-server-0.4.1/runit_server/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/layout.html` & `runit-server-0.4.1/runit_server/templates/admin/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
     <meta name="description" content="">
     <meta name="keywords" content="">
 
     <link href="/static/css/bootstrap.min.css" rel="stylesheet">
     <link href="/static/css/all.min.css" rel="stylesheet">
 
-    <link rel='icon' href="{{url_for('static', path='images/dark-terminal.svg')}}">
+    <link rel='icon' href="/static/images/dark-terminal.svg')}}">
 
     <meta name="msapplication-TileColor" content="#ffff00">
     
     <meta name="theme-color" content="#ffff00">
 </head>
 
 <body>
@@ -113,11 +113,11 @@
                 </div>
             </nav>
             {% block content %}
             {% endblock %}
         </div>
     </main>
     {% block scripts %}
-    <script src="{{url_for('static', path='js/bootstrap.bundle.min.js')}}"></script>
+    <script src="/static/js/bootstrap.bundle.min.js"></script>
     {% endblock %}
 </body>
 </html>
```

### Comparing `runit-server-0.4.0/runit_server/templates/admin/login.html` & `runit-server-0.4.1/runit_server/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/profile.html` & `runit-server-0.4.1/runit_server/templates/admin/profile.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/projects/details.html` & `runit-server-0.4.1/runit_server/templates/admin/projects/details.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/projects/grid.html` & `runit-server-0.4.1/runit_server/templates/admin/projects/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/projects/index.html` & `runit-server-0.4.1/runit_server/templates/admin/projects/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/projects/list.html` & `runit-server-0.4.1/runit_server/templates/admin/projects/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/projects/modal.html` & `runit-server-0.4.1/runit_server/templates/admin/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/sidebar.html` & `runit-server-0.4.1/runit_server/templates/admin/sidebar.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/users/details.html` & `runit-server-0.4.1/runit_server/templates/admin/users/details.html`

 * *Files 1% similar despite different names*

```diff
@@ -151,9 +151,9 @@
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
-<script src="{{url_for('static', path='js/users.js')}}"></script>
+<script src="/static/js/users.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/admin/users/grid.html` & `runit-server-0.4.1/runit_server/templates/admin/users/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/users/index.html` & `runit-server-0.4.1/runit_server/templates/admin/users/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/users/list.html` & `runit-server-0.4.1/runit_server/templates/admin/users/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/admin/users/modal.html` & `runit-server-0.4.1/runit_server/templates/admin/users/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/databases/details.html` & `runit-server-0.4.1/runit_server/templates/databases/details.html`

 * *Files 1% similar despite different names*

```diff
@@ -159,9 +159,9 @@
 
 {% block scripts %} 
 <!-- <script>
 let db = JSON.parse({{ database | tojson }})
 document.getElementById("database").textContent = JSON.stringify(db, null, 4);
 </script> -->
 {{super()}}
-<script src="{{url_for('static', path='js/databases.js')}}"></script>
+<script src="/static/js/databases.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/databases/grid.html` & `runit-server-0.4.1/runit_server/templates/databases/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/databases/index.html` & `runit-server-0.4.1/runit_server/templates/databases/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/databases/list.html` & `runit-server-0.4.1/runit_server/templates/databases/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/databases/modal.html` & `runit-server-0.4.1/runit_server/templates/databases/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/docker/php.dockerfile` & `runit-server-0.4.1/runit_server/templates/docker/php.dockerfile`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/exposed.html` & `runit-server-0.4.1/runit_server/templates/exposed.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/functions/index.html` & `runit-server-0.4.1/runit_server/templates/functions/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/layout.html` & `runit-server-0.4.1/runit_server/templates/layout.html`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         content='width=device-width,initial-scale=1,minimum-scale=1,maximum-scale=1,user-scalable=no' />
     <meta name="description" content="">
     <meta name="keywords" content="">
 
     <link href="/static/css/bootstrap.min.css" rel="stylesheet">
     <link href="/static/css/all.min.css" rel="stylesheet">
 
-    <link rel='icon' href="{{url_for('static', path='images/dark-terminal.svg')}}">
+    <link rel='icon' href="/static/images/dark-terminal.svg')}}">
 
     <meta name="msapplication-TileColor" content="#ffff00">
     
     <meta name="theme-color" content="#ffff00">
     <style>
         body {
             font-size: 14px;
@@ -35,11 +35,11 @@
 </head>
 
 <body class="bg-light bg-gradient">
     {% block content %}
     {% endblock %}
 
     {% block scripts %}
-    <script src="{{url_for('static', path='js/bootstrap.bundle.min.js')}}"></script>
+    <script src="/static/js/bootstrap.bundle.min.js"></script>
     {% endblock %}
 </body>
 </html>
```

### Comparing `runit-server-0.4.0/runit_server/templates/login.html` & `runit-server-0.4.1/runit_server/templates/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/modals/confirm.html` & `runit-server-0.4.1/runit_server/templates/modals/confirm.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/modals/create_database.html` & `runit-server-0.4.1/runit_server/templates/modals/create_database.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/projects/details.html` & `runit-server-0.4.1/runit_server/templates/projects/details.html`

 * *Files 0% similar despite different names*

```diff
@@ -189,9 +189,9 @@
         {{request.session['access_token']}}
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
-<script src="{{url_for('static', path='js/projects.js')}}"></script>
+<script src="/static/js/projects.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/projects/grid.html` & `runit-server-0.4.1/runit_server/templates/projects/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/projects/index.html` & `runit-server-0.4.1/runit_server/templates/projects/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     <i class="fas fa-th-large fa-4x p-3 border text-black-50 hover:text-dark" style="border-style: dashed !important;"></i>
     New Project
 </a>
 {% endif %}
 {% endblock %}
 {% block scripts %} 
 {{super()}}
-<script src="{{url_for('static', path='js/github.js')}}" async></script>
-<script src="{{url_for('static', path='js/projects.js')}}" async></script>
+<script src="/static/js/github.js" async></script>
+<script src="/static/js/projects.js" async></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/projects/list.html` & `runit-server-0.4.1/runit_server/templates/projects/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/projects/modal.html` & `runit-server-0.4.1/runit_server/templates/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/register.html` & `runit-server-0.4.1/runit_server/templates/register.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/templates/setup/index.html` & `runit-server-0.4.1/runit_server/templates/setup/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -104,9 +104,9 @@
             </div>
         </div>
     </div>
 </main>
 {% endblock %}
 {% block scripts %}
 {{super()}}
-<script src="{{url_for('static', path='js/setup.js')}}"></script>
+<script src="/static/js/setup.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.0/runit_server/templates/sidebar.html` & `runit-server-0.4.1/runit_server/templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server/test.py` & `runit-server-0.4.1/runit_server/test.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.0/runit_server.egg-info/PKG-INFO` & `runit-server-0.4.1/runit_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit-server-0.4.0/runit_server.egg-info/SOURCES.txt` & `runit-server-0.4.1/runit_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 MANIFEST.in
 README.md
 setup.py
 runit_server/Request.py
 runit_server/__init__.py
 runit_server/app.py
 runit_server/auth.py
+runit_server/aws.py
+runit_server/azure.py
 runit_server/cli.py
 runit_server/constants.py
 runit_server/core.py
 runit_server/dockerize.py
 runit_server/exceptions.py
 runit_server/favicon.ico
+runit_server/gcloud.py
 runit_server/kubernetes-1.py
 runit_server/kubernetes-2.py
 runit_server/test.py
 runit_server.egg-info/PKG-INFO
 runit_server.egg-info/SOURCES.txt
 runit_server.egg-info/dependency_links.txt
 runit_server.egg-info/entry_points.txt
```

### Comparing `runit-server-0.4.0/setup.py` & `runit-server-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='runit-server',
     version=VERSION,
```

