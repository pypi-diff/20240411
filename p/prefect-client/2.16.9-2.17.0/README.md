# Comparing `tmp/prefect-client-2.16.9.tar.gz` & `tmp/prefect-client-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-client-2.16.9.tar", last modified: Thu Apr  4 20:12:55 2024, max compression
+gzip compressed data, was "prefect-client-2.17.0.tar", last modified: Thu Apr 11 20:02:42 2024, max compression
```

## Comparing `prefect-client-2.16.9.tar` & `prefect-client-2.17.0.tar`

### file list

```diff
@@ -1,336 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.443944 prefect-client-2.16.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 20:12:52.000000 prefect-client-2.16.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 20:12:52.000000 prefect-client-2.16.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-04 20:12:55.443944 prefect-client-2.16.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-04 20:12:52.000000 prefect-client-2.16.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-04 20:12:52.000000 prefect-client-2.16.9/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 20:12:52.000000 prefect-client-2.16.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 20:12:52.000000 prefect-client-2.16.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-04 20:12:55.443944 prefect-client-2.16.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-04 20:12:52.000000 prefect-client-2.16.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.399943 prefect-client-2.16.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.407943 prefect-client-2.16.9/src/prefect/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/.prefectignore
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.407943 prefect-client-2.16.9/src/prefect/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.407943 prefect-client-2.16.9/src/prefect/_internal/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/compatibility/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/compatibility/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.407943 prefect-client-2.16.9/src/prefect/_internal/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/cancellation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/concurrency/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.411944 prefect-client-2.16.9/src/prefect/_internal/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.411944 prefect-client-2.16.9/src/prefect/_internal/pydantic/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/annotations/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.411944 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_dump_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_validate_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/type_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/v1_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pydantic/v2_validated_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/pytz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.411944 prefect-client-2.16.9/src/prefect/_internal/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/schemas/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/schemas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32606 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_internal/schemas/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.411944 prefect-client-2.16.9/src/prefect/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.415943 prefect-client-2.16.9/src/prefect/_vendor/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.415943 prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.415943 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.415943 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/param_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.419943 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/fastapi/websockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.419943 prefect-client-2.16.9/src/prefect/_vendor/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/convertors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/formparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.423944 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_vendor/starlette/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27791 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.423944 prefect-client-2.16.9/src/prefect/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26893 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/blocks/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.423944 prefect-client-2.16.9/src/prefect/client/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   111331 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/orchestration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.427944 prefect-client-2.16.9/src/prefect/client/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25567 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35514 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    51855 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/schemas/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/client/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.427944 prefect-client-2.16.9/src/prefect/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/concurrency/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.427944 prefect-client-2.16.9/src/prefect/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    40062 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    44306 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.427944 prefect-client-2.16.9/src/prefect/deployments/steps/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/steps/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/steps/pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deployments/steps/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.427944 prefect-client-2.16.9/src/prefect/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/data_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/deprecated/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/orion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/deprecated/packaging/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)   110035 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14019 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/related.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/events/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/schemas/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/schemas/deployment_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/schemas/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/schemas/labelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/events/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/flow_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70460 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/futures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/infrastructure/provisioners/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.431944 prefect-client-2.16.9/src/prefect/input/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/input/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/input/run_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/highlighters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/logging/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/manifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/profiles.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/pydantic/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48079 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runtime/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runtime/flow_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/runtime/task_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.399943 prefect-client-2.16.9/src/prefect/server/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.399943 prefect-client-2.16.9/src/prefect/server/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.399943 prefect-client-2.16.9/src/prefect/server/api/collections_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/server/api/collections_data/views/
--rw-r--r--   0 runner    (1001) docker     (127)    78423 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/server/api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/server/api/static/prefect-logo-mark-gradient.png
--rw-r--r--   0 runner    (1001) docker     (127)    72138 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.435944 prefect-client-2.16.9/src/prefect/software/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/software/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/software/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/software/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/software/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    20839 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/task_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/task_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    50477 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.439944 prefect-client-2.16.9/src/prefect/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/asyncutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/callables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/dockerutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/importtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/names.py
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/processutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/render_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.439944 prefect-client-2.16.9/src/prefect/utilities/schema_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/schema_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/schema_tools/hydration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/schema_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/slugify.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/utilities/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.443944 prefect-client-2.16.9/src/prefect/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44979 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-04 20:12:52.000000 prefect-client-2.16.9/src/prefect/workers/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:12:55.443944 prefect-client-2.16.9/src/prefect_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-04 20:12:55.000000 prefect-client-2.16.9/src/prefect_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-04 20:12:55.000000 prefect-client-2.16.9/src/prefect_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:12:55.000000 prefect-client-2.16.9/src/prefect_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 20:12:55.000000 prefect-client-2.16.9/src/prefect_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 20:12:55.000000 prefect-client-2.16.9/src/prefect_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    78066 2024-04-04 20:12:52.000000 prefect-client-2.16.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.543733 prefect-client-2.17.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 20:02:39.000000 prefect-client-2.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 20:02:39.000000 prefect-client-2.17.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-11 20:02:42.543733 prefect-client-2.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-11 20:02:39.000000 prefect-client-2.17.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-11 20:02:39.000000 prefect-client-2.17.0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 20:02:39.000000 prefect-client-2.17.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 20:02:39.000000 prefect-client-2.17.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-11 20:02:42.543733 prefect-client-2.17.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-11 20:02:39.000000 prefect-client-2.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.495734 prefect-client-2.17.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.499734 prefect-client-2.17.0/src/prefect/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/.prefectignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.499734 prefect-client-2.17.0/src/prefect/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.503733 prefect-client-2.17.0/src/prefect/_internal/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/compatibility/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/compatibility/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.503733 prefect-client-2.17.0/src/prefect/_internal/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/concurrency/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.503733 prefect-client-2.17.0/src/prefect/_internal/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.503733 prefect-client-2.17.0/src/prefect/_internal/pydantic/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/annotations/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.507733 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/config_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_fields_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/type_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/v1_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pydantic/v2_validated_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/pytz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.507733 prefect-client-2.17.0/src/prefect/_internal/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/schemas/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/schemas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32606 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_internal/schemas/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.507733 prefect-client-2.17.0/src/prefect/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.511734 prefect-client-2.17.0/src/prefect/_vendor/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.511734 prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.511734 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.515734 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/param_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.515734 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/fastapi/websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.519734 prefect-client-2.17.0/src/prefect/_vendor/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/convertors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/formparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.519734 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_vendor/starlette/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.523733 prefect-client-2.17.0/src/prefect/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26932 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/blocks/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.523733 prefect-client-2.17.0/src/prefect/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112936 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/orchestration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.523733 prefect-client-2.17.0/src/prefect/client/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52220 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/schemas/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/client/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.523733 prefect-client-2.17.0/src/prefect/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/concurrency/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.527733 prefect-client-2.17.0/src/prefect/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21353 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41221 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44302 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.527733 prefect-client-2.17.0/src/prefect/deployments/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/steps/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/steps/pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deployments/steps/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.527733 prefect-client-2.17.0/src/prefect/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/data_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.527733 prefect-client-2.17.0/src/prefect/deprecated/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/orion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/deprecated/packaging/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89809 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.527733 prefect-client-2.17.0/src/prefect/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/related.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.531734 prefect-client-2.17.0/src/prefect/events/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/schemas/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/schemas/deployment_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/schemas/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/schemas/labelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/events/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35260 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/flow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70512 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/futures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.531734 prefect-client-2.17.0/src/prefect/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.531734 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/infrastructure/provisioners/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.531734 prefect-client-2.17.0/src/prefect/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/input/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/input/run_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/highlighters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/logging/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/profiles.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/pydantic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48079 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runtime/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runtime/flow_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/runtime/task_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.495734 prefect-client-2.17.0/src/prefect/server/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.495734 prefect-client-2.17.0/src/prefect/server/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.495734 prefect-client-2.17.0/src/prefect/server/api/collections_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/server/api/collections_data/views/
+-rw-r--r--   0 runner    (1001) docker     (127)    78423 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/server/api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72895 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.535734 prefect-client-2.17.0/src/prefect/software/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/software/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/software/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/software/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/software/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20839 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/task_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/task_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50477 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.539734 prefect-client-2.17.0/src/prefect/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/asyncutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/callables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/dockerutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/processutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/render_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.539734 prefect-client-2.17.0/src/prefect/utilities/schema_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/schema_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/schema_tools/hydration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/schema_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/utilities/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.543733 prefect-client-2.17.0/src/prefect/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44977 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-11 20:02:39.000000 prefect-client-2.17.0/src/prefect/workers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:02:42.543733 prefect-client-2.17.0/src/prefect_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-11 20:02:42.000000 prefect-client-2.17.0/src/prefect_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-11 20:02:42.000000 prefect-client-2.17.0/src/prefect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:02:42.000000 prefect-client-2.17.0/src/prefect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 20:02:42.000000 prefect-client-2.17.0/src/prefect_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 20:02:42.000000 prefect-client-2.17.0/src/prefect_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    78066 2024-04-11 20:02:39.000000 prefect-client-2.17.0/versioneer.py
```

### Comparing `prefect-client-2.16.9/LICENSE` & `prefect-client-2.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/MANIFEST.in` & `prefect-client-2.17.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/PKG-INFO` & `prefect-client-2.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.16.9
+Version: 2.17.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.16.9/README.md` & `prefect-client-2.17.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/requirements-client.txt` & `prefect-client-2.17.0/requirements-client.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 graphviz >= 0.20.1
 griffe >= 0.20.0
 httpcore >=1.0.5, < 2.0.0
 httpx[http2] >= 0.23, != 0.23.2
 importlib_metadata >= 4.4; python_version < '3.10'
 importlib-resources >= 6.1.3, < 6.2.0
 jsonpatch >= 1.32, < 2.0
-jsonschema >= 3.2.0, < 5.0.0
+jsonschema >= 4.0.0, < 5.0.0
 orjson >= 3.7, < 4.0
 packaging >= 21.3, < 24.3
 pathspec >= 0.8.0
 # https://github.com/PrefectHQ/prefect/issues/11619
 pendulum < 3.0; python_version < '3.12'
 pendulum >= 3.0.0, <4; python_version >= '3.12'
 # the version constraints for pydantic are merged with those from fastapi 0.103.2
 pydantic[email]>=1.10.0,!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0
-pydantic_core >= 2.10.0, < 3.0.0
+pydantic_core >= 2.12.0, < 3.0.0
 python_dateutil >= 2.8.2, < 3.0.0
 python-slugify >= 5.0, < 9.0
 pyyaml >= 5.4.1, < 7.0.0
 rfc3339-validator >= 0.1.4, < 0.2.0
 rich >= 11.0, < 14.0
 ruamel.yaml >= 0.17.0
 sniffio >=1.3.0, < 2.0.0
```

### Comparing `prefect-client-2.16.9/requirements-dev.txt` & `prefect-client-2.17.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/setup.cfg` & `prefect-client-2.17.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/setup.py` & `prefect-client-2.17.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/__init__.py` & `prefect-client-2.17.0/src/prefect/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,32 +103,14 @@
 
 from prefect._internal.compatibility.deprecated import (
     inject_renamed_module_alias_finder,
     register_renamed_module,
 )
 
 register_renamed_module(
-    "prefect.client.orchestration",
-    "prefect.client.orchestration",
-    start_date="Feb 2023",
-)
-register_renamed_module(
-    "prefect.docker",
-    "prefect.utilities.dockerutils",
-    start_date="Mar 2023",
-)
-register_renamed_module(
-    "prefect.infrastructure.docker",
-    "prefect.infrastructure.container",
-    start_date="Mar 2023",
-)
-register_renamed_module(
-    "prefect.projects", "prefect.deployments", start_date="Jun 2023"
-)
-register_renamed_module(
     "prefect.packaging", "prefect.deprecated.packaging", start_date="Mar 2024"
 )
 inject_renamed_module_alias_finder()
 
 
 # Attempt to warn users who are importing Prefect 1.x attributes that they may
 # have accidentally installed Prefect 2.x
```

### Comparing `prefect-client-2.16.9/src/prefect/_internal/_logging.py` & `prefect-client-2.17.0/src/prefect/_internal/_logging.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/compatibility/experimental.py` & `prefect-client-2.17.0/src/prefect/_internal/compatibility/experimental.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/__init__.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/api.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/api.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/calls.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/calls.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/cancellation.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/cancellation.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/event_loop.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/event_loop.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/inspection.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/inspection.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/primitives.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/primitives.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/services.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/threads.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/threads.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/concurrency/waiters.py` & `prefect-client-2.17.0/src/prefect/_internal/concurrency/waiters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/__init__.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     model_copy,
     model_validate_json,
     TypeAdapter,
     validate_python,
     BaseModel,
     Field,
     FieldInfo,
+    field_validator,
+    model_validator,
 )
 
 from ._types import IncEx
 
 __all__ = [
     "model_dump",
     "model_json_schema",
@@ -35,8 +37,10 @@
     "model_validate_json",
     "TypeAdapter",
     "validate_python",
     "BaseModel",
     "HAS_PYDANTIC_V2",
     "Field",
     "FieldInfo",
+    "field_validator",
+    "model_validator",
 ]
```

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/_compat.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/_compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,43 @@
+"""
+Functions within this module check for Pydantic V2 compatibility and provide mechanisms for copying,
+ dumping, and validating models in a way that is agnostic to the underlying Pydantic version.
+"""
+import typing
+
 from ._base_model import BaseModel as PydanticBaseModel
-from ._base_model import Field, FieldInfo
+from ._base_model import (
+    ConfigDict,
+    Field,
+    FieldInfo,
+    PrivateAttr,
+    SecretStr,
+    ValidationError,
+)
 from ._flags import HAS_PYDANTIC_V2, USE_PYDANTIC_V2
+from .utilities.config_dict import ConfigMixin
+from .utilities.field_validator import field_validator
 from .utilities.model_construct import ModelConstructMixin, model_construct
 from .utilities.model_copy import ModelCopyMixin, model_copy
 from .utilities.model_dump import ModelDumpMixin, model_dump
 from .utilities.model_dump_json import ModelDumpJsonMixin, model_dump_json
 from .utilities.model_fields import ModelFieldMixin
+from .utilities.model_fields_set import ModelFieldsSetMixin, model_fields_set
 from .utilities.model_json_schema import ModelJsonSchemaMixin, model_json_schema
 from .utilities.model_validate import ModelValidateMixin, model_validate
 from .utilities.model_validate_json import ModelValidateJsonMixin, model_validate_json
+from .utilities.model_validator import model_validator
 from .utilities.type_adapter import TypeAdapter, validate_python
 
-if HAS_PYDANTIC_V2 and USE_PYDANTIC_V2:
+if typing.TYPE_CHECKING:
+
+    class BaseModel(PydanticBaseModel):  # type: ignore
+        pass
+
+elif HAS_PYDANTIC_V2 and USE_PYDANTIC_V2:
     # In this case, there's no functionality to add, so we just alias the Pydantic v2 BaseModel
     class BaseModel(PydanticBaseModel):  # type: ignore
         pass
 
 else:
     # In this case, we're working with a Pydantic v1 model, so we need to add Pydantic v2 functionality
     # TODO: Find a smarter way of attaching these methods so that they don't need to be redefined
@@ -25,26 +47,35 @@
         ModelCopyMixin,
         ModelDumpMixin,
         ModelDumpJsonMixin,
         ModelJsonSchemaMixin,
         ModelValidateMixin,
         ModelValidateJsonMixin,
         ModelFieldMixin,
+        ConfigMixin,
+        ModelFieldsSetMixin,
         PydanticBaseModel,
     ):
         pass
 
 
 __all__ = [
     "model_construct",
     "model_copy",
     "model_dump",
     "model_dump_json",
     "model_json_schema",
     "model_validate",
     "model_validate_json",
+    "model_fields_set",
     "TypeAdapter",
     "validate_python",
     "BaseModel",
     "Field",
     "FieldInfo",
+    "field_validator",
+    "model_validator",
+    "PrivateAttr",
+    "SecretStr",
+    "ConfigDict",
+    "ValidationError",
 ]
```

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/_flags.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/_flags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This file defines flags that determine whether Pydantic V2 is available and whether its features should be used.
+"""
 import os
 
 # Retrieve current version of Pydantic installed in environment
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 # Check if Pydantic version 2 is the installed version
 HAS_PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
```

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/annotations/pendulum.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/annotations/pendulum.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_construct.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_construct.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_copy.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_copy.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_dump.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_dump.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_dump_json.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_fields.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_json_schema.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_rebuild.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_validate.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_validate.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/model_validate_json.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/utilities/type_adapter.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/utilities/type_adapter.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/v1_schema.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/v1_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/v2_schema.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/v2_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pydantic/v2_validated_func.py` & `prefect-client-2.17.0/src/prefect/_internal/pydantic/v2_validated_func.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/pytz.py` & `prefect-client-2.17.0/src/prefect/_internal/pytz.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/schemas/bases.py` & `prefect-client-2.17.0/src/prefect/_internal/schemas/bases.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/schemas/fields.py` & `prefect-client-2.17.0/src/prefect/_internal/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/schemas/serializers.py` & `prefect-client-2.17.0/src/prefect/_internal/schemas/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_internal/schemas/validators.py` & `prefect-client-2.17.0/src/prefect/_internal/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/__init__.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/applications.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/concurrency.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/datastructures.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/models.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/dependencies/utils.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/encoders.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/exception_handlers.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/exceptions.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/docs.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/models.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/openapi/utils.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/param_functions.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/params.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/responses.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/routing.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/__init__.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/api_key.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/http.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/oauth2.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/security/open_id_connect_url.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/fastapi/utils.py` & `prefect-client-2.17.0/src/prefect/_vendor/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/_compat.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/_compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/_exception_handler.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/_utils.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/_utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/applications.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/authentication.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/background.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/background.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/concurrency.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/config.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/config.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/convertors.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/convertors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/datastructures.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/endpoints.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/endpoints.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/exceptions.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/formparsers.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/formparsers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/__init__.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/authentication.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/base.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/cors.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/errors.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/exceptions.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/gzip.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/httpsredirect.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/sessions.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/trustedhost.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/middleware/wsgi.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/requests.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/requests.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/responses.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/routing.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/schemas.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/schemas.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/staticfiles.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/staticfiles.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/status.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/status.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/templating.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/testclient.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/testclient.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/types.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/types.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_vendor/starlette/websockets.py` & `prefect-client-2.17.0/src/prefect/_vendor/starlette/websockets.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/_version.py` & `prefect-client-2.17.0/src/prefect/_version.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/agent.py` & `prefect-client-2.17.0/src/prefect/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         )
 
         # this piece of logic applies any overrides that may have been set on the
         # deployment; overrides are defined as dot.delimited paths on possibly nested
         # attributes of the infrastructure block
         doc_dict = infra_document.dict()
         infra_dict = doc_dict.get("data", {})
-        for override, value in (deployment.infra_overrides or {}).items():
+        for override, value in (deployment.job_variables or {}).items():
             nested_fields = override.split(".")
             data = infra_dict
             for field in nested_fields[:-1]:
                 data = data[field]
 
             # once we reach the end, set the value
             data[nested_fields[-1]] = value
```

### Comparing `prefect-client-2.16.9/src/prefect/artifacts.py` & `prefect-client-2.17.0/src/prefect/artifacts.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/abstract.py` & `prefect-client-2.17.0/src/prefect/blocks/abstract.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/core.py` & `prefect-client-2.17.0/src/prefect/blocks/core.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/fields.py` & `prefect-client-2.17.0/src/prefect/blocks/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/kubernetes.py` & `prefect-client-2.17.0/src/prefect/blocks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/notifications.py` & `prefect-client-2.17.0/src/prefect/blocks/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     _documentation_url = "https://docs.prefect.io/ui/notifications/"
     url: SecretStr = Field(
         default=...,
         title="Webhook URL",
         description="Incoming webhook URL used to send notifications.",
-        example="https://hooks.example.com/XXX",
+        examples=["https://hooks.example.com/XXX"],
     )
 
 
 # TODO: Move to prefect-slack once collection block auto-registration is
 # available
 class SlackWebhook(AppriseNotificationBlock):
     """
@@ -101,15 +101,15 @@
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/c1965ecbf8704ee1ea20d77786de9a41ce1087d1-500x500.png"
     _documentation_url = "https://docs.prefect.io/api-ref/prefect/blocks/notifications/#prefect.blocks.notifications.SlackWebhook"
 
     url: SecretStr = Field(
         default=...,
         title="Webhook URL",
         description="Slack incoming webhook URL used to send notifications.",
-        example="https://hooks.slack.com/XXX",
+        examples=["https://hooks.slack.com/XXX"],
     )
 
 
 class MicrosoftTeamsWebhook(AppriseNotificationBlock):
     """
     Enables sending notifications via a provided Microsoft Teams webhook.
 
@@ -127,17 +127,17 @@
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/817efe008a57f0a24f3587414714b563e5e23658-250x250.png"
     _documentation_url = "https://docs.prefect.io/api-ref/prefect/blocks/notifications/#prefect.blocks.notifications.MicrosoftTeamsWebhook"
 
     url: SecretStr = Field(
         ...,
         title="Webhook URL",
         description="The Teams incoming webhook URL used to send notifications.",
-        example=(
+        examples=[
             "https://your-org.webhook.office.com/webhookb2/XXX/IncomingWebhook/YYY/ZZZ"
-        ),
+        ],
     )
 
 
 class PagerDutyWebHook(AbstractAppriseNotificationBlock):
     """
     Enables sending notifications via a provided PagerDuty webhook.
     See [Apprise notify_pagerduty docs](https://github.com/caronc/apprise/wiki/Notify_pagerduty)
@@ -218,15 +218,15 @@
         default=True,
         description="Associate the notification status via a represented icon.",
     )
 
     custom_details: Optional[Dict[str, str]] = Field(
         default=None,
         description="Additional details to include as part of the payload.",
-        example='{"disk_space_left": "145GB"}',
+        examples=['{"disk_space_left": "145GB"}'],
     )
 
     def block_initialization(self) -> None:
         from apprise.plugins.NotifyPagerDuty import NotifyPagerDuty
 
         url = SecretStr(
             NotifyPagerDuty(
@@ -279,22 +279,22 @@
             "it can be found on the homepage of the Twilio console."
         ),
     )
 
     from_phone_number: str = Field(
         default=...,
         description="The valid Twilio phone number to send the message from.",
-        example="18001234567",
+        examples=["18001234567"],
     )
 
     to_phone_numbers: List[str] = Field(
         default=...,
         description="A list of valid Twilio phone number(s) to send the message to.",
         # not wrapped in brackets because of the way UI displays examples; in code should be ["18004242424"]
-        example="18004242424",
+        examples=["18004242424"],
     )
 
     def block_initialization(self) -> None:
         from apprise.plugins.NotifyTwilio import NotifyTwilio
 
         url = SecretStr(
             NotifyTwilio(
@@ -362,15 +362,15 @@
 
     tags: Optional[List] = Field(
         default=None,
         description=(
             "A comma-separated list of tags you can associate with your Opsgenie"
             " message."
         ),
-        example='["tag1", "tag2"]',
+        examples=['["tag1", "tag2"]'],
     )
 
     priority: Optional[str] = Field(
         default=3,
         description=(
             "The priority to associate with the message. It is on a scale between 1"
             " (LOW) and 5 (EMERGENCY)."
@@ -384,15 +384,15 @@
     entity: Optional[str] = Field(
         default=None, description="The entity to associate with the message."
     )
 
     details: Optional[Dict[str, str]] = Field(
         default=None,
         description="Additional details composed of key/values pairs.",
-        example='{"key1": "value1", "key2": "value2"}',
+        examples=['{"key1": "value1", "key2": "value2"}'],
     )
 
     def block_initialization(self) -> None:
         from apprise.plugins.NotifyOpsgenie import NotifyOpsgenie
 
         targets = []
         if self.target_user:
@@ -441,15 +441,15 @@
     _block_type_slug = "mattermost-webhook"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/1350a147130bf82cbc799a5f868d2c0116207736-250x250.png"
     _documentation_url = "https://docs.prefect.io/api-ref/prefect/blocks/notifications/#prefect.blocks.notifications.MattermostWebhook"
 
     hostname: str = Field(
         default=...,
         description="The hostname of your Mattermost server.",
-        example="Mattermost.example.com",
+        examples=["Mattermost.example.com"],
     )
 
     token: SecretStr = Field(
         default=...,
         description="The token associated with your Mattermost webhook.",
     )
 
@@ -613,57 +613,57 @@
     _documentation_url = "https://docs.prefect.io/api-ref/prefect/blocks/notifications/#prefect.blocks.notifications.CustomWebhookNotificationBlock"
 
     name: str = Field(title="Name", description="Name of the webhook.")
 
     url: str = Field(
         title="Webhook URL",
         description="The webhook URL.",
-        example="https://hooks.slack.com/XXX",
+        examples=["https://hooks.slack.com/XXX"],
     )
 
     method: Literal["GET", "POST", "PUT", "PATCH", "DELETE"] = Field(
         default="POST", description="The webhook request method. Defaults to `POST`."
     )
 
     params: Optional[Dict[str, str]] = Field(
         default=None, title="Query Params", description="Custom query params."
     )
     json_data: Optional[dict] = Field(
         default=None,
         title="JSON Data",
         description="Send json data as payload.",
-        example=(
+        examples=[
             '{"text": "{{subject}}\\n{{body}}", "title": "{{name}}", "token":'
             ' "{{tokenFromSecrets}}"}'
-        ),
+        ],
     )
     form_data: Optional[Dict[str, str]] = Field(
         default=None,
         title="Form Data",
         description=(
             "Send form data as payload. Should not be used together with _JSON Data_."
         ),
-        example=(
+        examples=[
             '{"text": "{{subject}}\\n{{body}}", "title": "{{name}}", "token":'
             ' "{{tokenFromSecrets}}"}'
-        ),
+        ],
     )
 
     headers: Optional[Dict[str, str]] = Field(None, description="Custom headers.")
     cookies: Optional[Dict[str, str]] = Field(None, description="Custom cookies.")
 
     timeout: float = Field(
         default=10, description="Request timeout in seconds. Defaults to 10."
     )
 
     secrets: SecretDict = Field(
         default_factory=lambda: SecretDict(dict()),
         title="Custom Secret Values",
         description="A dictionary of secret values to be substituted in other configs.",
-        example='{"tokenFromSecrets":"SomeSecretToken"}',
+        examples=['{"tokenFromSecrets":"SomeSecretToken"}'],
     )
 
     def _build_request_args(self, body: str, subject: Optional[str]):
         """Build kwargs for httpx.AsyncClient.request"""
         # prepare values
         values = self.secrets.get_secret_value()
         # use 'null' when subject is None
@@ -749,22 +749,22 @@
         title="API Key",
         description="The API Key associated with your sendgrid account.",
     )
 
     sender_email: str = Field(
         title="Sender email id",
         description="The sender email id.",
-        example="test-support@gmail.com",
+        examples=["test-support@gmail.com"],
     )
 
     to_emails: List[str] = Field(
         default=...,
         title="Recipient emails",
         description="Email ids of all recipients.",
-        example='"recipient1@gmail.com"',
+        examples=['"recipient1@gmail.com"'],
     )
 
     def block_initialization(self) -> None:
         from apprise.plugins.NotifySendGrid import NotifySendGrid
 
         url = SecretStr(
             NotifySendGrid(
```

### Comparing `prefect-client-2.16.9/src/prefect/blocks/system.py` & `prefect-client-2.17.0/src/prefect/blocks/system.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/blocks/webhook.py` & `prefect-client-2.17.0/src/prefect/blocks/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         default="POST", description="The webhook request method. Defaults to `POST`."
     )
 
     url: SecretStr = Field(
         default=...,
         title="Webhook URL",
         description="The webhook URL.",
-        example="https://hooks.slack.com/XXX",
+        examples=["https://hooks.slack.com/XXX"],
     )
 
     headers: SecretDict = Field(
         default_factory=lambda: SecretDict(dict()),
         title="Webhook Headers",
         description="A dictionary of headers to send with the webhook request.",
     )
```

### Comparing `prefect-client-2.16.9/src/prefect/client/base.py` & `prefect-client-2.17.0/src/prefect/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import anyio
 import httpx
 from asgi_lifespan import LifespanManager
 from httpx import HTTPStatusError, Request, Response
 from prefect._vendor.starlette import status
 from typing_extensions import Self
 
+import prefect
+from prefect.client import constants
 from prefect.client.schemas.objects import CsrfToken
 from prefect.exceptions import PrefectHTTPStatusError
 from prefect.logging import get_logger
 from prefect.settings import (
     PREFECT_CLIENT_MAX_RETRIES,
     PREFECT_CLIENT_RETRY_EXTRA_CODES,
     PREFECT_CLIENT_RETRY_JITTER_FACTOR,
@@ -195,14 +197,19 @@
         self.enable_csrf_support: bool = enable_csrf_support
         self.csrf_token: Optional[str] = None
         self.csrf_token_expiration: Optional[datetime] = None
         self.csrf_client_id: uuid.UUID = uuid.uuid4()
 
         super().__init__(*args, **kwargs)
 
+        user_agent = (
+            f"prefect/{prefect.__version__} (API {constants.SERVER_API_VERSION})"
+        )
+        self.headers["User-Agent"] = user_agent
+
     async def _send_with_retry(
         self,
         request: Request,
         send: Callable[[Request], Awaitable[Response]],
         send_args: Tuple,
         send_kwargs: Dict,
         retry_codes: Set[int] = set(),
```

### Comparing `prefect-client-2.16.9/src/prefect/client/cloud.py` & `prefect-client-2.17.0/src/prefect/client/cloud.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/client/collections.py` & `prefect-client-2.17.0/src/prefect/client/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/client/orchestration.py` & `prefect-client-2.17.0/src/prefect/client/orchestration.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 from uuid import UUID, uuid4
 
 import certifi
 import httpcore
 import httpx
 import pendulum
 
+from prefect._internal.compatibility.deprecated import (
+    handle_deprecated_infra_overrides_parameter,
+)
 from prefect._internal.compatibility.experimental import (
     EXPERIMENTAL_WARNING,
     ExperimentalFeature,
     experiment_enabled,
 )
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect.settings import (
@@ -64,14 +67,16 @@
     FlowRunNotificationPolicyUpdate,
     FlowRunUpdate,
     GlobalConcurrencyLimitCreate,
     GlobalConcurrencyLimitUpdate,
     LogCreate,
     TaskRunCreate,
     TaskRunUpdate,
+    VariableCreate,
+    VariableUpdate,
     WorkPoolCreate,
     WorkPoolUpdate,
     WorkQueueCreate,
     WorkQueueUpdate,
 )
 from prefect.client.schemas.filters import (
     ArtifactCollectionFilter,
@@ -1584,56 +1589,62 @@
         work_pool_name: str = None,
         tags: List[str] = None,
         storage_document_id: UUID = None,
         manifest_path: str = None,
         path: str = None,
         entrypoint: str = None,
         infrastructure_document_id: UUID = None,
-        infra_overrides: Optional[Dict[str, Any]] = None,
+        infra_overrides: Optional[Dict[str, Any]] = None,  # for backwards compat
         parameter_openapi_schema: Optional[Dict[str, Any]] = None,
         is_schedule_active: Optional[bool] = None,
         paused: Optional[bool] = None,
         pull_steps: Optional[List[dict]] = None,
         enforce_parameter_schema: Optional[bool] = None,
+        job_variables: Optional[Dict[str, Any]] = None,
     ) -> UUID:
         """
         Create a deployment.
 
         Args:
             flow_id: the flow ID to create a deployment for
             name: the name of the deployment
             version: an optional version string for the deployment
             schedule: an optional schedule to apply to the deployment
             tags: an optional list of tags to apply to the deployment
             storage_document_id: an reference to the storage block document
                 used for the deployed flow
             infrastructure_document_id: an reference to the infrastructure block document
                 to use for this deployment
+            job_variables: A dictionary of dot delimited infrastructure overrides that
+                will be applied at runtime; for example `env.CONFIG_KEY=config_value` or
+                `namespace='prefect'`. This argument was previously named `infra_overrides`.
+                Both arguments are supported for backwards compatibility.
 
         Raises:
             httpx.RequestError: if the deployment was not created for any reason
 
         Returns:
             the ID of the deployment in the backend
         """
+        jv = handle_deprecated_infra_overrides_parameter(job_variables, infra_overrides)
 
         deployment_create = DeploymentCreate(
             flow_id=flow_id,
             name=name,
             version=version,
             parameters=dict(parameters or {}),
             tags=list(tags or []),
             work_queue_name=work_queue_name,
             description=description,
             storage_document_id=storage_document_id,
             path=path,
             entrypoint=entrypoint,
             manifest_path=manifest_path,  # for backwards compat
             infrastructure_document_id=infrastructure_document_id,
-            infra_overrides=infra_overrides or {},
+            job_variables=jv,
             parameter_openapi_schema=parameter_openapi_schema,
             is_schedule_active=is_schedule_active,
             paused=paused,
             schedule=schedule,
             schedules=schedules or [],
             pull_steps=pull_steps,
             enforce_parameter_schema=enforce_parameter_schema,
@@ -1702,15 +1713,15 @@
             tags=deployment.tags,
             manifest_path=deployment.manifest_path,
             path=deployment.path,
             entrypoint=deployment.entrypoint,
             parameters=deployment.parameters,
             storage_document_id=deployment.storage_document_id,
             infrastructure_document_id=deployment.infrastructure_document_id,
-            infra_overrides=deployment.infra_overrides,
+            job_variables=deployment.job_variables,
             enforce_parameter_schema=deployment.enforce_parameter_schema,
         )
 
         if getattr(deployment, "work_pool_name", None) is not None:
             deployment_update.work_pool_name = deployment.work_pool_name
 
         exclude = set()
@@ -2922,19 +2933,48 @@
             await self._client.delete(f"/artifacts/{artifact_id}")
         except httpx.HTTPStatusError as e:
             if e.response.status_code == 404:
                 raise prefect.exceptions.ObjectNotFound(http_exc=e) from e
             else:
                 raise
 
+    async def create_variable(self, variable: VariableCreate) -> Variable:
+        """
+        Creates an variable with the provided configuration.
+
+        Args:
+            variable: Desired configuration for the new variable.
+        Returns:
+            Information about the newly created variable.
+        """
+        response = await self._client.post(
+            "/variables/",
+            json=variable.dict(json_compatible=True, exclude_unset=True),
+        )
+        return Variable(**response.json())
+
+    async def update_variable(self, variable: VariableUpdate) -> None:
+        """
+        Updates a variable with the provided configuration.
+
+        Args:
+            variable: Desired configuration for the updated variable.
+        Returns:
+            Information about the updated variable.
+        """
+        await self._client.patch(
+            f"/variables/name/{variable.name}",
+            json=variable.dict(json_compatible=True, exclude_unset=True),
+        )
+
     async def read_variable_by_name(self, name: str) -> Optional[Variable]:
         """Reads a variable by name. Returns None if no variable is found."""
         try:
             response = await self._client.get(f"/variables/name/{name}")
-            return pydantic.parse_obj_as(Variable, response.json())
+            return Variable(**response.json())
         except httpx.HTTPStatusError as e:
             if e.response.status_code == status.HTTP_404_NOT_FOUND:
                 return None
             else:
                 raise
 
     async def delete_variable_by_name(self, name: str):
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/__init__.py` & `prefect-client-2.17.0/src/prefect/client/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/actions.py` & `prefect-client-2.17.0/src/prefect/client/schemas/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, TypeVar, Union
 from uuid import UUID, uuid4
 
 import jsonschema
 
+from prefect._internal.compatibility.deprecated import DeprecatedInfraOverridesField
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, conint, root_validator, validator
 else:
     from pydantic import Field, conint, root_validator, validator
 
@@ -58,41 +59,41 @@
 
 
 class StateCreate(ActionBaseModel):
     """Data used by the Prefect REST API to create a new state."""
 
     type: StateType
     name: Optional[str] = Field(default=None)
-    message: Optional[str] = Field(default=None, example="Run started")
+    message: Optional[str] = Field(default=None, examples=["Run started"])
     state_details: StateDetails = Field(default_factory=StateDetails)
     data: Union["BaseResult[R]", "DataDocument[R]", Any] = Field(
         default=None,
     )
 
 
 class FlowCreate(ActionBaseModel):
     """Data used by the Prefect REST API to create a flow."""
 
     name: str = Field(
-        default=..., description="The name of the flow", example="my-flow"
+        default=..., description="The name of the flow", examples=["my-flow"]
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of flow tags",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
 
 
 class FlowUpdate(ActionBaseModel):
     """Data used by the Prefect REST API to update a flow."""
 
     tags: List[str] = Field(
         default_factory=list,
         description="A list of flow tags",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
 
 
 class DeploymentScheduleCreate(ActionBaseModel):
     schedule: SCHEDULE_TYPES = Field(
         default=..., description="The schedule for the deployment."
     )
@@ -106,15 +107,15 @@
         default=None, description="The schedule for the deployment."
     )
     active: bool = Field(
         default=True, description="Whether or not the schedule is active."
     )
 
 
-class DeploymentCreate(ActionBaseModel):
+class DeploymentCreate(DeprecatedInfraOverridesField, ActionBaseModel):
     """Data used by the Prefect REST API to create a deployment."""
 
     @root_validator(pre=True)
     def remove_old_fields(cls, values):
         return remove_old_deployment_fields(values)
 
     name: str = Field(..., description="The name of the deployment.")
@@ -140,46 +141,49 @@
     pull_steps: Optional[List[dict]] = Field(None)
 
     manifest_path: Optional[str] = Field(None)
     work_queue_name: Optional[str] = Field(None)
     work_pool_name: Optional[str] = Field(
         default=None,
         description="The name of the deployment's work pool.",
-        example="my-work-pool",
+        examples=["my-work-pool"],
     )
     storage_document_id: Optional[UUID] = Field(None)
     infrastructure_document_id: Optional[UUID] = Field(None)
     schedule: Optional[SCHEDULE_TYPES] = Field(None)
     description: Optional[str] = Field(None)
     path: Optional[str] = Field(None)
     version: Optional[str] = Field(None)
     entrypoint: Optional[str] = Field(None)
-    infra_overrides: Optional[Dict[str, Any]] = Field(None)
+    job_variables: Optional[Dict[str, Any]] = Field(
+        default_factory=dict,
+        description="Overrides to apply to flow run infrastructure at runtime.",
+    )
 
     def check_valid_configuration(self, base_job_template: dict):
         """Check that the combination of base_job_template defaults
-        and infra_overrides conforms to the specified schema.
+        and job_variables conforms to the specified schema.
         """
         variables_schema = deepcopy(base_job_template.get("variables"))
 
         if variables_schema is not None:
             # jsonschema considers required fields, even if that field has a default,
             # to still be required. To get around this we remove the fields from
             # required if there is a default present.
             required = variables_schema.get("required")
             properties = variables_schema.get("properties")
             if required is not None and properties is not None:
                 for k, v in properties.items():
                     if "default" in v and k in required:
                         required.remove(k)
 
-            jsonschema.validate(self.infra_overrides, variables_schema)
+            jsonschema.validate(self.job_variables, variables_schema)
 
 
-class DeploymentUpdate(ActionBaseModel):
+class DeploymentUpdate(DeprecatedInfraOverridesField, ActionBaseModel):
     """Data used by the Prefect REST API to update a deployment."""
 
     @root_validator(pre=True)
     def remove_old_fields(cls, values):
         return remove_old_deployment_fields(values)
 
     @validator("schedule")
@@ -195,32 +199,35 @@
         description="Parameters for flow runs scheduled by the deployment.",
     )
     tags: List[str] = Field(default_factory=list)
     work_queue_name: Optional[str] = Field(None)
     work_pool_name: Optional[str] = Field(
         default=None,
         description="The name of the deployment's work pool.",
-        example="my-work-pool",
+        examples=["my-work-pool"],
     )
     path: Optional[str] = Field(None)
-    infra_overrides: Optional[Dict[str, Any]] = Field(None)
+    job_variables: Optional[Dict[str, Any]] = Field(
+        default_factory=dict,
+        description="Overrides to apply to flow run infrastructure at runtime.",
+    )
     entrypoint: Optional[str] = Field(None)
     manifest_path: Optional[str] = Field(None)
     storage_document_id: Optional[UUID] = Field(None)
     infrastructure_document_id: Optional[UUID] = Field(None)
     enforce_parameter_schema: Optional[bool] = Field(
         default=None,
         description=(
             "Whether or not the deployment should enforce the parameter schema."
         ),
     )
 
     def check_valid_configuration(self, base_job_template: dict):
         """Check that the combination of base_job_template defaults
-        and infra_overrides conforms to the specified schema.
+        and job_variables conforms to the specified schema.
         """
         variables_schema = deepcopy(base_job_template.get("variables"))
 
         if variables_schema is not None:
             # jsonschema considers required fields, even if that field has a default,
             # to still be required. To get around this we remove the fields from
             # required if there is a default present.
@@ -228,15 +235,15 @@
             properties = variables_schema.get("properties")
             if required is not None and properties is not None:
                 for k, v in properties.items():
                     if "default" in v and k in required:
                         required.remove(k)
 
         if variables_schema is not None:
-            jsonschema.validate(self.infra_overrides, variables_schema)
+            jsonschema.validate(self.job_variables, variables_schema)
 
 
 class FlowRunUpdate(ActionBaseModel):
     """Data used by the Prefect REST API to update a flow run."""
 
     name: Optional[str] = Field(None)
     flow_version: Optional[str] = Field(None)
@@ -601,18 +608,18 @@
     message_template: Optional[str] = Field(
         default=None,
         description=(
             "A templatable notification message. Use {braces} to add variables."
             " Valid variables include:"
             f" {listrepr(sorted(objects.FLOW_RUN_NOTIFICATION_TEMPLATE_KWARGS), sep=', ')}"
         ),
-        example=(
+        examples=[
             "Flow run {flow_run_name} with id {flow_run_id} entered state"
             " {flow_run_state_name}."
-        ),
+        ],
     )
 
     @validator("message_template")
     def validate_message_template_variables(cls, v):
         return validate_message_template_variables(v)
 
 
@@ -652,42 +659,42 @@
 
 class VariableCreate(ActionBaseModel):
     """Data used by the Prefect REST API to create a Variable."""
 
     name: str = Field(
         default=...,
         description="The name of the variable",
-        example="my_variable",
+        examples=["my_variable"],
         max_length=objects.MAX_VARIABLE_NAME_LENGTH,
     )
     value: str = Field(
         default=...,
         description="The value of the variable",
-        example="my-value",
+        examples=["my-value"],
         max_length=objects.MAX_VARIABLE_VALUE_LENGTH,
     )
     tags: Optional[List[str]] = Field(default=None)
 
     # validators
     _validate_name_format = validator("name", allow_reuse=True)(validate_variable_name)
 
 
 class VariableUpdate(ActionBaseModel):
     """Data used by the Prefect REST API to update a Variable."""
 
     name: Optional[str] = Field(
         default=None,
         description="The name of the variable",
-        example="my_variable",
+        examples=["my_variable"],
         max_length=objects.MAX_VARIABLE_NAME_LENGTH,
     )
     value: Optional[str] = Field(
         default=None,
         description="The value of the variable",
-        example="my-value",
+        examples=["my-value"],
         max_length=objects.MAX_VARIABLE_NAME_LENGTH,
     )
     tags: Optional[List[str]] = Field(default=None)
 
     # validators
     _validate_name_format = validator("name", allow_reuse=True)(validate_variable_name)
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/filters.py` & `prefect-client-2.17.0/src/prefect/client/schemas/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,34 +44,34 @@
 
 class FlowFilterName(PrefectBaseModel):
     """Filter by `Flow.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of flow names to include",
-        example=["my-flow-1", "my-flow-2"],
+        examples=[["my-flow-1", "my-flow-2"]],
     )
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A case-insensitive partial match. For example, "
             " passing 'marvin' will match "
             "'marvin', 'sad-Marvin', and 'marvin-robot'."
         ),
-        example="marvin",
+        examples=["marvin"],
     )
 
 
 class FlowFilterTags(PrefectBaseModel, OperatorMixin):
     """Filter by `Flow.tags`."""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
         description=(
             "A list of tags. Flows will be returned only if their tags are a superset"
             " of the list"
         ),
     )
     is_null_: Optional[bool] = Field(
         default=None, description="If true, only include flows without tags"
@@ -105,34 +105,34 @@
 
 class FlowRunFilterName(PrefectBaseModel):
     """Filter by `FlowRun.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of flow run names to include",
-        example=["my-flow-run-1", "my-flow-run-2"],
+        examples=[["my-flow-run-1", "my-flow-run-2"]],
     )
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A case-insensitive partial match. For example, "
             " passing 'marvin' will match "
             "'marvin', 'sad-Marvin', and 'marvin-robot'."
         ),
-        example="marvin",
+        examples=["marvin"],
     )
 
 
 class FlowRunFilterTags(PrefectBaseModel, OperatorMixin):
     """Filter by `FlowRun.tags`."""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
         description=(
             "A list of tags. Flow runs will be returned only if their tags are a"
             " superset of the list"
         ),
     )
     is_null_: Optional[bool] = Field(
         default=None, description="If true, only include flow runs without tags"
@@ -153,15 +153,15 @@
 
 class FlowRunFilterWorkQueueName(PrefectBaseModel, OperatorMixin):
     """Filter by `FlowRun.work_queue_name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of work queue names to include",
-        example=["work_queue_1", "work_queue_2"],
+        examples=[["work_queue_1", "work_queue_2"]],
     )
     is_null_: Optional[bool] = Field(
         default=None,
         description="If true, only include flow runs without work queue names",
     )
 
 
@@ -339,34 +339,34 @@
 
 class TaskRunFilterName(PrefectBaseModel):
     """Filter by `TaskRun.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of task run names to include",
-        example=["my-task-run-1", "my-task-run-2"],
+        examples=[["my-task-run-1", "my-task-run-2"]],
     )
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A case-insensitive partial match. For example, "
             " passing 'marvin' will match "
             "'marvin', 'sad-Marvin', and 'marvin-robot'."
         ),
-        example="marvin",
+        examples=["marvin"],
     )
 
 
 class TaskRunFilterTags(PrefectBaseModel, OperatorMixin):
     """Filter by `TaskRun.tags`."""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
         description=(
             "A list of tags. Task runs will be returned only if their tags are a"
             " superset of the list"
         ),
     )
     is_null_: Optional[bool] = Field(
         default=None, description="If true, only include task runs without tags"
@@ -456,35 +456,35 @@
 
 class DeploymentFilterName(PrefectBaseModel):
     """Filter by `Deployment.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of deployment names to include",
-        example=["my-deployment-1", "my-deployment-2"],
+        examples=[["my-deployment-1", "my-deployment-2"]],
     )
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A case-insensitive partial match. For example, "
             " passing 'marvin' will match "
             "'marvin', 'sad-Marvin', and 'marvin-robot'."
         ),
-        example="marvin",
+        examples=["marvin"],
     )
 
 
 class DeploymentFilterWorkQueueName(PrefectBaseModel):
     """Filter by `Deployment.work_queue_name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of work queue names to include",
-        example=["work_queue_1", "work_queue_2"],
+        examples=[["work_queue_1", "work_queue_2"]],
     )
 
 
 class DeploymentFilterIsScheduleActive(PrefectBaseModel):
     """Filter by `Deployment.is_schedule_active`."""
 
     eq_: Optional[bool] = Field(
@@ -494,15 +494,15 @@
 
 
 class DeploymentFilterTags(PrefectBaseModel, OperatorMixin):
     """Filter by `Deployment.tags`."""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
         description=(
             "A list of tags. Deployments will be returned only if their tags are a"
             " superset of the list"
         ),
     )
     is_null_: Optional[bool] = Field(
         default=None, description="If true, only include deployments without tags"
@@ -531,31 +531,31 @@
 
 class LogFilterName(PrefectBaseModel):
     """Filter by `Log.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of log names to include",
-        example=["prefect.logger.flow_runs", "prefect.logger.task_runs"],
+        examples=[["prefect.logger.flow_runs", "prefect.logger.task_runs"]],
     )
 
 
 class LogFilterLevel(PrefectBaseModel):
     """Filter by `Log.level`."""
 
     ge_: Optional[int] = Field(
         default=None,
         description="Include logs with a level greater than or equal to this level",
-        example=20,
+        examples=[20],
     )
 
     le_: Optional[int] = Field(
         default=None,
         description="Include logs with a level less than or equal to this level",
-        example=50,
+        examples=[50],
     )
 
 
 class LogFilterTimestamp(PrefectBaseModel):
     """Filter by `Log.timestamp`."""
 
     before_: Optional[DateTimeTZ] = Field(
@@ -625,15 +625,15 @@
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A case-insensitive partial match. For example, "
             " passing 'marvin' will match "
             "'marvin', 'sad-Marvin', and 'marvin-robot'."
         ),
-        example="marvin",
+        examples=["marvin"],
     )
 
 
 class BlockTypeFilterSlug(PrefectBaseModel):
     """Filter by `BlockType.slug`"""
 
     any_: Optional[List[str]] = Field(
@@ -670,28 +670,28 @@
 
 
 class BlockSchemaFilterCapabilities(PrefectBaseModel):
     """Filter by `BlockSchema.capabilities`"""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["write-storage", "read-storage"],
+        examples=[["write-storage", "read-storage"]],
         description=(
             "A list of block capabilities. Block entities will be returned only if an"
             " associated block schema has a superset of the defined capabilities."
         ),
     )
 
 
 class BlockSchemaFilterVersion(PrefectBaseModel):
     """Filter by `BlockSchema.capabilities`"""
 
     any_: Optional[List[str]] = Field(
         default=None,
-        example=["2.0.0", "2.1.0"],
+        examples=[["2.0.0", "2.1.0"]],
         description="A list of block schema versions.",
     )
 
 
 class BlockSchemaFilter(PrefectBaseModel, OperatorMixin):
     """Filter BlockSchemas"""
 
@@ -744,15 +744,15 @@
     )
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A string to match block names against. This can include "
             "SQL wildcard characters like `%` and `_`."
         ),
-        example="my-block%",
+        examples=["my-block%"],
     )
 
 
 class BlockDocumentFilter(PrefectBaseModel, OperatorMixin):
     """Filter BlockDocuments. Only BlockDocuments matching all criteria will be returned"""
 
     id: Optional[BlockDocumentFilterId] = Field(
@@ -805,25 +805,25 @@
 
 class WorkQueueFilterName(PrefectBaseModel):
     """Filter by `WorkQueue.name`."""
 
     any_: Optional[List[str]] = Field(
         default=None,
         description="A list of work queue names to include",
-        example=["wq-1", "wq-2"],
+        examples=[["wq-1", "wq-2"]],
     )
 
     startswith_: Optional[List[str]] = Field(
         default=None,
         description=(
             "A list of case-insensitive starts-with matches. For example, "
             " passing 'marvin' will match "
             "'marvin', and 'Marvin-robot', but not 'sad-marvin'."
         ),
-        example=["marvin", "Marvin-robot"],
+        examples=[["marvin", "Marvin-robot"]],
     )
 
 
 class WorkQueueFilter(PrefectBaseModel, OperatorMixin):
     """Filter work queues. Only work queues matching all criteria will be
     returned"""
 
@@ -925,15 +925,15 @@
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A string to match artifact keys against. This can include "
             "SQL wildcard characters like `%` and `_`."
         ),
-        example="my-artifact-%",
+        examples=["my-artifact-%"],
     )
 
     exists_: Optional[bool] = Field(
         default=None,
         description=(
             "If `true`, only include artifacts with a non-null key. If `false`, "
             "only include artifacts with a null key."
@@ -1005,15 +1005,15 @@
 
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A string to match artifact keys against. This can include "
             "SQL wildcard characters like `%` and `_`."
         ),
-        example="my-artifact-%",
+        examples=["my-artifact-%"],
     )
 
     exists_: Optional[bool] = Field(
         default=None,
         description=(
             "If `true`, only include artifacts with a non-null key. If `false`, "
             "only include artifacts with a null key. Should return all rows in "
@@ -1085,15 +1085,15 @@
     )
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A string to match variable names against. This can include "
             "SQL wildcard characters like `%` and `_`."
         ),
-        example="my_variable_%",
+        examples=["my_variable_%"],
     )
 
 
 class VariableFilterValue(PrefectBaseModel):
     """Filter by `Variable.value`."""
 
     any_: Optional[List[str]] = Field(
@@ -1101,24 +1101,24 @@
     )
     like_: Optional[str] = Field(
         default=None,
         description=(
             "A string to match variable value against. This can include "
             "SQL wildcard characters like `%` and `_`."
         ),
-        example="my-value-%",
+        examples=["my-value-%"],
     )
 
 
 class VariableFilterTags(PrefectBaseModel, OperatorMixin):
     """Filter by `Variable.tags`."""
 
     all_: Optional[List[str]] = Field(
         default=None,
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
         description=(
             "A list of tags. Variables will be returned only if their tags are a"
             " superset of the list"
         ),
     )
     is_null_: Optional[bool] = Field(
         default=None, description="If true, only include Variables without tags"
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/objects.py` & `prefect-client-2.17.0/src/prefect/client/schemas/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     overload,
 )
 from uuid import UUID
 
 import orjson
 import pendulum
 
+from prefect._internal.compatibility.deprecated import (
+    DeprecatedInfraOverridesField,
+)
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, HttpUrl, conint, root_validator, validator
 else:
     from pydantic import Field, HttpUrl, conint, root_validator, validator
 
@@ -138,15 +141,15 @@
     """
     The state of a run.
     """
 
     type: StateType
     name: Optional[str] = Field(default=None)
     timestamp: DateTimeTZ = Field(default_factory=lambda: pendulum.now("UTC"))
-    message: Optional[str] = Field(default=None, example="Run started")
+    message: Optional[str] = Field(default=None, examples=["Run started"])
     state_details: StateDetails = Field(default_factory=StateDetails)
     data: Union["BaseResult[R]", "DataDocument[R]", Any] = Field(
         default=None,
     )
 
     @overload
     def result(self: "State[R]", raise_on_failure: bool = True) -> R:
@@ -406,56 +409,61 @@
 
 class FlowRun(ObjectBaseModel):
     name: str = Field(
         default_factory=lambda: generate_slug(2),
         description=(
             "The name of the flow run. Defaults to a random slug if not specified."
         ),
-        example="my-flow-run",
+        examples=["my-flow-run"],
     )
     flow_id: UUID = Field(default=..., description="The id of the flow being run.")
     state_id: Optional[UUID] = Field(
         default=None, description="The id of the flow run's current state."
     )
     deployment_id: Optional[UUID] = Field(
         default=None,
         description=(
             "The id of the deployment associated with this flow run, if available."
         ),
     )
+    deployment_version: Optional[str] = Field(
+        default=None,
+        description="The version of the deployment associated with this flow run.",
+        examples=["1.0"],
+    )
     work_queue_name: Optional[str] = Field(
         default=None, description="The work queue that handled this flow run."
     )
     flow_version: Optional[str] = Field(
         default=None,
         description="The version of the flow executed in this flow run.",
-        example="1.0",
+        examples=["1.0"],
     )
     parameters: Dict[str, Any] = Field(
         default_factory=dict, description="Parameters for the flow run."
     )
     idempotency_key: Optional[str] = Field(
         default=None,
         description=(
             "An optional idempotency key for the flow run. Used to ensure the same flow"
             " run is not created multiple times."
         ),
     )
     context: Dict[str, Any] = Field(
         default_factory=dict,
         description="Additional context for the flow run.",
-        example={"my_var": "my_val"},
+        examples=[{"my_var": "my_val"}],
     )
     empirical_policy: FlowRunPolicy = Field(
         default_factory=FlowRunPolicy,
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of tags on the flow run",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
     parent_task_run_id: Optional[UUID] = Field(
         default=None,
         description=(
             "If the flow run is a subflow, the id of the 'dummy' task in the parent"
             " flow used to track subflow state."
         ),
@@ -514,20 +522,20 @@
 
     work_pool_id: Optional[UUID] = Field(
         description="The work pool with which the queue is associated."
     )
     work_pool_name: Optional[str] = Field(
         default=None,
         description="The name of the flow run's work pool.",
-        example="my-work-pool",
+        examples=["my-work-pool"],
     )
     state: Optional[State] = Field(
         default=None,
         description="The state of the flow run.",
-        example=State(type=StateType.COMPLETED),
+        examples=[State(type=StateType.COMPLETED)],
     )
     job_variables: Optional[dict] = Field(
         default=None, description="Job variables for the flow run."
     )
 
     # These are server-side optimizations and should not be present on client models
     # TODO: Deprecate these fields
@@ -630,15 +638,17 @@
     """Represents constant input value to a task run."""
 
     input_type: Literal["constant"] = "constant"
     type: str
 
 
 class TaskRun(ObjectBaseModel):
-    name: str = Field(default_factory=lambda: generate_slug(2), example="my-task-run")
+    name: str = Field(
+        default_factory=lambda: generate_slug(2), examples=["my-task-run"]
+    )
     flow_run_id: Optional[UUID] = Field(
         default=None, description="The flow run id of the task run."
     )
     task_key: str = Field(
         default=..., description="A unique identifier for the task being run."
     )
     dynamic_key: str = Field(
@@ -664,15 +674,15 @@
     )
     empirical_policy: TaskRunPolicy = Field(
         default_factory=TaskRunPolicy,
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of tags for the task run.",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
     state_id: Optional[UUID] = Field(
         default=None, description="The id of the current task run state."
     )
     task_inputs: Dict[str, List[Union[TaskRunResult, Parameter, Constant]]] = Field(
         default_factory=dict,
         description=(
@@ -727,15 +737,15 @@
         default=datetime.timedelta(0),
         description="The difference between actual and expected start time.",
     )
 
     state: Optional[State] = Field(
         default=None,
         description="The state of the flow run.",
-        example=State(type=StateType.COMPLETED),
+        examples=[State(type=StateType.COMPLETED)],
     )
 
     @validator("name", pre=True)
     def set_default_name(cls, name):
         return get_or_create_run_name(name)
 
 
@@ -880,20 +890,20 @@
         return validate_name_present_on_nonanonymous_blocks(values)
 
 
 class Flow(ObjectBaseModel):
     """An ORM representation of flow data."""
 
     name: str = Field(
-        default=..., description="The name of the flow", example="my-flow"
+        default=..., description="The name of the flow", examples=["my-flow"]
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of flow tags",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
 
     @validator("name", check_fields=False)
     def validate_name_characters(cls, v):
         return raise_on_name_with_banned_characters(v)
 
 
@@ -915,15 +925,15 @@
         default=..., description="The schedule for the deployment."
     )
     active: bool = Field(
         default=True, description="Whether or not the schedule is active."
     )
 
 
-class Deployment(ObjectBaseModel):
+class Deployment(DeprecatedInfraOverridesField, ObjectBaseModel):
     """An ORM representation of deployment data."""
 
     name: str = Field(default=..., description="The name of the deployment.")
     version: Optional[str] = Field(
         default=None, description="An optional version for the deployment."
     )
     description: Optional[str] = Field(
@@ -940,30 +950,30 @@
     )
     paused: bool = Field(
         default=False, description="Whether or not the deployment is paused."
     )
     schedules: List[DeploymentSchedule] = Field(
         default_factory=list, description="A list of schedules for the deployment."
     )
-    infra_overrides: Dict[str, Any] = Field(
+    job_variables: Dict[str, Any] = Field(
         default_factory=dict,
-        description="Overrides to apply to the base infrastructure block at runtime.",
+        description="Overrides to apply to flow run infrastructure at runtime.",
     )
     parameters: Dict[str, Any] = Field(
         default_factory=dict,
         description="Parameters for flow runs scheduled by the deployment.",
     )
     pull_steps: Optional[List[dict]] = Field(
         default=None,
         description="Pull steps for cloning and running this deployment.",
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of tags for the deployment",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
     work_queue_name: Optional[str] = Field(
         default=None,
         description=(
             "The work queue for the deployment. If no work queue is set, work will not"
             " be scheduled."
         ),
@@ -1291,18 +1301,18 @@
     message_template: Optional[str] = Field(
         default=None,
         description=(
             "A templatable notification message. Use {braces} to add variables."
             " Valid variables include:"
             f" {listrepr(sorted(FLOW_RUN_NOTIFICATION_TEMPLATE_KWARGS), sep=', ')}"
         ),
-        example=(
+        examples=[
             "Flow run {flow_run_name} with id {flow_run_id} entered state"
             " {flow_run_state_name}."
-        ),
+        ],
     )
 
     @validator("message_template")
     def validate_message_template_variables(cls, v):
         return validate_message_template_variables(v)
 
 
@@ -1475,27 +1485,27 @@
     )
 
 
 class Variable(ObjectBaseModel):
     name: str = Field(
         default=...,
         description="The name of the variable",
-        example="my_variable",
+        examples=["my_variable"],
         max_length=MAX_VARIABLE_NAME_LENGTH,
     )
     value: str = Field(
         default=...,
         description="The value of the variable",
-        example="my-value",
+        examples=["my_value"],
         max_length=MAX_VARIABLE_VALUE_LENGTH,
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of variable tags",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
 
 
 class FlowRunInput(ObjectBaseModel):
     flow_run_id: UUID = Field(description="The flow run ID associated with the input.")
     key: str = Field(description="The key of the input.")
     value: str = Field(description="The value of the input.")
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/responses.py` & `prefect-client-2.17.0/src/prefect/client/schemas/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 from typing import Any, Dict, List, Optional, TypeVar, Union
 from uuid import UUID
 
+from prefect._internal.compatibility.deprecated import DeprecatedInfraOverridesField
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
@@ -156,56 +157,61 @@
 
 class FlowRunResponse(ObjectBaseModel):
     name: str = Field(
         default_factory=lambda: generate_slug(2),
         description=(
             "The name of the flow run. Defaults to a random slug if not specified."
         ),
-        example="my-flow-run",
+        examples=["my-flow-run"],
     )
     flow_id: UUID = Field(default=..., description="The id of the flow being run.")
     state_id: Optional[UUID] = Field(
         default=None, description="The id of the flow run's current state."
     )
     deployment_id: Optional[UUID] = Field(
         default=None,
         description=(
             "The id of the deployment associated with this flow run, if available."
         ),
     )
+    deployment_version: Optional[str] = Field(
+        default=None,
+        description="The version of the deployment associated with this flow run.",
+        examples=["1.0"],
+    )
     work_queue_name: Optional[str] = Field(
         default=None, description="The work queue that handled this flow run."
     )
     flow_version: Optional[str] = Field(
         default=None,
         description="The version of the flow executed in this flow run.",
-        example="1.0",
+        examples=["1.0"],
     )
     parameters: Dict[str, Any] = Field(
         default_factory=dict, description="Parameters for the flow run."
     )
     idempotency_key: Optional[str] = Field(
         default=None,
         description=(
             "An optional idempotency key for the flow run. Used to ensure the same flow"
             " run is not created multiple times."
         ),
     )
     context: Dict[str, Any] = Field(
         default_factory=dict,
         description="Additional context for the flow run.",
-        example={"my_var": "my_val"},
+        examples=[{"my_var": "my_val"}],
     )
     empirical_policy: objects.FlowRunPolicy = Field(
         default_factory=objects.FlowRunPolicy,
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of tags on the flow run",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
     parent_task_run_id: Optional[UUID] = Field(
         default=None,
         description=(
             "If the flow run is a subflow, the id of the 'dummy' task in the parent"
             " flow used to track subflow state."
         ),
@@ -264,20 +270,20 @@
 
     work_pool_id: Optional[UUID] = Field(
         description="The work pool with which the queue is associated."
     )
     work_pool_name: Optional[str] = Field(
         default=None,
         description="The name of the flow run's work pool.",
-        example="my-work-pool",
+        examples=["my-work-pool"],
     )
     state: Optional[objects.State] = Field(
         default=None,
         description="The state of the flow run.",
-        example=objects.State(type=objects.StateType.COMPLETED),
+        examples=[objects.State(type=objects.StateType.COMPLETED)],
     )
     job_variables: Optional[dict] = Field(
         default=None, description="Job variables for the flow run."
     )
 
     # These are server-side optimizations and should not be present on client models
     # TODO: Deprecate these fields
@@ -300,15 +306,15 @@
             exclude_fields = {"estimated_run_time", "estimated_start_time_delta"}
             return self.dict(exclude=exclude_fields) == other.dict(
                 exclude=exclude_fields
             )
         return super().__eq__(other)
 
 
-class DeploymentResponse(ObjectBaseModel):
+class DeploymentResponse(DeprecatedInfraOverridesField, ObjectBaseModel):
     name: str = Field(default=..., description="The name of the deployment.")
     version: Optional[str] = Field(
         default=None, description="An optional version for the deployment."
     )
     description: Optional[str] = Field(
         default=None, description="A description for the deployment."
     )
@@ -323,30 +329,30 @@
     )
     paused: bool = Field(
         default=False, description="Whether or not the deployment is paused."
     )
     schedules: List[objects.DeploymentSchedule] = Field(
         default_factory=list, description="A list of schedules for the deployment."
     )
-    infra_overrides: Dict[str, Any] = Field(
+    job_variables: Dict[str, Any] = Field(
         default_factory=dict,
-        description="Overrides to apply to the base infrastructure block at runtime.",
+        description="Overrides to apply to flow run infrastructure at runtime.",
     )
     parameters: Dict[str, Any] = Field(
         default_factory=dict,
         description="Parameters for flow runs scheduled by the deployment.",
     )
     pull_steps: Optional[List[dict]] = Field(
         default=None,
         description="Pull steps for cloning and running this deployment.",
     )
     tags: List[str] = Field(
         default_factory=list,
         description="A list of tags for the deployment",
-        example=["tag-1", "tag-2"],
+        examples=[["tag-1", "tag-2"]],
     )
     work_queue_name: Optional[str] = Field(
         default=None,
         description=(
             "The work queue for the deployment. If no work queue is set, work will not"
             " be scheduled."
         ),
@@ -414,12 +420,12 @@
         default=None,
         description="Current status of the deployment.",
     )
 
 
 class MinimalConcurrencyLimitResponse(PrefectBaseModel):
     class Config:
-        extra = "ignore"
+        extra = "ignore"  # 2024/4/1
 
     id: UUID
     name: str
     limit: int
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/schedules.py` & `prefect-client-2.17.0/src/prefect/client/schemas/schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 from typing import Optional, Union
 
 import dateutil
 import dateutil.rrule
 import pendulum
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
+from prefect._internal.schemas.bases import PrefectBaseModel
+from prefect._internal.schemas.fields import DateTimeTZ
 from prefect._internal.schemas.validators import (
     default_anchor_date,
     default_timezone,
     interval_schedule_must_be_positive,
     validate_cron_string,
     validate_rrule_string,
     validate_rrule_timezone,
 )
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
-
-from prefect._internal.schemas.bases import PrefectBaseModel
-from prefect._internal.schemas.fields import DateTimeTZ
-
 MAX_ITERATIONS = 1000
 # approx. 1 years worth of RDATEs + buffer
 MAX_RRULE_LENGTH = 6500
 
 
 class IntervalSchedule(PrefectBaseModel):
     """
@@ -64,15 +62,15 @@
 
     class Config:
         extra = "forbid"
         exclude_none = True
 
     interval: datetime.timedelta
     anchor_date: DateTimeTZ = None
-    timezone: Optional[str] = Field(default=None, example="America/New_York")
+    timezone: Optional[str] = Field(default=None, examples=["America/New_York"])
 
     @validator("interval")
     def validate_interval_schedule(cls, v):
         return interval_schedule_must_be_positive(v)
 
     @validator("anchor_date", always=True)
     def validate_anchor_date(cls, v):
@@ -107,16 +105,16 @@
             2nd friday of a month by setting the days of month and the weekday.
 
     """
 
     class Config:
         extra = "forbid"
 
-    cron: str = Field(default=..., example="0 0 * * *")
-    timezone: Optional[str] = Field(default=None, example="America/New_York")
+    cron: str = Field(default=..., examples=["0 0 * * *"])
+    timezone: Optional[str] = Field(default=None, examples=["America/New_York"])
     day_or: bool = Field(
         default=True,
         description=(
             "Control croniter behavior for handling day and day_of_week entries."
         ),
     )
 
@@ -152,15 +150,15 @@
         timezone (str, optional): a valid timezone string
     """
 
     class Config:
         extra = "forbid"
 
     rrule: str
-    timezone: Optional[str] = Field(default=None, example="America/New_York")
+    timezone: Optional[str] = Field(default=None, examples=["America/New_York"])
 
     @validator("rrule")
     def validate_rrule_str(cls, v):
         return validate_rrule_string(v)
 
     @classmethod
     def from_rrule(cls, rrule: dateutil.rrule.rrule):
```

### Comparing `prefect-client-2.16.9/src/prefect/client/schemas/sorting.py` & `prefect-client-2.17.0/src/prefect/client/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/client/subscriptions.py` & `prefect-client-2.17.0/src/prefect/client/subscriptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/client/utilities.py` & `prefect-client-2.17.0/src/prefect/client/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/concurrency/asyncio.py` & `prefect-client-2.17.0/src/prefect/concurrency/asyncio.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/concurrency/events.py` & `prefect-client-2.17.0/src/prefect/concurrency/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/concurrency/services.py` & `prefect-client-2.17.0/src/prefect/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/concurrency/sync.py` & `prefect-client-2.17.0/src/prefect/concurrency/sync.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/context.py` & `prefect-client-2.17.0/src/prefect/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from functools import update_wrapper
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     ContextManager,
     Dict,
+    Generator,
     List,
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -391,15 +392,15 @@
     if not settings_ctx:
         raise MissingContextError("No settings context found.")
 
     return settings_ctx
 
 
 @contextmanager
-def tags(*new_tags: str) -> Set[str]:
+def tags(*new_tags: str) -> Generator[Set[str], None, None]:
     """
     Context manager to add tags to flow and task run calls.
 
     Tags are always combined with any existing tags.
 
     Yields:
         The current set of tags
```

### Comparing `prefect-client-2.16.9/src/prefect/deployments/base.py` & `prefect-client-2.17.0/src/prefect/deployments/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,14 @@
 import sys
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, List, Optional, cast
 
 import anyio
 import yaml
-
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    from pydantic.v1 import BaseModel
-else:
-    from pydantic import BaseModel
-
 from ruamel.yaml import YAML
 
 from prefect.client.schemas.objects import MinimalDeploymentSchedule
 from prefect.client.schemas.schedules import IntervalSchedule
 from prefect.flows import load_flow_from_entrypoint
 from prefect.logging import get_logger
 from prefect.settings import PREFECT_DEBUG_MODE
@@ -405,30 +397,30 @@
     deployment.pop("parameter_openapi_schema")
     # Only want entrypoint to avoid errors
     deployment.pop("flow_name", None)
 
     if deployment.get("schedule"):
         if isinstance(deployment["schedule"], IntervalSchedule):
             deployment["schedule"] = _interval_schedule_to_dict(deployment["schedule"])
-        elif isinstance(deployment["schedule"], BaseModel):
+        else:  # all valid SCHEDULE_TYPES are subclasses of BaseModel
             deployment["schedule"] = deployment["schedule"].dict()
 
         if "is_schedule_active" in deployment:
             deployment["schedule"]["active"] = deployment.pop("is_schedule_active")
 
     if deployment.get("schedules"):
         schedules = []
         for deployment_schedule in cast(
             List[MinimalDeploymentSchedule], deployment["schedules"]
         ):
             if isinstance(deployment_schedule.schedule, IntervalSchedule):
                 schedule_config = _interval_schedule_to_dict(
                     deployment_schedule.schedule
                 )
-            elif isinstance(deployment_schedule.schedule, BaseModel):
+            else:  # all valid SCHEDULE_TYPES are subclasses of BaseModel
                 schedule_config = deployment_schedule.schedule.dict()
 
             schedule_config["active"] = deployment_schedule.active
             schedules.append(schedule_config)
 
         deployment["schedules"] = schedules
```

### Comparing `prefect-client-2.16.9/src/prefect/deployments/deployments.py` & `prefect-client-2.17.0/src/prefect/deployments/deployments.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 from uuid import UUID
 
 import anyio
 import pendulum
 import yaml
 
 from prefect._internal.compatibility.deprecated import (
+    DeprecatedInfraOverridesField,
     deprecated_callable,
     deprecated_class,
+    deprecated_parameter,
+    handle_deprecated_infra_overrides_parameter,
 )
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect._internal.schemas.validators import (
     handle_openapi_schema,
     infrastructure_must_have_capabilities,
     reconcile_schedules,
     storage_must_have_capabilities,
@@ -67,27 +70,33 @@
 from prefect.utilities.filesystem import relative_path_to_current_platform, tmpchdir
 from prefect.utilities.slugify import slugify
 
 logger = get_logger("deployments")
 
 
 @sync_compatible
+@deprecated_parameter(
+    "infra_overrides",
+    start_date="Apr 2024",
+    help="Use `job_variables` instead.",
+)
 @inject_client
 async def run_deployment(
     name: Union[str, UUID],
     client: Optional[PrefectClient] = None,
     parameters: Optional[dict] = None,
     scheduled_time: Optional[datetime] = None,
     flow_run_name: Optional[str] = None,
     timeout: Optional[float] = None,
     poll_interval: Optional[float] = 5,
     tags: Optional[Iterable[str]] = None,
     idempotency_key: Optional[str] = None,
     work_queue_name: Optional[str] = None,
     as_subflow: Optional[bool] = True,
+    infra_overrides: Optional[dict] = None,
     job_variables: Optional[dict] = None,
 ) -> FlowRun:
     """
     Create a flow run for a deployment and return it after completion or a timeout.
 
     By default, this function blocks until the flow run finishes executing.
     Specify a timeout (in seconds) to wait for the flow run to execute before
@@ -99,15 +108,15 @@
 
     If called within a flow or task, the flow run this function creates will
     be linked to the current flow run as a subflow. Disable this behavior by
     passing `as_subflow=False`.
 
     Args:
         name: The deployment id or deployment name in the form:
-            `<slugified-flow-name>/<slugified-deployment-name>`
+            `"flow name/deployment name"`
         parameters: Parameter overrides for this flow run. Merged with the deployment
             defaults.
         scheduled_time: The time to schedule the flow run for, defaults to scheduling
             the flow run to start now.
         flow_run_name: A name for the created flow run
         timeout: The amount of time to wait (in seconds) for the flow run to
             complete before returning. Setting `timeout` to 0 will return the flow
@@ -118,21 +127,26 @@
             automations and for organizational purposes.
         idempotency_key: A unique value to recognize retries of the same run, and
             prevent creating multiple flow runs.
         work_queue_name: The name of a work queue to use for this run. Defaults to
             the default work queue for the deployment.
         as_subflow: Whether to link the flow run as a subflow of the current
             flow or task run.
+        job_variables: A dictionary of dot delimited infrastructure overrides that
+            will be applied at runtime; for example `env.CONFIG_KEY=config_value` or
+            `namespace='prefect'`
     """
     if timeout is not None and timeout < 0:
         raise ValueError("`timeout` cannot be negative")
 
     if scheduled_time is None:
         scheduled_time = pendulum.now("UTC")
 
+    jv = handle_deprecated_infra_overrides_parameter(job_variables, infra_overrides)
+
     parameters = parameters or {}
 
     deployment_id = None
 
     if isinstance(name, UUID):
         deployment_id = name
     else:
@@ -200,15 +214,15 @@
         parameters=parameters,
         state=Scheduled(scheduled_time=scheduled_time),
         name=flow_run_name,
         tags=tags,
         idempotency_key=idempotency_key,
         parent_task_run_id=parent_task_run_id,
         work_queue_name=work_queue_name,
-        job_variables=job_variables,
+        job_variables=jv,
     )
 
     flow_run_id = flow_run.id
 
     if timeout == 0:
         return flow_run
 
@@ -330,15 +344,15 @@
 
 @deprecated_class(
     start_date="Mar 2024",
     help="Use `flow.deploy` to deploy your flows instead."
     " Refer to the upgrade guide for more information:"
     " https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.",
 )
-class Deployment(BaseModel):
+class Deployment(DeprecatedInfraOverridesField, BaseModel):
     """
     DEPRECATION WARNING:
 
     This class is deprecated as of March 2024 and will not be available after September 2024.
     It has been replaced by `flow.deploy`, which offers enhanced functionality and better a better user experience.
     For upgrade instructions, see https://docs.prefect.io/latest/guides/upgrade-guide-agents-to-workers/.
 
@@ -359,15 +373,15 @@
         work_pool_name: The work pool for the deployment
         flow_name: The name of the flow this deployment encapsulates
         parameters: A dictionary of parameter values to pass to runs created from this
             deployment
         infrastructure: An optional infrastructure block used to configure
             infrastructure for runs; if not provided, will default to running this
             deployment in Agent subprocesses
-        infra_overrides: A dictionary of dot delimited infrastructure overrides that
+        job_variables: A dictionary of dot delimited infrastructure overrides that
             will be applied at runtime; for example `env.CONFIG_KEY=config_value` or
             `namespace='prefect'`
         storage: An optional remote storage block used to store and retrieve this
             workflow; if not provided, will default to referencing this flow by its
             local path
         path: The path to the working directory for the workflow, relative to remote
             storage or, if stored on a local filesystem, an absolute path
@@ -401,15 +415,15 @@
         >>> storage = S3.load("dev-bucket") # load a pre-defined block
         >>> deployment = Deployment.build_from_flow(
         ...     flow=my_flow,
         ...     name="s3-example",
         ...     version="2",
         ...     tags=["aws"],
         ...     storage=storage,
-        ...     infra_overrides=dict("env.PREFECT_LOGGING_LEVEL"="DEBUG"),
+        ...     job_variables=dict("env.PREFECT_LOGGING_LEVEL"="DEBUG"),
         >>> )
         >>> deployment.apply()
 
     """
 
     class Config:
         json_encoders = {SecretDict: lambda v: v.dict()}
@@ -425,14 +439,19 @@
             "work_queue_name",
             "work_pool_name",
             "tags",
             "parameters",
             "schedule",
             "schedules",
             "is_schedule_active",
+            # The `infra_overrides` field has been renamed to `job_variables`.
+            # We will continue writing it in the YAML file as `infra_overrides`
+            # instead of `job_variables` for better backwards compat, but we'll
+            # accept either `job_variables` or `infra_overrides` when we read
+            # the file.
             "infra_overrides",
         ]
 
         # if infrastructure is baked as a pre-saved block, then
         # editing its fields will not update anything
         if self.infrastructure._block_document_id:
             return editable_fields
@@ -474,18 +493,24 @@
             for field in self._editable_fields:
                 # write any comments
                 if schema["properties"][field].get("yaml_comment"):
                     f.write(f"# {schema['properties'][field]['yaml_comment']}\n")
                 # write the field
                 yaml.dump({field: yaml_dict[field]}, f, sort_keys=False)
 
-            # write non-editable fields
+            # write non-editable fields, excluding `job_variables` because we'll
+            # continue writing it as `infra_overrides` for better backwards compat
+            # with the existing file format.
             f.write("\n###\n### DO NOT EDIT BELOW THIS LINE\n###\n")
             yaml.dump(
-                {k: v for k, v in yaml_dict.items() if k not in self._editable_fields},
+                {
+                    k: v
+                    for k, v in yaml_dict.items()
+                    if k not in self._editable_fields and k != "job_variables"
+                },
                 f,
                 sort_keys=False,
             )
 
     def _yaml_dict(self) -> dict:
         """
         Returns a YAML-compatible representation of this deployment as a dictionary.
@@ -554,15 +579,15 @@
     manifest_path: Optional[str] = Field(
         default=None,
         description=(
             "The path to the flow's manifest file, relative to the chosen storage."
         ),
     )
     infrastructure: Infrastructure = Field(default_factory=Process)
-    infra_overrides: Dict[str, Any] = Field(
+    job_variables: Dict[str, Any] = Field(
         default_factory=dict,
         description="Overrides to apply to the base infrastructure block at runtime.",
     )
     storage: Optional[Block] = Field(
         None,
         help="The remote storage to use for this workflow.",
     )
@@ -865,15 +890,15 @@
                 is_schedule_active=self.is_schedule_active,
                 parameters=self.parameters,
                 description=self.description,
                 tags=self.tags,
                 manifest_path=self.manifest_path,  # allows for backwards YAML compat
                 path=self.path,
                 entrypoint=self.entrypoint,
-                infra_overrides=self.infra_overrides,
+                job_variables=self.job_variables,
                 storage_document_id=storage_document_id,
                 infrastructure_document_id=infrastructure_document_id,
                 parameter_openapi_schema=self.parameter_openapi_schema.dict(),
                 enforce_parameter_schema=self.enforce_parameter_schema,
             )
 
             if client.server_type == ServerType.CLOUD:
```

### Comparing `prefect-client-2.16.9/src/prefect/deployments/runner.py` & `prefect-client-2.17.0/src/prefect/deployments/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,17 +302,17 @@
                 storage_document_id=None,
                 infrastructure_document_id=None,
                 parameter_openapi_schema=self._parameter_openapi_schema.dict(),
                 enforce_parameter_schema=self.enforce_parameter_schema,
             )
 
             if work_pool_name:
-                create_payload["infra_overrides"] = self.job_variables
+                create_payload["job_variables"] = self.job_variables
                 if image:
-                    create_payload["infra_overrides"]["image"] = image
+                    create_payload["job_variables"]["image"] = image
                 create_payload["path"] = None if self.storage else self._path
                 create_payload["pull_steps"] = (
                     [self.storage.to_pull_step()] if self.storage else []
                 )
 
             try:
                 deployment_id = await client.create_deployment(**create_payload)
```

### Comparing `prefect-client-2.16.9/src/prefect/deployments/schedules.py` & `prefect-client-2.17.0/src/prefect/deployments/schedules.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deployments/steps/core.py` & `prefect-client-2.17.0/src/prefect/deployments/steps/core.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deployments/steps/pull.py` & `prefect-client-2.17.0/src/prefect/deployments/steps/pull.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deployments/steps/utility.py` & `prefect-client-2.17.0/src/prefect/deployments/steps/utility.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/data_documents.py` & `prefect-client-2.17.0/src/prefect/deprecated/data_documents.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/packaging/base.py` & `prefect-client-2.17.0/src/prefect/deprecated/packaging/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/packaging/docker.py` & `prefect-client-2.17.0/src/prefect/deprecated/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/packaging/file.py` & `prefect-client-2.17.0/src/prefect/deprecated/packaging/file.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/packaging/orion.py` & `prefect-client-2.17.0/src/prefect/deprecated/packaging/orion.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/deprecated/packaging/serializers.py` & `prefect-client-2.17.0/src/prefect/deprecated/packaging/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/engine.py` & `prefect-client-2.17.0/src/prefect/engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,28 +78,25 @@
     See `orchestrate_task_run`, `call_soon_in_new_thread`
 
     _Ideally, for local and sequential task runners we would send the task run to the
     user thread as we do for flows. See [#9855](https://github.com/PrefectHQ/prefect/pull/9855).
 """
 
 import asyncio
-import contextlib
 import logging
 import os
 import random
-import signal
 import sys
 import threading
 import time
 from contextlib import AsyncExitStack, asynccontextmanager
 from functools import partial
 from typing import (
     Any,
     Awaitable,
-    Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Set,
     Type,
     TypeVar,
@@ -116,46 +113,42 @@
 import prefect
 import prefect.context
 import prefect.plugins
 from prefect._internal.compatibility.deprecated import deprecated_parameter
 from prefect._internal.compatibility.experimental import experimental_parameter
 from prefect._internal.concurrency.api import create_call, from_async, from_sync
 from prefect._internal.concurrency.calls import get_current_call
-from prefect._internal.concurrency.cancellation import CancelledError, get_deadline
+from prefect._internal.concurrency.cancellation import CancelledError
 from prefect._internal.concurrency.threads import wait_for_global_loop_exit
 from prefect.client.orchestration import PrefectClient, get_client
-from prefect.client.schemas import FlowRun, OrchestrationResult, TaskRun
+from prefect.client.schemas import FlowRun, TaskRun
 from prefect.client.schemas.filters import FlowRunFilter
 from prefect.client.schemas.objects import (
     StateDetails,
     StateType,
     TaskRunInput,
-    TaskRunResult,
 )
 from prefect.client.schemas.responses import SetStateStatus
 from prefect.client.schemas.sorting import FlowRunSort
 from prefect.client.utilities import inject_client
 from prefect.context import (
     FlowRunContext,
     PrefectObjectRegistry,
     TagsContext,
     TaskRunContext,
 )
 from prefect.deployments import load_flow_from_flow_run
-from prefect.events import Event, emit_event
 from prefect.exceptions import (
     Abort,
     FlowPauseTimeout,
     MappingLengthMismatch,
     MappingMissingIterable,
     NotPausedError,
     Pause,
     PausedRun,
-    PrefectException,
-    TerminationSignal,
     UpstreamTaskError,
 )
 from prefect.flows import Flow, load_flow_from_entrypoint
 from prefect.futures import PrefectFuture, call_repr, resolve_futures_to_states
 from prefect.input import keyset_from_paused_state
 from prefect.input.run_input import run_input_subclass_from_type
 from prefect.logging.configuration import setup_logging
@@ -163,35 +156,31 @@
 from prefect.logging.loggers import (
     flow_run_logger,
     get_logger,
     get_run_logger,
     patch_print,
     task_run_logger,
 )
-from prefect.results import BaseResult, ResultFactory, UnknownResult
+from prefect.results import ResultFactory, UnknownResult
 from prefect.settings import (
     PREFECT_DEBUG_MODE,
-    PREFECT_EXPERIMENTAL_ENABLE_TASK_SCHEDULING,
-    PREFECT_LOGGING_LOG_PRINTS,
     PREFECT_TASK_INTROSPECTION_WARN_THRESHOLD,
     PREFECT_TASKS_REFRESH_CACHE,
     PREFECT_UI_URL,
 )
 from prefect.states import (
     Completed,
     Paused,
     Pending,
     Running,
     Scheduled,
     State,
     Suspended,
     exception_to_crashed_state,
     exception_to_failed_state,
-    get_state_exception,
-    is_state,
     return_value_to_state,
 )
 from prefect.task_runners import (
     CONCURRENCY_MESSAGES,
     BaseTaskRunner,
     TaskConcurrencyType,
 )
@@ -204,25 +193,37 @@
 )
 from prefect.utilities.callables import (
     collapse_variadic_parameters,
     explode_variadic_parameter,
     get_parameter_defaults,
     parameters_to_args_kwargs,
 )
-from prefect.utilities.collections import StopVisiting, isiterable, visit_collection
-from prefect.utilities.text import truncated_to
+from prefect.utilities.collections import isiterable
+from prefect.utilities.engine import (
+    _dynamic_key_for_task_run,
+    _get_hook_name,
+    _observed_flow_pauses,
+    _resolve_custom_flow_run_name,
+    _resolve_custom_task_run_name,
+    capture_sigterm,
+    check_api_reachable,
+    collect_task_run_inputs,
+    emit_task_run_state_change_event,
+    propose_state,
+    resolve_inputs,
+    should_log_prints,
+    wait_for_task_runs_and_report_crashes,
+)
 
 R = TypeVar("R")
 T = TypeVar("T")
 EngineReturnType = Literal["future", "state", "result"]
 
 NUM_CHARS_DYNAMIC_KEY = 8
 
-API_HEALTHCHECKS = {}
-UNTRACKABLE_TYPES = {bool, type(None), type(...), type(NotImplemented)}
 engine_logger = get_logger("engine")
 
 
 def enter_flow_run_engine_from_flow_call(
     flow: Flow,
     parameters: Dict[str, Any],
     wait_for: Optional[Iterable[PrefectFuture]],
@@ -241,20 +242,14 @@
         engine_logger.warning(
             f"Script loading is in progress, flow {flow.name!r} will not be executed."
             " Consider updating the script to only call the flow if executed"
             f' directly:\n\n\tif __name__ == "__main__":\n\t\t{flow.fn.__name__}()'
         )
         return None
 
-    if TaskRunContext.get():
-        raise RuntimeError(
-            "Flows cannot be run from within tasks. Did you mean to call this "
-            "flow in a flow?"
-        )
-
     parent_flow_run_context = FlowRunContext.get()
     is_subflow_run = parent_flow_run_context is not None
 
     if wait_for is not None and not is_subflow_run:
         raise ValueError("Only flows run as subflows can wait for dependencies.")
 
     begin_run = create_call(
@@ -617,21 +612,29 @@
 
     parent_logger.debug(f"Resolving inputs to {flow.name!r}")
     task_inputs = {k: await collect_task_run_inputs(v) for k, v in parameters.items()}
 
     if wait_for:
         task_inputs["wait_for"] = await collect_task_run_inputs(wait_for)
 
-    rerunning = parent_flow_run_context.flow_run.run_count > 1
+    rerunning = (
+        parent_flow_run_context.flow_run.run_count > 1
+        if getattr(parent_flow_run_context, "flow_run", None)
+        else False
+    )
 
     # Generate a task in the parent flow run to represent the result of the subflow run
     dummy_task = Task(name=flow.name, fn=flow.fn, version=flow.version)
     parent_task_run = await client.create_task_run(
         task=dummy_task,
-        flow_run_id=parent_flow_run_context.flow_run.id,
+        flow_run_id=(
+            parent_flow_run_context.flow_run.id
+            if getattr(parent_flow_run_context, "flow_run", None)
+            else None
+        ),
         dynamic_key=_dynamic_key_for_task_run(parent_flow_run_context, dummy_task),
         task_inputs=task_inputs,
         state=Pending(),
     )
 
     # Resolve any task futures in the input
     parameters = await resolve_inputs(parameters)
@@ -851,15 +854,15 @@
                 # This check for a parent call is needed for cases where the engine
                 # was entered directly during testing
                 parent_call = get_current_call()
 
                 if parent_call and (
                     not parent_flow_run_context
                     or (
-                        parent_flow_run_context
+                        getattr(parent_flow_run_context, "flow", None)
                         and parent_flow_run_context.flow.isasync == flow.isasync
                     )
                 ):
                     from_async.call_soon_in_waiting_thread(
                         flow_call,
                         thread=user_thread,
                         timeout=flow.timeout_seconds,
@@ -1372,25 +1375,19 @@
     mapped: bool,
 ) -> Union[PrefectFuture, Awaitable[PrefectFuture], TaskRun]:
     """Sync entrypoint for task calls"""
 
     flow_run_context = FlowRunContext.get()
 
     if not flow_run_context:
-        if (
-            not PREFECT_EXPERIMENTAL_ENABLE_TASK_SCHEDULING.value()
-            or return_type == "future"
-            or mapped
-        ):
+        if return_type == "future" or mapped:
             raise RuntimeError(
-                "Tasks cannot be run outside of a flow by default."
-                " If you meant to submit an autonomous task, you need to set"
+                " If you meant to submit a background task, you need to set"
                 " `prefect config set PREFECT_EXPERIMENTAL_ENABLE_TASK_SCHEDULING=true`"
                 " and use `your_task.submit()` instead of `your_task()`."
-                " Mapping autonomous tasks is not yet supported."
             )
         from prefect.task_engine import submit_autonomous_task_run_to_engine
 
         return submit_autonomous_task_run_to_engine(
             task=task,
             task_run=None,
             parameters=parameters,
@@ -1523,60 +1520,14 @@
     runner = task_runner if task_runner else flow_run_context.task_runner
     if runner.concurrency_type == TaskConcurrencyType.SEQUENTIAL:
         return [await task_run() for task_run in task_runs]
 
     return await gather(*task_runs)
 
 
-async def collect_task_run_inputs(expr: Any, max_depth: int = -1) -> Set[TaskRunInput]:
-    """
-    This function recurses through an expression to generate a set of any discernible
-    task run inputs it finds in the data structure. It produces a set of all inputs
-    found.
-
-    Examples:
-        >>> task_inputs = {
-        >>>    k: await collect_task_run_inputs(v) for k, v in parameters.items()
-        >>> }
-    """
-    # TODO: This function needs to be updated to detect parameters and constants
-
-    inputs = set()
-    futures = set()
-
-    def add_futures_and_states_to_inputs(obj):
-        if isinstance(obj, PrefectFuture):
-            # We need to wait for futures to be submitted before we can get the task
-            # run id but we want to do so asynchronously
-            futures.add(obj)
-        elif is_state(obj):
-            if obj.state_details.task_run_id:
-                inputs.add(TaskRunResult(id=obj.state_details.task_run_id))
-        # Expressions inside quotes should not be traversed
-        elif isinstance(obj, quote):
-            raise StopVisiting
-        else:
-            state = get_state_for_result(obj)
-            if state and state.state_details.task_run_id:
-                inputs.add(TaskRunResult(id=state.state_details.task_run_id))
-
-    visit_collection(
-        expr,
-        visit_fn=add_futures_and_states_to_inputs,
-        return_data=False,
-        max_depth=max_depth,
-    )
-
-    await asyncio.gather(*[future._wait_for_submission() for future in futures])
-    for future in futures:
-        inputs.add(TaskRunResult(id=future.task_run.id))
-
-    return inputs
-
-
 async def get_task_call_return_value(
     task: Task,
     flow_run_context: FlowRunContext,
     parameters: Dict[str, Any],
     wait_for: Optional[Iterable[PrefectFuture]],
     return_type: EngineReturnType,
     task_runner: Optional[BaseTaskRunner],
@@ -2239,93 +2190,14 @@
     logger.log(
         level=logging.INFO if state.is_completed() else logging.ERROR,
         msg=f"Finished in state {display_state}",
     )
     return state
 
 
-async def wait_for_task_runs_and_report_crashes(
-    task_run_futures: Iterable[PrefectFuture], client: PrefectClient
-) -> Literal[True]:
-    crash_exceptions = []
-
-    # Gather states concurrently first
-    states = await gather(*(future._wait for future in task_run_futures))
-
-    for future, state in zip(task_run_futures, states):
-        logger = task_run_logger(future.task_run)
-
-        if not state.type == StateType.CRASHED:
-            continue
-
-        # We use this utility instead of `state.result` for type checking
-        exception = await get_state_exception(state)
-
-        task_run = await client.read_task_run(future.task_run.id)
-        if not task_run.state.is_crashed():
-            logger.info(f"Crash detected! {state.message}")
-            logger.debug("Crash details:", exc_info=exception)
-
-            # Update the state of the task run
-            result = await client.set_task_run_state(
-                task_run_id=future.task_run.id, state=state, force=True
-            )
-            if result.status == SetStateStatus.ACCEPT:
-                engine_logger.debug(
-                    f"Reported crashed task run {future.name!r} successfully."
-                )
-            else:
-                engine_logger.warning(
-                    f"Failed to report crashed task run {future.name!r}. "
-                    f"Orchestrator did not accept state: {result!r}"
-                )
-        else:
-            # Populate the state details on the local state
-            future._final_state.state_details = task_run.state.state_details
-
-        crash_exceptions.append(exception)
-
-    # Now that we've finished reporting crashed tasks, reraise any exit exceptions
-    for exception in crash_exceptions:
-        if isinstance(exception, (KeyboardInterrupt, SystemExit)):
-            raise exception
-
-    return True
-
-
-@contextlib.contextmanager
-def capture_sigterm():
-    def cancel_flow_run(*args):
-        raise TerminationSignal(signal=signal.SIGTERM)
-
-    original_term_handler = None
-    try:
-        original_term_handler = signal.signal(signal.SIGTERM, cancel_flow_run)
-    except ValueError:
-        # Signals only work in the main thread
-        pass
-
-    try:
-        yield
-    except TerminationSignal as exc:
-        # Termination signals are swapped out during a flow run to perform
-        # a graceful shutdown and raise this exception. This `os.kill` call
-        # ensures that the previous handler, likely the Python default,
-        # gets called as well.
-        if original_term_handler is not None:
-            signal.signal(exc.signal, original_term_handler)
-            os.kill(os.getpid(), exc.signal)
-
-        raise
-
-    finally:
-        if original_term_handler is not None:
-            signal.signal(signal.SIGTERM, original_term_handler)
-
-
 @asynccontextmanager
 async def report_flow_run_crashes(flow_run: FlowRun, client: PrefectClient, flow: Flow):
     """
     Detect flow run crashes during this context and update the run to a proper final
     state.
 
     This context _must_ reraise the exception to properly exit the run.
@@ -2388,378 +2260,14 @@
                 f"Reported crashed task run {task_run.name!r} successfully!"
             )
 
         # Reraise the exception
         raise
 
 
-async def resolve_inputs(
-    parameters: Dict[str, Any], return_data: bool = True, max_depth: int = -1
-) -> Dict[str, Any]:
-    """
-    Resolve any `Quote`, `PrefectFuture`, or `State` types nested in parameters into
-    data.
-
-    Returns:
-        A copy of the parameters with resolved data
-
-    Raises:
-        UpstreamTaskError: If any of the upstream states are not `COMPLETED`
-    """
-
-    futures = set()
-    states = set()
-    result_by_state = {}
-
-    if not parameters:
-        return {}
-
-    def collect_futures_and_states(expr, context):
-        # Expressions inside quotes should not be traversed
-        if isinstance(context.get("annotation"), quote):
-            raise StopVisiting()
-
-        if isinstance(expr, PrefectFuture):
-            futures.add(expr)
-        if is_state(expr):
-            states.add(expr)
-
-        return expr
-
-    visit_collection(
-        parameters,
-        visit_fn=collect_futures_and_states,
-        return_data=False,
-        max_depth=max_depth,
-        context={},
-    )
-
-    # Wait for all futures so we do not block when we retrieve the state in `resolve_input`
-    states.update(await asyncio.gather(*[future._wait() for future in futures]))
-
-    # Only retrieve the result if requested as it may be expensive
-    if return_data:
-        finished_states = [state for state in states if state.is_final()]
-
-        state_results = await asyncio.gather(
-            *[
-                state.result(raise_on_failure=False, fetch=True)
-                for state in finished_states
-            ]
-        )
-
-        for state, result in zip(finished_states, state_results):
-            result_by_state[state] = result
-
-    def resolve_input(expr, context):
-        state = None
-
-        # Expressions inside quotes should not be modified
-        if isinstance(context.get("annotation"), quote):
-            raise StopVisiting()
-
-        if isinstance(expr, PrefectFuture):
-            state = expr._final_state
-        elif is_state(expr):
-            state = expr
-        else:
-            return expr
-
-        # Do not allow uncompleted upstreams except failures when `allow_failure` has
-        # been used
-        if not state.is_completed() and not (
-            # TODO: Note that the contextual annotation here is only at the current level
-            #       if `allow_failure` is used then another annotation is used, this will
-            #       incorrectly evaluate to false — to resolve this, we must track all
-            #       annotations wrapping the current expression but this is not yet
-            #       implemented.
-            isinstance(context.get("annotation"), allow_failure) and state.is_failed()
-        ):
-            raise UpstreamTaskError(
-                f"Upstream task run '{state.state_details.task_run_id}' did not reach a"
-                " 'COMPLETED' state."
-            )
-
-        return result_by_state.get(state)
-
-    resolved_parameters = {}
-    for parameter, value in parameters.items():
-        try:
-            resolved_parameters[parameter] = visit_collection(
-                value,
-                visit_fn=resolve_input,
-                return_data=return_data,
-                # we're manually going 1 layer deeper here
-                max_depth=max_depth - 1,
-                remove_annotations=True,
-                context={},
-            )
-        except UpstreamTaskError:
-            raise
-        except Exception as exc:
-            raise PrefectException(
-                f"Failed to resolve inputs in parameter {parameter!r}. If your"
-                " parameter type is not supported, consider using the `quote`"
-                " annotation to skip resolution of inputs."
-            ) from exc
-
-    return resolved_parameters
-
-
-async def propose_state(
-    client: PrefectClient,
-    state: State,
-    force: bool = False,
-    task_run_id: UUID = None,
-    flow_run_id: UUID = None,
-) -> State:
-    """
-    Propose a new state for a flow run or task run, invoking Prefect orchestration logic.
-
-    If the proposed state is accepted, the provided `state` will be augmented with
-     details and returned.
-
-    If the proposed state is rejected, a new state returned by the Prefect API will be
-    returned.
-
-    If the proposed state results in a WAIT instruction from the Prefect API, the
-    function will sleep and attempt to propose the state again.
-
-    If the proposed state results in an ABORT instruction from the Prefect API, an
-    error will be raised.
-
-    Args:
-        state: a new state for the task or flow run
-        task_run_id: an optional task run id, used when proposing task run states
-        flow_run_id: an optional flow run id, used when proposing flow run states
-
-    Returns:
-        a [State model][prefect.client.schemas.objects.State] representation of the
-            flow or task run state
-
-    Raises:
-        ValueError: if neither task_run_id or flow_run_id is provided
-        prefect.exceptions.Abort: if an ABORT instruction is received from
-            the Prefect API
-    """
-
-    # Determine if working with a task run or flow run
-    if not task_run_id and not flow_run_id:
-        raise ValueError("You must provide either a `task_run_id` or `flow_run_id`")
-
-    # Handle task and sub-flow tracing
-    if state.is_final():
-        if isinstance(state.data, BaseResult) and state.data.has_cached_object():
-            # Avoid fetching the result unless it is cached, otherwise we defeat
-            # the purpose of disabling `cache_result_in_memory`
-            result = await state.result(raise_on_failure=False, fetch=True)
-        else:
-            result = state.data
-
-        link_state_to_result(state, result)
-
-    # Handle repeated WAITs in a loop instead of recursively, to avoid
-    # reaching max recursion depth in extreme cases.
-    async def set_state_and_handle_waits(set_state_func) -> OrchestrationResult:
-        response = await set_state_func()
-        while response.status == SetStateStatus.WAIT:
-            engine_logger.debug(
-                f"Received wait instruction for {response.details.delay_seconds}s: "
-                f"{response.details.reason}"
-            )
-            await anyio.sleep(response.details.delay_seconds)
-            response = await set_state_func()
-        return response
-
-    # Attempt to set the state
-    if task_run_id:
-        set_state = partial(client.set_task_run_state, task_run_id, state, force=force)
-        response = await set_state_and_handle_waits(set_state)
-    elif flow_run_id:
-        set_state = partial(client.set_flow_run_state, flow_run_id, state, force=force)
-        response = await set_state_and_handle_waits(set_state)
-    else:
-        raise ValueError(
-            "Neither flow run id or task run id were provided. At least one must "
-            "be given."
-        )
-
-    # Parse the response to return the new state
-    if response.status == SetStateStatus.ACCEPT:
-        # Update the state with the details if provided
-        state.id = response.state.id
-        state.timestamp = response.state.timestamp
-        if response.state.state_details:
-            state.state_details = response.state.state_details
-        return state
-
-    elif response.status == SetStateStatus.ABORT:
-        raise prefect.exceptions.Abort(response.details.reason)
-
-    elif response.status == SetStateStatus.REJECT:
-        if response.state.is_paused():
-            raise Pause(response.details.reason, state=response.state)
-        return response.state
-
-    else:
-        raise ValueError(
-            f"Received unexpected `SetStateStatus` from server: {response.status!r}"
-        )
-
-
-def _dynamic_key_for_task_run(context: FlowRunContext, task: Task) -> int:
-    if context.flow_run is None:  # this is an autonomous task run
-        context.task_run_dynamic_keys[task.task_key] = getattr(
-            task, "dynamic_key", str(uuid4())
-        )
-
-    elif task.task_key not in context.task_run_dynamic_keys:
-        context.task_run_dynamic_keys[task.task_key] = 0
-    else:
-        context.task_run_dynamic_keys[task.task_key] += 1
-
-    return context.task_run_dynamic_keys[task.task_key]
-
-
-def _observed_flow_pauses(context: FlowRunContext) -> int:
-    if "counter" not in context.observed_flow_pauses:
-        context.observed_flow_pauses["counter"] = 1
-    else:
-        context.observed_flow_pauses["counter"] += 1
-    return context.observed_flow_pauses["counter"]
-
-
-def get_state_for_result(obj: Any) -> Optional[State]:
-    """
-    Get the state related to a result object.
-
-    `link_state_to_result` must have been called first.
-    """
-    flow_run_context = FlowRunContext.get()
-    if flow_run_context:
-        return flow_run_context.task_run_results.get(id(obj))
-
-
-def link_state_to_result(state: State, result: Any) -> None:
-    """
-    Caches a link between a state and a result and its components using
-    the `id` of the components to map to the state. The cache is persisted to the
-    current flow run context since task relationships are limited to within a flow run.
-
-    This allows dependency tracking to occur when results are passed around.
-    Note: Because `id` is used, we cannot cache links between singleton objects.
-
-    We only cache the relationship between components 1-layer deep.
-    Example:
-        Given the result [1, ["a","b"], ("c",)], the following elements will be
-        mapped to the state:
-        - [1, ["a","b"], ("c",)]
-        - ["a","b"]
-        - ("c",)
-
-        Note: the int `1` will not be mapped to the state because it is a singleton.
-
-    Other Notes:
-    We do not hash the result because:
-    - If changes are made to the object in the flow between task calls, we can still
-      track that they are related.
-    - Hashing can be expensive.
-    - Not all objects are hashable.
-
-    We do not set an attribute, e.g. `__prefect_state__`, on the result because:
-
-    - Mutating user's objects is dangerous.
-    - Unrelated equality comparisons can break unexpectedly.
-    - The field can be preserved on copy.
-    - We cannot set this attribute on Python built-ins.
-    """
-
-    flow_run_context = FlowRunContext.get()
-
-    def link_if_trackable(obj: Any) -> None:
-        """Track connection between a task run result and its associated state if it has a unique ID.
-
-        We cannot track booleans, Ellipsis, None, NotImplemented, or the integers from -5 to 256
-        because they are singletons.
-
-        This function will mutate the State if the object is an untrackable type by setting the value
-        for `State.state_details.untrackable_result` to `True`.
-
-        """
-        if (type(obj) in UNTRACKABLE_TYPES) or (
-            isinstance(obj, int) and (-5 <= obj <= 256)
-        ):
-            state.state_details.untrackable_result = True
-            return
-        flow_run_context.task_run_results[id(obj)] = state
-
-    if flow_run_context:
-        visit_collection(expr=result, visit_fn=link_if_trackable, max_depth=1)
-
-
-def should_log_prints(flow_or_task: Union[Flow, Task]) -> bool:
-    flow_run_context = FlowRunContext.get()
-
-    if flow_or_task.log_prints is None:
-        if flow_run_context:
-            return flow_run_context.log_prints
-        else:
-            return PREFECT_LOGGING_LOG_PRINTS.value()
-
-    return flow_or_task.log_prints
-
-
-def _resolve_custom_flow_run_name(flow: Flow, parameters: Dict[str, Any]) -> str:
-    if callable(flow.flow_run_name):
-        flow_run_name = flow.flow_run_name()
-        if not isinstance(flow_run_name, str):
-            raise TypeError(
-                f"Callable {flow.flow_run_name} for 'flow_run_name' returned type"
-                f" {type(flow_run_name).__name__} but a string is required."
-            )
-    elif isinstance(flow.flow_run_name, str):
-        flow_run_name = flow.flow_run_name.format(**parameters)
-    else:
-        raise TypeError(
-            "Expected string or callable for 'flow_run_name'; got"
-            f" {type(flow.flow_run_name).__name__} instead."
-        )
-
-    return flow_run_name
-
-
-def _resolve_custom_task_run_name(task: Task, parameters: Dict[str, Any]) -> str:
-    if callable(task.task_run_name):
-        task_run_name = task.task_run_name()
-        if not isinstance(task_run_name, str):
-            raise TypeError(
-                f"Callable {task.task_run_name} for 'task_run_name' returned type"
-                f" {type(task_run_name).__name__} but a string is required."
-            )
-    elif isinstance(task.task_run_name, str):
-        task_run_name = task.task_run_name.format(**parameters)
-    else:
-        raise TypeError(
-            "Expected string or callable for 'task_run_name'; got"
-            f" {type(task.task_run_name).__name__} instead."
-        )
-
-    return task_run_name
-
-
-def _get_hook_name(hook: Callable) -> str:
-    return (
-        hook.__name__
-        if hasattr(hook, "__name__")
-        else (
-            hook.func.__name__ if isinstance(hook, partial) else hook.__class__.__name__
-        )
-    )
-
-
 async def _run_task_hooks(task: Task, task_run: TaskRun, state: State) -> None:
     """Run the on_failure and on_completion hooks for a task, making sure to
     catch and log any errors that occur.
     """
     hooks = None
     if state.is_failed() and task.on_failure:
         hooks = task.on_failure
@@ -2879,86 +2387,14 @@
                     f"An error was encountered while running hook {hook_name!r}",
                     exc_info=True,
                 )
             else:
                 logger.info(f"Hook {hook_name!r} finished running successfully")
 
 
-async def check_api_reachable(client: PrefectClient, fail_message: str):
-    # Do not perform a healthcheck if it exists and is not expired
-    api_url = str(client.api_url)
-    if api_url in API_HEALTHCHECKS:
-        expires = API_HEALTHCHECKS[api_url]
-        if expires > time.monotonic():
-            return
-
-    connect_error = await client.api_healthcheck()
-    if connect_error:
-        raise RuntimeError(
-            f"{fail_message}. Failed to reach API at {api_url}."
-        ) from connect_error
-
-    # Create a 10 minute cache for the healthy response
-    API_HEALTHCHECKS[api_url] = get_deadline(60 * 10)
-
-
-def emit_task_run_state_change_event(
-    task_run: TaskRun,
-    initial_state: Optional[State],
-    validated_state: State,
-    follows: Optional[Event] = None,
-) -> Event:
-    state_message_truncation_length = 100_000
-
-    return emit_event(
-        id=validated_state.id,
-        occurred=validated_state.timestamp,
-        event=f"prefect.task-run.{validated_state.name}",
-        payload={
-            "intended": {
-                "from": str(initial_state.type.value) if initial_state else None,
-                "to": str(validated_state.type.value) if validated_state else None,
-            },
-            "initial_state": (
-                {
-                    "type": str(initial_state.type.value),
-                    "name": initial_state.name,
-                    "message": truncated_to(
-                        state_message_truncation_length, initial_state.message
-                    ),
-                }
-                if initial_state
-                else None
-            ),
-            "validated_state": {
-                "type": str(validated_state.type.value),
-                "name": validated_state.name,
-                "message": truncated_to(
-                    state_message_truncation_length, validated_state.message
-                ),
-            },
-        },
-        resource={
-            "prefect.resource.id": f"prefect.task-run.{task_run.id}",
-            "prefect.resource.name": task_run.name,
-            "prefect.state-message": truncated_to(
-                state_message_truncation_length, validated_state.message
-            ),
-            "prefect.state-name": validated_state.name or "",
-            "prefect.state-timestamp": (
-                validated_state.timestamp.isoformat()
-                if validated_state and validated_state.timestamp
-                else ""
-            ),
-            "prefect.state-type": str(validated_state.type.value),
-        },
-        follows=follows,
-    )
-
-
 async def create_autonomous_task_run(task: Task, parameters: Dict[str, Any]) -> TaskRun:
     """Create a task run in the API for an autonomous task submission and store
     the provided parameters using the existing result storage mechanism.
     """
     async with get_client() as client:
         state = Scheduled()
         if parameters:
```

### Comparing `prefect-client-2.16.9/src/prefect/events/__init__.py` & `prefect-client-2.17.0/src/prefect/events/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/actions.py` & `prefect-client-2.17.0/src/prefect/events/actions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/clients.py` & `prefect-client-2.17.0/src/prefect/events/clients.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Type,
 )
 from uuid import UUID
 
 import orjson
 import pendulum
 from cachetools import TTLCache
+from typing_extensions import Self
 from websockets.client import WebSocketClientProtocol, connect
 from websockets.exceptions import (
     ConnectionClosed,
     ConnectionClosedError,
     ConnectionClosedOK,
 )
 
@@ -114,54 +115,53 @@
         raise ValueError(
             "api_url and api_key must be provided or set in the Prefect configuration"
         )
 
     return api_url, api_key
 
 
-class PrefectCloudEventsClient(EventsClient):
-    """A Prefect Events client that streams Events to a Prefect Cloud Workspace"""
+class PrefectEventsClient(EventsClient):
+    """A Prefect Events client that streams events to a Prefect server"""
 
     _websocket: Optional[WebSocketClientProtocol]
     _unconfirmed_events: List[Event]
 
     def __init__(
         self,
         api_url: str = None,
-        api_key: str = None,
         reconnection_attempts: int = 10,
         checkpoint_every: int = 20,
     ):
         """
         Args:
-            api_url: The base URL for a Prefect Cloud workspace
-            api_key: The API of an actor with the manage_events scope
+            api_url: The base URL for a Prefect server
             reconnection_attempts: When the client is disconnected, how many times
                 the client should attempt to reconnect
             checkpoint_every: How often the client should sync with the server to
                 confirm receipt of all previously sent events
         """
-        api_url, api_key = _get_api_url_and_key(api_url, api_key)
+        api_url = api_url or PREFECT_API_URL.value()
+        if not api_url:
+            raise ValueError(
+                "api_url must be provided or set in the Prefect configuration"
+            )
 
-        socket_url = (
+        self._events_socket_url = (
             api_url.replace("https://", "wss://")
             .replace("http://", "ws://")
             .rstrip("/")
+            + "/events/in"
         )
-
-        self._connect = connect(
-            socket_url + "/events/in",
-            extra_headers={"Authorization": f"bearer {api_key}"},
-        )
+        self._connect = connect(self._events_socket_url)
         self._websocket = None
         self._reconnection_attempts = reconnection_attempts
         self._unconfirmed_events = []
         self._checkpoint_every = checkpoint_every
 
-    async def __aenter__(self) -> "PrefectCloudEventsClient":
+    async def __aenter__(self) -> Self:
         # Don't handle any errors in the initial connection, because these are most
         # likely a permission or configuration issue that should propagate
         await super().__aenter__()
         await self._reconnect()
         return self
 
     async def __aexit__(
@@ -234,14 +234,46 @@
                 if i > 2:
                     # let the first two attempts happen quickly in case this is just
                     # a standard load balancer timeout, but after that, just take a
                     # beat to let things come back around.
                     await asyncio.sleep(1)
 
 
+class PrefectCloudEventsClient(PrefectEventsClient):
+    """A Prefect Events client that streams events to a Prefect Cloud Workspace"""
+
+    def __init__(
+        self,
+        api_url: str = None,
+        api_key: str = None,
+        reconnection_attempts: int = 10,
+        checkpoint_every: int = 20,
+    ):
+        """
+        Args:
+            api_url: The base URL for a Prefect Cloud workspace
+            api_key: The API of an actor with the manage_events scope
+            reconnection_attempts: When the client is disconnected, how many times
+                the client should attempt to reconnect
+            checkpoint_every: How often the client should sync with the server to
+                confirm receipt of all previously sent events
+        """
+        api_url, api_key = _get_api_url_and_key(api_url, api_key)
+        super().__init__(
+            api_url=api_url,
+            reconnection_attempts=reconnection_attempts,
+            checkpoint_every=checkpoint_every,
+        )
+
+        self._connect = connect(
+            self._events_socket_url,
+            extra_headers={"Authorization": f"bearer {api_key}"},
+        )
+
+
 SEEN_EVENTS_SIZE = 500_000
 SEEN_EVENTS_TTL = 120
 
 
 class PrefectCloudEventSubscriber:
     """
     Subscribes to a Prefect Cloud event stream, yielding events as they occur.
```

### Comparing `prefect-client-2.16.9/src/prefect/events/filters.py` & `prefect-client-2.17.0/src/prefect/events/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 from uuid import UUID
 
 import pendulum
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect._internal.schemas.bases import PrefectBaseModel
 from prefect._internal.schemas.fields import DateTimeTZ
+from prefect.utilities.collections import AutoEnum
 
 from .schemas.events import Event, Resource, ResourceSpecification
 
 if HAS_PYDANTIC_V2:
-    from pydantic.v1 import Field
+    from pydantic.v1 import Field, PrivateAttr
 else:
-    from pydantic import Field
+    from pydantic import Field, PrivateAttr
 
 
 class EventDataFilter(PrefectBaseModel, extra="forbid"):
     """A base class for filtering event data."""
 
+    _top_level_filter: "EventFilter | None" = PrivateAttr(None)
+
     def get_filters(self) -> List["EventDataFilter"]:
         return [
             filter
             for filter in [
                 getattr(self, name)
                 for name, field in self.__fields__.items()
                 if issubclass(field.type_, EventDataFilter)
@@ -99,14 +102,18 @@
         description=(
             "Only include events for resources with IDs starting with these prefixes."
         ),
     )
     labels: Optional[ResourceSpecification] = Field(
         None, description="Only include events for resources with these labels"
     )
+    distinct: bool = Field(
+        False,
+        description="Only include events for distinct resources",
+    )
 
     def includes(self, event: Event) -> bool:
         if self.id:
             if not any(event.resource.id == resource_id for resource_id in self.id):
                 return False
 
         if self.id_prefix:
@@ -185,14 +192,19 @@
         if self.id:
             if not any(event.id == id for id in self.id):
                 return False
 
         return True
 
 
+class EventOrder(AutoEnum):
+    ASC = "ASC"
+    DESC = "DESC"
+
+
 class EventFilter(EventDataFilter):
     occurred: EventOccurredFilter = Field(
         default_factory=EventOccurredFilter,
         description="Filter criteria for when the events occurred",
     )
     event: Optional[EventNameFilter] = Field(
         None,
@@ -207,7 +219,12 @@
     related: Optional[EventRelatedFilter] = Field(
         None, description="Filter criteria for the related resources of the event"
     )
     id: EventIDFilter = Field(
         default_factory=EventIDFilter,
         description="Filter criteria for the events' ID",
     )
+
+    order: EventOrder = Field(
+        EventOrder.DESC,
+        description="The order to return filtered events",
+    )
```

### Comparing `prefect-client-2.16.9/src/prefect/events/instrument.py` & `prefect-client-2.17.0/src/prefect/events/instrument.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/related.py` & `prefect-client-2.17.0/src/prefect/events/related.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/schemas/automations.py` & `prefect-client-2.17.0/src/prefect/events/schemas/automations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/schemas/deployment_triggers.py` & `prefect-client-2.17.0/src/prefect/events/schemas/deployment_triggers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/schemas/events.py` & `prefect-client-2.17.0/src/prefect/events/schemas/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/schemas/labelling.py` & `prefect-client-2.17.0/src/prefect/events/schemas/labelling.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/events/utilities.py` & `prefect-client-2.17.0/src/prefect/events/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import pendulum
 
 from prefect._internal.schemas.fields import DateTimeTZ
 
-from .clients import AssertingEventsClient, PrefectCloudEventsClient
+from .clients import (
+    AssertingEventsClient,
+    PrefectCloudEventsClient,
+    PrefectEventsClient,
+)
 from .schemas.events import Event, RelatedResource
-from .worker import EventsWorker, emit_events_to_cloud
+from .worker import EventsWorker, should_emit_events
 
 TIGHT_TIMING = timedelta(minutes=5)
 
 
 def emit_event(
     event: str,
     resource: Dict[str, str],
@@ -38,18 +42,22 @@
             happened more than 5 minutes prior to this event the follows
             relationship will not be set.
 
     Returns:
         The event that was emitted if worker is using a client that emit
         events, otherwise None
     """
-    if not emit_events_to_cloud():
+    if not should_emit_events():
         return None
 
-    operational_clients = [AssertingEventsClient, PrefectCloudEventsClient]
+    operational_clients = [
+        AssertingEventsClient,
+        PrefectCloudEventsClient,
+        PrefectEventsClient,
+    ]
     worker_instance = EventsWorker.instance()
 
     if worker_instance.client_type not in operational_clients:
         return None
 
     event_kwargs = {
         "event": event,
```

### Comparing `prefect-client-2.16.9/src/prefect/events/worker.py` & `prefect-client-2.17.0/src/prefect/events/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 from contextlib import asynccontextmanager
 from contextvars import Context, copy_context
 from typing import Any, Optional, Tuple, Type
 
 from typing_extensions import Self
 
-from prefect._internal.compatibility.experimental import experiment_enabled
 from prefect._internal.concurrency.services import QueueService
-from prefect.settings import PREFECT_API_KEY, PREFECT_API_URL, PREFECT_CLOUD_API_URL
+from prefect.settings import (
+    PREFECT_API_KEY,
+    PREFECT_API_URL,
+    PREFECT_CLOUD_API_URL,
+    PREFECT_EXPERIMENTAL_EVENTS,
+)
 from prefect.utilities.context import temporary_context
 
-from .clients import EventsClient, NullEventsClient, PrefectCloudEventsClient
+from .clients import (
+    EventsClient,
+    NullEventsClient,
+    PrefectCloudEventsClient,
+    PrefectEventsClient,
+)
 from .related import related_resources_from_run_context
 from .schemas.events import Event
 
 
+def should_emit_events() -> bool:
+    return emit_events_to_cloud() or should_emit_events_to_running_server()
+
+
 def emit_events_to_cloud() -> bool:
-    api = PREFECT_API_URL.value()
-    return (
-        experiment_enabled("events_client")
-        and api
-        and api.startswith(PREFECT_CLOUD_API_URL.value())
+    api_url = PREFECT_API_URL.value()
+    return isinstance(api_url, str) and api_url.startswith(
+        PREFECT_CLOUD_API_URL.value()
     )
 
 
+def should_emit_events_to_running_server() -> bool:
+    api_url = PREFECT_API_URL.value()
+    return isinstance(api_url, str) and PREFECT_EXPERIMENTAL_EVENTS
+
+
 class EventsWorker(QueueService[Event]):
     def __init__(
         self, client_type: Type[EventsClient], client_options: Tuple[Tuple[str, Any]]
     ):
         super().__init__(client_type, client_options)
         self.client_type = client_type
         self.client_options = client_options
@@ -63,14 +79,16 @@
         if client_type is None:
             if emit_events_to_cloud():
                 client_type = PrefectCloudEventsClient
                 client_kwargs = {
                     "api_url": PREFECT_API_URL.value(),
                     "api_key": PREFECT_API_KEY.value(),
                 }
+            elif should_emit_events_to_running_server():
+                client_type = PrefectEventsClient
 
             else:
                 client_type = NullEventsClient
 
         # The base class will take care of returning an existing worker with these
         # options if available
         return super().instance(client_type, tuple(client_kwargs.items()))
```

### Comparing `prefect-client-2.16.9/src/prefect/exceptions.py` & `prefect-client-2.17.0/src/prefect/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 """
 Prefect-specific exceptions.
 """
+
 import inspect
 import traceback
 from types import ModuleType, TracebackType
 from typing import Callable, Dict, Iterable, List, Optional, Type
 
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    import pydantic.v1 as pydantic
-else:
-    import pydantic
-
 from httpx._exceptions import HTTPStatusError
+from pydantic import ValidationError
 from rich.traceback import Traceback
 from typing_extensions import Self
 
 import prefect
 
 
 def _trim_traceback(
@@ -178,15 +173,15 @@
     Raised when a parameter does not pass Pydantic type validation.
     """
 
     def __init__(self, msg: str):
         super().__init__(msg)
 
     @classmethod
-    def from_validation_error(cls, exc: pydantic.ValidationError) -> Self:
+    def from_validation_error(cls, exc: ValidationError) -> Self:
         bad_params = [f'{err["loc"][0]}: {err["msg"]}' for err in exc.errors()]
         msg = "Flow run received invalid parameters:\n - " + "\n - ".join(bad_params)
         return cls(msg)
 
 
 class ParameterBindError(TypeError, PrefectException):
     """
```

### Comparing `prefect-client-2.16.9/src/prefect/filesystems.py` & `prefect-client-2.17.0/src/prefect/filesystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     _documentation_url = (
         "https://docs.prefect.io/concepts/filesystems/#remote-file-system"
     )
 
     basepath: str = Field(
         default=...,
         description="Default path for this block to write to.",
-        example="s3://my-bucket/my-folder/",
+        examples=["s3://my-bucket/my-folder/"],
     )
     settings: Dict[str, Any] = Field(
         default_factory=dict,
         description="Additional settings to pass through to fsspec.",
     )
 
     # Cache for the configured fsspec file system used for access
@@ -447,27 +447,27 @@
     _block_type_name = "S3"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/d74b16fe84ce626345adf235a47008fea2869a60-225x225.png"
     _documentation_url = "https://docs.prefect.io/concepts/filesystems/#s3"
 
     bucket_path: str = Field(
         default=...,
         description="An S3 bucket path.",
-        example="my-bucket/a-directory-within",
+        examples=["my-bucket/a-directory-within"],
     )
     aws_access_key_id: Optional[SecretStr] = Field(
         default=None,
         title="AWS Access Key ID",
         description="Equivalent to the AWS_ACCESS_KEY_ID environment variable.",
-        example="AKIAIOSFODNN7EXAMPLE",
+        examples=["AKIAIOSFODNN7EXAMPLE"],
     )
     aws_secret_access_key: Optional[SecretStr] = Field(
         default=None,
         title="AWS Secret Access Key",
         description="Equivalent to the AWS_SECRET_ACCESS_KEY environment variable.",
-        example="wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY",
+        examples=["wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY"],
     )
 
     _remote_file_system: RemoteFileSystem = None
 
     @property
     def basepath(self) -> str:
         return f"s3://{self.bucket_path}"
@@ -545,15 +545,15 @@
 
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/422d13bb838cf247eb2b2cf229ce6a2e717d601b-256x256.png"
     _documentation_url = "https://docs.prefect.io/concepts/filesystems/#gcs"
 
     bucket_path: str = Field(
         default=...,
         description="A GCS bucket path.",
-        example="my-bucket/a-directory-within",
+        examples=["my-bucket/a-directory-within"],
     )
     service_account_info: Optional[SecretStr] = Field(
         default=None,
         description="The contents of a service account keyfile as a JSON string.",
     )
     project: Optional[str] = Field(
         default=None,
@@ -649,15 +649,15 @@
     _block_type_name = "Azure"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/54e3fa7e00197a4fbd1d82ed62494cb58d08c96a-250x250.png"
     _documentation_url = "https://docs.prefect.io/concepts/filesystems/#azure"
 
     bucket_path: str = Field(
         default=...,
         description="An Azure storage bucket path.",
-        example="my-bucket/a-directory-within",
+        examples=["my-bucket/a-directory-within"],
     )
     azure_storage_connection_string: Optional[SecretStr] = Field(
         default=None,
         title="Azure storage connection string",
         description=(
             "Equivalent to the AZURE_STORAGE_CONNECTION_STRING environment variable."
         ),
@@ -800,15 +800,15 @@
     _block_type_name = "SMB"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/3f624663f7beb97d011d011bffd51ecf6c499efc-195x195.png"
     _documentation_url = "https://docs.prefect.io/concepts/filesystems/#smb"
 
     share_path: str = Field(
         default=...,
         description="SMB target (requires <SHARE>, followed by <PATH>).",
-        example="/SHARE/dir/subdir",
+        examples=["/SHARE/dir/subdir"],
     )
     smb_username: Optional[SecretStr] = Field(
         default=None,
         title="SMB Username",
         description="Username with access to the target SMB SHARE.",
     )
     smb_password: Optional[SecretStr] = Field(
```

### Comparing `prefect-client-2.16.9/src/prefect/flow_runs.py` & `prefect-client-2.17.0/src/prefect/flow_runs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/flows.py` & `prefect-client-2.17.0/src/prefect/flows.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,21 +586,21 @@
                 )
                 serialized_parameters[key] = f"<{type(value).__name__}>"
         return serialized_parameters
 
     @sync_compatible
     @deprecated_parameter(
         "schedule",
-        start_date="Mar 2023",
+        start_date="Mar 2024",
         when=lambda p: p is not None,
         help="Use `schedules` instead.",
     )
     @deprecated_parameter(
         "is_schedule_active",
-        start_date="Mar 2023",
+        start_date="Mar 2024",
         when=lambda p: p is not None,
         help="Use `paused` instead.",
     )
     async def to_deployment(
         self,
         name: str,
         interval: Optional[
@@ -1121,18 +1121,19 @@
                 "\nTo schedule a run for this deployment, use the following command:"
             )
             console.print(
                 f"\n\t$ prefect deployment run '{self.name}/{name}'\n",
                 style="blue",
             )
             if PREFECT_UI_URL:
-                console.print(
+                message = (
                     "\nYou can also run your flow via the Prefect UI:"
                     f" [blue]{PREFECT_UI_URL.value()}/deployments/deployment/{deployment_ids[0]}[/]\n"
                 )
+                console.print(message, soft_wrap=True)
 
         return deployment_ids[0]
 
     @overload
     def __call__(self: "Flow[P, NoReturn]", *args: P.args, **kwargs: P.kwargs) -> None:
         # `NoReturn` matches if a type can't be inferred for the function which stops a
         # sync function from matching the `Coroutine` overload
```

### Comparing `prefect-client-2.16.9/src/prefect/futures.py` & `prefect-client-2.17.0/src/prefect/futures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/__init__.py` & `prefect-client-2.17.0/src/prefect/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/base.py` & `prefect-client-2.17.0/src/prefect/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/container.py` & `prefect-client-2.17.0/src/prefect/infrastructure/container.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/kubernetes.py` & `prefect-client-2.17.0/src/prefect/infrastructure/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/process.py` & `prefect-client-2.17.0/src/prefect/infrastructure/process.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/provisioners/__init__.py` & `prefect-client-2.17.0/src/prefect/infrastructure/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/provisioners/cloud_run.py` & `prefect-client-2.17.0/src/prefect/infrastructure/provisioners/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/provisioners/container_instance.py` & `prefect-client-2.17.0/src/prefect/infrastructure/provisioners/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/provisioners/ecs.py` & `prefect-client-2.17.0/src/prefect/infrastructure/provisioners/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/infrastructure/provisioners/modal.py` & `prefect-client-2.17.0/src/prefect/infrastructure/provisioners/modal.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/input/__init__.py` & `prefect-client-2.17.0/src/prefect/input/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/input/actions.py` & `prefect-client-2.17.0/src/prefect/input/actions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/input/run_input.py` & `prefect-client-2.17.0/src/prefect/input/run_input.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/configuration.py` & `prefect-client-2.17.0/src/prefect/logging/configuration.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/filters.py` & `prefect-client-2.17.0/src/prefect/logging/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/formatters.py` & `prefect-client-2.17.0/src/prefect/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/handlers.py` & `prefect-client-2.17.0/src/prefect/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/highlighters.py` & `prefect-client-2.17.0/src/prefect/logging/highlighters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/loggers.py` & `prefect-client-2.17.0/src/prefect/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/logging/logging.yml` & `prefect-client-2.17.0/src/prefect/logging/logging.yml`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/plugins.py` & `prefect-client-2.17.0/src/prefect/plugins.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/pydantic/__init__.py` & `prefect-client-2.17.0/src/prefect/pydantic/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,56 @@
+"""
+This initialization file makes the `BaseModel` and `PrefectBaseModel` classes available for import from the pydantic module within Prefect. This setup allows other parts of the Prefect codebase to use these models without needing to understand the underlying compatibility layer.
+"""
 import typing
 from prefect._internal.pydantic._flags import HAS_PYDANTIC_V2, USE_PYDANTIC_V2
 
 if typing.TYPE_CHECKING:
     # import of virtually everything is supported via `__getattr__` below,
     # but we need them here for type checking and IDE support
     from pydantic import validator, root_validator
-    from .main import BaseModel, PrefectBaseModel, FieldInfo, Field
+    from .main import (
+        BaseModel,
+        PrefectBaseModel,
+        FieldInfo,
+        Field,
+        PrivateAttr,
+        SecretStr,
+        field_validator,
+        model_validator,
+        ConfigDict,
+        ValidationError,
+    )
 
 __all__ = [
     "BaseModel",
     "PrefectBaseModel",
     "Field",
     "FieldInfo",
+    "PrivateAttr",
+    "SecretStr",
     "validator",
     "root_validator",
+    "field_validator",
+    "model_validator",
+    "ConfigDict",
+    "ValidationError",
 ]
 
 _dynamic_imports: "typing.Dict[str, typing.Tuple[str, str]]" = {
     "BaseModel": ("prefect.pydantic", ".main"),
     "PrefectBaseModel": ("prefect.pydantic", ".main"),
     "Field": ("prefect.pydantic", ".main"),
     "FieldInfo": ("prefect.pydantic", ".main"),
+    "PrivateAttr": ("prefect.pydantic", ".main"),
+    "SecretStr": ("prefect.pydantic", ".main"),
+    "field_validator": ("prefect.pydantic", ".main"),
+    "model_validator": ("prefect.pydantic", ".main"),
+    "ConfigDict": ("prefect.pydantic", ".main"),
+    "ValidationError": ("prefect.pydantic", ".main"),
 }
 
 
 def __getattr__(attr_name: str) -> object:
     from importlib import import_module
 
     if attr_name in _dynamic_imports:
```

### Comparing `prefect-client-2.16.9/src/prefect/results.py` & `prefect-client-2.17.0/src/prefect/results.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runner/runner.py` & `prefect-client-2.17.0/src/prefect/runner/runner.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runner/server.py` & `prefect-client-2.17.0/src/prefect/runner/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runner/storage.py` & `prefect-client-2.17.0/src/prefect/runner/storage.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runner/submit.py` & `prefect-client-2.17.0/src/prefect/runner/submit.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runner/utils.py` & `prefect-client-2.17.0/src/prefect/runner/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runtime/deployment.py` & `prefect-client-2.17.0/src/prefect/runtime/deployment.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runtime/flow_run.py` & `prefect-client-2.17.0/src/prefect/runtime/flow_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/runtime/task_run.py` & `prefect-client-2.17.0/src/prefect/runtime/task_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/serializers.py` & `prefect-client-2.17.0/src/prefect/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json` & `prefect-client-2.17.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/server/api/static/prefect-logo-mark-gradient.png` & `prefect-client-2.17.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/settings.py` & `prefect-client-2.17.0/src/prefect/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 
 
 DEFAULT_PROFILES_PATH = Path(__file__).parent.joinpath("profiles.toml")
 
 REMOVED_EXPERIMENTAL_FLAGS = {
     "PREFECT_EXPERIMENTAL_ENABLE_ENHANCED_SCHEDULING_UI",
     "PREFECT_EXPERIMENTAL_ENABLE_ENHANCED_DEPLOYMENT_PARAMETERS",
+    "PREFECT_EXPERIMENTAL_ENABLE_EVENTS_CLIENT",
+    "PREFECT_EXPERIMENTAL_WARN_EVENTS_CLIENT",
 }
 
 
 class Setting(Generic[T]):
     """
     Setting definition type.
     """
@@ -1363,24 +1365,14 @@
 """
 
 PREFECT_EXPERIMENTAL_ENABLE_STATES_ON_FLOW_RUN_GRAPH = Setting(bool, default=True)
 """
 Whether or not to enable flow run states on the flow run graph.
 """
 
-PREFECT_EXPERIMENTAL_ENABLE_EVENTS_CLIENT = Setting(bool, default=True)
-"""
-Whether or not to enable experimental Prefect work pools.
-"""
-
-PREFECT_EXPERIMENTAL_WARN_EVENTS_CLIENT = Setting(bool, default=False)
-"""
-Whether or not to warn when experimental Prefect work pools are used.
-"""
-
 PREFECT_EXPERIMENTAL_ENABLE_WORK_POOLS = Setting(bool, default=True)
 """
 Whether or not to enable experimental Prefect work pools.
 """
 
 PREFECT_EXPERIMENTAL_WARN_WORK_POOLS = Setting(bool, default=False)
 """
@@ -1675,14 +1667,45 @@
 """
 
 PREFECT_API_SERVICES_EVENT_LOGGER_ENABLED = Setting(bool, default=True)
 """
 Whether or not to start the event debug logger service in the server application.
 """
 
+PREFECT_API_SERVICES_TRIGGERS_ENABLED = Setting(bool, default=True)
+"""
+Whether or not to start the triggers service in the server application.
+"""
+
+PREFECT_EVENTS_EXPIRED_BUCKET_BUFFER = Setting(timedelta, default=timedelta(seconds=60))
+"""
+The amount of time to retain expired automation buckets
+"""
+
+PREFECT_EVENTS_PROACTIVE_GRANULARITY = Setting(timedelta, default=timedelta(seconds=5))
+"""
+How frequently proactive automations are evaluated
+"""
+
+PREFECT_API_SERVICES_EVENT_PERSISTER_ENABLED = Setting(bool, default=True)
+"""
+Whether or not to start the event persister service in the server application.
+"""
+
+PREFECT_API_SERVICES_EVENT_PERSISTER_BATCH_SIZE = Setting(int, default=20, gt=0)
+"""
+The number of events the event persister will attempt to insert in one batch.
+"""
+
+PREFECT_API_SERVICES_EVENT_PERSISTER_FLUSH_INTERVAL = Setting(float, default=5, gt=0.0)
+"""
+The maximum number of seconds between flushes of the event persister.
+"""
+
+
 # Deprecated settings ------------------------------------------------------------------
 
 
 # Collect all defined settings ---------------------------------------------------------
 
 SETTING_VARIABLES: Dict[str, Any] = {
     name: val for name, val in tuple(globals().items()) if isinstance(val, Setting)
```

### Comparing `prefect-client-2.16.9/src/prefect/software/base.py` & `prefect-client-2.17.0/src/prefect/software/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/software/conda.py` & `prefect-client-2.17.0/src/prefect/software/conda.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/software/pip.py` & `prefect-client-2.17.0/src/prefect/software/pip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/software/python.py` & `prefect-client-2.17.0/src/prefect/software/python.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/states.py` & `prefect-client-2.17.0/src/prefect/states.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/task_engine.py` & `prefect-client-2.17.0/src/prefect/task_engine.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/task_runners.py` & `prefect-client-2.17.0/src/prefect/task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/task_server.py` & `prefect-client-2.17.0/src/prefect/task_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     )
     task_accepts_parameters = bool(inspect.signature(task.fn).parameters)
 
     return new_enough_state_details and task_accepts_parameters
 
 
 class TaskServer:
-    """This class is responsible for serving tasks that may be executed autonomously by a
-    task runner in the engine.
+    """This class is responsible for serving tasks that may be executed in the background
+    by a task runner via the traditional engine machinery.
 
     When `start()` is called, the task server will open a websocket connection to a
     server-side queue of scheduled task runs. When a scheduled task run is found, the
     scheduled task run is submitted to the engine for execution with a minimal `EngineContext`
     so that the task run can be governed by orchestration rules.
 
     Args:
```

### Comparing `prefect-client-2.16.9/src/prefect/tasks.py` & `prefect-client-2.17.0/src/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/annotations.py` & `prefect-client-2.17.0/src/prefect/utilities/annotations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/asyncutils.py` & `prefect-client-2.17.0/src/prefect/utilities/asyncutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/callables.py` & `prefect-client-2.17.0/src/prefect/utilities/callables.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/collections.py` & `prefect-client-2.17.0/src/prefect/utilities/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/compat.py` & `prefect-client-2.17.0/src/prefect/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/context.py` & `prefect-client-2.17.0/src/prefect/utilities/context.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/dispatch.py` & `prefect-client-2.17.0/src/prefect/utilities/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class Foo(Base):
     ...
 
 key = get_dispatch_key(Foo)  # 'foo'
 lookup_type(Base, key) # Foo
 ```
 """
+
 import abc
 import inspect
 import warnings
 from typing import Any, Dict, Optional, Type, TypeVar
 
 T = TypeVar("T", bound=Type)
```

### Comparing `prefect-client-2.16.9/src/prefect/utilities/dockerutils.py` & `prefect-client-2.17.0/src/prefect/utilities/dockerutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/filesystem.py` & `prefect-client-2.17.0/src/prefect/utilities/filesystem.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/hashing.py` & `prefect-client-2.17.0/src/prefect/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/importtools.py` & `prefect-client-2.17.0/src/prefect/utilities/importtools.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/math.py` & `prefect-client-2.17.0/src/prefect/utilities/math.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/names.py` & `prefect-client-2.17.0/src/prefect/utilities/names.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/processutils.py` & `prefect-client-2.17.0/src/prefect/utilities/processutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/pydantic.py` & `prefect-client-2.17.0/src/prefect/utilities/pydantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     return (subclass_class_fields - parent_class_fields) | (
         subclass_class_fields & parent_class_fields
     )
 
 
 def add_type_dispatch(model_cls: Type[M]) -> Type[M]:
     """
-    Extend a Pydantic model to add a 'type' field that is used a discriminator field
+    Extend a Pydantic model to add a 'type' field that is used as a discriminator field
     to dynamically determine the subtype that when deserializing models.
 
     This allows automatic resolution to subtypes of the decorated model.
 
     If a type field already exists, it should be a string literal field that has a
     constant value for each subclass. The default value of this field will be used as
     the dispatch key.
```

### Comparing `prefect-client-2.16.9/src/prefect/utilities/render_swagger.py` & `prefect-client-2.17.0/src/prefect/utilities/render_swagger.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/schema_tools/hydration.py` & `prefect-client-2.17.0/src/prefect/utilities/schema_tools/hydration.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/schema_tools/validation.py` & `prefect-client-2.17.0/src/prefect/utilities/schema_tools/validation.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/services.py` & `prefect-client-2.17.0/src/prefect/utilities/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/templating.py` & `prefect-client-2.17.0/src/prefect/utilities/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/utilities/visualization.py` & `prefect-client-2.17.0/src/prefect/utilities/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     def link_viz_return_value_to_viz_task(
         self, viz_return_value: Any, viz_task: VizTask
     ) -> None:
         """
         We cannot track booleans, Ellipsis, None, NotImplemented, or the integers from -5 to 256
         because they are singletons.
         """
-        from prefect.engine import UNTRACKABLE_TYPES
+        from prefect.utilities.engine import UNTRACKABLE_TYPES
 
         if (type(viz_return_value) in UNTRACKABLE_TYPES) or (
             isinstance(viz_return_value, int) and (-5 <= viz_return_value <= 256)
         ):
             return
         self.object_id_to_task[id(viz_return_value)] = viz_task
```

### Comparing `prefect-client-2.16.9/src/prefect/workers/base.py` & `prefect-client-2.17.0/src/prefect/workers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
     async def _get_configuration(
         self,
         flow_run: "FlowRun",
     ) -> BaseJobConfiguration:
         deployment = await self._client.read_deployment(flow_run.deployment_id)
         flow = await self._client.read_flow(flow_run.flow_id)
 
-        deployment_vars = deployment.infra_overrides or {}
+        deployment_vars = deployment.job_variables or {}
         flow_run_vars = flow_run.job_variables or {}
         job_variables = {**deployment_vars, **flow_run_vars}
 
         configuration = await self.job_configuration.from_template_and_values(
             base_job_template=self._work_pool.base_job_template,
             values=job_variables,
             client=self._client,
```

### Comparing `prefect-client-2.16.9/src/prefect/workers/block.py` & `prefect-client-2.17.0/src/prefect/workers/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         )
 
         # this piece of logic applies any overrides that may have been set on the
         # deployment; overrides are defined as dot.delimited paths on possibly nested
         # attributes of the infrastructure block
         doc_dict = infra_document.dict()
         infra_dict = doc_dict.get("data", {})
-        for override, value in (deployment.infra_overrides or {}).items():
+        for override, value in (deployment.job_variables or {}).items():
             nested_fields = override.split(".")
             if nested_fields == ["command"]:
                 value = shlex.split(value)
             data = infra_dict
             for field in nested_fields[:-1]:
                 data = data[field]
```

### Comparing `prefect-client-2.16.9/src/prefect/workers/process.py` & `prefect-client-2.17.0/src/prefect/workers/process.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/workers/server.py` & `prefect-client-2.17.0/src/prefect/workers/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect/workers/utilities.py` & `prefect-client-2.17.0/src/prefect/workers/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.16.9/src/prefect_client.egg-info/PKG-INFO` & `prefect-client-2.17.0/src/prefect_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.16.9
+Version: 2.17.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.16.9/src/prefect_client.egg-info/SOURCES.txt` & `prefect-client-2.17.0/src/prefect_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,23 +56,27 @@
 src/prefect/_internal/pydantic/schemas.py
 src/prefect/_internal/pydantic/v1_schema.py
 src/prefect/_internal/pydantic/v2_schema.py
 src/prefect/_internal/pydantic/v2_validated_func.py
 src/prefect/_internal/pydantic/annotations/__init__.py
 src/prefect/_internal/pydantic/annotations/pendulum.py
 src/prefect/_internal/pydantic/utilities/__init__.py
+src/prefect/_internal/pydantic/utilities/config_dict.py
+src/prefect/_internal/pydantic/utilities/field_validator.py
 src/prefect/_internal/pydantic/utilities/model_construct.py
 src/prefect/_internal/pydantic/utilities/model_copy.py
 src/prefect/_internal/pydantic/utilities/model_dump.py
 src/prefect/_internal/pydantic/utilities/model_dump_json.py
 src/prefect/_internal/pydantic/utilities/model_fields.py
+src/prefect/_internal/pydantic/utilities/model_fields_set.py
 src/prefect/_internal/pydantic/utilities/model_json_schema.py
 src/prefect/_internal/pydantic/utilities/model_rebuild.py
 src/prefect/_internal/pydantic/utilities/model_validate.py
 src/prefect/_internal/pydantic/utilities/model_validate_json.py
+src/prefect/_internal/pydantic/utilities/model_validator.py
 src/prefect/_internal/pydantic/utilities/type_adapter.py
 src/prefect/_internal/schemas/__init__.py
 src/prefect/_internal/schemas/bases.py
 src/prefect/_internal/schemas/fields.py
 src/prefect/_internal/schemas/serializers.py
 src/prefect/_internal/schemas/validators.py
 src/prefect/_vendor/__init__.py
@@ -257,14 +261,15 @@
 src/prefect/utilities/asyncutils.py
 src/prefect/utilities/callables.py
 src/prefect/utilities/collections.py
 src/prefect/utilities/compat.py
 src/prefect/utilities/context.py
 src/prefect/utilities/dispatch.py
 src/prefect/utilities/dockerutils.py
+src/prefect/utilities/engine.py
 src/prefect/utilities/filesystem.py
 src/prefect/utilities/hashing.py
 src/prefect/utilities/importtools.py
 src/prefect/utilities/math.py
 src/prefect/utilities/names.py
 src/prefect/utilities/processutils.py
 src/prefect/utilities/pydantic.py
```

### Comparing `prefect-client-2.16.9/src/prefect_client.egg-info/requires.txt` & `prefect-client-2.17.0/src/prefect_client.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 fsspec>=2022.5.0
 graphviz>=0.20.1
 griffe>=0.20.0
 httpcore<2.0.0,>=1.0.5
 httpx[http2]!=0.23.2,>=0.23
 importlib-resources<6.2.0,>=6.1.3
 jsonpatch<2.0,>=1.32
-jsonschema<5.0.0,>=3.2.0
+jsonschema<5.0.0,>=4.0.0
 orjson<4.0,>=3.7
 packaging<24.3,>=21.3
 pathspec>=0.8.0
 pydantic[email]!=2.0.0,!=2.0.1,!=2.1.0,<3.0.0,>=1.10.0
-pydantic_core<3.0.0,>=2.10.0
+pydantic_core<3.0.0,>=2.12.0
 python_dateutil<3.0.0,>=2.8.2
 python-slugify<9.0,>=5.0
 pyyaml<7.0.0,>=5.4.1
 rfc3339-validator<0.2.0,>=0.1.4
 rich<14.0,>=11.0
 ruamel.yaml>=0.17.0
 sniffio<2.0.0,>=1.3.0
```

### Comparing `prefect-client-2.16.9/versioneer.py` & `prefect-client-2.17.0/versioneer.py`

 * *Files identical despite different names*

