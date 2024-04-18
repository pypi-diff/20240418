# Comparing `tmp/prefect-client-2.17.1.tar.gz` & `tmp/prefect-client-2.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-client-2.17.1.tar", last modified: Thu Apr 11 23:58:53 2024, max compression
+gzip compressed data, was "prefect-client-2.18.0.tar", last modified: Thu Apr 18 20:53:58 2024, max compression
```

## Comparing `prefect-client-2.17.1.tar` & `prefect-client-2.18.0.tar`

### file list

```diff
@@ -1,341 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.883499 prefect-client-2.17.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 23:58:51.000000 prefect-client-2.17.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 23:58:51.000000 prefect-client-2.17.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-11 23:58:53.883499 prefect-client-2.17.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-11 23:58:51.000000 prefect-client-2.17.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-11 23:58:51.000000 prefect-client-2.17.1/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 23:58:51.000000 prefect-client-2.17.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 23:58:51.000000 prefect-client-2.17.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-11 23:58:53.883499 prefect-client-2.17.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-11 23:58:51.000000 prefect-client-2.17.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.835499 prefect-client-2.17.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.839499 prefect-client-2.17.1/src/prefect/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/.prefectignore
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.839499 prefect-client-2.17.1/src/prefect/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.839499 prefect-client-2.17.1/src/prefect/_internal/compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/compatibility/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/compatibility/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.843499 prefect-client-2.17.1/src/prefect/_internal/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/cancellation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/concurrency/waiters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.843499 prefect-client-2.17.1/src/prefect/_internal/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.843499 prefect-client-2.17.1/src/prefect/_internal/pydantic/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/annotations/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.847499 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/config_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_construct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_dump_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_fields_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_rebuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validate_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/type_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/v1_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/v2_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pydantic/v2_validated_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/pytz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.847499 prefect-client-2.17.1/src/prefect/_internal/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/schemas/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/schemas/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    32606 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_internal/schemas/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.847499 prefect-client-2.17.1/src/prefect/_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.851499 prefect-client-2.17.1/src/prefect/_vendor/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/datastructures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.851499 prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.851499 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.851499 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/param_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/params.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.855499 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/fastapi/websockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.859499 prefect-client-2.17.1/src/prefect/_vendor/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/_exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/convertors.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/formparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.859499 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/httpsredirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/trustedhost.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/testclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_vendor/starlette/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.859499 prefect-client-2.17.1/src/prefect/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26932 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/blocks/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.863499 prefect-client-2.17.1/src/prefect/client/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   112936 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/orchestration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.863499 prefect-client-2.17.1/src/prefect/client/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    52220 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/schemas/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/client/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.863499 prefect-client-2.17.1/src/prefect/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/concurrency/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.867499 prefect-client-2.17.1/src/prefect/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21353 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41221 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    44302 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.867499 prefect-client-2.17.1/src/prefect/deployments/steps/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/steps/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/steps/pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deployments/steps/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.867499 prefect-client-2.17.1/src/prefect/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/data_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.867499 prefect-client-2.17.1/src/prefect/deprecated/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/orion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/deprecated/packaging/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    89809 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.867499 prefect-client-2.17.1/src/prefect/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/related.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.871499 prefect-client-2.17.1/src/prefect/events/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/schemas/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18422 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/schemas/deployment_triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/schemas/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/schemas/labelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/events/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    35260 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/flow_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70512 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/futures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.871499 prefect-client-2.17.1/src/prefect/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.871499 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/infrastructure/provisioners/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.871499 prefect-client-2.17.1/src/prefect/input/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/input/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/input/run_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.871499 prefect-client-2.17.1/src/prefect/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/highlighters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/logging/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/manifests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/profiles.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/pydantic/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    24731 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48079 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runtime/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runtime/flow_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/runtime/task_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.831499 prefect-client-2.17.1/src/prefect/server/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.831499 prefect-client-2.17.1/src/prefect/server/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.831499 prefect-client-2.17.1/src/prefect/server/api/collections_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/server/api/collections_data/views/
--rw-r--r--   0 runner    (1001) docker     (127)    78423 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/server/api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/server/api/static/prefect-logo-mark-gradient.png
--rw-r--r--   0 runner    (1001) docker     (127)    72895 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.875499 prefect-client-2.17.1/src/prefect/software/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/software/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/software/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/software/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/software/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    20839 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/task_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/task_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    50477 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.879499 prefect-client-2.17.1/src/prefect/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/asyncutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/callables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/dockerutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/importtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/names.py
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/processutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/render_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.879499 prefect-client-2.17.1/src/prefect/utilities/schema_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/schema_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/schema_tools/hydration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/schema_tools/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/slugify.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/utilities/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.883499 prefect-client-2.17.1/src/prefect/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44977 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-11 23:58:51.000000 prefect-client-2.17.1/src/prefect/workers/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:58:53.883499 prefect-client-2.17.1/src/prefect_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-11 23:58:53.000000 prefect-client-2.17.1/src/prefect_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-11 23:58:53.000000 prefect-client-2.17.1/src/prefect_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:58:53.000000 prefect-client-2.17.1/src/prefect_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 23:58:53.000000 prefect-client-2.17.1/src/prefect_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 23:58:53.000000 prefect-client-2.17.1/src/prefect_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    78066 2024-04-11 23:58:51.000000 prefect-client-2.17.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.223805 prefect-client-2.18.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 20:53:54.000000 prefect-client-2.18.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 20:53:54.000000 prefect-client-2.18.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-18 20:53:58.223805 prefect-client-2.18.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-18 20:53:55.000000 prefect-client-2.18.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 20:53:55.000000 prefect-client-2.18.0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-18 20:53:55.000000 prefect-client-2.18.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 20:53:55.000000 prefect-client-2.18.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-18 20:53:58.223805 prefect-client-2.18.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 20:53:55.000000 prefect-client-2.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.171805 prefect-client-2.18.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.179805 prefect-client-2.18.0/src/prefect/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/.prefectignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.179805 prefect-client-2.18.0/src/prefect/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.179805 prefect-client-2.18.0/src/prefect/_internal/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/compatibility/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/compatibility/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.183805 prefect-client-2.18.0/src/prefect/_internal/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18201 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/concurrency/waiters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.183805 prefect-client-2.18.0/src/prefect/_internal/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.183805 prefect-client-2.18.0/src/prefect/_internal/pydantic/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/annotations/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.187805 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/config_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_construct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_fields_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/type_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/v1_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/v2_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pydantic/v2_validated_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13749 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/pytz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.187805 prefect-client-2.18.0/src/prefect/_internal/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/schemas/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/schemas/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32417 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_internal/schemas/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.187805 prefect-client-2.18.0/src/prefect/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.191805 prefect-client-2.18.0/src/prefect/_vendor/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40983 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/datastructures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.191805 prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31968 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.191805 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.191805 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/param_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57083 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.191805 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/fastapi/websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.195805 prefect-client-2.18.0/src/prefect/_vendor/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/_exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/convertors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10450 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/formparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.199805 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/trustedhost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/testclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_vendor/starlette/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24597 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27789 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.199805 prefect-client-2.18.0/src/prefect/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27251 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/blocks/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114797 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/orchestration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/client/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52281 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/schemas/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/client/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/concurrency/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41212 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44293 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/deployments/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/steps/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/steps/pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deployments/steps/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.203805 prefect-client-2.18.0/src/prefect/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/data_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.207805 prefect-client-2.18.0/src/prefect/deprecated/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/orion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/deprecated/packaging/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89809 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.207805 prefect-client-2.18.0/src/prefect/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.207805 prefect-client-2.18.0/src/prefect/events/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19295 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/related.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.207805 prefect-client-2.18.0/src/prefect/events/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/schemas/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/schemas/deployment_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/schemas/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/schemas/labelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/events/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35260 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/flow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70512 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/futures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.211805 prefect-client-2.18.0/src/prefect/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.211805 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41231 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47674 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/infrastructure/provisioners/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.211805 prefect-client-2.18.0/src/prefect/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/input/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18023 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/input/run_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.211805 prefect-client-2.18.0/src/prefect/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/highlighters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/logging/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/profiles.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.211805 prefect-client-2.18.0/src/prefect/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/pydantic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25466 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48079 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runtime/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runtime/flow_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/runtime/task_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.171805 prefect-client-2.18.0/src/prefect/server/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.171805 prefect-client-2.18.0/src/prefect/server/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.171805 prefect-client-2.18.0/src/prefect/server/api/collections_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/server/api/collections_data/views/
+-rw-r--r--   0 runner    (1001) docker     (127)    78423 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/server/api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    73430 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72815 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/software/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/software/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/software/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/software/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/software/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20839 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/task_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/task_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50477 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.215805 prefect-client-2.18.0/src/prefect/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.219805 prefect-client-2.18.0/src/prefect/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/asyncutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/callables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20180 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/dockerutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/processutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/render_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.219805 prefect-client-2.18.0/src/prefect/utilities/schema_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/schema_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/schema_tools/hydration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/schema_tools/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/utilities/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.219805 prefect-client-2.18.0/src/prefect/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44977 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-18 20:53:55.000000 prefect-client-2.18.0/src/prefect/workers/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:53:58.223805 prefect-client-2.18.0/src/prefect_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-18 20:53:57.000000 prefect-client-2.18.0/src/prefect_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-18 20:53:58.000000 prefect-client-2.18.0/src/prefect_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:53:57.000000 prefect-client-2.18.0/src/prefect_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 20:53:57.000000 prefect-client-2.18.0/src/prefect_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 20:53:57.000000 prefect-client-2.18.0/src/prefect_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86829 2024-04-18 20:53:55.000000 prefect-client-2.18.0/versioneer.py
```

### Comparing `prefect-client-2.17.1/LICENSE` & `prefect-client-2.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/MANIFEST.in` & `prefect-client-2.18.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/PKG-INFO` & `prefect-client-2.18.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.17.1
+Version: 2.18.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.17.1/README.md` & `prefect-client-2.18.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/requirements-client.txt` & `prefect-client-2.18.0/requirements-client.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/requirements-dev.txt` & `prefect-client-2.18.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/setup.cfg` & `prefect-client-2.18.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 ignore_errors = True
 
 [versioneer]
 vcs = git
 style = pep440
 versionfile_source = src/prefect/_version.py
 versionfile_build = prefect/_version.py
+version_regex = ^(\d+\.\d+\.\d+)$
 tag_prefix = 
 parentdir_prefix = 
 
 [coverage:run]
 branch = True
 
 [coverage:report]
```

### Comparing `prefect-client-2.17.1/setup.py` & `prefect-client-2.18.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/__init__.py` & `prefect-client-2.18.0/src/prefect/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/_logging.py` & `prefect-client-2.18.0/src/prefect/_internal/_logging.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/compatibility/deprecated.py` & `prefect-client-2.18.0/src/prefect/_internal/compatibility/deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,16 @@
         exclude: Union[set, Dict[str, Any]] = kwargs.pop("exclude", set())
         exclude_type = type(exclude)
 
         if exclude_type is set:
             exclude.add("job_variables")
         elif exclude_type is dict:
             exclude["job_variables"] = True
+        else:
+            exclude = {"job_variables"}
         kwargs["exclude"] = exclude
 
         return super().dict(**kwargs)
 
     @classmethod
     def schema(
         cls, by_alias: bool = True, ref_template: str = default_ref_template
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/compatibility/experimental.py` & `prefect-client-2.18.0/src/prefect/_internal/compatibility/experimental.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/__init__.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/api.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/api.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/calls.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/calls.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/cancellation.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/cancellation.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/event_loop.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/event_loop.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/inspection.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/inspection.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/primitives.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/primitives.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/services.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/threads.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/threads.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/concurrency/waiters.py` & `prefect-client-2.18.0/src/prefect/_internal/concurrency/waiters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/__init__.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/_base_model.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/_base_model.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/_compat.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Functions within this module check for Pydantic V2 compatibility and provide mechanisms for copying,
  dumping, and validating models in a way that is agnostic to the underlying Pydantic version.
 """
+
 import typing
 
 from ._base_model import BaseModel as PydanticBaseModel
 from ._base_model import (
     ConfigDict,
     Field,
     FieldInfo,
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/_flags.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/_flags.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/annotations/pendulum.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/annotations/pendulum.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/config_dict.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/config_dict.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/field_validator.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/field_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Conditional decorator for fields depending on Pydantic version.
 """
 
 import functools
 from inspect import signature
-from typing import TYPE_CHECKING, Any, Callable, Dict, Literal, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Literal, TypeVar, Union
 
 from typing_extensions import TypeAlias
 
 from prefect._internal.pydantic._flags import HAS_PYDANTIC_V2, USE_V2_MODELS
 
 FieldValidatorModes: TypeAlias = Literal["before", "after", "wrap", "plain"]
 T = TypeVar("T", bound=Callable[..., Any])
@@ -17,30 +17,47 @@
     from prefect._internal.pydantic._compat import BaseModel
 
 
 def field_validator(
     field: str,
     /,
     *fields: str,
-    mode: FieldValidatorModes = "after",  # v2 only
+    mode: FieldValidatorModes = "after",
     check_fields: Union[bool, None] = None,
-    pre: bool = False,  # v1 only
-    allow_reuse: Optional[bool] = None,
-    always: bool = False,  # v1 only
 ) -> Callable[[Any], Any]:
     """Usage docs: https://docs.pydantic.dev/2.7/concepts/validators/#field-validators
     Returns a decorator that conditionally applies Pydantic's `field_validator` or `validator`,
     based on the Pydantic version available, for specified field(s) of a Pydantic model.
 
     In Pydantic V2, it uses `field_validator` allowing more granular control over validation,
     including pre-validation and post-validation modes. In Pydantic V1, it falls back to
     using `validator`, which is less flexible but maintains backward compatibility.
 
     Decorate methods on the class indicating that they should be used to validate fields.
 
+    !!! note Replacing Pydantic V1 `pre=True` kwarg:
+    To replace a @validator that uses Pydantic V1's `pre` parameter, e.g. `@validator('a', pre=True)`,
+    you can use `mode='before'`, e.g. @field_validator('a', mode='before').
+
+    If a user has Pydantic V1 installed, `mode` will map to the `pre` parameter of `validator` if the value is `before`.
+
+    !!! note Replacing Pydantic V1 `always=True` kwarg:
+    To replace a @validator that uses Pydantic V1's `always` parameter, e.g. `@validator('a', always=True)`,
+    you can use the @model_validator (not the @field_validator) with the `mode='before'` parameter, (and also add a check that the field is not None, if necessary).
+
+    Read more discussion on that here: https://github.com/pydantic/pydantic/discussions/6337
+
+    !!! note Replacing Pydantic V1 `allow_reuse=True` kwarg:
+    To replace a @validator that uses Pydantic V1's `allow_reuse=True` parameter, e.g. `@validator('a', allow_reuse=True)`,
+    you can simply remove the `allow_reuse` parameter when replacing the decorator, e.g. `@field_validator('a')`. This is because
+    Pydantic V2 by default allows reuse of the decorated function, rendering the kwarg necessary), while Pydantic V1 required explicit
+    declaration of `allow_reuse=True`.
+
+    https://docs.pydantic.dev/2.0/migration/#the-allow_reuse-keyword-argument-is-no-longer-necessary
+
     Example usage:
     ```py
     from typing import Any
 
     from pydantic import (
         BaseModel,
         ValidationError,
@@ -116,20 +133,18 @@
         ) -> Any:
             filtered_kwargs: Dict[str, Any] = {
                 k: v for k, v in kwargs.items() if k in validate_func_params
             }
 
             return validate_func(cls, v, **filtered_kwargs)
 
-        # In Pydantic V1, `allow_reuse` is by default False, while in Pydantic V2, it is by default True.
-        # We default to False in Pydantic V1 to maintain backward compatibility
-        # e.g. One uses @validator("a", pre=True, allow_reuse=True) in Pydantic V1
+        # Map Pydantic V2's `mode` to Pydantic V1's `pre` parameter for use in `@validator`
+        pre: bool = mode == "before"
+
         validator_kwargs: Dict[str, Any] = {
             "pre": pre,
-            "always": always,
             "check_fields": check_fields if check_fields is not None else True,
-            "allow_reuse": allow_reuse if allow_reuse is not None else False,
         }
 
         return validator(field, *fields, **validator_kwargs)(wrapper)  # type: ignore
 
     return decorator
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_construct.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_construct.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_copy.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_copy.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_dump.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         round_trip: If True, dumped values should be valid as input for non-idempotent types such as Json[T].
         warnings: Whether to log warnings when invalid fields are encountered.
         serialize_as_any: Whether to serialize fields with duck-typing serialization behavior.
 
     Returns:
         A dictionary representation of the model.
     """
-    if USE_V2_MODELS:
+    if USE_V2_MODELS and hasattr(model_instance, "model_dump"):
         return model_instance.model_dump(
             mode=mode,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_dump_json.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_dump_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_fields.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_fields_set.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_fields_set.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_json_schema.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_json_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_rebuild.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_rebuild.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validate.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return model_instance.model_validate(
             obj,
             strict=strict,
             from_attributes=from_attributes,
             context=context,
         )
     else:
-        return getattr(model_instance, "validate")(obj)
+        return getattr(model_instance, "parse_obj")(obj)
 
 
 class ModelValidateMixin(BaseModel):
     @classmethod
     def model_validate(
         cls: typing.Type["Self"],
         obj: typing.Any,
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validate_json.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validate_json.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/model_validator.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/model_validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     from prefect._internal.pydantic._compat import BaseModel
 
 
 def model_validator(
     _func: Optional[Callable] = None,
     *,
     mode: Literal["wrap", "before", "after"] = "before",  # v2 only
-    pre: bool = False,  # v1 only
-    skip_on_failure: bool = False,  # v1 only
 ) -> Any:
     """Usage docs: https://docs.pydantic.dev/2.6/concepts/validators/#model-validators
 
     A decorator designed for Pydantic model methods to facilitate additional validations.
     It can be applied to instance methods, class methods, or static methods of a class,
     wrapping around the designated function to inject validation logic.
 
@@ -29,14 +27,23 @@
 
     The actual handling of method types (instance, class, or static) is governed by the class
     definition itself, using Python's standard `@classmethod` and `@staticmethod` decorators
     where appropriate. This decorator simply intercepts the method call, allowing for custom
     validation logic before, after, or wrapping the original method call, depending on the
     `mode` parameter.
 
+    !!! note Replacing Pydantic V1 `pre=True` kwarg:
+    To replace a @root_validator that uses Pydantic V1's `pre=True` parameter, e.g. `@root_validator('a', pre=True)`,
+    you can use the @model_validator with the `mode='before'` parameter, (and also add a check that the field is not None, if necessary).
+    This will map to the `pre` parameter of `root_validator` in Pydantic V1, if the value is `True`.
+
+    !!! note Replacing Pydantic V1 `skip_on_failure=True` kwarg:
+    To replace a @root_validator that uses Pydantic V1's `skip_on_failure=True` parameter, e.g. `@root_validator('a', skip_on_failure=True)`,
+    we'll simply remove it. Pydantic V2 does not have an equivalent parameter, and we use it in only 3 places in Prefect, none of which are critical.
+
     Args:
         _func: The function to be decorated. If None, the decorator is applied with parameters.
         mode: Specifies when the validation should occur. 'before' or 'after' are for v1 compatibility,
               'wrap' introduces v2 behavior where the validation wraps the original call.
         pre: (v1 only) If True, the validator is called before Pydantic's own validators.
         skip_on_failure: (v1 only) If True, skips validation if an earlier validation failed.
 
@@ -65,15 +72,16 @@
         @functools.wraps(validate_func)
         def wrapper(
             cls: "BaseModel",
             v: Any,
         ) -> Any:
             return validate_func(cls, v)
 
+        pre: bool = mode == "before"
+
         return root_validator(
             pre=pre,
-            skip_on_failure=skip_on_failure,
         )(wrapper)  # type: ignore
 
     if _func is None:
         return decorator
     return decorator(_func)
```

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/utilities/type_adapter.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/utilities/type_adapter.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/v1_schema.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/v1_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/v2_schema.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/v2_schema.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pydantic/v2_validated_func.py` & `prefect-client-2.18.0/src/prefect/_internal/pydantic/v2_validated_func.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/pytz.py` & `prefect-client-2.18.0/src/prefect/_internal/pytz.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/schemas/bases.py` & `prefect-client-2.18.0/src/prefect/_internal/schemas/bases.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/schemas/fields.py` & `prefect-client-2.18.0/src/prefect/_internal/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/schemas/serializers.py` & `prefect-client-2.18.0/src/prefect/_internal/schemas/serializers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_internal/schemas/validators.py` & `prefect-client-2.18.0/src/prefect/_internal/schemas/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,20 +368,14 @@
     else:
         values["paused"] = False
         values["is_schedule_active"] = True
 
     return values
 
 
-def interval_schedule_must_be_positive(v: datetime.timedelta) -> datetime.timedelta:
-    if v.total_seconds() <= 0:
-        raise ValueError("The interval must be positive")
-    return v
-
-
 def default_anchor_date(v: DateTimeTZ) -> DateTimeTZ:
     if v is None:
         return pendulum.now("UTC")
     return pendulum.instance(v)
 
 
 def get_valid_timezones(v: str) -> Tuple[str, ...]:
```

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/__init__.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/applications.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/concurrency.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/datastructures.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/models.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/dependencies/utils.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/encoders.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/exception_handlers.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/exceptions.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/docs.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/models.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/models.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/openapi/utils.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/param_functions.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/params.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/responses.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/routing.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/__init__.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/api_key.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/http.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/oauth2.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/security/open_id_connect_url.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/fastapi/utils.py` & `prefect-client-2.18.0/src/prefect/_vendor/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/_compat.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/_compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/_exception_handler.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/_exception_handler.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/_utils.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/_utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/applications.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/applications.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/authentication.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/background.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/background.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/concurrency.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/config.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/config.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/convertors.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/convertors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/datastructures.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/datastructures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/endpoints.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/endpoints.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/exceptions.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/formparsers.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/formparsers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/__init__.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/authentication.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/base.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/cors.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/errors.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/exceptions.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/gzip.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/httpsredirect.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/sessions.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/trustedhost.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/middleware/wsgi.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/requests.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/requests.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/responses.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/routing.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/routing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/schemas.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/schemas.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/staticfiles.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/staticfiles.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/status.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/status.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/templating.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/testclient.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/testclient.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/types.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/types.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_vendor/starlette/websockets.py` & `prefect-client-2.18.0/src/prefect/_vendor/starlette/websockets.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/_version.py` & `prefect-client-2.18.0/src/prefect/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.20 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
+import functools
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "$Format:%d$"
     git_full = "$Format:%H$"
     git_date = "$Format:%ci$"
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "pep440"
     cfg.tag_prefix = ""
@@ -47,50 +57,64 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
 
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen(
                 [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
             )
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
@@ -102,15 +126,19 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -133,21 +161,21 @@
             "Tried directories %s but none started with prefix %s"
             % (str(rootdirs), parentdir_prefix)
         )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -155,21 +183,25 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -232,26 +264,35 @@
         "dirty": False,
         "error": "no suitable tags",
         "date": None,
     }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
@@ -260,28 +301,28 @@
         [
             "describe",
             "--tags",
             "--dirty",
             "--always",
             "--long",
             "--match",
-            "%s*" % tag_prefix,
+            f"{tag_prefix}[[:digit:]]*",
         ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
@@ -352,35 +393,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -396,15 +437,15 @@
         # exception #1
         rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -425,31 +466,49 @@
             rendered += ".dev0"
         rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -468,15 +527,15 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -497,15 +556,15 @@
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -519,15 +578,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -539,15 +598,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -559,15 +618,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {
             "version": "unknown",
             "full-revisionid": pieces.get("long"),
             "dirty": None,
             "error": pieces["error"],
@@ -601,15 +660,15 @@
         "full-revisionid": pieces["long"],
         "dirty": pieces["dirty"],
         "error": None,
         "date": pieces.get("date"),
     }
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
```

### Comparing `prefect-client-2.17.1/src/prefect/agent.py` & `prefect-client-2.18.0/src/prefect/agent.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/artifacts.py` & `prefect-client-2.18.0/src/prefect/artifacts.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/blocks/abstract.py` & `prefect-client-2.18.0/src/prefect/blocks/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 from abc import ABC, abstractmethod
+from contextlib import contextmanager
 from logging import Logger
 from pathlib import Path
-from typing import Any, BinaryIO, Dict, Generic, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    BinaryIO,
+    Dict,
+    Generator,
+    Generic,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 from typing_extensions import Self
 
 from prefect.blocks.core import Block
 from prefect.exceptions import MissingContextError
 from prefect.logging.loggers import get_logger, get_run_logger
 
@@ -44,14 +56,21 @@
 
         If a service offers various clients, this method can accept
         a `client_type` keyword argument to get the desired client
         within the service.
         """
 
 
+class NotificationError(Exception):
+    """Raised if a notification block fails to send a notification."""
+
+    def __init__(self, log: str) -> None:
+        self.log = log
+
+
 class NotificationBlock(Block, ABC):
     """
     Block that represents a resource in an external system that is able to send notifications.
     """
 
     _block_schema_capabilities = ["notify"]
     _events_excluded_methods = Block._events_excluded_methods + ["notify"]
@@ -78,14 +97,28 @@
         Send a notification.
 
         Args:
             body: The body of the notification.
             subject: The subject of the notification.
         """
 
+    _raise_on_failure: bool = False
+
+    @contextmanager
+    def raise_on_failure(self) -> Generator[None, None, None]:
+        """
+        Context manager that, while active, causes the block to raise errors if it
+        encounters a failure sending notifications.
+        """
+        self._raise_on_failure = True
+        try:
+            yield
+        finally:
+            self._raise_on_failure = False
+
 
 class JobRun(ABC, Generic[T]):  # not a block
     """
     Represents a job run in an external system. Allows waiting
     for the job run's completion and fetching its results.
     """
```

### Comparing `prefect-client-2.17.1/src/prefect/blocks/core.py` & `prefect-client-2.18.0/src/prefect/blocks/core.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/blocks/fields.py` & `prefect-client-2.18.0/src/prefect/blocks/fields.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/blocks/kubernetes.py` & `prefect-client-2.18.0/src/prefect/blocks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/blocks/notifications.py` & `prefect-client-2.18.0/src/prefect/blocks/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import logging
 from abc import ABC
 from typing import Dict, List, Optional
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
+from prefect.logging import LogEavesdropper
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import AnyHttpUrl, Field, SecretStr
 else:
     from pydantic import AnyHttpUrl, Field, SecretStr
 
 from typing_extensions import Literal
 
-from prefect.blocks.abstract import NotificationBlock
+from prefect.blocks.abstract import NotificationBlock, NotificationError
 from prefect.blocks.fields import SecretDict
 from prefect.events.instrument import instrument_instance_method_call
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.templating import apply_values, find_placeholders
 
 PREFECT_NOTIFY_TYPE_DEFAULT = "prefect_default"
 
@@ -57,18 +59,25 @@
         self._apprise_client.add(url.get_secret_value())
 
     def block_initialization(self) -> None:
         self._start_apprise_client(self.url)
 
     @sync_compatible
     @instrument_instance_method_call()
-    async def notify(self, body: str, subject: Optional[str] = None):
-        await self._apprise_client.async_notify(
-            body=body, title=subject, notify_type=self.notify_type
-        )
+    async def notify(
+        self,
+        body: str,
+        subject: Optional[str] = None,
+    ):
+        with LogEavesdropper("apprise", level=logging.DEBUG) as eavesdropper:
+            result = await self._apprise_client.async_notify(
+                body=body, title=subject, notify_type=self.notify_type
+            )
+        if not result and self._raise_on_failure:
+            raise NotificationError(log=eavesdropper.text())
 
 
 class AppriseNotificationBlock(AbstractAppriseNotificationBlock, ABC):
     """
     A base class for sending notifications using Apprise, through webhook URLs.
     """
```

### Comparing `prefect-client-2.17.1/src/prefect/blocks/system.py` & `prefect-client-2.18.0/src/prefect/blocks/system.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/blocks/webhook.py` & `prefect-client-2.18.0/src/prefect/blocks/webhook.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/base.py` & `prefect-client-2.18.0/src/prefect/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,19 +189,26 @@
 
     Additionally, this client will always call `raise_for_status` on responses.
 
     For more details on rate limit headers, see:
     [Configuring Cloudflare Rate Limiting](https://support.cloudflare.com/hc/en-us/articles/115001635128-Configuring-Rate-Limiting-from-UI)
     """
 
-    def __init__(self, *args, enable_csrf_support: bool = False, **kwargs):
+    def __init__(
+        self,
+        *args,
+        enable_csrf_support: bool = False,
+        raise_on_all_errors: bool = True,
+        **kwargs,
+    ):
         self.enable_csrf_support: bool = enable_csrf_support
         self.csrf_token: Optional[str] = None
         self.csrf_token_expiration: Optional[datetime] = None
         self.csrf_client_id: uuid.UUID = uuid.uuid4()
+        self.raise_on_all_errors: bool = raise_on_all_errors
 
         super().__init__(*args, **kwargs)
 
         user_agent = (
             f"prefect/{prefect.__version__} (API {constants.SERVER_API_VERSION})"
         )
         self.headers["User-Agent"] = user_agent
@@ -341,18 +348,16 @@
                 httpx.LocalProtocolError,
             ),
         )
 
         # Convert to a Prefect response to add nicer errors messages
         response = PrefectResponse.from_httpx_response(response)
 
-        # Always raise bad responses
-        # NOTE: We may want to remove this and handle responses per route in the
-        #       `PrefectClient`
-        response.raise_for_status()
+        if self.raise_on_all_errors:
+            response.raise_for_status()
 
         return response
 
     async def _add_csrf_headers(self, request: Request):
         now = datetime.now(timezone.utc)
 
         if not self.enable_csrf_support:
```

### Comparing `prefect-client-2.17.1/src/prefect/client/cloud.py` & `prefect-client-2.18.0/src/prefect/client/cloud.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/collections.py` & `prefect-client-2.18.0/src/prefect/client/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/orchestration.py` & `prefect-client-2.18.0/src/prefect/client/orchestration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from contextlib import AsyncExitStack
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
+    NoReturn,
     Optional,
     Set,
     Tuple,
     Union,
 )
 from uuid import UUID, uuid4
 
@@ -19,23 +20,18 @@
 import httpcore
 import httpx
 import pendulum
 
 from prefect._internal.compatibility.deprecated import (
     handle_deprecated_infra_overrides_parameter,
 )
-from prefect._internal.compatibility.experimental import (
-    EXPERIMENTAL_WARNING,
-    ExperimentalFeature,
-    experiment_enabled,
-)
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect.settings import (
-    PREFECT_EXPERIMENTAL_WARN,
-    PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES,
+    PREFECT_API_SERVICES_TRIGGERS_ENABLED,
+    PREFECT_EXPERIMENTAL_EVENTS,
 )
 
 if HAS_PYDANTIC_V2:
     import pydantic.v1 as pydantic
 else:
     import pydantic
 
@@ -129,15 +125,15 @@
     DeploymentSort,
     FlowRunSort,
     FlowSort,
     LogSort,
     TaskRunSort,
 )
 from prefect.deprecated.data_documents import DataDocument
-from prefect.events.schemas.automations import Automation, ExistingAutomation
+from prefect.events.schemas.automations import Automation, AutomationCore
 from prefect.logging import get_logger
 from prefect.settings import (
     PREFECT_API_DATABASE_CONNECTION_URL,
     PREFECT_API_ENABLE_HTTP2,
     PREFECT_API_KEY,
     PREFECT_API_REQUEST_TIMEOUT,
     PREFECT_API_SSL_CERT_FILE,
@@ -157,14 +153,20 @@
 
 
 class ServerType(AutoEnum):
     EPHEMERAL = AutoEnum.auto()
     SERVER = AutoEnum.auto()
     CLOUD = AutoEnum.auto()
 
+    def supports_automations(self) -> bool:
+        if self == ServerType.CLOUD:
+            return True
+
+        return PREFECT_EXPERIMENTAL_EVENTS and PREFECT_API_SERVICES_TRIGGERS_ENABLED
+
 
 def get_client(httpx_settings: Optional[dict] = None) -> "PrefectClient":
     """
     Retrieve a HTTP client for communicating with the Prefect REST API.
 
     The client must be context managed; for example:
 
@@ -564,29 +566,14 @@
 
         Raises:
             httpx.RequestError: if the Prefect API does not successfully create a run for any reason
 
         Returns:
             The flow run model
         """
-        if job_variables is not None and experiment_enabled("flow_run_infra_overrides"):
-            if (
-                PREFECT_EXPERIMENTAL_WARN
-                and PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES
-            ):
-                warnings.warn(
-                    EXPERIMENTAL_WARNING.format(
-                        feature="Flow run job variables",
-                        group="flow_run_infra_overrides",
-                        help="To use this feature, update your workers to Prefect 2.16.4 or later. ",
-                    ),
-                    ExperimentalFeature,
-                    stacklevel=3,
-                )
-
         parameters = parameters or {}
         context = context or {}
         state = state or prefect.states.Scheduled()
         tags = tags or []
 
         flow_run_create = DeploymentFlowRunCreate(
             parameters=parameters,
@@ -699,29 +686,14 @@
                 any existing tags.
             infrastructure_pid: The id of flow run as returned by an
                 infrastructure block.
 
         Returns:
             an `httpx.Response` object from the PATCH request
         """
-        if job_variables is not None and experiment_enabled("flow_run_infra_overrides"):
-            if (
-                PREFECT_EXPERIMENTAL_WARN
-                and PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES
-            ):
-                warnings.warn(
-                    EXPERIMENTAL_WARNING.format(
-                        feature="Flow run job variables",
-                        group="flow_run_infra_overrides",
-                        help="To use this feature, update your workers to Prefect 2.16.4 or later. ",
-                    ),
-                    ExperimentalFeature,
-                    stacklevel=3,
-                )
-
         params = {}
         if flow_version is not None:
             params["flow_version"] = flow_version
         if parameters is not None:
             params["parameters"] = parameters
         if name is not None:
             params["name"] = name
@@ -2994,42 +2966,14 @@
 
     async def read_worker_metadata(self) -> Dict[str, Any]:
         """Reads worker metadata stored in Prefect collection registry."""
         response = await self._client.get("collections/views/aggregate-worker-metadata")
         response.raise_for_status()
         return response.json()
 
-    async def create_automation(self, automation: Automation) -> UUID:
-        """Creates an automation in Prefect Cloud."""
-        if self.server_type != ServerType.CLOUD:
-            raise RuntimeError("Automations are only supported for Prefect Cloud.")
-
-        response = await self._client.post(
-            "/automations/",
-            json=automation.dict(json_compatible=True),
-        )
-
-        return UUID(response.json()["id"])
-
-    async def read_resource_related_automations(
-        self, resource_id: str
-    ) -> List[ExistingAutomation]:
-        if self.server_type != ServerType.CLOUD:
-            raise RuntimeError("Automations are only supported for Prefect Cloud.")
-
-        response = await self._client.get(f"/automations/related-to/{resource_id}")
-        response.raise_for_status()
-        return pydantic.parse_obj_as(List[ExistingAutomation], response.json())
-
-    async def delete_resource_owned_automations(self, resource_id: str):
-        if self.server_type != ServerType.CLOUD:
-            raise RuntimeError("Automations are only supported for Prefect Cloud.")
-
-        await self._client.delete(f"/automations/owned-by/{resource_id}")
-
     async def increment_concurrency_slots(
         self, names: List[str], slots: int, mode: str
     ) -> httpx.Response:
         return await self._client.post(
             "/v2/concurrency_limits/increment",
             json={"names": names, "slots": slots, "mode": mode},
         )
@@ -3161,14 +3105,129 @@
         Args:
             flow_run_id: The flow run id.
             key: The input key.
         """
         response = await self._client.delete(f"/flow_runs/{flow_run_id}/input/{key}")
         response.raise_for_status()
 
+    def _raise_for_unsupported_automations(self) -> NoReturn:
+        if not PREFECT_EXPERIMENTAL_EVENTS:
+            raise RuntimeError(
+                "The current server and client configuration does not support "
+                "events.  Enable experimental events support with the "
+                "PREFECT_EXPERIMENTAL_EVENTS setting."
+            )
+        else:
+            raise RuntimeError(
+                "The current server and client configuration does not support "
+                "automations.  Enable experimental automations with the "
+                "PREFECT_API_SERVICES_TRIGGERS_ENABLED setting."
+            )
+
+    async def create_automation(self, automation: AutomationCore) -> UUID:
+        """Creates an automation in Prefect Cloud."""
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.post(
+            "/automations/",
+            json=automation.dict(json_compatible=True),
+        )
+
+        return UUID(response.json()["id"])
+
+    async def read_automations(self) -> List[Automation]:
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.post("/automations/filter")
+        response.raise_for_status()
+        return pydantic.parse_obj_as(List[Automation], response.json())
+
+    async def find_automation(
+        self, id_or_name: str, exit_if_not_found: bool = True
+    ) -> Optional[Automation]:
+        try:
+            id = UUID(id_or_name)
+        except ValueError:
+            id = None
+
+        if id:
+            automation = await self.read_automation(id)
+            if automation:
+                return automation
+
+        automations = await self.read_automations()
+
+        # Look for it by an exact name
+        for automation in automations:
+            if automation.name == id_or_name:
+                return automation
+
+        # Look for it by a case-insensitive name
+        for automation in automations:
+            if automation.name.lower() == id_or_name.lower():
+                return automation
+
+        return None
+
+    async def read_automation(self, automation_id: UUID) -> Optional[Automation]:
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.get(f"/automations/{automation_id}")
+        if response.status_code == 404:
+            return None
+        response.raise_for_status()
+        return Automation.parse_obj(response.json())
+
+    async def pause_automation(self, automation_id: UUID):
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.patch(
+            f"/automations/{automation_id}", json={"enabled": False}
+        )
+        response.raise_for_status()
+
+    async def resume_automation(self, automation_id: UUID):
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.patch(
+            f"/automations/{automation_id}", json={"enabled": True}
+        )
+        response.raise_for_status()
+
+    async def delete_automation(self, automation_id: UUID):
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.delete(f"/automations/{automation_id}")
+        if response.status_code == 404:
+            return
+
+        response.raise_for_status()
+
+    async def read_resource_related_automations(
+        self, resource_id: str
+    ) -> List[Automation]:
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        response = await self._client.get(f"/automations/related-to/{resource_id}")
+        response.raise_for_status()
+        return pydantic.parse_obj_as(List[Automation], response.json())
+
+    async def delete_resource_owned_automations(self, resource_id: str):
+        if not self.server_type.supports_automations():
+            self._raise_for_unsupported_automations()
+
+        await self._client.delete(f"/automations/owned-by/{resource_id}")
+
     async def __aenter__(self):
         """
         Start the client.
 
         If the client is already started, this will raise an exception.
 
         If the client is already closed, this will raise an exception. Use a new client
```

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/__init__.py` & `prefect-client-2.18.0/src/prefect/client/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/actions.py` & `prefect-client-2.18.0/src/prefect/client/schemas/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import jsonschema
 
 from prefect._internal.compatibility.deprecated import DeprecatedInfraOverridesField
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 
 if HAS_PYDANTIC_V2:
-    from pydantic.v1 import Field, conint, root_validator, validator
+    from pydantic.v1 import Field, root_validator, validator
 else:
-    from pydantic import Field, conint, root_validator, validator
+    from pydantic import Field, root_validator, validator
 
 import prefect.client.schemas.objects as objects
 from prefect._internal.schemas.bases import ActionBaseModel
 from prefect._internal.schemas.fields import DateTimeTZ
 from prefect._internal.schemas.serializers import orjson_dumps_extra_compatible
 from prefect._internal.schemas.validators import (
     raise_on_name_alphanumeric_dashes_only,
@@ -22,14 +22,15 @@
     remove_old_deployment_fields,
     return_none_schedule,
     validate_message_template_variables,
     validate_name_present_on_nonanonymous_blocks,
 )
 from prefect.client.schemas.objects import StateDetails, StateType
 from prefect.client.schemas.schedules import SCHEDULE_TYPES
+from prefect.types import NonNegativeInteger
 from prefect.utilities.collections import listrepr
 from prefect.utilities.pydantic import get_class_fields_only
 
 if TYPE_CHECKING:
     from prefect.deprecated.data_documents import DataDocument
     from prefect.results import BaseResult
 
@@ -521,15 +522,15 @@
         default_factory=dict,
         description="The base job template for the work pool.",
     )
     is_paused: bool = Field(
         default=False,
         description="Whether the work pool is paused.",
     )
-    concurrency_limit: Optional[conint(ge=0)] = Field(
+    concurrency_limit: Optional[NonNegativeInteger] = Field(
         default=None, description="A concurrency limit for the work pool."
     )
 
 
 class WorkPoolUpdate(ActionBaseModel):
     """Data used by the Prefect REST API to update a work pool."""
```

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/filters.py` & `prefect-client-2.18.0/src/prefect/client/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/objects.py` & `prefect-client-2.18.0/src/prefect/client/schemas/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 import orjson
 import pendulum
 
 from prefect._internal.compatibility.deprecated import (
     DeprecatedInfraOverridesField,
 )
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
+from prefect.types import NonNegativeInteger, PositiveInteger
 
 if HAS_PYDANTIC_V2:
-    from pydantic.v1 import Field, HttpUrl, conint, root_validator, validator
+    from pydantic.v1 import Field, HttpUrl, root_validator, validator
 else:
-    from pydantic import Field, HttpUrl, conint, root_validator, validator
+    from pydantic import Field, HttpUrl, root_validator, validator
 
 from typing_extensions import Literal
 
 from prefect._internal.schemas.bases import ObjectBaseModel, PrefectBaseModel
 from prefect._internal.schemas.fields import CreatedBy, DateTimeTZ, UpdatedBy
 from prefect._internal.schemas.validators import (
     get_or_create_run_name,
@@ -1184,18 +1185,18 @@
     name: str = Field(default=..., description="The name of the work queue.")
     description: Optional[str] = Field(
         default="", description="An optional description for the work queue."
     )
     is_paused: bool = Field(
         default=False, description="Whether or not the work queue is paused."
     )
-    concurrency_limit: Optional[conint(ge=0)] = Field(
+    concurrency_limit: Optional[NonNegativeInteger] = Field(
         default=None, description="An optional concurrency limit for the work queue."
     )
-    priority: conint(ge=1) = Field(
+    priority: PositiveInteger = Field(
         default=1,
         description=(
             "The queue's priority. Lower values are higher priority (1 is the highest)."
         ),
     )
     work_pool_name: Optional[str] = Field(default=None)
     # Will be required after a future migration
@@ -1347,15 +1348,15 @@
     base_job_template: Dict[str, Any] = Field(
         default_factory=dict, description="The work pool's base job template."
     )
     is_paused: bool = Field(
         default=False,
         description="Pausing the work pool stops the delivery of all work.",
     )
-    concurrency_limit: Optional[conint(ge=0)] = Field(
+    concurrency_limit: Optional[NonNegativeInteger] = Field(
         default=None, description="A concurrency limit for the work pool."
     )
     status: Optional[WorkPoolStatus] = Field(
         default=None, description="The current status of the work pool."
     )
 
     # this required field has a default of None so that the custom validator
```

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/responses.py` & `prefect-client-2.18.0/src/prefect/client/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/schedules.py` & `prefect-client-2.18.0/src/prefect/client/schemas/schedules.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect._internal.schemas.bases import PrefectBaseModel
 from prefect._internal.schemas.fields import DateTimeTZ
 from prefect._internal.schemas.validators import (
     default_anchor_date,
     default_timezone,
-    interval_schedule_must_be_positive,
     validate_cron_string,
     validate_rrule_string,
     validate_rrule_timezone,
 )
+from prefect.types import PositiveDuration
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, validator
 else:
     from pydantic import Field, validator
 
 MAX_ITERATIONS = 1000
@@ -60,22 +60,18 @@
         timezone (str, optional): a valid timezone string
     """
 
     class Config:
         extra = "forbid"
         exclude_none = True
 
-    interval: datetime.timedelta
+    interval: PositiveDuration
     anchor_date: DateTimeTZ = None
     timezone: Optional[str] = Field(default=None, examples=["America/New_York"])
 
-    @validator("interval")
-    def validate_interval_schedule(cls, v):
-        return interval_schedule_must_be_positive(v)
-
     @validator("anchor_date", always=True)
     def validate_anchor_date(cls, v):
         return default_anchor_date(v)
 
     @validator("timezone", always=True)
     def validate_default_timezone(cls, v, values):
         return default_timezone(v, values=values)
```

### Comparing `prefect-client-2.17.1/src/prefect/client/schemas/sorting.py` & `prefect-client-2.18.0/src/prefect/client/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/subscriptions.py` & `prefect-client-2.18.0/src/prefect/client/subscriptions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/client/utilities.py` & `prefect-client-2.18.0/src/prefect/client/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/concurrency/asyncio.py` & `prefect-client-2.18.0/src/prefect/concurrency/asyncio.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/concurrency/events.py` & `prefect-client-2.18.0/src/prefect/concurrency/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/concurrency/services.py` & `prefect-client-2.18.0/src/prefect/concurrency/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/concurrency/sync.py` & `prefect-client-2.18.0/src/prefect/concurrency/sync.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/context.py` & `prefect-client-2.18.0/src/prefect/context.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deployments/base.py` & `prefect-client-2.18.0/src/prefect/deployments/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,37 @@
 """
-Core primitives for managing Prefect projects.  Projects provide a minimally opinionated
+Core primitives for managing Prefect deployments via `prefect deploy`, providing a minimally opinionated
 build system for managing flows and deployments.
 
 To get started, follow along with [the deloyments tutorial](/tutorials/deployments/).
 """
 
 import ast
 import asyncio
-import json
 import math
 import os
 import subprocess
 import sys
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, List, Optional, cast
 
 import anyio
 import yaml
 from ruamel.yaml import YAML
 
 from prefect.client.schemas.objects import MinimalDeploymentSchedule
 from prefect.client.schemas.schedules import IntervalSchedule
-from prefect.flows import load_flow_from_entrypoint
 from prefect.logging import get_logger
 from prefect.settings import PREFECT_DEBUG_MODE
-from prefect.utilities.asyncutils import LazySemaphore, run_sync_in_worker_thread
+from prefect.utilities.asyncutils import LazySemaphore
 from prefect.utilities.filesystem import create_default_ignore_file, get_open_file_limit
 from prefect.utilities.templating import apply_values
 
 
-def find_prefect_directory(path: Path = None) -> Optional[Path]:
-    """
-    Given a path, recurses upward looking for .prefect/ directories.
-
-    Once found, returns absolute path to the ./prefect directory, which is assumed to reside within the
-    root for the current project.
-
-    If one is never found, `None` is returned.
-    """
-    path = Path(path or ".").resolve()
-    parent = path.parent.resolve()
-    while path != parent:
-        prefect_dir = path.joinpath(".prefect")
-        if prefect_dir.is_dir():
-            return prefect_dir
-
-        path = parent.resolve()
-        parent = path.parent.resolve()
-
-
-def set_prefect_hidden_dir(path: str = None) -> bool:
-    """
-    Creates default `.prefect/` directory if one does not already exist.
-    Returns boolean specifying whether or not a directory was created.
-
-    If a path is provided, the directory will be created in that location.
-    """
-    path = Path(path or ".") / ".prefect"
-
-    # use exists so that we dont accidentally overwrite a file
-    if path.exists():
-        return False
-    path.mkdir(mode=0o0700)
-    return True
-
-
 def create_default_prefect_yaml(
     path: str, name: str = None, contents: Optional[Dict[str, Any]] = None
 ) -> bool:
     """
     Creates default `prefect.yaml` file in the provided path if one does not already exist;
     returns boolean specifying whether a file was created.
 
@@ -266,122 +228,18 @@
     project_name = name or dir_name
 
     files = []
     if create_default_ignore_file("."):
         files.append(".prefectignore")
     if create_default_prefect_yaml(".", name=project_name, contents=configuration):
         files.append("prefect.yaml")
-    if set_prefect_hidden_dir():
-        files.append(".prefect/")
 
     return files
 
 
-async def register_flow(entrypoint: str, force: bool = False):
-    """
-    Register a flow with this project from an entrypoint.
-
-    Args:
-        entrypoint (str): the entrypoint to the flow to register
-        force (bool, optional): whether or not to overwrite an existing flow with the same name
-
-    Raises:
-        ValueError: if `force` is `False` and registration would overwrite an existing flow
-    """
-    try:
-        fpath, obj_name = entrypoint.rsplit(":", 1)
-    except ValueError as exc:
-        if str(exc) == "not enough values to unpack (expected 2, got 1)":
-            missing_flow_name_msg = (
-                "Your flow entrypoint must include the name of the function that is"
-                f" the entrypoint to your flow.\nTry {entrypoint}:<flow_name> as your"
-                f" entrypoint. If you meant to specify '{entrypoint}' as the deployment"
-                f" name, try `prefect deploy -n {entrypoint}`."
-            )
-            raise ValueError(missing_flow_name_msg)
-        else:
-            raise exc
-
-    flow = await run_sync_in_worker_thread(load_flow_from_entrypoint, entrypoint)
-
-    fpath = Path(fpath).absolute()
-    prefect_dir = find_prefect_directory()
-    if not prefect_dir:
-        raise FileNotFoundError(
-            "No .prefect directory could be found - run `prefect project"
-            " init` to create one."
-        )
-
-    entrypoint = f"{fpath.relative_to(prefect_dir.parent)!s}:{obj_name}"
-
-    flows_file = prefect_dir / "flows.json"
-    if flows_file.exists():
-        with flows_file.open(mode="r") as f:
-            flows = json.load(f)
-    else:
-        flows = {}
-
-    ## quality control
-    if flow.name in flows and flows[flow.name] != entrypoint:
-        if not force:
-            raise ValueError(
-                f"Conflicting entry found for flow with name {flow.name!r}.\nExisting"
-                f" entrypoint: {flows[flow.name]}\nAttempted entrypoint:"
-                f" {entrypoint}\n\nYou can try removing the existing entry for"
-                f" {flow.name!r} from your [yellow]~/.prefect/flows.json[/yellow]."
-            )
-
-    flows[flow.name] = entrypoint
-
-    with flows_file.open(mode="w") as f:
-        json.dump(flows, f, sort_keys=True, indent=2)
-
-    return flow
-
-
-def _copy_deployments_into_prefect_file():
-    """
-    Copy deployments from the `deloyment.yaml` file into the `prefect.yaml` file.
-
-    Used to migrate users from the old `prefect.yaml` + `deployment.yaml` structure
-    to a single `prefect.yaml` file.
-    """
-    prefect_file = Path("prefect.yaml")
-    deployment_file = Path("deployment.yaml")
-    if not deployment_file.exists() or not prefect_file.exists():
-        raise FileNotFoundError(
-            "Could not find `prefect.yaml` or `deployment.yaml` files."
-        )
-
-    with deployment_file.open(mode="r") as f:
-        raw_deployment_file_contents = f.read()
-        parsed_deployment_file_contents = yaml.safe_load(raw_deployment_file_contents)
-
-    deployments = parsed_deployment_file_contents.get("deployments")
-
-    with prefect_file.open(mode="a") as f:
-        # If deployment.yaml is empty, write an empty deployments list to prefect.yaml.
-        if not parsed_deployment_file_contents:
-            f.write("\n")
-            f.write(yaml.dump({"deployments": []}, sort_keys=False))
-        # If there is no 'deployments' key in deployment.yaml, assume that the
-        # entire file is a single deployment.
-        elif not deployments:
-            f.write("\n")
-            f.write(
-                yaml.dump(
-                    {"deployments": [parsed_deployment_file_contents]}, sort_keys=False
-                )
-            )
-        # Write all of deployment.yaml to prefect.yaml.
-        else:
-            f.write("\n")
-            f.write(raw_deployment_file_contents)
-
-
 def _format_deployment_for_saving_to_prefect_file(
     deployment: Dict,
 ) -> Dict:
     """
     Formats a deployment into a templated deploy config for saving to prefect.yaml.
 
     Args:
```

### Comparing `prefect-client-2.17.1/src/prefect/deployments/deployments.py` & `prefect-client-2.18.0/src/prefect/deployments/deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import BaseModel, Field, parse_obj_as, root_validator, validator
 else:
     from pydantic import BaseModel, Field, parse_obj_as, root_validator, validator
 
 from prefect.blocks.core import Block
 from prefect.blocks.fields import SecretDict
-from prefect.client.orchestration import PrefectClient, ServerType, get_client
+from prefect.client.orchestration import PrefectClient, get_client
 from prefect.client.schemas.objects import (
     FlowRun,
     MinimalDeploymentSchedule,
 )
 from prefect.client.schemas.schedules import SCHEDULE_TYPES
 from prefect.client.utilities import inject_client
 from prefect.context import FlowRunContext, PrefectObjectRegistry, TaskRunContext
@@ -897,15 +897,15 @@
                 job_variables=self.job_variables,
                 storage_document_id=storage_document_id,
                 infrastructure_document_id=infrastructure_document_id,
                 parameter_openapi_schema=self.parameter_openapi_schema.dict(),
                 enforce_parameter_schema=self.enforce_parameter_schema,
             )
 
-            if client.server_type == ServerType.CLOUD:
+            if client.server_type.supports_automations():
                 # The triggers defined in the deployment spec are, essentially,
                 # anonymous and attempting truly sync them with cloud is not
                 # feasible. Instead, we remove all automations that are owned
                 # by the deployment, meaning that they were created via this
                 # mechanism below, and then recreate them.
                 await client.delete_resource_owned_automations(
                     f"prefect.deployment.{deployment_id}"
```

### Comparing `prefect-client-2.17.1/src/prefect/deployments/runner.py` & `prefect-client-2.18.0/src/prefect/deployments/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from prefect.utilities.collections import get_from_dict, isiterable
 
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import BaseModel, Field, PrivateAttr, root_validator, validator
 else:
     from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 
-from prefect.client.orchestration import ServerType, get_client
+from prefect.client.orchestration import get_client
 from prefect.client.schemas.objects import MinimalDeploymentSchedule
 from prefect.client.schemas.schedules import (
     SCHEDULE_TYPES,
     construct_schedule,
 )
 from prefect.deployments.schedules import (
     FlexibleScheduleList,
@@ -321,15 +321,15 @@
                     detail = exc.response.json().get("detail")
                     if detail:
                         raise DeploymentApplyError(detail) from exc
                 raise DeploymentApplyError(
                     f"Error while applying deployment: {str(exc)}"
                 ) from exc
 
-            if client.server_type == ServerType.CLOUD:
+            if client.server_type.supports_automations():
                 # The triggers defined in the deployment spec are, essentially,
                 # anonymous and attempting truly sync them with cloud is not
                 # feasible. Instead, we remove all automations that are owned
                 # by the deployment, meaning that they were created via this
                 # mechanism below, and then recreate them.
                 await client.delete_resource_owned_automations(
                     f"prefect.deployment.{deployment_id}"
```

### Comparing `prefect-client-2.17.1/src/prefect/deployments/schedules.py` & `prefect-client-2.18.0/src/prefect/deployments/schedules.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deployments/steps/core.py` & `prefect-client-2.18.0/src/prefect/deployments/steps/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Core primitives for running Prefect project steps.
+Core primitives for running Prefect deployment steps.
 
-Project steps are YAML representations of Python functions along with their inputs.
+Deployment steps are YAML representations of Python functions along with their inputs.
 
 Whenever a step is run, the following actions are taken:
 
-- The step's inputs and block / variable references are resolved (see [the projects concepts documentation](/concepts/projects/#templating-options) for more details)
+- The step's inputs and block / variable references are resolved (see [the `prefect deploy` documentation](/guides/prefect-deploy/#templating-options) for more details)
 - The step's function is imported; if it cannot be found, the `requires` keyword is used to install the necessary packages
 - The step's function is called with the resolved inputs
 - The step's output is returned and used to resolve inputs for subsequent steps
 """
 import os
 import re
 import subprocess
```

### Comparing `prefect-client-2.17.1/src/prefect/deployments/steps/pull.py` & `prefect-client-2.18.0/src/prefect/deployments/steps/pull.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deployments/steps/utility.py` & `prefect-client-2.18.0/src/prefect/deployments/steps/utility.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/data_documents.py` & `prefect-client-2.18.0/src/prefect/deprecated/data_documents.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/packaging/base.py` & `prefect-client-2.18.0/src/prefect/deprecated/packaging/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/packaging/docker.py` & `prefect-client-2.18.0/src/prefect/deprecated/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/packaging/file.py` & `prefect-client-2.18.0/src/prefect/deprecated/packaging/file.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/packaging/orion.py` & `prefect-client-2.18.0/src/prefect/deprecated/packaging/orion.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/deprecated/packaging/serializers.py` & `prefect-client-2.18.0/src/prefect/deprecated/packaging/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,29 @@
     Wraps pickles in base64 for safe transmission.
     """
 
     type: Literal["pickle"] = "pickle"
 
     picklelib: str = "cloudpickle"
     picklelib_version: str = None
+
     pickle_modules: List[str] = pydantic.Field(default_factory=list)
 
     @pydantic.validator("picklelib")
     def check_picklelib(cls, value):
         return validate_picklelib(value)
 
     @pydantic.root_validator
-    def check_picklelib_version(cls, values):
-        return validate_picklelib_version(values)
-
-    @pydantic.root_validator
     def check_picklelib_and_modules(cls, values):
         return validate_picklelib_and_modules(values)
 
+    @pydantic.root_validator
+    def check_picklelib_version(cls, values):
+        return validate_picklelib_version(values)
+
     def dumps(self, obj: Any) -> bytes:
         pickler = from_qualified_name(self.picklelib)
 
         for module in self.pickle_modules:
             pickler.register_pickle_by_value(from_qualified_name(module))
 
         blob = pickler.dumps(obj)
```

### Comparing `prefect-client-2.17.1/src/prefect/engine.py` & `prefect-client-2.18.0/src/prefect/engine.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/clients.py` & `prefect-client-2.18.0/src/prefect/events/clients.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,89 @@
     Mapping,
     Optional,
     Tuple,
     Type,
 )
 from uuid import UUID
 
+import httpx
 import orjson
 import pendulum
 from cachetools import TTLCache
 from typing_extensions import Self
 from websockets.client import WebSocketClientProtocol, connect
 from websockets.exceptions import (
     ConnectionClosed,
     ConnectionClosedError,
     ConnectionClosedOK,
 )
 
+from prefect.client.base import PrefectHttpxClient
 from prefect.events import Event
 from prefect.logging import get_logger
-from prefect.settings import PREFECT_API_KEY, PREFECT_API_URL
+from prefect.settings import (
+    PREFECT_API_KEY,
+    PREFECT_API_URL,
+    PREFECT_CLOUD_API_URL,
+    PREFECT_EXPERIMENTAL_EVENTS,
+)
 
 if TYPE_CHECKING:
     from prefect.events.filters import EventFilter
 
 logger = get_logger(__name__)
 
 
+def get_events_client(
+    reconnection_attempts: int = 10,
+    checkpoint_every: int = 20,
+) -> "EventsClient":
+    api_url = PREFECT_API_URL.value()
+    if isinstance(api_url, str) and api_url.startswith(PREFECT_CLOUD_API_URL.value()):
+        return PrefectCloudEventsClient(
+            reconnection_attempts=reconnection_attempts,
+            checkpoint_every=checkpoint_every,
+        )
+    elif PREFECT_EXPERIMENTAL_EVENTS:
+        if PREFECT_API_URL:
+            return PrefectEventsClient(
+                reconnection_attempts=reconnection_attempts,
+                checkpoint_every=checkpoint_every,
+            )
+        else:
+            return PrefectEphemeralEventsClient()
+
+    raise RuntimeError(
+        "The current server and client configuration does not support "
+        "events.  Enable experimental events support with the "
+        "PREFECT_EXPERIMENTAL_EVENTS setting."
+    )
+
+
+def get_events_subscriber(
+    filter: "EventFilter" = None,
+    reconnection_attempts: int = 10,
+) -> "PrefectEventSubscriber":
+    api_url = PREFECT_API_URL.value()
+    if isinstance(api_url, str) and api_url.startswith(PREFECT_CLOUD_API_URL.value()):
+        return PrefectCloudEventSubscriber(
+            filter=filter, reconnection_attempts=reconnection_attempts
+        )
+    elif PREFECT_EXPERIMENTAL_EVENTS:
+        return PrefectEventSubscriber(
+            filter=filter, reconnection_attempts=reconnection_attempts
+        )
+
+    raise RuntimeError(
+        "The current server and client configuration does not support "
+        "events.  Enable experimental events support with the "
+        "PREFECT_EXPERIMENTAL_EVENTS setting."
+    )
+
+
 class EventsClient(abc.ABC):
     """The abstract interface for all Prefect Events clients"""
 
     async def emit(self, event: Event) -> None:
         """Emit a single event"""
         if not hasattr(self, "_in_context"):
             raise TypeError(
@@ -115,14 +169,60 @@
         raise ValueError(
             "api_url and api_key must be provided or set in the Prefect configuration"
         )
 
     return api_url, api_key
 
 
+class PrefectEphemeralEventsClient(EventsClient):
+    """A Prefect Events client that sends events to an ephemeral Prefect server"""
+
+    def __init__(self):
+        if not PREFECT_EXPERIMENTAL_EVENTS:
+            raise ValueError(
+                "PrefectEphemeralEventsClient can only be used when "
+                "PREFECT_EXPERIMENTAL_EVENTS is set to True"
+            )
+        if PREFECT_API_KEY.value():
+            raise ValueError(
+                "PrefectEphemeralEventsClient cannot be used when PREFECT_API_KEY is set."
+                " Please use PrefectEventsClient or PrefectCloudEventsClient instead."
+            )
+        from prefect.server.api.server import create_app
+
+        app = create_app()
+
+        self._http_client = PrefectHttpxClient(
+            transport=httpx.ASGITransport(app=app, raise_app_exceptions=False),
+            base_url="http://ephemeral-prefect/api",
+            enable_csrf_support=False,
+        )
+
+    async def __aenter__(self) -> Self:
+        await super().__aenter__()
+        await self._http_client.__aenter__()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[Exception]],
+        exc_val: Optional[Exception],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        self._websocket = None
+        await self._http_client.__aexit__(exc_type, exc_val, exc_tb)
+        return await super().__aexit__(exc_type, exc_val, exc_tb)
+
+    async def _emit(self, event: Event) -> None:
+        await self._http_client.post(
+            "/events",
+            json=[event.dict(json_compatible=True)],
+        )
+
+
 class PrefectEventsClient(EventsClient):
     """A Prefect Events client that streams events to a Prefect server"""
 
     _websocket: Optional[WebSocketClientProtocol]
     _unconfirmed_events: List[Event]
 
     def __init__(
@@ -270,65 +370,65 @@
         )
 
 
 SEEN_EVENTS_SIZE = 500_000
 SEEN_EVENTS_TTL = 120
 
 
-class PrefectCloudEventSubscriber:
+class PrefectEventSubscriber:
     """
     Subscribes to a Prefect Cloud event stream, yielding events as they occur.
 
     Example:
 
-        from prefect.events.clients import PrefectCloudEventSubscriber
+        from prefect.events.clients import PrefectEventSubscriber
         from prefect.events.filters import EventFilter, EventNameFilter
 
         filter = EventFilter(event=EventNameFilter(prefix=["prefect.flow-run."]))
 
-        async with PrefectCloudEventSubscriber(api_url, api_key, filter) as subscriber:
+        async with PrefectEventSubscriber(filter=filter) as subscriber:
             async for event in subscriber:
                 print(event.occurred, event.resource.id, event.event)
 
     """
 
     _websocket: Optional[WebSocketClientProtocol]
     _filter: "EventFilter"
     _seen_events: Mapping[UUID, bool]
 
     def __init__(
         self,
         api_url: str = None,
-        api_key: str = None,
         filter: "EventFilter" = None,
         reconnection_attempts: int = 10,
     ):
         """
         Args:
             api_url: The base URL for a Prefect Cloud workspace
             api_key: The API of an actor with the manage_events scope
             reconnection_attempts: When the client is disconnected, how many times
                 the client should attempt to reconnect
         """
-        api_url, api_key = _get_api_url_and_key(api_url, api_key)
+        if not api_url:
+            api_url = PREFECT_API_URL.value()
+            self._api_key = None
 
         from prefect.events.filters import EventFilter
 
         self._filter = filter or EventFilter()
         self._seen_events = TTLCache(maxsize=SEEN_EVENTS_SIZE, ttl=SEEN_EVENTS_TTL)
 
         socket_url = (
             api_url.replace("https://", "wss://")
             .replace("http://", "ws://")
             .rstrip("/")
         ) + "/events/out"
 
         logger.debug("Connecting to %s", socket_url)
 
-        self._api_key = api_key
         self._connect = connect(
             socket_url,
             subprotocols=["prefect"],
         )
         self._websocket = None
         self._reconnection_attempts = reconnection_attempts
         if self._reconnection_attempts < 0:
@@ -437,7 +537,33 @@
                     raise
 
                 if i > 2:
                     # let the first two attempts happen quickly in case this is just
                     # a standard load balancer timeout, but after that, just take a
                     # beat to let things come back around.
                     await asyncio.sleep(1)
+
+
+class PrefectCloudEventSubscriber(PrefectEventSubscriber):
+    def __init__(
+        self,
+        api_url: str = None,
+        api_key: str = None,
+        filter: "EventFilter" = None,
+        reconnection_attempts: int = 10,
+    ):
+        """
+        Args:
+            api_url: The base URL for a Prefect Cloud workspace
+            api_key: The API of an actor with the manage_events scope
+            reconnection_attempts: When the client is disconnected, how many times
+                the client should attempt to reconnect
+        """
+        api_url, api_key = _get_api_url_and_key(api_url, api_key)
+
+        super().__init__(
+            api_url=api_url,
+            filter=filter,
+            reconnection_attempts=reconnection_attempts,
+        )
+
+        self._api_key = api_key
```

### Comparing `prefect-client-2.17.1/src/prefect/events/filters.py` & `prefect-client-2.18.0/src/prefect/events/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/instrument.py` & `prefect-client-2.18.0/src/prefect/events/instrument.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/related.py` & `prefect-client-2.18.0/src/prefect/events/related.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/schemas/automations.py` & `prefect-client-2.18.0/src/prefect/events/schemas/automations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+import textwrap
 from datetime import timedelta
 from enum import Enum
 from typing import (
     Any,
     Dict,
     List,
     Literal,
@@ -41,14 +42,18 @@
     """
     Base class describing a set of criteria that must be satisfied in order to trigger
     an automation.
     """
 
     type: str
 
+    @abc.abstractmethod
+    def describe_for_cli(self, indent: int = 0) -> str:
+        """Return a human-readable description of this trigger for the CLI"""
+
 
 class ResourceTrigger(Trigger, abc.ABC):
     """
     Base class for triggers that may filter by the labels of resources.
     """
 
     type: str
@@ -97,15 +102,15 @@
             "resources by specifying `related:<role>:<label>`.  This will use the "
             "value of that label for the first related resource in that role.  For "
             'example, `"for_each": ["related:flow:prefect.resource.id"]` would '
             "evaluate the trigger for each flow."
         ),
     )
     posture: Literal[Posture.Reactive, Posture.Proactive] = Field(  # type: ignore[valid-type]
-        ...,
+        Posture.Reactive,
         description=(
             "The posture of this trigger, either Reactive or Proactive.  Reactive "
             "triggers respond to the _presence_ of the expected events, while "
             "Proactive triggers respond to the _absence_ of those expected events."
         ),
     )
     threshold: int = Field(
@@ -144,14 +149,36 @@
             elif within < timedelta(seconds=10.0):
                 raise ValueError(
                     "The minimum within for Proactive triggers is 10 seconds"
                 )
 
         return values
 
+    def describe_for_cli(self, indent: int = 0) -> str:
+        """Return a human-readable description of this trigger for the CLI"""
+        if self.posture == Posture.Reactive:
+            return textwrap.indent(
+                "\n".join(
+                    [
+                        f"Reactive: expecting {self.threshold} of {self.expect}",
+                    ],
+                ),
+                prefix="  " * indent,
+            )
+        else:
+            return textwrap.indent(
+                "\n".join(
+                    [
+                        f"Proactive: expecting {self.threshold} {self.expect} event "
+                        f"within {self.within}",
+                    ],
+                ),
+                prefix="  " * indent,
+            )
+
 
 class MetricTriggerOperator(Enum):
     LT = "<"
     LTE = "<="
     GT = ">"
     GTE = ">="
 
@@ -220,14 +247,26 @@
     )
 
     metric: MetricTriggerQuery = Field(
         ...,
         description="The metric query to evaluate for this trigger. ",
     )
 
+    def describe_for_cli(self, indent: int = 0) -> str:
+        """Return a human-readable description of this trigger for the CLI"""
+        m = self.metric
+        return textwrap.indent(
+            "\n".join(
+                [
+                    f"Metric: {m.name.value} {m.operator.value} {m.threshold} for {m.range}",
+                ]
+            ),
+            prefix="  " * indent,
+        )
+
 
 class CompositeTrigger(Trigger, abc.ABC):
     """
     Requires some number of triggers to have fired within the given time period.
     """
 
     type: Literal["compound", "sequence"]
@@ -252,32 +291,66 @@
             if require > len(values["triggers"]):
                 raise ValueError(
                     "required must be less than or equal to the number of triggers"
                 )
 
         return values
 
+    def describe_for_cli(self, indent: int = 0) -> str:
+        """Return a human-readable description of this trigger for the CLI"""
+        return textwrap.indent(
+            "\n".join(
+                [
+                    f"{str(self.require).capitalize()} of:",
+                    "\n".join(
+                        [
+                            trigger.describe_for_cli(indent=indent + 1)
+                            for trigger in self.triggers
+                        ]
+                    ),
+                ]
+            ),
+            prefix="  " * indent,
+        )
+
 
 class SequenceTrigger(CompositeTrigger):
     """A composite trigger that requires some number of triggers to have fired
     within the given time period in a specific order"""
 
     type: Literal["sequence"] = "sequence"
 
+    def describe_for_cli(self, indent: int = 0) -> str:
+        """Return a human-readable description of this trigger for the CLI"""
+        return textwrap.indent(
+            "\n".join(
+                [
+                    "In this order:",
+                    "\n".join(
+                        [
+                            trigger.describe_for_cli(indent=indent + 1)
+                            for trigger in self.triggers
+                        ]
+                    ),
+                ]
+            ),
+            prefix="  " * indent,
+        )
+
 
 TriggerTypes: TypeAlias = Union[
     EventTrigger, MetricTrigger, CompoundTrigger, SequenceTrigger
 ]
 """The union of all concrete trigger types that a user may actually create"""
 
 CompoundTrigger.update_forward_refs()
 SequenceTrigger.update_forward_refs()
 
 
-class Automation(PrefectBaseModel, extra="ignore"):
+class AutomationCore(PrefectBaseModel, extra="ignore"):
     """Defines an action a user wants to take when a certain number of events
     do or don't happen to the matching resources"""
 
     name: str = Field(..., description="The name of this automation")
     description: str = Field("", description="A longer description of this automation")
 
     enabled: bool = Field(True, description="Whether this automation will be evaluated")
@@ -306,9 +379,9 @@
     )
 
     owner_resource: Optional[str] = Field(
         default=None, description="The owning resource of this automation"
     )
 
 
-class ExistingAutomation(Automation):
+class Automation(AutomationCore):
     id: UUID = Field(..., description="The ID of this automation")
```

### Comparing `prefect-client-2.17.1/src/prefect/events/schemas/deployment_triggers.py` & `prefect-client-2.18.0/src/prefect/events/schemas/deployment_triggers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 closely as possible (because otherwise users will get validation errors creating
 triggers), but we can be more liberal with the defaults here to make it simpler to
 create them from YAML.
 """
 
 import abc
 import textwrap
-import warnings
 from datetime import timedelta
 from typing import (
     Any,
     Dict,
     List,
     Literal,
     Optional,
@@ -33,28 +32,19 @@
 if HAS_PYDANTIC_V2:
     from pydantic.v1 import Field, PrivateAttr, root_validator, validator
     from pydantic.v1.fields import ModelField
 else:
     from pydantic import Field, PrivateAttr, root_validator, validator
     from pydantic.fields import ModelField
 
-from prefect._internal.compatibility.experimental import (
-    EXPERIMENTAL_WARNING,
-    PREFECT_EXPERIMENTAL_WARN,
-    ExperimentalFeature,
-    experiment_enabled,
-)
 from prefect._internal.schemas.bases import PrefectBaseModel
 from prefect.events.actions import RunDeployment
-from prefect.settings import (
-    PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES,
-)
 
 from .automations import (
-    Automation,
+    AutomationCore,
     CompoundTrigger,
     EventTrigger,
     MetricTrigger,
     MetricTriggerQuery,
     Posture,
     SequenceTrigger,
     Trigger,
@@ -102,48 +92,28 @@
     def set_deployment_id(self, deployment_id: UUID):
         self._deployment_id = deployment_id
 
     def owner_resource(self) -> Optional[str]:
         return f"prefect.deployment.{self._deployment_id}"
 
     def actions(self) -> List[RunDeployment]:
-        if self.job_variables is not None and experiment_enabled(
-            "flow_run_infra_overrides"
-        ):
-            if (
-                PREFECT_EXPERIMENTAL_WARN
-                and PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES
-            ):
-                warnings.warn(
-                    EXPERIMENTAL_WARNING.format(
-                        feature="Flow run job variables",
-                        group="flow_run_infra_overrides",
-                        help="To use this feature, update your workers to Prefect 2.16.4 or later. ",
-                    ),
-                    ExperimentalFeature,
-                    stacklevel=3,
-                )
-        if not experiment_enabled("flow_run_infra_overrides"):
-            # nullify job_variables if the flag is disabled
-            self.job_variables = None
-
         assert self._deployment_id
         return [
             RunDeployment(
                 parameters=self.parameters,
                 deployment_id=self._deployment_id,
                 job_variables=self.job_variables,
             )
         ]
 
-    def as_automation(self) -> Automation:
+    def as_automation(self) -> AutomationCore:
         if not self.name:
             raise ValueError("name is required")
 
-        return Automation(
+        return AutomationCore(
             name=self.name,
             description=self.description,
             enabled=self.enabled,
             trigger=self.as_trigger(),
             actions=self.actions(),
             owner_resource=self.owner_resource(),
         )
@@ -172,14 +142,16 @@
 
 class DeploymentEventTrigger(DeploymentResourceTrigger):
     """
     A trigger that fires based on the presence or absence of events within a given
     period of time.
     """
 
+    trigger_type = EventTrigger
+
     type: Literal["event"] = "event"
 
     after: Set[str] = Field(
         default_factory=set,
         description=(
             "The event(s) which must first been seen to fire this trigger.  If "
             "empty, then fire this trigger immediately.  Events may include "
@@ -252,15 +224,15 @@
                 raise ValueError(
                     "The minimum within for Proactive triggers is 10 seconds"
                 )
 
         return values
 
     def as_trigger(self) -> Trigger:
-        return EventTrigger(
+        return self.trigger_type(
             match=self.match,
             match_related=self.match_related,
             after=self.after,
             expect=self.expect,
             for_each=self.for_each,
             posture=self.posture,
             threshold=self.threshold,
@@ -269,28 +241,30 @@
 
 
 class DeploymentMetricTrigger(DeploymentResourceTrigger):
     """
     A trigger that fires based on the results of a metric query.
     """
 
+    trigger_type = MetricTrigger
+
     type: Literal["metric"] = "metric"
 
     posture: Literal[Posture.Metric] = Field(  # type: ignore[valid-type]
         Posture.Metric,
         description="Periodically evaluate the configured metric query.",
     )
 
     metric: MetricTriggerQuery = Field(
         ...,
         description="The metric query to evaluate for this trigger. ",
     )
 
     def as_trigger(self) -> Trigger:
-        return MetricTrigger(
+        return self.trigger_type(
             match=self.match,
             match_related=self.match_related,
             posture=self.posture,
             metric=self.metric,
             job_variables=self.job_variables,
         )
 
@@ -305,14 +279,16 @@
     within: Optional[timedelta]
 
 
 class DeploymentCompoundTrigger(DeploymentCompositeTrigger):
     """A composite trigger that requires some number of triggers to have
     fired within the given time period"""
 
+    trigger_type = CompoundTrigger
+
     type: Literal["compound"] = "compound"
     require: Union[int, Literal["any", "all"]]
 
     @root_validator
     def validate_require(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         require = values.get("require")
 
@@ -323,30 +299,32 @@
                 raise ValueError(
                     "required must be less than or equal to the number of triggers"
                 )
 
         return values
 
     def as_trigger(self) -> Trigger:
-        return CompoundTrigger(
+        return self.trigger_type(
             require=self.require,
             triggers=self.triggers,
             within=self.within,
             job_variables=self.job_variables,
         )
 
 
 class DeploymentSequenceTrigger(DeploymentCompositeTrigger):
     """A composite trigger that requires some number of triggers to have fired
     within the given time period in a specific order"""
 
+    trigger_type = SequenceTrigger
+
     type: Literal["sequence"] = "sequence"
 
     def as_trigger(self) -> Trigger:
-        return SequenceTrigger(
+        return self.trigger_type(
             triggers=self.triggers,
             within=self.within,
             job_variables=self.job_variables,
         )
 
 
 # Concrete deployment trigger types
@@ -476,15 +454,15 @@
         None,
         description=(
             "The parameters to pass to the deployment, or None to use the "
             "deployment's default parameters"
         ),
     )
 
-    def as_automation(self) -> Automation:
+    def as_automation(self) -> AutomationCore:
         assert self.name
 
         if self.posture == Posture.Metric:
             trigger = MetricTrigger(
                 type="metric",
                 match=self.match,
                 match_related=self.match_related,
@@ -499,15 +477,15 @@
                 expect=self.expect,
                 for_each=self.for_each,
                 posture=self.posture,
                 threshold=self.threshold,
                 within=self.within,
             )
 
-        return Automation(
+        return AutomationCore(
             name=self.name,
             description=self.description,
             enabled=self.enabled,
             trigger=trigger,
             actions=self.actions(),
             owner_resource=self.owner_resource(),
         )
@@ -515,34 +493,14 @@
     def set_deployment_id(self, deployment_id: UUID):
         self._deployment_id = deployment_id
 
     def owner_resource(self) -> Optional[str]:
         return f"prefect.deployment.{self._deployment_id}"
 
     def actions(self) -> List[RunDeployment]:
-        if self.job_variables is not None and experiment_enabled(
-            "flow_run_infra_overrides"
-        ):
-            if (
-                PREFECT_EXPERIMENTAL_WARN
-                and PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES
-            ):
-                warnings.warn(
-                    EXPERIMENTAL_WARNING.format(
-                        feature="Flow run job variables",
-                        group="flow_run_infra_overrides",
-                        help="To use this feature, update your workers to Prefect 2.16.4 or later. ",
-                    ),
-                    ExperimentalFeature,
-                    stacklevel=3,
-                )
-        if not experiment_enabled("flow_run_infra_overrides"):
-            # nullify job_variables if the flag is disabled
-            self.job_variables = None
-
         assert self._deployment_id
         return [
             RunDeployment(
                 parameters=self.parameters,
                 deployment_id=self._deployment_id,
                 job_variables=self.job_variables,
             )
```

### Comparing `prefect-client-2.17.1/src/prefect/events/schemas/events.py` & `prefect-client-2.18.0/src/prefect/events/schemas/events.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/schemas/labelling.py` & `prefect-client-2.18.0/src/prefect/events/schemas/labelling.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/events/utilities.py` & `prefect-client-2.18.0/src/prefect/events/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pendulum
 
 from prefect._internal.schemas.fields import DateTimeTZ
 
 from .clients import (
     AssertingEventsClient,
     PrefectCloudEventsClient,
+    PrefectEphemeralEventsClient,
     PrefectEventsClient,
 )
 from .schemas.events import Event, RelatedResource
 from .worker import EventsWorker, should_emit_events
 
 TIGHT_TIMING = timedelta(minutes=5)
 
@@ -49,14 +50,15 @@
     if not should_emit_events():
         return None
 
     operational_clients = [
         AssertingEventsClient,
         PrefectCloudEventsClient,
         PrefectEventsClient,
+        PrefectEphemeralEventsClient,
     ]
     worker_instance = EventsWorker.instance()
 
     if worker_instance.client_type not in operational_clients:
         return None
 
     event_kwargs = {
```

### Comparing `prefect-client-2.17.1/src/prefect/events/worker.py` & `prefect-client-2.18.0/src/prefect/events/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,36 +13,45 @@
 )
 from prefect.utilities.context import temporary_context
 
 from .clients import (
     EventsClient,
     NullEventsClient,
     PrefectCloudEventsClient,
+    PrefectEphemeralEventsClient,
     PrefectEventsClient,
 )
 from .related import related_resources_from_run_context
 from .schemas.events import Event
 
 
 def should_emit_events() -> bool:
-    return emit_events_to_cloud() or should_emit_events_to_running_server()
+    return (
+        emit_events_to_cloud()
+        or should_emit_events_to_running_server()
+        or should_emit_events_to_ephemeral_server()
+    )
 
 
 def emit_events_to_cloud() -> bool:
     api_url = PREFECT_API_URL.value()
     return isinstance(api_url, str) and api_url.startswith(
         PREFECT_CLOUD_API_URL.value()
     )
 
 
 def should_emit_events_to_running_server() -> bool:
     api_url = PREFECT_API_URL.value()
     return isinstance(api_url, str) and PREFECT_EXPERIMENTAL_EVENTS
 
 
+def should_emit_events_to_ephemeral_server() -> bool:
+    return PREFECT_API_KEY.value() is None and PREFECT_EXPERIMENTAL_EVENTS
+
+
 class EventsWorker(QueueService[Event]):
     def __init__(
         self, client_type: Type[EventsClient], client_options: Tuple[Tuple[str, Any]]
     ):
         super().__init__(client_type, client_options)
         self.client_type = client_type
         self.client_options = client_options
@@ -81,14 +90,15 @@
                 client_type = PrefectCloudEventsClient
                 client_kwargs = {
                     "api_url": PREFECT_API_URL.value(),
                     "api_key": PREFECT_API_KEY.value(),
                 }
             elif should_emit_events_to_running_server():
                 client_type = PrefectEventsClient
-
+            elif should_emit_events_to_ephemeral_server():
+                client_type = PrefectEphemeralEventsClient
             else:
                 client_type = NullEventsClient
 
         # The base class will take care of returning an existing worker with these
         # options if available
         return super().instance(client_type, tuple(client_kwargs.items()))
```

### Comparing `prefect-client-2.17.1/src/prefect/exceptions.py` & `prefect-client-2.18.0/src/prefect/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     """
 
     def __init__(self, msg: str):
         super().__init__(msg)
 
     @classmethod
     def from_validation_error(cls, exc: ValidationError) -> Self:
-        bad_params = [f'{err["loc"][0]}: {err["msg"]}' for err in exc.errors()]
+        bad_params = [f'{".".join(err["loc"])}: {err["msg"]}' for err in exc.errors()]
         msg = "Flow run received invalid parameters:\n - " + "\n - ".join(bad_params)
         return cls(msg)
 
 
 class ParameterBindError(TypeError, PrefectException):
     """
     Raised when args and kwargs cannot be converted to parameters.
```

### Comparing `prefect-client-2.17.1/src/prefect/filesystems.py` & `prefect-client-2.18.0/src/prefect/filesystems.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/flow_runs.py` & `prefect-client-2.18.0/src/prefect/flow_runs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/flows.py` & `prefect-client-2.18.0/src/prefect/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/futures.py` & `prefect-client-2.18.0/src/prefect/futures.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/__init__.py` & `prefect-client-2.18.0/src/prefect/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/base.py` & `prefect-client-2.18.0/src/prefect/infrastructure/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/container.py` & `prefect-client-2.18.0/src/prefect/infrastructure/container.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/kubernetes.py` & `prefect-client-2.18.0/src/prefect/infrastructure/kubernetes.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/process.py` & `prefect-client-2.18.0/src/prefect/infrastructure/process.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/provisioners/__init__.py` & `prefect-client-2.18.0/src/prefect/infrastructure/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/provisioners/cloud_run.py` & `prefect-client-2.18.0/src/prefect/infrastructure/provisioners/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/provisioners/container_instance.py` & `prefect-client-2.18.0/src/prefect/infrastructure/provisioners/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/provisioners/ecs.py` & `prefect-client-2.18.0/src/prefect/infrastructure/provisioners/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/infrastructure/provisioners/modal.py` & `prefect-client-2.18.0/src/prefect/infrastructure/provisioners/modal.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/input/__init__.py` & `prefect-client-2.18.0/src/prefect/input/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/input/actions.py` & `prefect-client-2.18.0/src/prefect/input/actions.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/input/run_input.py` & `prefect-client-2.18.0/src/prefect/input/run_input.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/configuration.py` & `prefect-client-2.18.0/src/prefect/logging/configuration.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/filters.py` & `prefect-client-2.18.0/src/prefect/logging/filters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/formatters.py` & `prefect-client-2.18.0/src/prefect/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/handlers.py` & `prefect-client-2.18.0/src/prefect/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/highlighters.py` & `prefect-client-2.18.0/src/prefect/logging/highlighters.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/logging/loggers.py` & `prefect-client-2.18.0/src/prefect/logging/loggers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import io
 import logging
 import sys
 import warnings
 from builtins import print
 from contextlib import contextmanager
 from functools import lru_cache
-from typing import TYPE_CHECKING, Dict, Optional, Union
+from logging import LogRecord
+from typing import TYPE_CHECKING, Dict, List, Optional, Union
+
+from typing_extensions import Self
 
 import prefect
 from prefect.exceptions import MissingContextError
 from prefect.logging.filters import ObfuscateApiKeyFilter
 
 if TYPE_CHECKING:
     from prefect.client.schemas import FlowRun as ClientFlowRun
@@ -291,7 +294,67 @@
     original = builtins.print
 
     try:
         builtins.print = print_as_log
         yield
     finally:
         builtins.print = original
+
+
+class LogEavesdropper(logging.Handler):
+    """A context manager that collects logs for the duration of the context
+
+    Example:
+
+        ```python
+        import logging
+        from prefect.logging import LogEavesdropper
+
+        with LogEavesdropper("my_logger") as eavesdropper:
+            logging.getLogger("my_logger").info("Hello, world!")
+            logging.getLogger("my_logger.child_module").info("Another one!")
+
+        print(eavesdropper.text())
+
+        # Outputs: "Hello, world!\nAnother one!"
+    """
+
+    _target_logger: logging.Logger
+    _lines: List[str]
+
+    def __init__(self, eavesdrop_on: str, level: int = logging.NOTSET):
+        """
+        Args:
+            eavesdrop_on (str): the name of the logger to eavesdrop on
+            level (int): the minimum log level to eavesdrop on; if omitted, all levels
+                are captured
+        """
+
+        super().__init__(level=level)
+        self.eavesdrop_on = eavesdrop_on
+        self._target_logger = None
+
+        # It's important that we use a very minimalistic formatter for use cases where
+        # we may present these logs back to the user.  We shouldn't leak filenames,
+        # versions, or other environmental information.
+        self.formatter = logging.Formatter("[%(levelname)s]: %(message)s")
+
+    def __enter__(self) -> Self:
+        self._target_logger = logging.getLogger(self.eavesdrop_on)
+        self._original_level = self._target_logger.level
+        self._target_logger.level = self.level
+        self._target_logger.addHandler(self)
+        self._lines = []
+        return self
+
+    def __exit__(self, *_):
+        if self._target_logger:
+            self._target_logger.removeHandler(self)
+            self._target_logger.level = self._original_level
+
+    def emit(self, record: LogRecord) -> None:
+        """The logging.Handler implementation, not intended to be called directly."""
+        self._lines.append(self.format(record))
+
+    def text(self) -> str:
+        """Return the collected logs as a single newline-delimited string"""
+        return "\n".join(self._lines)
```

### Comparing `prefect-client-2.17.1/src/prefect/logging/logging.yml` & `prefect-client-2.18.0/src/prefect/logging/logging.yml`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/manifests.py` & `prefect-client-2.18.0/src/prefect/manifests.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/plugins.py` & `prefect-client-2.18.0/src/prefect/plugins.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/pydantic/__init__.py` & `prefect-client-2.18.0/src/prefect/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/pydantic/main.py` & `prefect-client-2.18.0/src/prefect/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/results.py` & `prefect-client-2.18.0/src/prefect/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,14 @@
 )
 from uuid import UUID
 
 from typing_extensions import Self
 
 import prefect
 from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    import pydantic.v1 as pydantic
-
-else:
-    import pydantic
-
 from prefect.blocks.core import Block
 from prefect.client.utilities import inject_client
 from prefect.exceptions import MissingResult
 from prefect.filesystems import (
     LocalFileSystem,
     ReadableFileSystem,
     WritableFileSystem,
@@ -42,15 +35,22 @@
     PREFECT_LOCAL_STORAGE_PATH,
     PREFECT_RESULTS_DEFAULT_SERIALIZER,
     PREFECT_RESULTS_PERSIST_BY_DEFAULT,
     PREFECT_TASK_SCHEDULING_DEFAULT_STORAGE_BLOCK,
 )
 from prefect.utilities.annotations import NotSet
 from prefect.utilities.asyncutils import sync_compatible
-from prefect.utilities.pydantic import add_type_dispatch
+from prefect.utilities.pydantic import get_dispatch_key, lookup_type, register_base_type
+
+if HAS_PYDANTIC_V2:
+    import pydantic.v1 as pydantic
+
+else:
+    import pydantic
+
 
 if TYPE_CHECKING:
     from prefect import Flow, Task
     from prefect.client.orchestration import PrefectClient
 
 
 ResultStorage = Union[WritableFileSystem, str]
@@ -476,20 +476,35 @@
         ), "Unexpected storage block ID. Was it persisted?"
         blob = PersistedResultBlob.parse_raw(
             await self.storage_block.read_path(f"parameters/{identifier}")
         )
         return self.serializer.loads(blob.data)
 
 
-@add_type_dispatch
+@register_base_type
 class BaseResult(pydantic.BaseModel, abc.ABC, Generic[R]):
     type: str
     artifact_type: Optional[str]
     artifact_description: Optional[str]
 
+    def __init__(self, **data: Any) -> None:
+        type_string = get_dispatch_key(self) if type(self) != BaseResult else "__base__"
+        data.setdefault("type", type_string)
+        super().__init__(**data)
+
+    def __new__(cls: Type[Self], **kwargs) -> Self:
+        if "type" in kwargs:
+            try:
+                subcls = lookup_type(cls, dispatch_key=kwargs["type"])
+            except KeyError as exc:
+                raise pydantic.ValidationError(errors=[exc], model=cls)
+            return super().__new__(subcls)
+        else:
+            return super().__new__(cls)
+
     _cache: Any = pydantic.PrivateAttr(NotSet)
 
     def _cache_object(self, obj: Any) -> None:
         self._cache = obj
 
     def has_cached_object(self) -> bool:
         return self._cache is not NotSet
@@ -507,14 +522,18 @@
         **kwargs: Any,
     ) -> "BaseResult[R]":
         ...
 
     class Config:
         extra = "forbid"
 
+    @classmethod
+    def __dispatch_key__(cls, **kwargs):
+        return cls.__fields__.get("type").get_default()
+
 
 class UnpersistedResult(BaseResult):
     """
     Result type for results that are not persisted outside of local memory.
     """
 
     type = "unpersisted"
@@ -709,15 +728,15 @@
 
     def to_bytes(self) -> bytes:
         return self.json().encode()
 
 
 class UnknownResult(BaseResult):
     """
-    Result type for unknown results. Typipcally used to represent the result
+    Result type for unknown results. Typically used to represent the result
     of tasks that were forced from a failure state into a completed state.
 
     The value for this result is always None and is not persisted to external
     result storage, but orchestration treats the result the same as persisted
     results when determining orchestration rules, such as whether to rerun a
     completed task.
     """
```

### Comparing `prefect-client-2.17.1/src/prefect/runner/runner.py` & `prefect-client-2.18.0/src/prefect/runner/runner.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runner/server.py` & `prefect-client-2.18.0/src/prefect/runner/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runner/storage.py` & `prefect-client-2.18.0/src/prefect/runner/storage.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runner/submit.py` & `prefect-client-2.18.0/src/prefect/runner/submit.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runner/utils.py` & `prefect-client-2.18.0/src/prefect/runner/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runtime/deployment.py` & `prefect-client-2.18.0/src/prefect/runtime/deployment.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runtime/flow_run.py` & `prefect-client-2.18.0/src/prefect/runtime/flow_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/runtime/task_run.py` & `prefect-client-2.18.0/src/prefect/runtime/task_run.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/serializers.py` & `prefect-client-2.18.0/src/prefect/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,39 +9,49 @@
 
 All serializers must implement `dumps` and `loads` which convert objects to bytes and
 bytes to an object respectively.
 """
 
 import abc
 import base64
-from typing import Any, Dict, Generic, Optional, TypeVar
+from typing import Any, Dict, Generic, Optional, Type, TypeVar
+
+from typing_extensions import Literal, Self
 
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
 from prefect._internal.schemas.validators import (
     cast_type_names_to_serializers,
     validate_compressionlib,
     validate_dump_kwargs,
     validate_load_kwargs,
     validate_picklelib,
     validate_picklelib_version,
 )
+from prefect.pydantic import HAS_PYDANTIC_V2
+from prefect.utilities.dispatch import get_dispatch_key, lookup_type, register_base_type
+from prefect.utilities.importtools import from_qualified_name, to_qualified_name
+from prefect.utilities.pydantic import custom_pydantic_encoder
 
 if HAS_PYDANTIC_V2:
-    import pydantic.v1 as pydantic
-    from pydantic.v1 import BaseModel
-    from pydantic.v1.json import pydantic_encoder
+    from pydantic.v1 import (
+        BaseModel,
+        Field,
+        ValidationError,
+        parse_obj_as,
+        root_validator,
+        validator,
+    )
 else:
-    import pydantic
-    from pydantic import BaseModel
-    from pydantic.json import pydantic_encoder
-
-from typing_extensions import Literal
-
-from prefect.utilities.importtools import from_qualified_name, to_qualified_name
-from prefect.utilities.pydantic import add_type_dispatch
+    from pydantic import (
+        BaseModel,
+        Field,
+        ValidationError,
+        parse_obj_as,
+        root_validator,
+        validator,
+    )
 
 D = TypeVar("D")
 
 
 def prefect_json_object_encoder(obj: Any) -> Any:
     """
     `JSONEncoder.default` for encoding objects into JSON with extended type support.
@@ -49,52 +59,70 @@
     Raises a `TypeError` to fallback on other encoders on failure.
     """
     if isinstance(obj, BaseException):
         return {"__exc_type__": to_qualified_name(obj.__class__), "message": str(obj)}
     else:
         return {
             "__class__": to_qualified_name(obj.__class__),
-            "data": pydantic_encoder(obj),
+            "data": custom_pydantic_encoder({}, obj),
         }
 
 
 def prefect_json_object_decoder(result: dict):
     """
     `JSONDecoder.object_hook` for decoding objects from JSON when previously encoded
     with `prefect_json_object_encoder`
     """
     if "__class__" in result:
-        return pydantic.parse_obj_as(
-            from_qualified_name(result["__class__"]), result["data"]
-        )
+        return parse_obj_as(from_qualified_name(result["__class__"]), result["data"])
     elif "__exc_type__" in result:
         return from_qualified_name(result["__exc_type__"])(result["message"])
     else:
         return result
 
 
-@add_type_dispatch
+@register_base_type
 class Serializer(BaseModel, Generic[D], abc.ABC):
     """
     A serializer that can encode objects of type 'D' into bytes.
     """
 
+    def __init__(self, **data: Any) -> None:
+        type_string = get_dispatch_key(self) if type(self) != Serializer else "__base__"
+        data.setdefault("type", type_string)
+        super().__init__(**data)
+
+    def __new__(cls: Type[Self], **kwargs) -> Self:
+        if "type" in kwargs:
+            try:
+                subcls = lookup_type(cls, dispatch_key=kwargs["type"])
+            except KeyError as exc:
+                raise ValidationError(errors=[exc], model=cls)
+
+            return super().__new__(subcls)
+        else:
+            return super().__new__(cls)
+
     type: str
 
     @abc.abstractmethod
     def dumps(self, obj: D) -> bytes:
         """Encode the object into a blob of bytes."""
 
     @abc.abstractmethod
     def loads(self, blob: bytes) -> D:
         """Decode the blob of bytes into an object."""
 
     class Config:
         extra = "forbid"
 
+    @classmethod
+    def __dispatch_key__(cls):
+        return cls.__fields__.get("type").get_default()
+
 
 class PickleSerializer(Serializer):
     """
     Serializes objects using the pickle protocol.
 
     - Uses `cloudpickle` by default. See `picklelib` for using alternative libraries.
     - Stores the version of the pickle library to check for compatibility during
@@ -103,19 +131,19 @@
     """
 
     type: Literal["pickle"] = "pickle"
 
     picklelib: str = "cloudpickle"
     picklelib_version: str = None
 
-    @pydantic.validator("picklelib")
+    @validator("picklelib")
     def check_picklelib(cls, value):
         return validate_picklelib(value)
 
-    @pydantic.root_validator
+    @root_validator
     def check_picklelib_version(cls, values):
         return validate_picklelib_version(values)
 
     def dumps(self, obj: Any) -> bytes:
         pickler = from_qualified_name(self.picklelib)
         blob = pickler.dumps(obj)
         return base64.encodebytes(blob)
@@ -131,40 +159,41 @@
 
     Input types must be compatible with the stdlib json library.
 
     Wraps the `json` library to serialize to UTF-8 bytes instead of string types.
     """
 
     type: Literal["json"] = "json"
+
     jsonlib: str = "json"
-    object_encoder: Optional[str] = pydantic.Field(
+    object_encoder: Optional[str] = Field(
         default="prefect.serializers.prefect_json_object_encoder",
         description=(
             "An optional callable to use when serializing objects that are not "
             "supported by the JSON encoder. By default, this is set to a callable that "
-            "adds support for all types supported by Pydantic."
+            "adds support for all types supported by "
         ),
     )
-    object_decoder: Optional[str] = pydantic.Field(
+    object_decoder: Optional[str] = Field(
         default="prefect.serializers.prefect_json_object_decoder",
         description=(
             "An optional callable to use when deserializing objects. This callable "
             "is passed each dictionary encountered during JSON deserialization. "
             "By default, this is set to a callable that deserializes content created "
             "by our default `object_encoder`."
         ),
     )
-    dumps_kwargs: Dict[str, Any] = pydantic.Field(default_factory=dict)
-    loads_kwargs: Dict[str, Any] = pydantic.Field(default_factory=dict)
+    dumps_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    loads_kwargs: Dict[str, Any] = Field(default_factory=dict)
 
-    @pydantic.validator("dumps_kwargs")
+    @validator("dumps_kwargs")
     def dumps_kwargs_cannot_contain_default(cls, value):
         return validate_dump_kwargs(value)
 
-    @pydantic.validator("loads_kwargs")
+    @validator("loads_kwargs")
     def loads_kwargs_cannot_contain_object_hook(cls, value):
         return validate_load_kwargs(value)
 
     def dumps(self, data: Any) -> bytes:
         json = from_qualified_name(self.jsonlib)
         kwargs = self.dumps_kwargs.copy()
         if self.object_encoder:
@@ -196,19 +225,19 @@
     """
 
     type: Literal["compressed"] = "compressed"
 
     serializer: Serializer
     compressionlib: str = "lzma"
 
-    @pydantic.validator("serializer", pre=True)
+    @validator("serializer", pre=True)
     def validate_serializer(cls, value):
         return cast_type_names_to_serializers(value)
 
-    @pydantic.validator("compressionlib")
+    @validator("compressionlib")
     def check_compressionlib(cls, value):
         return validate_compressionlib(value)
 
     def dumps(self, obj: Any) -> bytes:
         blob = self.serializer.dumps(obj)
         compressor = from_qualified_name(self.compressionlib)
         return base64.encodebytes(compressor.compress(blob))
@@ -221,17 +250,19 @@
 
 class CompressedPickleSerializer(CompressedSerializer):
     """
     A compressed serializer preconfigured to use the pickle serializer.
     """
 
     type: Literal["compressed/pickle"] = "compressed/pickle"
-    serializer: Serializer = pydantic.Field(default_factory=PickleSerializer)
+
+    serializer: Serializer = Field(default_factory=PickleSerializer)
 
 
 class CompressedJSONSerializer(CompressedSerializer):
     """
     A compressed serializer preconfigured to use the json serializer.
     """
 
     type: Literal["compressed/json"] = "compressed/json"
-    serializer: Serializer = pydantic.Field(default_factory=JSONSerializer)
+
+    serializer: Serializer = Field(default_factory=JSONSerializer)
```

### Comparing `prefect-client-2.17.1/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json` & `prefect-client-2.18.0/src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/server/api/static/prefect-logo-mark-gradient.png` & `prefect-client-2.18.0/src/prefect/server/api/static/prefect-logo-mark-gradient.png`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/settings.py` & `prefect-client-2.18.0/src/prefect/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,16 @@
 DEFAULT_PROFILES_PATH = Path(__file__).parent.joinpath("profiles.toml")
 
 REMOVED_EXPERIMENTAL_FLAGS = {
     "PREFECT_EXPERIMENTAL_ENABLE_ENHANCED_SCHEDULING_UI",
     "PREFECT_EXPERIMENTAL_ENABLE_ENHANCED_DEPLOYMENT_PARAMETERS",
     "PREFECT_EXPERIMENTAL_ENABLE_EVENTS_CLIENT",
     "PREFECT_EXPERIMENTAL_WARN_EVENTS_CLIENT",
+    "PREFECT_EXPERIMENTAL_ENABLE_FLOW_RUN_INFRA_OVERRIDES",
+    "PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES",
 }
 
 
 class Setting(Generic[T]):
     """
     Setting definition type.
     """
@@ -1538,24 +1540,14 @@
 )
 """
 How long before a PENDING task are made available to another task server.  In practice,
 a task server should move a task from PENDING to RUNNING very quickly, so runs stuck in
 PENDING for a while is a sign that the task server may have crashed.
 """
 
-PREFECT_EXPERIMENTAL_ENABLE_FLOW_RUN_INFRA_OVERRIDES = Setting(bool, default=False)
-"""
-Whether or not to enable infrastructure overrides made on flow runs.
-"""
-
-PREFECT_EXPERIMENTAL_WARN_FLOW_RUN_INFRA_OVERRIDES = Setting(bool, default=True)
-"""
-Whether or not to warn infrastructure when experimental flow runs overrides are used.
-"""
-
 PREFECT_EXPERIMENTAL_ENABLE_EXTRA_RUNNER_ENDPOINTS = Setting(bool, default=False)
 """
 Whether or not to enable experimental worker webserver endpoints.
 """
 
 PREFECT_EXPERIMENTAL_ENABLE_ARTIFACTS = Setting(bool, default=True)
 """
@@ -1697,14 +1689,18 @@
 """
 
 PREFECT_API_SERVICES_EVENT_PERSISTER_FLUSH_INTERVAL = Setting(float, default=5, gt=0.0)
 """
 The maximum number of seconds between flushes of the event persister.
 """
 
+PREFECT_API_EVENTS_STREAM_OUT_ENABLED = Setting(bool, default=True)
+"""
+Whether or not to allow streaming events out of via websockets.
+"""
 
 # Deprecated settings ------------------------------------------------------------------
 
 
 # Collect all defined settings ---------------------------------------------------------
 
 SETTING_VARIABLES: Dict[str, Any] = {
```

### Comparing `prefect-client-2.17.1/src/prefect/software/base.py` & `prefect-client-2.18.0/src/prefect/software/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/software/conda.py` & `prefect-client-2.18.0/src/prefect/software/conda.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/software/pip.py` & `prefect-client-2.18.0/src/prefect/software/pip.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/software/python.py` & `prefect-client-2.18.0/src/prefect/software/python.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/states.py` & `prefect-client-2.18.0/src/prefect/states.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/task_engine.py` & `prefect-client-2.18.0/src/prefect/task_engine.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/task_runners.py` & `prefect-client-2.18.0/src/prefect/task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/task_server.py` & `prefect-client-2.18.0/src/prefect/task_server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/tasks.py` & `prefect-client-2.18.0/src/prefect/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/annotations.py` & `prefect-client-2.18.0/src/prefect/utilities/annotations.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/asyncutils.py` & `prefect-client-2.18.0/src/prefect/utilities/asyncutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/callables.py` & `prefect-client-2.18.0/src/prefect/utilities/callables.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/collections.py` & `prefect-client-2.18.0/src/prefect/utilities/collections.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/compat.py` & `prefect-client-2.18.0/src/prefect/utilities/compat.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/context.py` & `prefect-client-2.18.0/src/prefect/utilities/context.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/dispatch.py` & `prefect-client-2.18.0/src/prefect/utilities/dispatch.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/dockerutils.py` & `prefect-client-2.18.0/src/prefect/utilities/dockerutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/engine.py` & `prefect-client-2.18.0/src/prefect/utilities/engine.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/filesystem.py` & `prefect-client-2.18.0/src/prefect/utilities/filesystem.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/hashing.py` & `prefect-client-2.18.0/src/prefect/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/importtools.py` & `prefect-client-2.18.0/src/prefect/utilities/importtools.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/math.py` & `prefect-client-2.18.0/src/prefect/utilities/math.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/names.py` & `prefect-client-2.18.0/src/prefect/utilities/names.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/processutils.py` & `prefect-client-2.18.0/src/prefect/utilities/processutils.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/pydantic.py` & `prefect-client-2.18.0/src/prefect/utilities/pydantic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from functools import partial
-from typing import Any, Callable, Generic, Type, TypeVar, cast, overload
-
-from prefect._internal.pydantic import HAS_PYDANTIC_V2
-
-if HAS_PYDANTIC_V2:
-    import pydantic.v1 as pydantic
-else:
-    import pydantic
+from typing import Any, Callable, Dict, Generic, Optional, Type, TypeVar, cast, overload
 
 from jsonpatch import JsonPatch as JsonPatchBase
+from pydantic_core import to_jsonable_python
 from typing_extensions import Self
 
+from prefect._internal.pydantic.utilities.model_dump import model_dump
+from prefect.pydantic import HAS_PYDANTIC_V2
 from prefect.utilities.dispatch import get_dispatch_key, lookup_type, register_base_type
 from prefect.utilities.importtools import from_qualified_name, to_qualified_name
 
+if HAS_PYDANTIC_V2:
+    import pydantic.v1 as pydantic_v1
+else:
+    import pydantic as pydantic_v1
+
 D = TypeVar("D", bound=Any)
-M = TypeVar("M", bound=pydantic.BaseModel)
+M = TypeVar("M", bound=pydantic_v1.BaseModel)
 
 
-def _reduce_model(model: pydantic.BaseModel):
+def _reduce_model(model: pydantic_v1.BaseModel):
     """
     Helper for serializing a cythonized model with cloudpickle.
 
     Keyword arguments can provide additional settings to the `json` call. Since
     `__reduce__` takes no arguments, these are set on the `__reduce_kwargs__` attr.
     """
     return (
@@ -78,24 +79,24 @@
             partial(
                 add_cloudpickle_reduction,
                 **kwargs,
             ),
         )
 
 
-def get_class_fields_only(model: Type[pydantic.BaseModel]) -> set:
+def get_class_fields_only(model: Type[pydantic_v1.BaseModel]) -> set:
     """
     Gets all the field names defined on the model class but not any parent classes.
     Any fields that are on the parent but redefined on the subclass are included.
     """
     subclass_class_fields = set(model.__annotations__.keys())
     parent_class_fields = set()
 
     for base in model.__class__.__bases__:
-        if issubclass(base, pydantic.BaseModel):
+        if issubclass(base, pydantic_v1.BaseModel):
             parent_class_fields.update(base.__annotations__.keys())
 
     return (subclass_class_fields - parent_class_fields) | (
         subclass_class_fields & parent_class_fields
     )
 
 
@@ -130,15 +131,15 @@
         raise ValueError(
             f"Model class {model_cls.__name__!r} does not define a `__dispatch_key__` "
             "or a type field. One of these is required for dispatch."
         )
 
     elif defines_dispatch_key and not defines_type_field:
         # Add a type field to store the value of the dispatch key
-        model_cls.__fields__["type"] = pydantic.fields.ModelField(
+        model_cls.__fields__["type"] = pydantic_v1.fields.ModelField(
             name="type",
             type_=str,
             required=True,
             class_validators=None,
             model_config=model_cls.__config__,
         )
 
@@ -176,15 +177,15 @@
         cls_init(__pydantic_self__, **data)
 
     def __new__(cls: Type[Self], **kwargs) -> Self:
         if "type" in kwargs:
             try:
                 subcls = lookup_type(cls, dispatch_key=kwargs["type"])
             except KeyError as exc:
-                raise pydantic.ValidationError(errors=[exc], model=cls)
+                raise pydantic_v1.ValidationError(errors=[exc], model=cls)
             return cls_new(subcls)
         else:
             return cls_new(cls)
 
     model_cls.__init__ = __init__
     model_cls.__new__ = __new__
 
@@ -202,15 +203,15 @@
 
     Pydantic validation does not occur until finalization.
 
     Each field can only be set once and a `ValueError` will be raised on assignment if
     a field already has a value.
 
     Example:
-        >>> class MyModel(pydantic.BaseModel):
+        >>> class MyModel(pydantic_v1.BaseModel):
         >>>     x: int
         >>>     y: str
         >>>     z: float
         >>>
         >>> partial_model = PartialModel(MyModel, x=1)
         >>> partial_model.y = "two"
         >>> model = partial_model.finalize(z=3.0)
@@ -263,7 +264,25 @@
                 "format": "rfc6902",
                 "items": {
                     "type": "object",
                     "additionalProperties": {"type": "string"},
                 },
             }
         )
+
+
+def custom_pydantic_encoder(
+    type_encoders: Optional[Dict[Any, Callable[[Type[Any]], Any]]], obj: Any
+) -> Any:
+    # Check the class type and its superclasses for a matching encoder
+    for base in obj.__class__.__mro__[:-1]:
+        try:
+            encoder = type_encoders[base]
+        except KeyError:
+            continue
+
+        return encoder(obj)
+    else:  # We have exited the for loop without finding a suitable encoder
+        if isinstance(obj, pydantic_v1.BaseModel):
+            return model_dump(obj, mode="json")
+        else:
+            return to_jsonable_python(obj)
```

### Comparing `prefect-client-2.17.1/src/prefect/utilities/render_swagger.py` & `prefect-client-2.18.0/src/prefect/utilities/render_swagger.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/schema_tools/validation.py` & `prefect-client-2.18.0/src/prefect/utilities/schema_tools/validation.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/services.py` & `prefect-client-2.18.0/src/prefect/utilities/services.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/templating.py` & `prefect-client-2.18.0/src/prefect/utilities/templating.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/utilities/visualization.py` & `prefect-client-2.18.0/src/prefect/utilities/visualization.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/variables.py` & `prefect-client-2.18.0/src/prefect/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         value: str,
         tags: Optional[List[str]] = None,
         overwrite: bool = False,
     ) -> Optional[str]:
         """
         Sets a new variable. If one exists with the same name, user must pass `overwrite=True`
         ```
-            from prefect import variables
+            from prefect.variables import Variable
 
             @flow
             def my_flow():
-                var = variables.Variable.set(name="my_var",value="test_value", tags=["hi", "there"], overwrite=True)
+                var = Variable.set(name="my_var",value="test_value", tags=["hi", "there"], overwrite=True)
         ```
         or
         ```
             from prefect.variables import Variable
 
             @flow
             async def my_flow():
@@ -65,19 +65,19 @@
 
     @classmethod
     @sync_compatible
     async def get(cls, name: str, default: Optional[str] = None) -> Optional[str]:
         """
         Get a variable by name. If doesn't exist return the default.
         ```
-            from prefect import variables
+            from prefect.variables import Variable
 
             @flow
             def my_flow():
-                var = variables.Variable.get("my_var")
+                var = Variable.get("my_var")
         ```
         or
         ```
             from prefect.variables import Variable
 
             @flow
             async def my_flow():
```

### Comparing `prefect-client-2.17.1/src/prefect/workers/base.py` & `prefect-client-2.18.0/src/prefect/workers/base.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/workers/block.py` & `prefect-client-2.18.0/src/prefect/workers/block.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/workers/process.py` & `prefect-client-2.18.0/src/prefect/workers/process.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/workers/server.py` & `prefect-client-2.18.0/src/prefect/workers/server.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect/workers/utilities.py` & `prefect-client-2.18.0/src/prefect/workers/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/src/prefect_client.egg-info/PKG-INFO` & `prefect-client-2.18.0/src/prefect_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-client
-Version: 2.17.1
+Version: 2.18.0
 Summary: Workflow orchestration and management.
 Home-page: https://www.prefect.io
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/PrefectHQ/prefect/blob/main/RELEASE-NOTES.md
 Project-URL: Documentation, https://docs.prefect.io
```

### Comparing `prefect-client-2.17.1/src/prefect_client.egg-info/SOURCES.txt` & `prefect-client-2.18.0/src/prefect_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,16 @@
 src/prefect/events/actions.py
 src/prefect/events/clients.py
 src/prefect/events/filters.py
 src/prefect/events/instrument.py
 src/prefect/events/related.py
 src/prefect/events/utilities.py
 src/prefect/events/worker.py
+src/prefect/events/cli/__init__.py
+src/prefect/events/cli/automations.py
 src/prefect/events/schemas/__init__.py
 src/prefect/events/schemas/automations.py
 src/prefect/events/schemas/deployment_triggers.py
 src/prefect/events/schemas/events.py
 src/prefect/events/schemas/labelling.py
 src/prefect/infrastructure/__init__.py
 src/prefect/infrastructure/base.py
@@ -252,14 +254,15 @@
 src/prefect/server/api/collections_data/views/aggregate-worker-metadata.json
 src/prefect/server/api/static/prefect-logo-mark-gradient.png
 src/prefect/software/__init__.py
 src/prefect/software/base.py
 src/prefect/software/conda.py
 src/prefect/software/pip.py
 src/prefect/software/python.py
+src/prefect/types/__init__.py
 src/prefect/utilities/__init__.py
 src/prefect/utilities/annotations.py
 src/prefect/utilities/asyncutils.py
 src/prefect/utilities/callables.py
 src/prefect/utilities/collections.py
 src/prefect/utilities/compat.py
 src/prefect/utilities/context.py
```

### Comparing `prefect-client-2.17.1/src/prefect_client.egg-info/requires.txt` & `prefect-client-2.18.0/src/prefect_client.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-client-2.17.1/versioneer.py` & `prefect-client-2.18.0/versioneer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,63 @@
-# Version: 0.20
-# versioneer is on 0.29, would be good to update
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -227,17 +254,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -259,54 +287,88 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
+import functools
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, Dict, List, NoReturn, Optional, Tuple, Union, cast
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods # noqa
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
+
 
-def get_root():
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = (
             "Versioneer was unable to run the project root directory. "
             "Versioneer requires setup.py to be executed from "
             "its immediate directory (like 'python setup.py COMMAND'), "
             "or in a way that lets it use sys.argv[0] to find the root "
             "(like 'python path/to/setup.py COMMAND')."
         )
@@ -317,92 +379,125 @@
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print(
                 "Warning: build in %s is using versioneer.py from %s"
                 % (os.path.dirname(my_path), versioneer_py)
             )
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, "rb") as fobj:
+                pp = tomllib.load(fobj)
+            section = pp["tool"]["versioneer"]
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
 
-    # pylint:disable=attribute-defined-outside-init # noqa
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
-    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
     cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
-    cfg.verbose = section.get("verbose")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
 
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen(
                 [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
             )
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
@@ -421,44 +516,54 @@
 LONG_VERSION_PY["git"] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.20 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
     git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
-class VersioneerConfig:  # pylint: disable=too-few-public-methods
+class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -468,46 +573,58 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-# pylint:disable=too-many-arguments,consider-using-with # noqa
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
@@ -519,15 +636,19 @@
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -544,21 +665,21 @@
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -566,21 +687,25 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -636,48 +761,60 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match", "%%s*" %% tag_prefix],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
                              cwd=root)
     # --abbrev-ref was added in git-1.6.3
@@ -748,35 +885,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -793,15 +930,15 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -823,31 +960,49 @@
         rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -866,15 +1021,15 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -895,15 +1050,15 @@
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -917,15 +1072,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -937,15 +1092,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -957,15 +1112,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
@@ -993,15 +1148,15 @@
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -1041,21 +1196,21 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -1063,21 +1218,25 @@
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["full"] = mo.group(1)
                 if line.strip().startswith("git_date ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["date"] = mo.group(1)
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -1140,26 +1299,35 @@
         "dirty": False,
         "error": "no suitable tags",
         "date": None,
     }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
@@ -1168,28 +1336,28 @@
         [
             "describe",
             "--tags",
             "--dirty",
             "--always",
             "--long",
             "--match",
-            "%s*" % tag_prefix,
+            f"{tag_prefix}[[:digit:]]*",
         ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
@@ -1260,65 +1428,70 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
                         break
-    except EnvironmentError:
+    except OSError:
         pass
     if not present:
         with open(".gitattributes", "a+") as fobj:
             fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -1341,15 +1514,15 @@
             "Tried directories %s but none started with prefix %s"
             % (str(rootdirs), parentdir_prefix)
         )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.20) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1358,51 +1531,50 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(
         r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
     )
     if not mo:
         mo = re.search(
             r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
         )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1418,15 +1590,15 @@
         # exception #1
         rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -1447,31 +1619,49 @@
             rendered += ".dev0"
         rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post0.devDISTANCE] -- No -dirty.
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
         if pieces["distance"]:
-            rendered += ".post0.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1490,15 +1680,15 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -1519,15 +1709,15 @@
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1541,15 +1731,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1561,15 +1751,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1581,15 +1771,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {
             "version": "unknown",
             "full-revisionid": pieces.get("long"),
             "dirty": None,
             "error": pieces["error"],
@@ -1627,30 +1817,30 @@
     }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert (
         cfg.versionfile_source is not None
     ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
@@ -1708,20 +1898,20 @@
         "full-revisionid": None,
         "dirty": None,
         "error": "unable to compute version",
         "date": None,
     }
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass=None):
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
     """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
@@ -1736,111 +1926,127 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
+    # we add "version" to setuptools
     from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
 
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if "build_py" in cmds:
-        _build_py = cmds["build_py"]
-    elif "setuptools" in sys.modules:
+        _build_py: Any = cmds["build_py"]
+    else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
     cmds["build_py"] = cmd_build_py
 
     if "build_ext" in cmds:
-        _build_ext = cmds["build_ext"]
-    elif "setuptools" in sys.modules:
+        _build_ext: Any = cmds["build_ext"]
+    else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
             if self.inplace:
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
+            if not cfg.versionfile_build:
+                return
             target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
+                return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
 
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
-
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1859,18 +2065,21 @@
                         }
                     )
 
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if "py2exe" in sys.modules:  # py2exe enabled?
-        from py2exe.setuptools_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1887,31 +2096,70 @@
                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         }
                     )
 
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if "egg_info" in cmds:
+        _egg_info: Any = cmds["egg_info"]
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append("versioneer.py")
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
+
+    cmds["egg_info"] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if "sdist" in cmds:
-        _sdist = cmds["sdist"]
-    elif "setuptools" in sys.modules:
+        _sdist: Any = cmds["sdist"]
+    else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
-            # pylint:disable=attribute-defined-outside-init # noqa
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1970,25 +2218,21 @@
 
 INIT_PY_SNIPPET = """
 from . import {0}
 __version__ = {0}.get_versions()['version']
 """
 
 
-def do_setup():
+def do_setup() -> int:
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
@@ -2002,19 +2246,20 @@
                 "TAG_PREFIX": cfg.tag_prefix,
                 "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
             print(" replacing boilerplate in %s" % ipy)
             with open(ipy, "w") as f:
                 f.write(old.replace(OLD_SNIPPET, snippet))
@@ -2022,58 +2267,24 @@
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -2102,14 +2313,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

