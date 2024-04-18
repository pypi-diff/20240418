# Comparing `tmp/lilya-0.3.5.tar.gz` & `tmp/lilya-0.4.0.tar.gz`

## Comparing `lilya-0.3.5.tar` & `lilya-0.4.0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/__main__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_utils.py
--rw-r--r--   0        0        0    29346 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/apps.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/background.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/compat.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/concurrency.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/context.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/controllers.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/crypto.py
--rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/datastructures.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/encoders.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/enums.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/exceptions.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/logging.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/py.typed
--rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/requests.py
--rw-r--r--   0        0        0    16901 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/responses.py
--rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/routing.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/staticfiles.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/status.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/transformers.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/types.py
--rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/websockets.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/__init__.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_connection.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_encoders.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_events.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_exception_handlers.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_helpers.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_message.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_module_loading.py
--rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_parsers.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_path.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_path_transformers.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_representation.py
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_responses.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/__init__.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/base.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/cli.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/constants.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/env.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/parsers.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/templates.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/_constants.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/createapp.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/createproject.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/list.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/run.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/runserver.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/terminal/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/terminal/base.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/terminal/print.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/cli/terminal/terminal.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/conf/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/conf/enums.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/conf/exceptions.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/conf/functional.py
--rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/conf/global_settings.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/app_settings.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/asyncexit.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/authentication.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/base.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/compression.py
--rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/cors.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/csrf.py
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/exceptions.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/httpsredirect.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/server_error.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/sessions.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/trustedhost.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/styles/__init__.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/middleware/styles/errors.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/permissions/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/permissions/base.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/permissions/deny_all.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/protocols/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/protocols/authentication.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/protocols/middleware.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/protocols/permissions.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/templating/__init__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/templating/base.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/templating/jinja.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/testclient/__init__.py
--rw-r--r--   0        0        0    32033 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/testclient/base.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 lilya-0.3.5/lilya/testclient/helpers.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.3.5/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.3.5/LICENSE
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.3.5/README.md
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 lilya-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 lilya-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/__main__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_utils.py
+-rw-r--r--   0        0        0    29346 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/apps.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/background.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/compat.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/concurrency.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/context.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/controllers.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/crypto.py
+-rw-r--r--   0        0        0    22252 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/datastructures.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/encoders.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/enums.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/exceptions.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/logging.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/py.typed
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/requests.py
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/responses.py
+-rw-r--r--   0        0        0    53033 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/routing.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/staticfiles.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/status.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/transformers.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/types.py
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/websockets.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/__init__.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_connection.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_encoders.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_events.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_exception_handlers.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_helpers.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_message.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_module_loading.py
+-rw-r--r--   0        0        0    16818 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_parsers.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_path.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_path_transformers.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_representation.py
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_responses.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/_internal/_templates/project_template_simple/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/__init__.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/base.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/cli.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/constants.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/env.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/parsers.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/templates.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/list.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/run.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/terminal/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/terminal/base.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/terminal/print.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/cli/terminal/terminal.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/conf/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/conf/enums.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/conf/exceptions.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/conf/functional.py
+-rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/conf/global_settings.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/app_settings.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/asyncexit.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/authentication.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/base.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/compression.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/cors.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/csrf.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/exceptions.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/httpsredirect.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/server_error.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/sessions.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/trustedhost.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/styles/__init__.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/middleware/styles/errors.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/permissions/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/permissions/base.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/permissions/deny_all.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/protocols/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/protocols/authentication.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/protocols/middleware.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/protocols/permissions.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/templating/__init__.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/templating/base.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/templating/jinja.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/testclient/__init__.py
+-rw-r--r--   0        0        0    32033 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/testclient/base.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 lilya-0.4.0/lilya/testclient/helpers.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lilya-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 lilya-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 lilya-0.4.0/README.md
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 lilya-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 lilya-0.4.0/PKG-INFO
```

### Comparing `lilya-0.3.5/lilya/_utils.py` & `lilya-0.4.0/lilya/_utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/apps.py` & `lilya-0.4.0/lilya/apps.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/background.py` & `lilya-0.4.0/lilya/background.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/compat.py` & `lilya-0.4.0/lilya/compat.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/concurrency.py` & `lilya-0.4.0/lilya/concurrency.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/context.py` & `lilya-0.4.0/lilya/context.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/controllers.py` & `lilya-0.4.0/lilya/controllers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/crypto.py` & `lilya-0.4.0/lilya/crypto.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/datastructures.py` & `lilya-0.4.0/lilya/datastructures.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/enums.py` & `lilya-0.4.0/lilya/enums.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/exceptions.py` & `lilya-0.4.0/lilya/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/logging.py` & `lilya-0.4.0/lilya/logging.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/requests.py` & `lilya-0.4.0/lilya/requests.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/responses.py` & `lilya-0.4.0/lilya/responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     AsyncIterable,
     Awaitable,
     Callable,
     Iterable,
     Literal,
     Mapping,
     NoReturn,
+    Sequence,
     Union,
 )
 from urllib.parse import quote
 
 import anyio
 
 from lilya import status
 from lilya._internal._encoders import json_encoder
 from lilya._internal._helpers import HeaderHelper
 from lilya.background import Task
 from lilya.compat import md5_hexdigest
 from lilya.concurrency import iterate_in_threadpool
 from lilya.datastructures import URL, Header
+from lilya.encoders import Encoder, register_encoder
 from lilya.enums import Event, HTTPMethod, MediaType
 from lilya.types import Receive, Scope, Send
 
 Content = Union[str, bytes]
 SyncContentStream = Iterable[Content]
 AsyncContentStream = AsyncIterable[Content]
 ContentStream = Union[AsyncContentStream, SyncContentStream]
@@ -49,21 +51,27 @@
         self,
         content: Any = None,
         status_code: int = status.HTTP_200_OK,
         headers: Mapping[str, str] | None = None,
         cookies: Mapping[str, str] | Any | None = None,
         media_type: str | None = None,
         background: Task | None = None,
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ) -> None:
         if status_code is not None:
             self.status_code = status_code
         if media_type is not None:
             self.media_type = media_type
         self.background = background
         self.cookies = cookies
+        self.encoders = encoders or []
+
+        for encoder in self.encoders:
+            register_encoder(encoder)
+
         self.body = self.make_response(content)
         self.raw_headers: list[Any] = []
         self.make_headers(headers)
 
     def make_response(self, content: Any) -> bytes | str:
         """
         Makes the Response object type.
@@ -248,21 +256,23 @@
     def __init__(
         self,
         content: Any,
         status_code: int = status.HTTP_200_OK,
         headers: Mapping[str, str] | None = None,
         media_type: str | None = None,
         background: Task | None = None,
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ) -> None:
         super().__init__(
             content=content,
             status_code=status_code,
             headers=headers,
             media_type=media_type,
             background=background,
+            encoders=encoders,
         )
 
     def make_response(self, content: Any) -> bytes:
         return json.dumps(
             content,
             ensure_ascii=False,
             allow_nan=False,
@@ -278,32 +288,42 @@
 class RedirectResponse(Response):
     def __init__(
         self,
         url: str | URL,
         status_code: int = status.HTTP_307_TEMPORARY_REDIRECT,
         headers: Mapping[str, str] | None = None,
         background: Task | None = None,
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ) -> None:
         super().__init__(
-            content=b"", status_code=status_code, headers=headers, background=background
+            content=b"",
+            status_code=status_code,
+            headers=headers,
+            background=background,
+            encoders=encoders,
         )
         self.headers["location"] = quote(str(url), safe=":/%#?=@[]!$&'()*+,;")
 
 
 class StreamingResponse(Response):
     body_iterator: AsyncContentStream
 
     def __init__(
         self,
         content: ContentStream,
         status_code: int = status.HTTP_200_OK,
         headers: Mapping[str, str] | None = None,
         media_type: str | None = None,
         background: Task | None = None,
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ) -> None:
+        self.encoders = encoders or []
+        for encoder in self.encoders:
+            register_encoder(encoder)
+
         if isinstance(content, AsyncIterable):
             self.body_iterator = content
         else:
             self.body_iterator = iterate_in_threadpool(content)
         self.status_code = status_code
         self.media_type = self.media_type if media_type is None else media_type
         self.background = background
@@ -349,23 +369,29 @@
         headers: typing.Mapping[str, str] | None = None,
         media_type: str | None = None,
         background: Task | None = None,
         filename: str | None = None,
         stat_result: os.stat_result | None = None,
         method: str | None = None,
         content_disposition_type: str = "attachment",
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ) -> None:
         self.path = path
         self.status_code = status_code
         self.filename = filename
         self.send_header_only = method is not None and method.upper() == HTTPMethod.HEAD
         if media_type is None:
             media_type = guess_type(filename or path)[0] or MediaType.TEXT
         self.media_type = media_type
         self.background = background
+
+        self.encoders = encoders or []
+        for encoder in self.encoders:
+            register_encoder(encoder)
+
         self.make_headers(headers)
 
         if self.filename is not None:
             content_disposition_filename = quote(self.filename)
             if content_disposition_filename != self.filename:
                 content_disposition = (
                     f"{content_disposition_type}; filename*=utf-8''{content_disposition_filename}"
@@ -426,24 +452,26 @@
         self,
         template: Any,
         status_code: int = status.HTTP_200_OK,
         context: dict[str, Any] | None = None,
         background: Task | None = None,
         headers: dict[str, Any] | None = None,
         media_type: MediaType | str = MediaType.HTML,
+        encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
     ):
         self.template = template
         self.context = context or {}
         content = self.template.render(context)
         super().__init__(
             content=content,
             status_code=status_code,
             headers=headers,
             media_type=media_type,
             background=background,
+            encoders=encoders,
         )
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         request = self.context.get("request", {})
         extensions = request.get("extensions", {})
         if "http.response.debug" in extensions:
             await send(
@@ -457,21 +485,23 @@
 
 def make_response(
     content: Any,
     response_class: type[Response] = JSONResponse,
     status_code: int = status.HTTP_200_OK,
     headers: Mapping[str, str] | None = None,
     background: Task | None = None,
+    encoders: Sequence[Encoder[Any]] | Sequence[type[Encoder[Any]]] | None = None,
 ) -> Response:
     """
     Build JSON responses from a given content and
     providing extra parameters.
     """
     app = json_encoder(content) if content is not None else None
 
     return response_class(
         content=app,
         status_code=status_code,
         headers=headers,
         media_type=MediaType.JSON,
         background=background,
+        encoders=encoders,
     )
```

### Comparing `lilya-0.3.5/lilya/routing.py` & `lilya-0.4.0/lilya/routing.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/staticfiles.py` & `lilya-0.4.0/lilya/staticfiles.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/status.py` & `lilya-0.4.0/lilya/status.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/types.py` & `lilya-0.4.0/lilya/types.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/websockets.py` & `lilya-0.4.0/lilya/websockets.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_connection.py` & `lilya-0.4.0/lilya/_internal/_connection.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_encoders.py` & `lilya-0.4.0/lilya/_internal/_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     PurePathEncoder(),
     PrimitiveEncoder(),
     DictEncoder(),
     StructureEncoder(),
 }
 
 
-def register_encoder(encoder: Encoder[Any]) -> None:
+def register_encoder(encoder: Encoder[Any] | type[Encoder[Any]]) -> None:
     if is_class_and_subclass(encoder, Encoder):
         encoder = encoder()  # type: ignore
-    ENCODER_TYPES.add(encoder)
+    ENCODER_TYPES.add(cast(Encoder[Any], encoder))
 
 
 def json_encoder(value: Any) -> Any:
     result: Any = None
 
     for encoder in ENCODER_TYPES:
         try:
```

### Comparing `lilya-0.3.5/lilya/_internal/_events.py` & `lilya-0.4.0/lilya/_internal/_events.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_exception_handlers.py` & `lilya-0.4.0/lilya/_internal/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_helpers.py` & `lilya-0.4.0/lilya/_internal/_helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_module_loading.py` & `lilya-0.4.0/lilya/_internal/_module_loading.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_parsers.py` & `lilya-0.4.0/lilya/_internal/_parsers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_path.py` & `lilya-0.4.0/lilya/_internal/_path.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_path_transformers.py` & `lilya-0.4.0/lilya/_internal/_path_transformers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_representation.py` & `lilya-0.4.0/lilya/_internal/_representation.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_responses.py` & `lilya-0.4.0/lilya/_internal/_responses.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_urls.py` & `lilya-0.4.0/lilya/_internal/_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template/.gitignore.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template/Makefile.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/main.py-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/serve.py-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template/project_name/urls.py-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template_simple/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template_simple/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl` & `lilya-0.4.0/lilya/_internal/_templates/project_template_simple/project_name/app.py-tpl`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/base.py` & `lilya-0.4.0/lilya/cli/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/cli.py` & `lilya-0.4.0/lilya/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/env.py` & `lilya-0.4.0/lilya/cli/env.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/templates.py` & `lilya-0.4.0/lilya/cli/templates.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/utils.py` & `lilya-0.4.0/lilya/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/createapp.py` & `lilya-0.4.0/lilya/cli/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/createdeployment.py` & `lilya-0.4.0/lilya/cli/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/createproject.py` & `lilya-0.4.0/lilya/cli/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/list.py` & `lilya-0.4.0/lilya/cli/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/run.py` & `lilya-0.4.0/lilya/cli/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/runserver.py` & `lilya-0.4.0/lilya/cli/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/show_urls.py` & `lilya-0.4.0/lilya/cli/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/shell/base.py` & `lilya-0.4.0/lilya/cli/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/shell/ipython.py` & `lilya-0.4.0/lilya/cli/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/shell/ptpython.py` & `lilya-0.4.0/lilya/cli/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/directives/operations/shell/utils.py` & `lilya-0.4.0/lilya/cli/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/terminal/base.py` & `lilya-0.4.0/lilya/cli/terminal/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/terminal/print.py` & `lilya-0.4.0/lilya/cli/terminal/print.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/cli/terminal/terminal.py` & `lilya-0.4.0/lilya/cli/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/conf/__init__.py` & `lilya-0.4.0/lilya/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/conf/functional.py` & `lilya-0.4.0/lilya/conf/functional.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/conf/global_settings.py` & `lilya-0.4.0/lilya/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/app_settings.py` & `lilya-0.4.0/lilya/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/asyncexit.py` & `lilya-0.4.0/lilya/middleware/asyncexit.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/authentication.py` & `lilya-0.4.0/lilya/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/base.py` & `lilya-0.4.0/lilya/middleware/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/compression.py` & `lilya-0.4.0/lilya/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/cors.py` & `lilya-0.4.0/lilya/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/csrf.py` & `lilya-0.4.0/lilya/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/exceptions.py` & `lilya-0.4.0/lilya/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/httpsredirect.py` & `lilya-0.4.0/lilya/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/server_error.py` & `lilya-0.4.0/lilya/middleware/server_error.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/sessions.py` & `lilya-0.4.0/lilya/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/trustedhost.py` & `lilya-0.4.0/lilya/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/wsgi.py` & `lilya-0.4.0/lilya/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/middleware/styles/errors.py` & `lilya-0.4.0/lilya/middleware/styles/errors.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/permissions/base.py` & `lilya-0.4.0/lilya/permissions/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/permissions/deny_all.py` & `lilya-0.4.0/lilya/permissions/deny_all.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/protocols/authentication.py` & `lilya-0.4.0/lilya/protocols/authentication.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/protocols/middleware.py` & `lilya-0.4.0/lilya/protocols/middleware.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/protocols/permissions.py` & `lilya-0.4.0/lilya/protocols/permissions.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/templating/base.py` & `lilya-0.4.0/lilya/templating/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/templating/jinja.py` & `lilya-0.4.0/lilya/templating/jinja.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/testclient/base.py` & `lilya-0.4.0/lilya/testclient/base.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/lilya/testclient/helpers.py` & `lilya-0.4.0/lilya/testclient/helpers.py`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/LICENSE` & `lilya-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/README.md` & `lilya-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/pyproject.toml` & `lilya-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lilya-0.3.5/PKG-INFO` & `lilya-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lilya
-Version: 0.3.5
+Version: 0.4.0
 Summary: Yet another ASGI toolkit that delivers
 Project-URL: Homepage, https://github.com/dymmond/lilya
 Project-URL: Documentation, https://lilya.dev
 Project-URL: Changelog, https://lilya.dev/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/lilya
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
```

