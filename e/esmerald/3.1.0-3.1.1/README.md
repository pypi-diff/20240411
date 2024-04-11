# Comparing `tmp/esmerald-3.1.0.tar.gz` & `tmp/esmerald-3.1.1.tar.gz`

## Comparing `esmerald-3.1.0.tar` & `esmerald-3.1.1.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/__main__.py
--rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/applications.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/concurrency.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/enums.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/exceptions.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/injector.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/logging.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/param_functions.py
--rw-r--r--   0        0        0    22300 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/py.typed
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/requests.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/testclient.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/types.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/typing.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/websockets.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/enums.py
--rw-r--r--   0        0        0    47597 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/cors.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/csrf.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/jwt.py
--rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/openapi.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/session.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/static_files.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/edgy/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/__init__.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/base_user.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/mongoz/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/di/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/di/provider.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/json.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/msgspec.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/app_settings.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/cors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/https.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/constants.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/models.py
--rw-r--r--   0        0        0    20509 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/base.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/api_key/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/api_key/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/http/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/http/base.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/oauth2/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/oauth2/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/openid_connect/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/openapi/security/openid_connect/base.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/protocols/template.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/base.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/json.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/base.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/events.py
--rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/gateways.py
--rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/router.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/views.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/_metaclasses.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/_mixins.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/base.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/generics.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/apis/views.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/webhooks/__init__.py
--rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/routing/webhooks/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/signature.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/constants.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/inspect.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/models.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.0/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 esmerald-3.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.0/LICENSE
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 esmerald-3.1.0/README.md
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 esmerald-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 esmerald-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/__main__.py
+-rw-r--r--   0        0        0    91447 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/applications.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/concurrency.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/enums.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/exceptions.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/injector.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22300 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/py.typed
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/requests.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/testclient.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/types.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/typing.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/websockets.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    47597 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/cors.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/csrf.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/jwt.py
+-rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/openapi.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/session.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/static_files.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/edgy/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/edgy/base_user.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/edgy/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/mongoz/__init__.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/mongoz/base_user.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/mongoz/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/di/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/di/provider.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/msgspec.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/app_settings.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    20510 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/base.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/api_key/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/http/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/http/base.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/oauth2/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/openapi/security/openid_connect/base.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    23674 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/events.py
+-rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/router.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/views.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/_metaclasses.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/_mixins.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/base.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/generics.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/apis/views.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/webhooks/__init__.py
+-rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/routing/webhooks/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/constants.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/inspect.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/models.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.1/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 esmerald-3.1.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.1/LICENSE
+-rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 esmerald-3.1.1/README.md
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 esmerald-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 esmerald-3.1.1/PKG-INFO
```

### Comparing `esmerald-3.1.0/esmerald/__init__.py` & `esmerald-3.1.1/esmerald/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 
 from lilya import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.context import Context
```

### Comparing `esmerald-3.1.0/esmerald/applications.py` & `esmerald-3.1.1/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/backgound.py` & `esmerald-3.1.1/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/context.py` & `esmerald-3.1.1/esmerald/context.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/enums.py` & `esmerald-3.1.1/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/exception_handlers.py` & `esmerald-3.1.1/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/exceptions.py` & `esmerald-3.1.1/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/injector.py` & `esmerald-3.1.1/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/logging.py` & `esmerald-3.1.1/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/params.py` & `esmerald-3.1.1/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/parsers.py` & `esmerald-3.1.1/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/requests.py` & `esmerald-3.1.1/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/testclient.py` & `esmerald-3.1.1/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/types.py` & `esmerald-3.1.1/esmerald/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,46 +9,49 @@
     Mapping,
     Type,
     TypeVar,
     Union,
     get_args,
 )
 
-from lilya.middleware import DefineMiddleware  # noqa
-from lilya.responses import Response as LilyaResponse  # noqa
-from lilya.types import ASGIApp  # noqa
+from lilya.middleware import DefineMiddleware
+from lilya.types import ASGIApp
 from typing_extensions import Literal
 
 from esmerald.backgound import BackgroundTask, BackgroundTasks
 from esmerald.exceptions import MissingDependency
 from esmerald.routing.gateways import WebSocketGateway
 from esmerald.routing.router import Include
 
 try:
-    from asyncz.schedulers import AsyncIOScheduler  # noqa
+    from asyncz.schedulers import AsyncIOScheduler
 except ImportError:
     AsyncIOScheduler = Any  # type: ignore
 
 try:
-    from esmerald.config.template import TemplateConfig as TemplateConfig  # noqa
+    from esmerald.config.template import TemplateConfig as TemplateConfig
 except MissingDependency:
     TemplateConfig = Any  # type: ignore
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
-    from esmerald.conf.global_settings import EsmeraldAPISettings  # noqa
-    from esmerald.datastructures import Cookie, ResponseHeader, State  # noqa: TC004
-    from esmerald.injector import Inject  # noqa
-    from esmerald.protocols.middleware import MiddlewareProtocol
-    from esmerald.requests import Request  # noqa
-    from esmerald.responses import Response  # noqa
-    from esmerald.routing.apis.base import View  # noqa
-    from esmerald.routing.gateways import Gateway, WebhookGateway  # noqa
-    from esmerald.routing.router import HTTPHandler, Router, WebSocketHandler  # noqa
-    from esmerald.websockets import WebSocket  # noqa
+    from esmerald.conf.global_settings import EsmeraldAPISettings
+    from esmerald.datastructures import Cookie, ResponseHeader, State as State
+    from esmerald.injector import Inject
+    from esmerald.protocols.middleware import MiddlewareProtocol as MiddlewareProtocol
+    from esmerald.requests import Request
+    from esmerald.responses import Response
+    from esmerald.routing.apis.base import View
+    from esmerald.routing.gateways import Gateway, WebhookGateway
+    from esmerald.routing.router import (
+        HTTPHandler as HTTPHandler,
+        Router,
+        WebSocketHandler as WebSocketHandler,
+    )
+    from esmerald.websockets import WebSocket
 else:
     HTTPHandler = Any
     Message = Any
     Receive = Any
     Scope = Any
     Send = Any
     BaseHTTPMiddleware = Any
```

### Comparing `esmerald-3.1.0/esmerald/websockets.py` & `esmerald-3.1.1/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/__init__.py` & `esmerald-3.1.1/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/global_settings.py` & `esmerald-3.1.1/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/.gitignore.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/Makefile.e-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/main.py-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/urls.py-tpl`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 The `route_patterns` list routes URLs to views.
 
 Examples:
     Function views:
         1. Add an import:  from my_app.views import home
         2. Add a URL to route_patterns:  Gateway('/', handler=home, name='home')
     Class-based views:
-        1. Add an import:  from other_app.views import Home
+        1. Add an import: from other_app.views import Home
         2. Add a URL to route_patterns:  Gateway('/', handler=Home, name='home')
     Including another configuration:
         1. Import the Include object: from esmerald import Include
-        2. Add a URL to route_patterns:  Gateway('/api/v1/', Include(namespace='myapp.urls'))
+        2. Add a URL to route_patterns: Include('/api/v1/', namespace='myapp.urls'))
 """
 from esmerald import Include, Gateway
 
 route_patterns = [
 
 ]
```

### Comparing `esmerald-3.1.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl` & `esmerald-3.1.1/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/cors.py` & `esmerald-3.1.1/esmerald/config/cors.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/csrf.py` & `esmerald-3.1.1/esmerald/config/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/jwt.py` & `esmerald-3.1.1/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/openapi.py` & `esmerald-3.1.1/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/session.py` & `esmerald-3.1.1/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/static_files.py` & `esmerald-3.1.1/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/config/template.py` & `esmerald-3.1.1/esmerald/config/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/encoding.py` & `esmerald-3.1.1/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/hashers.py` & `esmerald-3.1.1/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/common/middleware.py` & `esmerald-3.1.1/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/edgy/base_user.py` & `esmerald-3.1.1/esmerald/contrib/auth/edgy/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/edgy/middleware.py` & `esmerald-3.1.1/esmerald/contrib/auth/edgy/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/mongoz/base_user.py` & `esmerald-3.1.1/esmerald/contrib/auth/mongoz/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/mongoz/middleware.py` & `esmerald-3.1.1/esmerald/contrib/auth/mongoz/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-3.1.1/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-3.1.1/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/di/provider.py` & `esmerald-3.1.1/esmerald/core/di/provider.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/cli.py` & `esmerald-3.1.1/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/env.py` & `esmerald-3.1.1/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/templates.py` & `esmerald-3.1.1/esmerald/core/directives/templates.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     def handle(self, app_or_project: str, name: str, **options: Any) -> Any:
         self.app_or_project = app_or_project
         self.name = name
         self.a_or_an = "an" if app_or_project == "app" else "a"
         self.verbosity = options["verbosity"]
         self.with_deployment = options.get("with_deployment", False)
         self.deployment_folder_name = options.get("deployment_folder_name", None)
+        self.with_basic_controller = options.get("with_basic_controller", False)
 
         if self.app_or_project not in TREAT_AS_PROJECT_DIRECTIVE:
             self.validate_name(name)
             top_dir = os.path.join(os.getcwd(), name)
         else:
             top_dir = os.path.join(os.getcwd(), self.deployment_folder_name)
 
@@ -57,14 +58,16 @@
         base_deployment = "deployment_template"
 
         context = {
             base_name: name,
             "esmerald_version": self.get_version(),
             "project_secret": options.get("secret_key"),
             "deployment_folder": self.deployment_folder_name,
+            "with_basic_controller": self.with_basic_controller,
+            "name": name,
         }
 
         template_dir = os.path.join(esmerald.__path__[0], "conf/directives", base_subdir)
         prefix_length = len(template_dir) + 1
 
         # Creates the project or application structure
         self.iterate_templates(
```

### Comparing `esmerald-3.1.0/esmerald/core/directives/utils.py` & `esmerald-3.1.1/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/createapp.py` & `esmerald-3.1.1/esmerald/core/directives/operations/createapp.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,26 +6,34 @@
 from esmerald.core.terminal import Print
 from esmerald.utils.crypto import get_random_secret_key
 
 printer = Print()
 
 
 @click.option("-v", "--verbosity", default=1, type=int, help="Displays the files generated")
+@click.option(
+    "--with-basic-controller",
+    default=False,
+    is_flag=True,
+    type=bool,
+    help="Should generate a basic controller",
+)
 @click.argument("name", type=str)
 @click.command(name="createapp")
-def create_app(name: str, verbosity: int) -> None:
+def create_app(name: str, with_basic_controller: bool, verbosity: int) -> None:
     """Creates the scaffold of an application
 
     How to run: `esmerald createapp <NAME>`
 
     Example: `esmerald createapp myapp`
     """
     options = {
         "secret_key": SECRET_KEY_INSECURE_PREFIX + get_random_secret_key(),
         "verbosity": verbosity,
+        "with_basic_controller": with_basic_controller,
     }
     directive = TemplateDirective()
 
     try:
         directive.handle("app", name=name, **options)
         printer.write_success(f"App {name} generated successfully!")
     except DirectiveError as e:
```

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/createdeployment.py` & `esmerald-3.1.1/esmerald/core/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/createproject.py` & `esmerald-3.1.1/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/list.py` & `esmerald-3.1.1/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/run.py` & `esmerald-3.1.1/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/runserver.py` & `esmerald-3.1.1/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/show_urls.py` & `esmerald-3.1.1/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/shell/base.py` & `esmerald-3.1.1/esmerald/core/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/shell/ipython.py` & `esmerald-3.1.1/esmerald/core/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/shell/ptpython.py` & `esmerald-3.1.1/esmerald/core/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/directives/operations/shell/utils.py` & `esmerald-3.1.1/esmerald/core/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/terminal/base.py` & `esmerald-3.1.1/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/terminal/print.py` & `esmerald-3.1.1/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/terminal/terminal.py` & `esmerald-3.1.1/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/core/urls/base.py` & `esmerald-3.1.1/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/__init__.py` & `esmerald-3.1.1/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/base.py` & `esmerald-3.1.1/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/encoders.py` & `esmerald-3.1.1/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/file.py` & `esmerald-3.1.1/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/json.py` & `esmerald-3.1.1/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/msgspec.py` & `esmerald-3.1.1/esmerald/datastructures/msgspec.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/redirect.py` & `esmerald-3.1.1/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/stream.py` & `esmerald-3.1.1/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/datastructures/template.py` & `esmerald-3.1.1/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/interceptors/interceptor.py` & `esmerald-3.1.1/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/__init__.py` & `esmerald-3.1.1/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/_exception_handlers.py` & `esmerald-3.1.1/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/app_settings.py` & `esmerald-3.1.1/esmerald/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/asyncexitstack.py` & `esmerald-3.1.1/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/authentication.py` & `esmerald-3.1.1/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/exceptions.py` & `esmerald-3.1.1/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/middleware/settings_middleware.py` & `esmerald-3.1.1/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/_internal.py` & `esmerald-3.1.1/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/datastructures.py` & `esmerald-3.1.1/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/docs.py` & `esmerald-3.1.1/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/models.py` & `esmerald-3.1.1/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/openapi.py` & `esmerald-3.1.1/esmerald/openapi/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     else:
         operation.summary = route.name.replace("_", " ").replace("-", " ").title()
 
     if route.description:
         operation.description = route.description
 
     operation_id = route.operation_id
+
     if operation_id in operation_ids:
         message = (
             f"Duplicate Operation ID {operation_id} for function " + f"{route.handler.__name__}"
         )
         file_name = getattr(route.handler, "__globals__", {}).get("__file__")
         if file_name:
             message += f" at {file_name}"
```

### Comparing `esmerald-3.1.0/esmerald/openapi/responses.py` & `esmerald-3.1.1/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/utils.py` & `esmerald-3.1.1/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/validation.py` & `esmerald-3.1.1/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/security/base.py` & `esmerald-3.1.1/esmerald/openapi/security/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/security/api_key/base.py` & `esmerald-3.1.1/esmerald/openapi/security/api_key/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/security/http/base.py` & `esmerald-3.1.1/esmerald/openapi/security/http/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/security/oauth2/base.py` & `esmerald-3.1.1/esmerald/openapi/security/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/openapi/security/openid_connect/base.py` & `esmerald-3.1.1/esmerald/openapi/security/openid_connect/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/permissions/base.py` & `esmerald-3.1.1/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/permissions/utils.py` & `esmerald-3.1.1/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/pluggables/base.py` & `esmerald-3.1.1/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/protocols/asyncdao.py` & `esmerald-3.1.1/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/protocols/dao.py` & `esmerald-3.1.1/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/protocols/interceptor.py` & `esmerald-3.1.1/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/protocols/template.py` & `esmerald-3.1.1/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/responses/base.py` & `esmerald-3.1.1/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/responses/encoders.py` & `esmerald-3.1.1/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/responses/json.py` & `esmerald-3.1.1/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/responses/template.py` & `esmerald-3.1.1/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/_internal.py` & `esmerald-3.1.1/esmerald/routing/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/base.py` & `esmerald-3.1.1/esmerald/routing/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
             if status_code:
                 data.status_code = status_code
             return data
 
         return response_content
 
-    def starlette_response_handler(
+    def lilya_response_handler(
         self,
         cookies: "ResponseCookies",
         headers: Optional["ResponseHeaders"] = None,
     ) -> "AsyncAnyCallable":
         """Creates an handler for Lilya Responses."""
 
         async def response_content(data: LilyaResponse, **kwargs: Dict[str, Any]) -> LilyaResponse:
@@ -431,15 +431,15 @@
                 handler = self.response_handler(
                     cookies=cookies,
                     status_code=self.status_code,
                     media_type=self.media_type,
                     headers=headers,
                 )
             elif is_class_and_subclass(self.handler_signature.return_annotation, LilyaResponse):
-                handler = self.starlette_response_handler(
+                handler = self.lilya_response_handler(
                     cookies=cookies,
                     headers=headers,
                 )
             else:
                 handler = self._handler(
                     background=self.background,
                     cookies=cookies,
```

### Comparing `esmerald-3.1.0/esmerald/routing/events.py` & `esmerald-3.1.1/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/gateways.py` & `esmerald-3.1.1/esmerald/routing/gateways.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,48 @@
             if isinstance(middleware, DefineMiddleware):
                 _middleware.append(middleware)
             else:
                 _middleware.append(DefineMiddleware(middleware))  # type: ignore
         return _middleware
 
 
-class Gateway(LilyaPath, BaseInterceptorMixin, BaseMiddleware):
+class GatewayUtil:
+
+    def is_class_based(
+        self, handler: Union["HTTPHandler", "WebSocketHandler", "ParentType"]
+    ) -> bool:
+        return bool(is_class_and_subclass(handler, View) or isinstance(handler, View))
+
+    def is_handler(self, handler: Union["HTTPHandler", "WebSocketHandler", "ParentType"]) -> bool:
+        return bool(not is_class_and_subclass(handler, View) and not isinstance(handler, View))
+
+    def generate_operation_id(
+        self, name: Union[str, None], handler: Union["HTTPHandler", "WebSocketHandler", View]
+    ) -> str:
+        """
+        Generates an unique operation if for the handler.
+
+        We need to be able to handle with edge cases when a view does not default a path like `/format` and a default name needs to be passed when its a class based view.
+        """
+        if self.is_class_based(handler.parent):
+            operation_id = (
+                handler.parent.__class__.__name__.lower() + f"_{name}" + handler.path_format
+            )
+        else:
+            operation_id = name + handler.path_format
+
+        operation_id = re.sub(r"\W", "_", operation_id)
+        methods = list(handler.methods)  # type: ignore
+
+        assert handler.methods  # type: ignore
+        operation_id = f"{operation_id}_{methods[0].lower()}"
+        return operation_id
+
+
+class Gateway(LilyaPath, BaseInterceptorMixin, BaseMiddleware, GatewayUtil):
     """
     `Gateway` object class used by Esmerald routes.
 
     The Gateway act as a brigde between the router handlers and
     the main Esmerald routing system.
 
     Read more about [Gateway](https://esmerald.dev/routing/routes/#gateway) and
@@ -279,40 +312,28 @@
         self.parent = parent
         self.security = security
         self.tags = tags or []
         (handler.path_regex, handler.path_format, handler.param_convertors, _) = compile_path(
             self.path
         )
 
-        if not is_class_and_subclass(self.handler, View) and not isinstance(self.handler, View):
+        if self.is_handler(self.handler):  # type: ignore
             self.handler.name = self.name
 
             if not handler.operation_id:
-                handler.operation_id = self.generate_operation_id()
+                handler.operation_id = self.generate_operation_id(
+                    name=self.name, handler=self.handler  # type: ignore
+                )
 
     async def handle_dispatch(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         """
         Handles the interception of messages and calls from the API.
-        if self._middleware:
-            self.is_middleware = True
         """
         await self.app(scope, receive, send)
 
-    def generate_operation_id(self) -> str:
-        """
-        Generates an unique operation if for the handler
-        """
-        operation_id = self.name + self.handler.path_format
-        operation_id = re.sub(r"\W", "_", operation_id)
-        methods = list(self.handler.methods)
-
-        assert self.handler.methods
-        operation_id = f"{operation_id}_{methods[0].lower()}"
-        return cast(str, operation_id)
-
 
 class WebSocketGateway(LilyaWebSocketPath, BaseInterceptorMixin, BaseMiddleware):
     """
     `WebSocketGateway` object class used by Esmerald routes.
 
     The WebSocketGateway act as a brigde between the router handlers and
     the main Esmerald routing system.
@@ -504,15 +525,15 @@
         Handles the interception of messages and calls from the API.
         if self._middleware:
             self.is_middleware = True
         """
         await self.app(scope, receive, send)
 
 
-class WebhookGateway(LilyaPath, BaseInterceptorMixin):
+class WebhookGateway(LilyaPath, BaseInterceptorMixin, GatewayUtil):
     """
     `WebhookGateway` object class used by Esmerald routes.
 
     The WebhookGateway act as a brigde between the webhook handlers and
     the main Esmerald routing system.
 
     Read more about [WebhookGateway](https://esmerald.dev/routing/webhooks/) and
@@ -644,24 +665,14 @@
         self.parent = parent
         self.security = security
         self.tags = tags or []
         (handler.path_regex, handler.path_format, handler.param_convertors, _) = compile_path(
             self.path
         )
 
-        if not is_class_and_subclass(self.handler, View) and not isinstance(self.handler, View):
+        if self.is_handler(self.handler):  # type: ignore
             self.handler.name = self.name
 
             if not handler.operation_id:
-                handler.operation_id = self.generate_operation_id()
-
-    def generate_operation_id(self) -> str:
-        """
-        Generates an unique operation if for the handler
-        """
-        operation_id = self.name + self.handler.path_format
-        operation_id = re.sub(r"\W", "_", operation_id)
-        methods = list(self.handler.methods)
-
-        assert self.handler.methods
-        operation_id = f"{operation_id}_{methods[0].lower()}"
-        return cast(str, operation_id)
+                handler.operation_id = self.generate_operation_id(
+                    name=self.name, handler=self.handler  # type: ignore
+                )
```

### Comparing `esmerald-3.1.0/esmerald/routing/handlers.py` & `esmerald-3.1.1/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/router.py` & `esmerald-3.1.1/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/apis/_metaclasses.py` & `esmerald-3.1.1/esmerald/routing/apis/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/apis/_mixins.py` & `esmerald-3.1.1/esmerald/routing/apis/_mixins.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/apis/base.py` & `esmerald-3.1.1/esmerald/routing/apis/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/apis/generics.py` & `esmerald-3.1.1/esmerald/routing/apis/generics.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/apis/views.py` & `esmerald-3.1.1/esmerald/routing/apis/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/routing/webhooks/handlers.py` & `esmerald-3.1.1/esmerald/routing/webhooks/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/security/jwt/token.py` & `esmerald-3.1.1/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/template/jinja.py` & `esmerald-3.1.1/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/template/mako.py` & `esmerald-3.1.1/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/transformers/datastructures.py` & `esmerald-3.1.1/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/transformers/model.py` & `esmerald-3.1.1/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/transformers/signature.py` & `esmerald-3.1.1/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/transformers/utils.py` & `esmerald-3.1.1/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/constants.py` & `esmerald-3.1.1/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/dependency.py` & `esmerald-3.1.1/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/functional.py` & `esmerald-3.1.1/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/helpers.py` & `esmerald-3.1.1/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/models.py` & `esmerald-3.1.1/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/sync.py` & `esmerald-3.1.1/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/esmerald/utils/pydantic/schema.py` & `esmerald-3.1.1/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/LICENSE` & `esmerald-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/README.md` & `esmerald-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/pyproject.toml` & `esmerald-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.0/PKG-INFO` & `esmerald-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esmerald
-Version: 3.1.0
+Version: 3.1.1
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
```

