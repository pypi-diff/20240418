# Comparing `tmp/runit-server-0.4.1.tar.gz` & `tmp/runit_server-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit-server-0.4.1.tar", last modified: Thu Apr 11 19:13:09 2024, max compression
+gzip compressed data, was "runit_server-0.4.2.tar", last modified: Thu Apr 18 18:09:55 2024, max compression
```

## Comparing `runit-server-0.4.1.tar` & `runit_server-0.4.2.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.803169 runit-server-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-11 19:13:05.000000 runit-server-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 19:13:05.000000 runit-server-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 19:13:09.799169 runit-server-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-11 19:13:05.000000 runit-server-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.775169 runit-server-0.4.1/runit_server/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.775169 runit-server-0.4.1/runit_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/dockerize.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/kubernetes-1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/kubernetes-2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/models/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/modules/account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.779169 runit-server-0.4.1/runit_server/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/routers/api/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/api/public.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/routers/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.771169 runit-server-0.4.1/runit_server/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   232948 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589161 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/dark-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40957 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.783169 runit-server-0.4.1/runit_server/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/html5.svg
--rw-r--r--   0 runner    (1001) docker     (127)    46753 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/nodejs.png
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/nodejs.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/php.svg
--rw-r--r--   0 runner    (1001) docker     (127)   150090 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python.png
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/python1.svg
--rw-r--r--   0 runner    (1001) docker     (127)   587840 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/images/terminal.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.787169 runit-server-0.4.1/runit_server/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    80663 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   331886 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/databases.js
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/github.js
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/profile.js
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/projects.js
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/js/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.791169 runit-server-0.4.1/runit_server/static/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   133034 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   715890 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    89824 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76612 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34390 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144322 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   202902 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   897426 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   202616 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   103300 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    79444 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/account/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/account/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/databases/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/modals/database.html
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/databases/modals/document.html
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.795169 runit-server-0.4.1/runit_server/templates/admin/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/projects/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/admin/users/
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/admin/users/modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/databases/modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/bun.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/node.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/php.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/docker/python.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/exposed.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/functions/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/modals/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/modals/confirm.html
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/modals/create_database.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/projects/
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/projects/modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server/templates/setup/
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/setup/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/templates/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 19:13:05.000000 runit-server-0.4.1/runit_server/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:13:09.799169 runit-server-0.4.1/runit_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 19:13:09.000000 runit-server-0.4.1/runit_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:13:09.803169 runit-server-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-11 19:13:05.000000 runit-server-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 18:09:51.000000 runit_server-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 18:09:51.000000 runit_server-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-18 18:09:55.701317 runit_server-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-18 18:09:51.000000 runit_server-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.673316 runit_server-0.4.2/runit_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.677317 runit_server-0.4.2/runit_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/common/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/common/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/dockerize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/kubernetes-1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/kubernetes-2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.677317 runit_server-0.4.2/runit_server/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.677317 runit_server-0.4.2/runit_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/modules/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.681316 runit_server-0.4.2/runit_server/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.681316 runit_server-0.4.2/runit_server/routers/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/api/public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/routers/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.669316 runit_server-0.4.2/runit_server/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.681316 runit_server-0.4.2/runit_server/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    58578 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   232948 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589161 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.681316 runit_server-0.4.2/runit_server/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/dark-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40957 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.685317 runit_server-0.4.2/runit_server/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    46753 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/nodejs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/nodejs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/php.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   150090 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/python.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/python1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   587840 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/images/terminal.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.685317 runit_server-0.4.2/runit_server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    80663 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   331886 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/databases.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/github.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/profile.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/projects.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/js/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.693317 runit_server-0.4.2/runit_server/static/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   133034 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   715890 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   132728 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    89824 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76612 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34390 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144322 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   202902 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   897426 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   202616 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   103300 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    79444 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.693317 runit_server-0.4.2/runit_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.693317 runit_server-0.4.2/runit_server/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/account/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/account/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/account/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.693317 runit_server-0.4.2/runit_server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.697317 runit_server-0.4.2/runit_server/templates/admin/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.697317 runit_server-0.4.2/runit_server/templates/admin/databases/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/modals/database.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/databases/modals/document.html
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.697317 runit_server-0.4.2/runit_server/templates/admin/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/projects/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/projects/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/projects/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/projects/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/projects/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.697317 runit_server-0.4.2/runit_server/templates/admin/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/users/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/users/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/users/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/admin/users/modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.697317 runit_server-0.4.2/runit_server/templates/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/databases/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/databases/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/databases/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/databases/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/databases/modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/docker/bun.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/docker/node.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/docker/php.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/docker/python.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/exposed.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server/templates/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/functions/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server/templates/modals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/modals/confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/modals/create_database.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server/templates/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/projects/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/projects/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/projects/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/projects/list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/projects/modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server/templates/setup/
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/setup/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/templates/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-18 18:09:51.000000 runit_server-0.4.2/runit_server/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:09:55.701317 runit_server-0.4.2/runit_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 18:09:55.000000 runit_server-0.4.2/runit_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:09:55.701317 runit_server-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-18 18:09:51.000000 runit_server-0.4.2/setup.py
```

### Comparing `runit-server-0.4.1/LICENSE` & `runit_server-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/PKG-INFO` & `runit_server-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.4.1
+Version: 0.4.2
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit-server-0.4.1/README.md` & `runit_server-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/Request.py` & `runit_server-0.4.2/runit_server/Request.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/app.py` & `runit_server-0.4.2/runit_server/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,67 @@
 from typing import Optional
 from pathlib import Path
 from sys import platform
 from datetime import timedelta
 
-
 from fastapi import FastAPI, Request, status, Depends
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse
-from starlette.middleware import Middleware
 from starlette.middleware.sessions import SessionMiddleware
 
-from dotenv import load_dotenv
-
 from .core import lifespan, templates
 from .exceptions import UnauthorizedException, UnauthorizedAdminException
-from .constants import RUNIT_WORKDIR, SESSION_SECRET_KEY
+from .constants import RUNIT_WORKDIR, SESSION_SECRET_KEY, DOTENV_FILE
 
+from dotenv import load_dotenv
 
 from .routers import account
 from .routers import project
 from .routers import database
 from .routers import github_router
 from .routers import admin
 from .routers import public
 from .routers import setup
 
 from .routers.api import api_router
 
-load_dotenv()
+load_dotenv(DOTENV_FILE)
 
 app = FastAPI(dependencies=[Depends(lifespan)], force_https=True)
 app.add_middleware(
     SessionMiddleware,
     secret_key=SESSION_SECRET_KEY,
     max_age=3600,
     https_only=True
 )
 
 static = Path(__file__).resolve().parent / "static"
 uploads = Path(RUNIT_WORKDIR, 'accounts')
 app.mount('/static', StaticFiles(directory=static, html=True),  name='static')
-
-if not Path(RUNIT_WORKDIR).exists():
-    Path(RUNIT_WORKDIR).mkdir()
     
-if not Path(uploads).resolve().exists():
-    Path(uploads).resolve().mkdir()
+if not uploads.resolve().exists():
+    uploads.resolve().mkdir()
     
 
 app.mount('/uploads', StaticFiles(directory=uploads, html=True),  name='uploads')
 
+# # Create Database tables
+# Admin.create_table()
+# User.create_table()
+# Permission.create_table()
+# Role.create_table()   
+# Project.create_table()   
+# Database.create_table()   
+
+# # print('[--] Database setup complete')
+# # Populate tables initially
+# if not Role.count():
+#     print('[#] Populating Roles')
+    
+#     print('[--] Roles populated')
 
 app.include_router(api_router)
 app.include_router(admin)
 app.include_router(account)
 app.include_router(project)
 app.include_router(database)
 app.include_router(github_router)
```

### Comparing `runit-server-0.4.1/runit_server/auth.py` & `runit_server-0.4.2/runit_server/auth.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/aws.py` & `runit_server-0.4.2/runit_server/aws.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/azure.py` & `runit_server-0.4.2/runit_server/azure.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/cli.py` & `runit_server-0.4.2/runit_server/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import os
+from pathlib import Path
 import sys
 import logging
 import argparse
 from getpass import getpass
 
 from dotenv import load_dotenv, set_key, find_dotenv, dotenv_values
 
 from .app import app
 
 from odbms import DBMS
-from .models import Role, Admin
+from .models import Role, Admin, User, Permission
 
 from runit import RunIt
 
-from .constants import RUNIT_WORKDIR, VERSION
+from .constants import RUNIT_WORKDIR, RUNIT_HOMEDIR, DOTENV_FILE, VERSION
 import uvicorn
 
 logging.getLogger('uvicorn').setLevel(logging.INFO)
 
-load_dotenv()
+load_dotenv(DOTENV_FILE)
 
-CURDIR = os.path.dirname(os.path.realpath(__file__))
 RunIt.RUNTIME_ENV = 'server'
 
 def setup_database():
     '''
     Connect to database using connection settings from .env
     
     @params None
     @return None
     '''
-    settings = dotenv_values(find_dotenv())
-    DBMS.initialize(settings['DBMS'], settings['DATABASE_HOST'], settings['DATABASE_PORT'], # type: ignore
+    settings = dotenv_values(find_dotenv(str(DOTENV_FILE)))
+    if settings.get('DBMS') == 'sqlite':
+        DBMS.initialize_with_defaults('sqlitle', settings.get('DATABASE_NAME'))
+    
+    else:
+        DBMS.initialize(settings['DBMS'], settings['DATABASE_HOST'], settings['DATABASE_PORT'], # type: ignore
                     settings['DATABASE_USERNAME'], settings['DATABASE_PASSWORD'],  # type: ignore
                     settings['DATABASE_NAME']) # type: ignore
-    if settings['DBMS'] == 'mysql':
-        DBMS.Database.setup() # type: ignore
     
+    # Create tables if they do not exist in relational datatabases
+    # [sqlite, mysql, postgresql]
+    Admin.create_table()
+    User.create_table()
+    Permission.create_table()
+    Role.create_table()   
+     
     # print('[--] Database setup complete')
-    
+    # Populate tables initially
     if not Role.count():
         print('[#] Populating Roles')
         Role('developer', []).save()
         Role('superadmin', []).save()
         Role('subadmin', []).save()
         print('[--] Roles populated')
     
@@ -61,17 +70,19 @@
     '''
     Create .env file and populate with {settings}
     
     @param settings dict Dictionary of default settings
     @return None
     '''
     
-    open('.env', 'wt').close()
+    if not DOTENV_FILE.resolve().exists():
+        open(DOTENV_FILE, 'wt').close()
+        
     for key, value in settings.items():
-        set_key(find_dotenv(), key, value)
+        set_key(str(DOTENV_FILE), key, value)
 
 def create_default_admin(args_is_true: bool = False):
     '''
     Create the default administrator account
     
     @params None
     @return None
@@ -111,79 +122,74 @@
 def setup_runit(args):
     '''
     Setup Runit server side
     
     @params args
     @return None
     '''
-    if args.admin:
-        return create_default_admin(args.admin)
+    try:
+        if args.admin:
+            return create_default_admin(args.admin)
+            
+        domain = args.domain if hasattr(args, 'domain') else ''
+        allowed = ['DBMS', 'DATABASE_HOST', 'DATABASE_PORT', 
+                'DATABASE_USERNAME', 'DATABASE_PASSWORD', 
+                'DATABASE_NAME', 'RUNTIME_PYTHON', 'RUNTIME_PHP',
+                'RUNTIME_JAVASCRIPT', 'GITHUB_APP_CLIENT_ID',
+                'GITHUB_APP_CLIENT_SECRET']
+        
+        default_settings = {
+            'RUNIT_WORKDIR': str(RUNIT_WORKDIR),
+            'RUNIT_HOMEDIR': str(RUNIT_HOMEDIR),
+            'RUNIT_SERVERNAME': '',
+            'DBMS': 'sqlite',
+            'DATABASE_HOST': '127.0.0.1',
+            'DATABASE_PORT': '',
+            'DATABASE_USERNAME': '',
+            'DATABASE_PASSWORD': '',
+            'DATABASE_NAME': 'runit',
+            'RUNTIME_PYTHON': 'python',
+            'RUNTIME_PHP': 'php',
+            'RUNTIME_JAVASCRIPT': 'node',
+            'GITHUB_APP_CLIENT_ID': '',
+            'GITHUB_APP_CLIENT_SECRET': '',
+            'SETUP': ''
+        }
+
+        settings = dotenv_values(find_dotenv(str(DOTENV_FILE)))
         
-    domain = args.domain if hasattr(args, 'domain') else ''
-    allowed = ['DBMS', 'DATABASE_HOST', 'DATABASE_PORT', 
-               'DATABASE_USERNAME', 'DATABASE_PASSWORD', 
-               'DATABASE_NAME', 'RUNTIME_PYTHON', 'RUNTIME_PHP',
-               'RUNTIME_JAVASCRIPT', 'GITHUB_APP_CLIENT_ID',
-               'GITHUB_APP_CLIENT_SECRET']
-    
-    default_settings = {
-        'RUNIT_WORKDIR': os.path.join(os.path.expanduser('~'), 'RUNIT_WORKDIR'),
-        'RUNIT_HOMEDIR': CURDIR,
-        'RUNIT_SERVERNAME': '',
-        'DBMS': 'mongodb',
-        'DATABASE_HOST': 'localhost',
-        'DATABASE_PORT': '27017',
-        'DATABASE_USERNAME': '',
-        'DATABASE_PASSWORD': '',
-        'DATABASE_NAME': 'runit',
-        'RUNTIME_PYTHON': 'python',
-        'RUNTIME_PHP': 'php',
-        'RUNTIME_JAVASCRIPT': 'node',
-        'GITHUB_APP_CLIENT_ID': '',
-        'GITHUB_APP_CLIENT_SECRET': '',
-        'SETUP': ''
-    }
-
-    settings = dotenv_values(find_dotenv())
-    
-    if settings is None or settings.keys() != default_settings.keys():
-        create_dot_env(default_settings)
-
-    settings = dotenv_values(find_dotenv())
-    
-    if not domain:
-        default = settings['RUNIT_SERVERNAME']
-        domain = input(f'RUNIT_SERVERNAME [{default}]: ')
-        domain = domain if domain else default
-    
-    for key, value in settings.items():
-        if key in allowed:
-            settings[key] = input(f'{key} [{value}]: ')
-            if key != 'DATABASE_USERNAME' and key != 'dbpassword':
-                settings[key] = settings[key] if settings[key] else value
-    
-    settings['RUNIT_SERVERNAME'] = domain
-    settings['RUNIT_HOMEDIR'] = os.path.join('..', os.path.realpath(os.path.split(__file__)[0]))
-    
-    if settings['DBMS'] and settings['DATABASE_HOST'] \
-        and settings['DATABASE_PORT'] and settings['DATABASE_NAME']:
-        settings['SETUP'] = 'completed'
-    
-    for key, value in settings.items():
-        set_key(find_dotenv(), key, str(value))
-    
-    setup_database()
-    create_default_admin()
+        if settings is None or settings.keys() != default_settings.keys():
+            create_dot_env(default_settings)
 
-def run_server(args = {}):
-    if not find_dotenv():
-        print('[#] Complete Setup configuration first.\n')
-        setup_runit(args)
+        settings = dotenv_values(find_dotenv(str(DOTENV_FILE)))
+        
         print('')
+        for key, value in settings.items():
+            if key in allowed:
+                settings[key] = input(f'{key} [{value}]: ')
+                if key != 'DATABASE_USERNAME' and key != 'dbpassword':
+                    settings[key] = settings[key] if settings[key] else value
+        
+        settings['RUNIT_HOMEDIR'] = RUNIT_HOMEDIR           # type: ignore
+        
+        if settings['DBMS'] and settings['DATABASE_HOST'] \
+            and settings['DATABASE_PORT'] and settings['DATABASE_NAME']:
+            settings['SETUP'] = 'completed'
+        
+        for key, value in settings.items():
+            set_key(DOTENV_FILE, key, str(value))
+        
+        setup_database()
+        create_default_admin()
+    
+    except Exception as e:
+        print(str(e))
+        sys.exit(1)
 
+def run_server(args = {}):
     RunIt.DOCKER = args.docker
     RunIt.KUBERNETES = args.kubernetes
 
     uvicorn.run(app, host=args.host, port=args.port, log_level='info', proxy_headers=True, forwarded_allow_ips="*")
 
 def get_arguments():
     global parser
```

### Comparing `runit-server-0.4.1/runit_server/common/fast_api.py` & `runit_server-0.4.2/runit_server/common/fast_api.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/common/security.py` & `runit_server-0.4.2/runit_server/common/security.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/common/utils.py` & `runit_server-0.4.2/runit_server/common/utils.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/constants.py` & `runit_server-0.4.2/runit_server/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import os
 from enum import Enum
 from typing import Literal
-from dotenv import load_dotenv
+from dotenv import find_dotenv, load_dotenv
+from pathlib import Path
 
-load_dotenv()
-
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = os.path.realpath(os.curdir)
 SESSION_SECRET_KEY = 'dsafidsalkjdsaofwpdsncdsfdsafdsafjhdkjsfndsfkjsldfdsfjaskljdf'
 JWT_SECRET_KEY = '972a444fb071aa8ee83bf128808d255ec72e3a6b464a836b7d06254529c6'
 JWT_ALGORITHM = 'HS256'
 API_VERSION = 'v1'
 SUBSCRIPTION_EVENTS = Literal['all', 'create', 'update', 'delete']
 
-RUNIT_HOMEDIR = os.getenv(
-    'RUNIT_HOMEDIR',
-    os.path.dirname(os.path.realpath(__file__))
-)
+RUNIT_WORKDIR = Path(os.path.expanduser('~')).joinpath('RUNIT_WORKDIR')
+
+RUNIT_HOMEDIR = Path(__file__).resolve().parent
+
+if not RUNIT_WORKDIR.exists():
+    RUNIT_WORKDIR.mkdir()
+
+DOTENV_FILE = RUNIT_WORKDIR.joinpath('.env')
+if not DOTENV_FILE.exists():
+    with open(DOTENV_FILE, 'w') as file:
+        pass 
 
-RUNIT_WORKDIR = os.path.join(os.path.expanduser('~'), 'RUNIT_WORKDIR')
+load_dotenv(find_dotenv(str(DOTENV_FILE)))
 
 GITHUB_APP_CLIENT_ID = os.getenv('GITHUB_APP_CLIENT_ID','')
 GITHUB_APP_CLIENT_SECRET = os.getenv('GITHUB_APP_CLIENT_SECRET','')
 
 PROJECTS_DIR = os.path.join(RUNIT_WORKDIR, 'projects')
 TEMPLATES_PATH = os.path.join(RUNIT_HOMEDIR, 'templates')
 DOCKER_TEMPLATES = os.path.join(TEMPLATES_PATH, 'docker')
```

### Comparing `runit-server-0.4.1/runit_server/core.py` & `runit_server-0.4.2/runit_server/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from odbms import DBMS
 from dotenv import dotenv_values, find_dotenv
 from fastapi import FastAPI, WebSocket, Request
 from fastapi.templating import Jinja2Templates
 from fastapi.responses import RedirectResponse
 
-from .constants import RUNIT_WORKDIR, SUBSCRIPTION_EVENTS
+from .constants import DOTENV_FILE, RUNIT_WORKDIR, SUBSCRIPTION_EVENTS
 
 app_initialized = False
 
 def flash(request: Request, message: str, category: str = "primary") -> None:
    if "_messages" not in request.session:
        request.session["_messages"] = []
        request.session["_messages"].append((category, message))
@@ -26,31 +26,32 @@
 templates_path = Path(__file__).resolve().parent / 'templates'
 templates = Jinja2Templates(templates_path)
 templates.env.globals['get_flashed_messages'] = get_flashed_messages
 
 async def lifespan(request: Request):
     global app_initialized
     
-    if not Path(RUNIT_WORKDIR).resolve().exists():
-        Path(RUNIT_WORKDIR).resolve().mkdir()
+    if not RUNIT_WORKDIR.resolve().exists():
+        RUNIT_WORKDIR.resolve().mkdir()
     
-    if not Path(RUNIT_WORKDIR, 'accounts').resolve().exists():
-        Path(RUNIT_WORKDIR, 'account').resolve().mkdir()
+    if not RUNIT_WORKDIR.joinpath('accounts').resolve().exists():
+        RUNIT_WORKDIR.joinpath('account').resolve().mkdir()
         
-    if not Path(RUNIT_WORKDIR, 'projects').resolve().exists():
-        Path(RUNIT_WORKDIR, 'projects').resolve().mkdir()
+    if not RUNIT_WORKDIR.joinpath('projects').resolve().exists():
+        RUNIT_WORKDIR.joinpath('projects').resolve().mkdir()
 
-    settings = dotenv_values(find_dotenv())
-    setup = os.getenv('SETUP') or settings['SETUP']
-    DB_DBMS = os.getenv('DBMS') or settings['DBMS']
-    DB_HOST = os.getenv('DATABASE_HOST') or settings['DATABASE_HOST']
-    DB_PORT = os.getenv('DATABASE_PORT') or settings['DATABASE_PORT']
-    DB_USERNAME = os.getenv('DATABASE_USERNAME') or settings['DATABASE_USERNAME']
-    DB_PASSWORD = os.getenv('DATABASE_PASSWORD') or settings['DATABASE_PASSWORD']
-    DB_DATABASE = os.getenv('DATABASE_NAME') or settings['DATABASE_NAME']
+    settings = dotenv_values(find_dotenv(str(DOTENV_FILE)))
+    setup = os.getenv('SETUP') or settings.get('SETUP')
+    
+    DB_DBMS = os.getenv('DBMS') or settings.get('DBMS')
+    DB_HOST = os.getenv('DATABASE_HOST') or settings.get('DATABASE_HOST')
+    DB_PORT = os.getenv('DATABASE_PORT') or settings.get('DATABASE_PORT')
+    DB_USERNAME = os.getenv('DATABASE_USERNAME') or settings.get('DATABASE_USERNAME')
+    DB_PASSWORD = os.getenv('DATABASE_PASSWORD') or settings.get('DATABASE_PASSWORD')
+    DB_DATABASE = os.getenv('DATABASE_NAME') or settings.get('DATABASE_NAME')
     
     if not app_initialized and setup and setup == 'completed':
         DBMS.initialize(DB_DBMS, DB_HOST, DB_PORT, DB_USERNAME, DB_PASSWORD,DB_DATABASE) # type: ignore
         app_initialized = True
     else:
         return RedirectResponse(request.url_for('setup_index'))
     return True
```

### Comparing `runit-server-0.4.1/runit_server/dockerize.py` & `runit_server-0.4.2/runit_server/dockerize.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/favicon.ico` & `runit_server-0.4.2/runit_server/favicon.ico`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/gcloud.py` & `runit_server-0.4.2/runit_server/gcloud.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/kubernetes-1.py` & `runit_server-0.4.2/runit_server/kubernetes-1.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/kubernetes-2.py` & `runit_server-0.4.2/runit_server/kubernetes-2.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/models/admin.py` & `runit_server-0.4.2/runit_server/models/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from datetime import datetime
-import uuid
-
-from bson.objectid import ObjectId
-
+from bson import ObjectId
 from odbms import DBMS, Model
 from ..common.utils import Utils
 
 
 class Admin(Model):
     '''A model class for admin'''
     TABLE_NAME = 'admins'
 
-    def __init__(self, email, name, username, password, role, created_at=None, updated_at=None, id=None):
+    def __init__(self, email: str, name: str, username: str, password: str, role: str, created_at=None, updated_at=None, id=None):
         super().__init__(created_at, updated_at, id)
         self.email = email
         self.username = username
         self.name = name
         self.password = password
         self.role = role
         
@@ -25,21 +22,27 @@
         Instance Method for saving Admin instance to database
 
         @params None
         @return None
         '''
 
         data = self.__dict__.copy()
-        data['password'] =  Utils.hash_password(self.password)
-
+        data['updated_at'] = (datetime.now()).strftime("%a %b %d %Y %H:%M:%S")
+        
         if DBMS.Database.dbms != 'mongodb':
             del data["created_at"]
             del data["updated_at"]
 
-        return DBMS.Database.insert(Admin.TABLE_NAME, data)
+        if isinstance(self.id, ObjectId):
+            data['password'] =  Utils.hash_password(self.password)
+            return DBMS.Database.insert(self.TABLE_NAME, self.normalise(data, 'params'))
+        
+        # Update the existing record in database
+        del data['password']
+        return DBMS.Database.update(self.TABLE_NAME, self.normalise({'id': self.id}, 'params'), self.normalise(data, 'params'))
     
     def reset_password(self, new_password: str):
         '''
         Instance Method for resetting admin password
 
         @param new_password Admin's new password
         @return None
@@ -54,15 +57,15 @@
 
         @paramas None
         @return dict() format of Function instance
         '''
         
         data = super().json()
         data['id'] = str(self.id)
-        data['role'] = self.normalise(self.get_role())
+        data['role'] = self.normalise(self.get_role(), 'params') # type: ignore
 
         return data
     
     def get_role(self):
         '''
         Instance Method for retrieving Admin Role
 
@@ -77,20 +80,27 @@
     def get_by_username(cls, username: str):
         '''
         Class Method for retrieving admin by username 
 
         @param username username of the admin 
         @return Admin instance
         '''
-        admin = DBMS.Database.find_one(Admin.TABLE_NAME, {"username": username})
-        return cls(**Model.normalise(admin)) if admin else None
+        admin = DBMS.Database.find_one(Admin.TABLE_NAME, Admin.normalise({"username": username}, 'params'))
+        
+        if isinstance(admin, dict):
+            return cls(**cls.normalise(admin)) if len(admin.keys()) else None
+        elif isinstance(admin, list) or isinstance(admin, tuple):
+            return cls(*admin) if len(admin) else None
     
     @classmethod
     def get_by_role(cls, role: str):
         '''
         Class Method for retrieving admin by role 
 
         @param role Role of the admin 
         @return Admin instance
         '''
         admin = DBMS.Database.find_one(Admin.TABLE_NAME, {"role": role})
-        return cls(**Model.normalise(admin)) if admin else None
+        if isinstance(admin, dict):
+            return cls(**cls.normalise(admin)) if len(admin.keys()) else None
+        elif isinstance(admin, list) or isinstance(admin, tuple):
+            return cls(*admin) if len(admin) else None
```

### Comparing `runit-server-0.4.1/runit_server/models/collection.py` & `runit_server-0.4.2/runit_server/models/collection.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/models/database.py` & `runit_server-0.4.2/runit_server/models/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 from odbms import DBMS, Model
 
 class Database(Model):
     TABLE_NAME = 'databases'
 
-    def __init__(self, name, collection_name, user_id, project_id = None, schema={}, created_at=None, updated_at=None, id=None, **kwargs):
+    def __init__(self, name: str, collection_name: str, user_id: str, project_id: str = '', schema: str = '{}', created_at=None, updated_at=None, id=None, **kwargs):
         super().__init__(created_at, updated_at, id)
         self.name = name
         self.collection_name = collection_name
         self.user_id = user_id
         self.project_id = project_id
         self.schema = schema
 
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
-    def save(self):
-        '''
-        Instance Method for saving Database instance to database
-
-        @params None
-        @return None
-        '''
-
-        data = self.__dict__
-        
-        del data['id']
-
-        if DBMS.Database.dbms == 'mongodb':
-            data["created_at"]: self.created_at
-            data["updated_at"]: self.updated_at
-
-        return DBMS.Database.insert(Database.TABLE_NAME, Model.normalise(data, 'params'))
-    
     def user(self):
         '''
         Instance Method for retrieving User of Database instance
         
         @params None
         @return User Instance
         '''
 
-        return Model.normalise(DBMS.Database.find_one('users', Model.normalise({'id': self.user_id}, 'params')))
+        return Model.normalise(DBMS.Database.find_one('users', Model.normalise({'id': self.user_id}, 'params'))) # type: ignore
 
     @classmethod
     def get_by_name(cls, collection_name: str)-> list:
         '''
         Class Method for retrieving collection by a name
 
         @param collectinon_name:str name of the collection
```

### Comparing `runit-server-0.4.1/runit_server/models/function.py` & `runit_server-0.4.2/runit_server/models/function.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/models/role.py` & `runit_server-0.4.2/runit_server/models/role.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..common.utils import Utils
 
 
 class Role(Model):
     '''A model class for role'''
     TABLE_NAME = 'roles'
 
-    def __init__(self, name, permission_ids, created_at=None, updated_at=None, id=None):
+    def __init__(self, name: str, permission_ids: list, created_at=None, updated_at=None, id=None):
         super().__init__(created_at, updated_at, id)
         self.name = name
         #self.permission_ids =  permission_ids.split('::') if type(permission_ids) == str \
         #                        else permission_ids
         self.permission_ids = permission_ids
         
 
@@ -28,15 +28,15 @@
 
         data = self.__dict__.copy()
 
         if DBMS.Database.dbms != 'mongodb':
             del data["created_at"]
             del data["updated_at"]
 
-        return DBMS.Database.insert(Role.TABLE_NAME, data)
+        return DBMS.Database.insert(Role.TABLE_NAME, Role.normalise(data, 'params'))
     
     def json(self)-> dict:
         '''
         Instance Method for converting Role Instance to Dict
 
         @paramas None
         @return dict() format of Function instance
@@ -53,15 +53,19 @@
         '''
         Class Method for retrieving role by name 
 
         @param name Name of the role 
         @return Role instance
         '''
         role = DBMS.Database.find_one(Role.TABLE_NAME, {"name": name})
-        return cls(**Model.normalise(role)) if role else None
+        
+        if isinstance(role, dict):
+            return cls(**cls.normalise(role)) if len(role.keys()) else None
+        elif isinstance(role, list) or isinstance(role, tuple):
+            return cls(*role) if len(role) else None
 
     def permissions(self):
         '''
         Class Method for retrieving role by username 
 
         @param username username of the role 
         @return Role instance
```

### Comparing `runit-server-0.4.1/runit_server/models/user.py` & `runit_server-0.4.2/runit_server/models/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-import uuid
+from bson.objectid import ObjectId
 from odbms import DBMS, Model
 
 from ..common.utils import Utils
 
 class User(Model):
     '''A model class for user'''
     TABLE_NAME = 'users'
@@ -26,28 +26,27 @@
         Instance Method for saving User instance to Database
 
         @params None
         @return None
         '''
         
         data = self.__dict__.copy()
-        data['updated_at'] = (datetime.utcnow()).strftime("%a %b %d %Y %H:%M:%S")
-
-
+        data['updated_at'] = (datetime.now()).strftime("%a %b %d %Y %H:%M:%S")
+        
         if DBMS.Database.dbms != 'mongodb':
             del data["created_at"]
             del data["updated_at"]
 
-        if isinstance(self.id, uuid.UUID):
+        if isinstance(self.id, ObjectId):
             data['password'] = Utils.hash_password(self.password)
             return DBMS.Database.insert(User.TABLE_NAME, Model.normalise(data, 'params'))
         
         # Update the existing record in database
         del data['password']
-        return DBMS.Database.update(self.TABLE_NAME, self.normalise({'id': self.id}, 'params'), data)
+        return DBMS.Database.update(self.TABLE_NAME, self.normalise({'id': self.id}, 'params'), self.normalise(data, 'params'))
         
         
     
     def reset_password(self, new_password: str):
         '''
         Instance Method for resetting user password
 
@@ -65,15 +64,15 @@
 
         @params None
         @return List of Project Instances
         '''
 
         return DBMS.Database.find('projects', {'user_id': self.id})
     
-    def count_projects(self)-> int:
+    def count_projects(self):
         '''
         Instance Method for counting User Projects
 
         @params None
         @return int Count of Projects
         '''
 
@@ -97,8 +96,12 @@
         '''
         Class Method for retrieving user by email address
 
         @param email email address of the user 
         @return User instance
         '''
         user = DBMS.Database.find_one(User.TABLE_NAME, {"email": email})
-        return cls(**Model.normalise(user)) if user else None
+        
+        if isinstance(user, dict):
+            return cls(**cls.normalise(user)) if len(user.keys()) else None
+        elif isinstance(user, list) or isinstance(user, tuple):
+            return cls(*user) if len(user) else None
```

### Comparing `runit-server-0.4.1/runit_server/modules/account.py` & `runit_server-0.4.2/runit_server/modules/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             elif 'msg' in result.keys():
                 print('[Error]', result['msg'])
             else:
                 print('[Error]', result['message'])
         except Exception as e:
             print(str(e))
     
+    @staticmethod
     def logout(args):
         '''
         Logout of Current Account
 
         @param args Input from argparse
         @return None
         '''
@@ -138,15 +139,15 @@
             result = request.json()
             if 'msg' in result.keys():
                 raise Exception(result['msg'])
             return result
 
         except Exception as e:
             print(str(e))
-            return None
+            return {}
   
     @staticmethod
     def info(args):
         '''
         Retrieve account details
         
         @param args Input from argparse
@@ -278,15 +279,15 @@
             request = requests.delete(url, headers=BASE_HEADERS)
             print(request.json())
 
         except Exception as e:
             print(str(e))
     
     @staticmethod
-    def functions(args)-> dict:
+    def functions(args):
         '''
         Retrieve Functions
         
         @param args Input from argparse
         @return None
         '''
         try:
```

### Comparing `runit-server-0.4.1/runit_server/routers/account.py` & `runit_server-0.4.2/runit_server/routers/account.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/routers/admin.py` & `runit_server-0.4.2/runit_server/routers/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 @admin.get('/users/{user_id}/')
 async def admin_get_user(request: Request, user_id: str):
     try:
         user: User = User.get(user_id) # type: ignore
         if not User:
             raise Exception('User not found')
         
-        projects = Project.get_by_user(user.id)
+        projects = Project.get_by_user(str(user.id))
         
         return templates.TemplateResponse('admin/users/details.html', context={
             'request': request, 'page': 'users', 'user': user.json(),
             'projects': projects, 'icons': LANGUAGE_TO_ICONS})
     except Exception as e:
         flash(request, str(e), 'danger')
         return RedirectResponse(request.url_for('admin_list_users'))
@@ -87,27 +87,27 @@
     if view:
         request.session['view'] = view
     elif 'view' not in request.session.keys():
         request.session['view'] = 'grid'
         
     return templates.TemplateResponse('admin/projects/index.html', context={
             'request': request, 'page': 'projects', 'projects': projects,
-            'icons': LANGUAGE_TO_ICONS})
+            'user': {}, 'icons': LANGUAGE_TO_ICONS})
 
 @admin.get('/projects/{project_id}')
 @admin.get('/projects/{project_id}/')
 async def admin_get_project(request: Request, project_id):
     old_curdir = os.curdir
     
     project = Project.get(project_id)
     if not project:
         flash(request, 'Project does not exist', 'danger')
         return RedirectResponse(request.url_for('admin_list_projects'))
     
-    os.chdir(Path(PROJECTS_DIR, project.id))
+    os.chdir(Path(PROJECTS_DIR, str(project.id)))
     if not os.path.isfile('.env'):
         open('.env', 'w').close()
 
     environs = dotenv_values('.env')
 
     runit = RunIt(**RunIt.load_config())
 
@@ -195,15 +195,15 @@
 async def admin_delete_project(request: Request, project_id, background_task: BackgroundTasks):
     try:
         user_id = request.session['user_id']
         project = Project.get(project_id)
         
         if project:
             Project.remove({'_id': project_id, 'user_id': user_id})
-            background_task.add_task(shutil.rmtree, Path(PROJECTS_DIR, project.id))
+            background_task.add_task(shutil.rmtree, Path(PROJECTS_DIR, str(project.id)))
             flash(request, 'Project deleted successfully', category='success')
         else:
             flash(request, 'Project was not found. Operation not successful.', category='danger')
         return RedirectResponse(request.url_for(ADMIN_PROJECTS_INDEX))
     except Exception:
         flash(request, 'Project deleted successfully', category='success')
         return RedirectResponse(request.url_for(ADMIN_PROJECTS_INDEX))
@@ -232,15 +232,15 @@
 
 @admin.get('/databases/{database_id}')
 @admin.get('/databases/{database_id}/')
 async def admin_get_database(request: Request, database_id: str):
     database = Database.get(database_id)
     
     if database:
-        Collection.TABLE_NAME = database.collection_name
+        Collection.TABLE_NAME = database.collection_name            # type: ignore
         collections = Collection.find({})
         
         result = []
         for col in collections:
             result.append(col.json())
         
         schema_names_to_input_types = {
@@ -308,15 +308,22 @@
         flash(request, 'Database deleted successfully', category='success')
     else:
         flash(request, 'Database was not found. Operation not successful.', category='danger')
     return RedirectResponse(request.url_for(ADMIN_DATABASE_INDEX), status_code=status.HTTP_303_SEE_OTHER)
 
 @admin.get('/profile/')
 async def admin_profile(request: Request):
+    user_id = request.session['admin_id']
+    user = Admin.get(user_id)
+    
+    if not user:
+        flash(request, "User does not exist", "danger")
+        return RedirectResponse(request.url_for('admin_dashboard'), status_code=status.HTTP_303_SEE_OTHER)
+    
     return templates.TemplateResponse('admin/profile.html', context={
-        'request': request, 'page': 'profile'})
+        'request': request, 'page': 'profile', 'user': user.json()})
 
 @admin.get('/logout/')
 async def admin_logout(request: Request):
     request.session.clear()
     return RedirectResponse(request.url_for(ADMIN_LOGIN_PAGE), status_code=status.HTTP_303_SEE_OTHER)
```

### Comparing `runit-server-0.4.1/runit_server/routers/api/account.py` & `runit_server-0.4.2/runit_server/routers/api/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 async def api_user_profile(user: Annotated[User, Depends(get_current_user)]):
     user = User.get(str(user.id)) # type: ignore
     user_json = user.json()
     del user_json['password']
     del user_json['gat']
     del user_json['grt']
     
+    print('---Account Info', user_json)
+    
     return JSONResponse(user_json)
 
 @account_api.post('/profile')
 async def api_update_user_profile(
     user: Annotated[User, Depends(get_current_user)],
     account: AccountData
 ):
```

### Comparing `runit-server-0.4.1/runit_server/routers/api/database.py` & `runit_server-0.4.2/runit_server/routers/api/database.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/routers/api/project.py` & `runit_server-0.4.2/runit_server/routers/api/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,24 @@
 
 from fastapi.responses import JSONResponse, StreamingResponse
 from fastapi import APIRouter, BackgroundTasks,  Request, \
     Depends, status, UploadFile
 from dotenv import load_dotenv, dotenv_values
 from pydantic import BaseModel
 
+from odbms import DBMS
+
 from ...common import get_current_user
 from ...models import Database
 from ...models import Project
 from ...models import User
 from ...models import ProjectData
+from ...models import Collection
+
+from ...core import flash
 
 from runit import RunIt
 from ...constants import (
     DOCKER_TEMPLATES,
     PROJECTS_DIR,
     LANGUAGE_TO_RUNTIME
 )
@@ -70,20 +75,21 @@
         config['language'] = project_data.language.value
         config['runtime'] = LANGUAGE_TO_RUNTIME[project_data.language.value]
         config['description'] = project_data.description
         config['author'] = {}
         config['author']['name'] = user.name
         config['author']['email'] = user.email
         
-        project = Project(user.id, **config)
-        project_id = project.save().inserted_id # type: ignore
+        project = Project(str(user.id), **config)
+        saved_project = project.save()
+        project_id = saved_project.inserted_id if DBMS.Database.dbms == 'mongodb' else saved_project # type: ignore
         project_id = str(project_id)
         project.id = project_id
         
-        homepage = f"{request.base_url}{project_id}/"
+        homepage = f"{request.base_url}{project_id}"
         Project.update({'id': project_id}, {'homepage': homepage})
 
         config['_id'] = project_id
         config['homepage'] = homepage
         
         os.chdir(PROJECTS_DIR)
         
@@ -100,29 +106,34 @@
         os.chdir(str(project_folder))
         new_runit.update_config()
         
         # os.chdir(RUNIT_HOMEDIR)
         
         if (project_data.database):
             # Create database for project
+            collection_name = f"{project_data.name}_{str(user.id)}_{project_id}"
             Database(
                 project_data.name+'_db',
-                user.id,
+                collection_name,
+                str(user.id),
                 project_id
             ).save()
+            Collection.TABLE_NAME = collection_name # type: ignore
+            Collection.create_table()
+        flash(request, 'Project created successfully', category='success')
         response['project'] = Project.get(project_id).json() # type: ignore
     except Exception as e:
         logging.exception(e)
         response['status'] = 'error'
         response['message'] = 'Error creating project'
-    
-    return JSONResponse(
-        response,
-        status_code=status.HTTP_201_CREATED if response['status'] == 'success' else status.HTTP_204_NO_CONTENT
-    )
+    finally:
+        return JSONResponse(
+            response,
+            status_code=status.HTTP_201_CREATED if response['status'] == 'success' else status.HTTP_500_INTERNAL_SERVER_ERROR
+        )
 
 @projects_api.post('/publish')
 async def api_publish_user_project(
     request: Request,
     user: Annotated[User, Depends(get_current_user)],
     background_task: BackgroundTasks
 ):
@@ -137,72 +148,79 @@
     data = await request.form()
     data = data._dict
     file = data['file']
     del data['file']
     
     result = {'status': 'success'}
 
-    if '_id' not in data.keys() or not data['_id']:
-        del data['_id']
-        
-        project = Project(user_id=user.id, **data)      # type: ignore
-        project_id = project.save().inserted_id         # type: ignore
-        project_id = str(project_id)
-        project.id = project_id
-        homepage = f"{os.getenv('RUNIT_PROTOCOL')}{os.getenv('RUNIT_SERVERNAME')}/{project_id}/"
-        project.update({'homepage': homepage})
-        result['project_id'] = project_id
-    else:
-        project_id = str(data['_id'])
-        project = Project.get(data['_id'])
-        if project:
+    try:
+        if '_id' not in data.keys() or not data['_id']:
             del data['_id']
-            project.update(data, {'id': project.id})
-
-    PROJECT_PATH = Path(PROJECTS_DIR, project_id).resolve()
-    if not os.path.exists(PROJECT_PATH):
-        os.mkdir(PROJECT_PATH)
-        
-    filepath = Path(PROJECT_PATH, file.filename)                                 # type: ignore
-    contents = await file.read()                                    # type: ignore
-    async with aiofiles.open(filepath, 'wb') as f:
-        await f.write(contents)
-    await file.close()                                                           # type: ignore
-
-    RunIt.extract_project(filepath)
-    os.chdir(PROJECT_PATH)
-
-    runit = RunIt(**RunIt.load_config())
+            
+            project = Project(user_id=user.id, **data)      # type: ignore
+            saved_project = project.save()
+            project_id = saved_project.inserted_id if DBMS.Database.dbms == 'mongodb' else saved_project # type: ignore
+            project_id = str(project_id)
+            project.id = project_id
+            homepage = f"{request.base_url}{project_id}"
+            Project.update({'id': project_id}, {'homepage': homepage})
+            result['project_id'] = project_id
+        else:
+            project_id = str(data['_id'])
+            project = Project.get(str(data['_id']))
+            if project:
+                del data['_id']
+                Project.update({'id': project_id}, data)
+
+        PROJECT_PATH = Path(PROJECTS_DIR, project_id).resolve()
+        if not PROJECT_PATH.exists():
+            os.mkdir(PROJECT_PATH)
+            
+        filepath = Path(PROJECT_PATH, file.filename)                                 # type: ignore
+        contents = await file.read()                                    # type: ignore
+        async with aiofiles.open(filepath, 'wb') as f:
+            await f.write(contents)
+        await file.close()                                                           # type: ignore
+
+        RunIt.extract_project(filepath)
+        os.chdir(PROJECT_PATH)
+
+        runit = RunIt(**RunIt.load_config())
+        
+        if RunIt.DOCKER:
+            docker_file = f"{runit.runtime}.dockerfile"
+            full_docker_filepath = f"{os.path.join(DOCKER_TEMPLATES, docker_file)}"
+            print(f'[~] {full_docker_filepath}')
+            project_docker_file = os.path.join(PROJECT_PATH, 'Dockerfile')
+            
+            if not os.path.exists(project_docker_file):
+                with open(full_docker_filepath, 'rt') as nf:
+                    with open(project_docker_file, 'wt') as pf:
+                        content = nf.read()
+                        pf.write(content)
 
-    if RunIt.DOCKER:
-        docker_file = f"{runit.runtime}.dockerfile"
-        full_docker_filepath = f"{os.path.join(DOCKER_TEMPLATES, docker_file)}"
-        print(f'[~] {full_docker_filepath}')
-        project_docker_file = os.path.join(PROJECT_PATH, 'Dockerfile')
-        
-        if not os.path.exists(project_docker_file):
-            with open(full_docker_filepath, 'rt') as nf:
-                with open(project_docker_file, 'wt') as pf:
-                    content = nf.read()
-                    pf.write(content)
-
-        background_task.add_task(RunIt.dockerize, str(PROJECT_PATH))   # type: ignore
-    else:
-        runit.install_dependency_packages()
-    
-    runit._id = project_id
-    runit.update_config()
+            background_task.add_task(RunIt.dockerize, str(PROJECT_PATH))   # type: ignore
+        else:
+            runit.install_dependency_packages()
+        
+        runit._id = project_id
+        runit.update_config()
+        
+        funcs = []
+        for func in runit.get_functions():
+            funcs.append(f"{request.base_url}{project_id}/{func}/")
+        
+        result['functions'] = funcs                                                         # type: ignore
+        result['homepage'] = funcs[0] if len(funcs) else ''
+        return result
     
-    funcs = []
-    for func in runit.get_functions():
-        funcs.append(f"{request.base_url}{project_id}/{func}/")
+    except Exception as e:
+        logging.exception(e)
+        return JSONResponse({'status': 'error', 'message': "Error publishing project."})
     
-    result['functions'] = funcs                                                         # type: ignore
-    result['homepage'] = funcs[0] if len(funcs) else ''
-    return result
 
 @projects_api.get('/clone/{project_name}')
 async def api_clone_user_project(
     request: Request,
     user: Annotated[User, Depends(get_current_user)],
     project_name: str
 ):
@@ -214,27 +232,28 @@
     '''
     global PROJECTS_DIR
     
     try:
         project = Project.find_one({'name': project_name, 'user_id': user.id})
         
         if project:
-            if not Path(PROJECTS_DIR, project.id).resolve().exists():
+            project_path = Path(PROJECTS_DIR, str(project.id)).resolve()
+            if not project_path.exists():
                 raise FileNotFoundError('Project not found!')
                 
-            os.chdir(Path(PROJECTS_DIR, project.id).resolve())
+            os.chdir(project_path)
             config = RunIt.load_config()
             
             if not config:
-                raise FileNotFoundError
+                raise FileNotFoundError('Project not found!')
             
             runit_project = RunIt(**config)
             filename = runit_project.compress()
             # os.chdir(WORKDIR)
-            file_path = Path(PROJECTS_DIR, project.id, filename)
+            file_path = Path(project_path, filename)
             
             def iterfile():
                 with open(file_path, mode="rb") as file:  
                     yield from file
             
             return StreamingResponse(iterfile(), media_type="application/octet-stream", headers={"Content-Disposition": f"attachment; filename={filename}"})
 
@@ -256,19 +275,19 @@
     
     project = Project.get(project_id)
     
     if not project:
         logging.error(f'Project {project_id} does not exist')
         return JSONResponse(response)
     
-    if not Path(PROJECTS_DIR, project.id).resolve().exists():
-        logging.error(f'Project Path {str(Path(PROJECTS_DIR, project.id))} does not exist')
+    if not Path(PROJECTS_DIR, str(project.id)).resolve().exists():
+        logging.error(f'Project Path {str(Path(PROJECTS_DIR, str(project.id)))} does not exist')
         return JSONResponse(response)
     
-    os.chdir(Path(PROJECTS_DIR, project.id).resolve())
+    os.chdir(Path(PROJECTS_DIR, str(project.id)).resolve())
     if not Path('.env').is_file():
         async with aiofiles.open('.env', 'w') as file:
             await file.close()
 
     environs = dotenv_values('.env')
     
     runit = RunIt(**RunIt.load_config())
@@ -309,15 +328,15 @@
             'id': project_id,
             'user_id': user_id
         })
         
         if len(project):
             project = project[0]
             Project.remove({'_id': project_id, 'user_id': user_id})
-            background_task.add_task(shutil.rmtree, Path(PROJECTS_DIR, project.id).resolve())
+            background_task.add_task(shutil.rmtree, Path(PROJECTS_DIR, str(project.id)).resolve())
             
         else:
             response['status'] = 'error'
             response['message'] = 'Project was not found. Operation not successful'
 
     except Exception:
         response['status'] = 'error'
```

### Comparing `runit-server-0.4.1/runit_server/routers/api/public.py` & `runit_server-0.4.2/runit_server/routers/api/public.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     access_token = create_access_token(
         data={"email": user.email}, expires_delta=access_token_expires
     )
 
     return JSONResponse({"access_token": access_token, "token_type": "bearer"})
 
 @public_api.post('/register', response_model=Token)
-async def register(
+async def api_register(
     data: UserData
 ):
     if data.password != data.cpassword:
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Passwords do not match",
             headers={"WWW-Authenticate": "Bearer"},
```

### Comparing `runit-server-0.4.1/runit_server/routers/database.py` & `runit_server-0.4.2/runit_server/routers/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,28 +67,28 @@
     user_id = request.session['user_id']
     
     if name and project_id:
         collection_name = f"{name}_{user_id}_{project_id}"
         data = {'name': name, 'collection_name': collection_name,
                 'project_id': project_id,'user_id': user_id}
         
-        new_db = Database(**data)
-        results = new_db.save().inserted_id     # type: ignore
-                
+        Database(**data).save()
+        Collection.TABLE_NAME = collection_name # type: ignore
+        Collection.create_table()
         flash(request, 'Database Created Successfully.', category='success')
     else:
         flash(request, 'Missing required fields.', category='danger')
     return RedirectResponse(request.url_for(DATABASE_INDEX), status_code=status.HTTP_303_SEE_OTHER)
 
 @database.get('/{database_id}/')
 async def user_database_details(request: Request, database_id):
     database = Database.get(database_id)
     
     if database:
-        Collection.TABLE_NAME = database.collection_name
+        Collection.TABLE_NAME = database.collection_name                # type: ignore
         collections = Collection.find({})
         
         result = []
         for col in collections:
             result.append(col.json())
         
         schema_names_to_input_types = {
```

### Comparing `runit-server-0.4.1/runit_server/routers/functions.py` & `runit_server-0.4.2/runit_server/routers/functions.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/routers/github.py` & `runit_server-0.4.2/runit_server/routers/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     error_count = 0
     response: dict = {'status': 'success'}
     repos: list[dict] = []
     
     try:
         if not user or not user.gat:
             raise Exception('User is not authenticated')
-
+        
         g = await user_access_token(user.gat) # type: ignore
         repos = await fetch_repositories(g, repo_name)
         response['data'] = repos
     except GithubException:
         error_count += 1
         
         if error_count >= 2:
@@ -129,13 +129,13 @@
         g = await refresh_access_token(user) # type: ignore
         response['data'] = await fetch_repositories(g)
     except requests.ConnectionError:
         logging.error('Connection error')
         response['status'] = 'error'
         response['message'] = 'Error connecting to github'
     except Exception as e:
-        logging.exception(e)
+        logging.warning(str(e))
         response['status'] = 'error'
         response['message'] = 'Expired access tokens'
     finally:
         return JSONResponse(response)
```

### Comparing `runit-server-0.4.1/runit_server/routers/project.py` & `runit_server-0.4.2/runit_server/routers/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,24 @@
 
 project = APIRouter(
     prefix="/projects",
     tags=["projects"],
     dependencies=[Depends(get_session)]
 )
 
+def create_runit_project(config: dict, name: str):
+    os.chdir(PROJECTS_DIR)
+    new_runit = RunIt(**config)
+    
+    new_runit._id = config['name']
+    new_runit.name = name
+
+    os.chdir(Path(PROJECTS_DIR, config['name']))
+    new_runit.update_config()
+
 @project.get('/')
 async def list_user_projects(request: Request, view: Optional[str] = None):
     user_id = request.session['user_id']
     user = User.get(user_id)
     user = user.json() if user else None
     
     if view:
@@ -142,23 +152,16 @@
                     async with aiofiles.open(Path(PROJECTS_DIR, project_id, file_content.path).resolve(), 'wb') as file:
                         await file.write(file_content.decoded_content)
             
             
             runit = RunIt(**RunIt.load_config())
             background_task.add_task(runit.install_dependency_packages)
         else:
-            os.chdir(PROJECTS_DIR)
             config['name'] = project_id
-            new_runit = RunIt(**config)
-            
-            new_runit._id = project_id
-            new_runit.name = project_data.name
-        
-            os.chdir(Path(PROJECTS_DIR, project_id))
-            new_runit.update_config()
+            background_task.add_task(create_runit_project, config, project.name)
         
         # os.chdir(RUNIT_HOMEDIR)
         
         if (project_data.database):
             # Create database for project
             collection_name = f"{project_data.name}_db_{user_id}_{project_id}"
             Database(project_data.name, collection_name, project_id).save()
@@ -177,19 +180,19 @@
     old_curdir = os.curdir
     
     project = Project.get(project_id)
     if not project:
         flash(request, PROJECT_404_ERROR, 'danger')
         return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
     
-    elif not Path(PROJECTS_DIR, project.id).resolve().exists():
+    elif not Path(PROJECTS_DIR, str(project.id)).resolve().exists():
         flash(request, PROJECT_404_ERROR, 'danger')
         return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
     
-    os.chdir(Path(PROJECTS_DIR, project.id).resolve())
+    os.chdir(Path(PROJECTS_DIR, str(project.id)).resolve())
     if not Path('.env').is_file():
         async with aiofiles.open('.env', 'w') as file:
             await file.close()
 
     environs = dotenv_values('.env')
     
     runit = RunIt(**RunIt.load_config())
@@ -218,19 +221,19 @@
         old_curdir = os.curdir
         
         project = Project.get(project_id)
         if not project:
             flash(request, PROJECT_404_ERROR, 'danger')
             return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
         
-        if not Path(PROJECTS_DIR, project.id).resolve().exists():
+        if not Path(PROJECTS_DIR, str(project.id)).resolve().exists():
             flash(request, PROJECT_404_ERROR, 'danger')
             return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
 
-        os.chdir(Path(PROJECTS_DIR, project.id).resolve())
+        os.chdir(Path(PROJECTS_DIR, str(project.id)).resolve())
         runit = RunIt(**RunIt.load_config())
         background_task.add_task(runit.install_dependency_packages)
         
         os.chdir(old_curdir)
         flash(request, "Dependencies installation has started", "success")
     except Exception as e:
         logging.error(str(e))
@@ -242,16 +245,16 @@
 @project.get('/delete/{project_id}/')
 async def delete_user_project(request: Request, project_id, background_task: BackgroundTasks):
     try:
         user_id = request.session['user_id']
         project = Project.get(project_id)
         
         if project:
-            Project.remove({'_id': project_id, 'user_id': user_id})
-            project_folder = Path(PROJECTS_DIR, project.id).resolve()
+            Project.remove({'id': project_id, 'user_id': user_id})
+            project_folder = Path(PROJECTS_DIR, str(project.id)).resolve()
             if project_folder.exists() and project_folder.is_dir():
                 background_task.add_task(shutil.rmtree, project_folder)
             flash(request, 'Project deleted successfully', category='success')
         else:
             flash(request, 'Project was not found. Operation not successful.', category='danger')
         return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
     except Exception:
@@ -261,15 +264,15 @@
 @project.post('environ/{project_id}/')
 async def user_project_environ(request: Request, project_id):
     project = Project.get(project_id)
     if not project:
         flash(request, PROJECT_404_ERROR, 'danger')
         return RedirectResponse(request.url_for(PROJECT_INDEX_URL_NAME))
     
-    env_file = Path(PROJECTS_DIR, project.id, '.env').resolve()
+    env_file = Path(PROJECTS_DIR, str(project.id), '.env').resolve()
     async with aiofiles.open(env_file, 'w') as file:
         await file.close()
     
     for key, value in request.form.items():
         set_key(env_file, key, value)
 
     # project = Project.get(project_id)
```

### Comparing `runit-server-0.4.1/runit_server/routers/public.py` & `runit_server-0.4.2/runit_server/routers/public.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ..common import Utils
 
 from runit import RunIt
 
 from dotenv import load_dotenv, find_dotenv, dotenv_values
 
 from ..constants import (
+    DOTENV_FILE,
     RUNIT_HOMEDIR,
     PROJECTS_DIR
 )
 
 REGISTER_HTML_TEMPLATE = 'register.html'
 HOME_PAGE = 'index'
 
@@ -76,16 +77,16 @@
         return templates.TemplateResponse('exposed.html', context={'request': request})
     else:
         return templates.TemplateResponse('404.html', context={'request': request})
 
 @public.get('/')
 @public.get('/login')
 async def index(request: Request):
-    settings = dotenv_values(find_dotenv())
-    setup = os.getenv('SETUP') or settings['SETUP']
+    settings = dotenv_values(find_dotenv(str(DOTENV_FILE)))
+    setup = os.getenv('SETUP') or settings.get('SETUP')
     
     if setup != 'completed':
         return RedirectResponse(request.url_for('setup_index'))
     if 'user_id' in request.session.keys():
         return RedirectResponse(request.url_for('user_home'))
     return templates.TemplateResponse('login.html', context={'request': request})
 
@@ -103,19 +104,21 @@
 ):
     try:
         if password != cpassword:
             flash(request, 'Passwords do not match!', 'danger')
             return templates.TemplateResponse(REGISTER_HTML_TEMPLATE, context={'request': request})
         
         user = User.get_by_email(email)
+ 
         if user:
-            flash(request, 'User is already registered!', 'danger')
+            flash(request, 'User already exists!', 'danger')
             return templates.TemplateResponse(REGISTER_HTML_TEMPLATE, context={'request': request})
         
-        User(email, name, password).save()
+        user = User(email, name, password).save()
+
         #print(user.inserted_id)
         flash(request, 'Registration Successful!', 'success')
         return RedirectResponse(request.url_for(HOME_PAGE), status_code=status.HTTP_303_SEE_OTHER)
 
     except Exception as e:
         logging.exception(e)
         flash(request, 'Error during registration', 'danger')
@@ -132,58 +135,53 @@
     request.session['user_id'] = user.id
     request.session['user_name'] = user.name
     request.session['user_email'] = user.email
     request.session['access_token'] = access_token
 
     return RedirectResponse(request.url_for('user_home'), status_code=status.HTTP_303_SEE_OTHER)
 
-@public.get('/login/admin')
+@public.get('/admin/login')
 def admin_login_page(request: Request):
     if 'admin_id' in request.session and request.session['admin_id']:
         return RedirectResponse(request.url_for('admin_dashboard'))
     return templates.TemplateResponse('admin/login.html', context={'request': request, 'title':'Admin Login'})
 
-@public.post('/login/admin')
+@public.post('/admin/login')
 def admin_login(request: Request, form_data: OAuth2PasswordRequestForm = Depends()):
     admin = Admin.get_by_username(form_data.username)
+
     if admin and Utils.check_hashed_password(form_data.password, admin.password):
-            
             access_token = create_access_token(admin.json())
             request.session['admin_id'] = admin.id
             request.session['admin_name'] = admin.name
             request.session['admin_username'] = admin.email
             request.session['access_token'] = access_token
 
             return RedirectResponse(request.url_for('admin_dashboard'), status_code=status.HTTP_303_SEE_OTHER)
     flash(request, 'Invalid Login Credentials', 'danger')
     return RedirectResponse(request.url_for('admin_login_page'), status_code=status.HTTP_303_SEE_OTHER)
 
-    if settings is None or settings['SETUP'] != 'completed':
-        return RedirectResponse(request.url_for('setup.index'))
-    if 'user_id' in request.session.keys():
-        return RedirectResponse(request.url_for('user_home'))
-    return templates.TemplateResponse('login.html', context={'request': request})
-
 @public.get('/{project_id}')
 @public.get('/{project_id}/{function}')
 async def run_project(request: Request, project_id: str, function: Optional[str] = None):
     t0 = time.perf_counter()
     excluded = ['favicon.ico']
     if project_id in excluded:
         return None
     project = Project.get(project_id)
     if not project:
         return RunIt.notfound()
+    if project.private and request.session.get('user_id') != project.user_id:
+        return RunIt.notfound()
     
-    current_project_dir = Path(PROJECTS_DIR, project.id).resolve()
+    current_project_dir = Path(PROJECTS_DIR, str(project.id)).resolve()
     function = function if function else 'index'
     if current_project_dir.is_dir():
-        if not RunIt.is_private(project_id, str(current_project_dir)):
-            result = RunIt.start(project_id, function, str(current_project_dir), request.query_params._dict)
-            os.chdir(RUNIT_HOMEDIR)
-            response = await jsonify(result)
+        result = RunIt.start(project_id, function, PROJECTS_DIR, request.query_params._dict)
+        os.chdir(RUNIT_HOMEDIR)
+        response = await jsonify(result)
         t1 = time.perf_counter() # Record the stop time
         elapsed_time = t1 - t0 # Calculate elapsed time
         print(f'Time taken: {elapsed_time:.8f} seconds')
         return JSONResponse(response) if type(response) is dict else response
     
     return RunIt.notfound()
```

### Comparing `runit-server-0.4.1/runit_server/static/css/all.min.css` & `runit_server-0.4.2/runit_server/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/css/bootstrap.min.css` & `runit_server-0.4.2/runit_server/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/css/bootstrap.min.css.map` & `runit_server-0.4.2/runit_server/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/css/styles.css` & `runit_server-0.4.2/runit_server/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/loading.gif` & `runit_server-0.4.2/runit_server/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/html5.svg` & `runit_server-0.4.2/runit_server/static/images/logos/html5.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/nodejs.png` & `runit_server-0.4.2/runit_server/static/images/logos/nodejs.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/nodejs.svg` & `runit_server-0.4.2/runit_server/static/images/logos/nodejs.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/php.svg` & `runit_server-0.4.2/runit_server/static/images/logos/php.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/python.png` & `runit_server-0.4.2/runit_server/static/images/logos/python.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/python.svg` & `runit_server-0.4.2/runit_server/static/images/logos/python.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/python1.svg` & `runit_server-0.4.2/runit_server/static/images/logos/python1.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png` & `runit_server-0.4.2/runit_server/static/images/logos/screenshot-nicepage.com-2022.06.22-14_05_33.png`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/images/terminal.svg` & `runit_server-0.4.2/runit_server/static/images/terminal.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js` & `runit_server-0.4.2/runit_server/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/bootstrap.bundle.min.js.map` & `runit_server-0.4.2/runit_server/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/databases.js` & `runit_server-0.4.2/runit_server/static/js/databases.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/github.js` & `runit_server-0.4.2/runit_server/static/js/github.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -25,16 +25,18 @@
         this.reposElem = document.getElementById(options.repos)
         this.projectName = document.getElementById(options.name)
         this.submitBtn = document.getElementById(options.submitBtn)
         this.branchesElem = document.getElementById(options.branches)
         this.projectDescription = document.getElementById(options.description)
         this.branchesParentElem = document.getElementById(options.branchesParent)
 
-        this.reposElem.onchange = (e) => {
-            this.getRepos(e.target.value)
+        if (this.reposElem) {
+            this.reposElem.onchange = (e) => {
+                this.getRepos(e.target.value)
+            }
         }
         this.getRepos()
     }
 
     static async getRepos(repo_name = null) {
         this.setLoading(true)
         let url = '/github/repos'
@@ -45,21 +47,17 @@
 
         const {
             status,
             message,
             data
         } = response
         this.setLoading(false)
-        status === 'success' ?
-            repo_name ?
-            this.setRepo(data[0]) :
+        status === 'success' ? repo_name ? this.setRepo(data[0]) :
             this.setRepos(data) :
-            message === 'Expired access tokens' ?
-            window.location.reload() :
-            console.error(message)
+            console.log(message)
     }
 
     static setRepos(repos = []) {
         this.repos = repos
         repos.forEach((repo) => {
             let option = document.createElement('option')
             option.value = repo.name
```

### Comparing `runit-server-0.4.1/runit_server/static/js/main.js` & `runit_server-0.4.2/runit_server/static/js/main.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/profile.js` & `runit_server-0.4.2/runit_server/static/js/profile.js`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/js/projects.js` & `runit_server-0.4.2/runit_server/static/js/projects.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
         setLoading(true)
 
         try {
             let data = Object.fromEntries(new FormData(form))
             let access_token = document.getElementById('accessToken').innerText.trim()
             let modalCloseBtn = document.querySelector('.btn-close')
 
-            let url = '/projects/'
+            let url = '/api/v1/projects/'
 
             let response = await fetch(url, {
                 headers: {
                     'Content-Type': 'application/json',
                     Authorization: `Bearer ${access_token}`
                 },
                 method: 'POST',
@@ -143,18 +143,17 @@
             const {
                 status,
                 message,
                 project
             } = result
 
             if (status === 'success') {
-                console.log(message)
-                console.log(project)
-                modalCloseBtn.click()
-                return new Project(project)
+                // modalCloseBtn.click()
+                window.location.reload()
+                // return new Project(project)
             }
             console.error(message)
             return null
 
         } catch (error) {
             setLoading(false)
             console.log(error)
@@ -172,32 +171,34 @@
 
     }
 
 
 }
 
 window.onload = async (e) => {
-    Github.init({
-        name: 'name',
-        repos: 'github_repo',
-        description: 'description',
-        branches: 'github_repo_branch',
-        branchesParent: 'branches_elem',
-        submitBtn: 'submitBtn'
-    })
+    if (window.location.pathname === '/projects/') {
+        Github.init({
+            name: 'name',
+            repos: 'github_repo',
+            description: 'description',
+            branches: 'github_repo_branch',
+            branchesParent: 'branches_elem',
+            submitBtn: 'submitBtn'
+        })
+    }
 
     let url_parts = window.location.pathname.split('/')
 
     if (url_parts.length >= 3 && url_parts[1] === 'projects') {
         let project_id = url_parts[2]
         let project = await Project.get(project_id)
     }
 
     let projectForm = document.getElementById('projectForm')
-    console.log(projectForm)
+
     if (projectForm) {
         projectForm.onsubmit = (e) => {
             e.preventDefault()
 
             Project.create(projectForm)
         }
     }
```

### Comparing `runit-server-0.4.1/runit_server/static/js/setup.js` & `runit_server-0.4.2/runit_server/static/js/setup.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,17 @@
  * Description
  * @authors Amos Amissah (theonlyamos@gmail.com)
  * @date    2022-08-06 13:48:51
  * @version 1.0.0
  */
 
 const DB_PORTS = {
-    'mysql': 33060,
-    'mongodb': 27017
+    mysql: 33060,
+    mongodb: 27017,
+    postgresql: 5432
 }
 
 class SetupWizard {
     static form;
     static containerElem;
     static children = [];
 
@@ -132,15 +133,15 @@
         if (SetupWizard.validateForm()) {
             SetupWizard.form.submit();
         }
     }
 }
 
 const selectDMEngine = (value) => {
-    document.querySelector("[name='dbport']").value = DB_PORTS[value]
+    document.querySelector("[name='DATABASE_PORT']").value = DB_PORTS[value] || ''
 }
 
 window.onload = (e) => {
     SetupWizard.init({
         form: 'setupForm',
         parent: 'setupWizard',
         children: 'setup-step',
```

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.eot` & `runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.svg` & `runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.ttf` & `runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff` & `runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-brands-400.woff2` & `runit_server-0.4.2/runit_server/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.eot` & `runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.svg` & `runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.ttf` & `runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff` & `runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-regular-400.woff2` & `runit_server-0.4.2/runit_server/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.eot` & `runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.svg` & `runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.ttf` & `runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff` & `runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/static/webfonts/fa-solid-900.woff2` & `runit_server-0.4.2/runit_server/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/404.html` & `runit_server-0.4.2/runit_server/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/account/home.html` & `runit_server-0.4.2/runit_server/templates/account/home.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/account/layout.html` & `runit_server-0.4.2/runit_server/templates/account/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
         @media screen and (min-width: 576px) {
             .main-content {
                 height: 80vh;
             }
         }
     </style>
+    <div class="d-none" id="accessToken">
+        {{request.session['access_token']}}
+    </div>
     <div class="offcanvas offcanvas-start w-auto" tabindex="-1" id="offcanvasMenu" aria-labelledby="offcanvasMenuLabel">
         <div class="offcanvas-header">
             <h5 class="offcanvas-title" id="offcanvasMenuLabel">Menu</h5>
             <!--<button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>-->
         </div>
         {% set menu = [
             {'name': 'home', 'icon': 'home', 'url': 'user_home'},
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{{request.session['access_token']}}
 **** MMeennuu ****
 {% set menu = [ {'name': 'home', 'icon': 'home', 'url': 'user_home'}, {'name':
 'projects', 'icon': 'sitemap', 'url': 'list_user_projects'}, {'name':
 'functions', 'icon': 'terminal', 'url': 'list_user_functions'}, {'name':
 'databases', 'icon': 'database', 'url': 'list_user_databases'}, {'name':
 'profile', 'icon': 'user', 'url': 'user_profile'} ] %}
 {% for item in menu %} {% endfor %}
```

### Comparing `runit-server-0.4.1/runit_server/templates/account/profile.html` & `runit_server-0.4.2/runit_server/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/details.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/details.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/grid.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/index.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/list.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/modals/database.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/modals/database.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/databases/modals/document.html` & `runit_server-0.4.2/runit_server/templates/admin/databases/modals/document.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/index.html` & `runit_server-0.4.2/runit_server/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/layout.html` & `runit_server-0.4.2/runit_server/templates/admin/layout.html`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
         @media screen and (min-width: 576px) {
             .main-content {
                 height: 80vh;
             }
         }
     </style>
+    <div class="d-none" id="accessToken">
+        {{request.session['access_token']}}
+    </div>
     <div class="offcanvas offcanvas-start w-auto" tabindex="-1" id="offcanvasMenu" aria-labelledby="offcanvasMenuLabel">
         <div class="offcanvas-header">
             <h5 class="offcanvas-title" id="offcanvasMenuLabel">Menu</h5>
             <!--<button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>-->
         </div>
         {% set menu = [
             {'name': 'home', 'icon': 'home', 'url': 'admin_dashboard'},
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{{request.session['access_token']}}
 **** MMeennuu ****
 {% set menu = [ {'name': 'home', 'icon': 'home', 'url': 'admin_dashboard'},
 {'name': 'users', 'icon': 'users', 'url': 'admin_list_users'}, {'name':
 'projects', 'icon': 'sitemap', 'url': 'admin_list_projects'}, {'name':
 'databases', 'icon': 'database', 'url': 'admin_list_databases'}, {'name':
 'profile', 'icon': 'user', 'url': 'admin_profile'} ] %}
 {% for item in menu %} {% endfor %}
```

### Comparing `runit-server-0.4.1/runit_server/templates/admin/login.html` & `runit_server-0.4.2/runit_server/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/projects/details.html` & `runit_server-0.4.2/runit_server/templates/admin/projects/details.html`

 * *Files 2% similar despite different names*

```diff
@@ -110,9 +110,10 @@
         </div>
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
+<script src="{{url_for('static', path='js/github.js')}}"></script>
 <script src="{{url_for('static', path='js/projects.js')}}"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.1/runit_server/templates/admin/projects/grid.html` & `runit_server-0.4.2/runit_server/templates/admin/projects/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/projects/index.html` & `runit_server-0.4.2/runit_server/templates/admin/projects/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/projects/list.html` & `runit_server-0.4.2/runit_server/templates/admin/projects/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/projects/modal.html` & `runit_server-0.4.2/runit_server/templates/admin/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/sidebar.html` & `runit_server-0.4.2/runit_server/templates/admin/sidebar.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/users/details.html` & `runit_server-0.4.2/runit_server/templates/admin/users/details.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/users/grid.html` & `runit_server-0.4.2/runit_server/templates/admin/users/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/users/index.html` & `runit_server-0.4.2/runit_server/templates/admin/users/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/users/list.html` & `runit_server-0.4.2/runit_server/templates/admin/users/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/admin/users/modal.html` & `runit_server-0.4.2/runit_server/templates/admin/users/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/databases/details.html` & `runit_server-0.4.2/runit_server/templates/databases/details.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/databases/grid.html` & `runit_server-0.4.2/runit_server/templates/databases/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/databases/index.html` & `runit_server-0.4.2/runit_server/templates/databases/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/databases/list.html` & `runit_server-0.4.2/runit_server/templates/databases/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/databases/modal.html` & `runit_server-0.4.2/runit_server/templates/databases/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/docker/php.dockerfile` & `runit_server-0.4.2/runit_server/templates/docker/php.dockerfile`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/exposed.html` & `runit_server-0.4.2/runit_server/templates/exposed.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/functions/index.html` & `runit_server-0.4.2/runit_server/templates/functions/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/layout.html` & `runit_server-0.4.2/runit_server/templates/layout.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/login.html` & `runit_server-0.4.2/runit_server/templates/login.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/modals/confirm.html` & `runit_server-0.4.2/runit_server/templates/modals/confirm.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/modals/create_database.html` & `runit_server-0.4.2/runit_server/templates/modals/create_database.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/projects/details.html` & `runit_server-0.4.2/runit_server/templates/projects/details.html`

 * *Files 1% similar despite different names*

```diff
@@ -189,9 +189,10 @@
         {{request.session['access_token']}}
     </div>
 </div>
 {% endblock %}
 
 {% block scripts %} 
 {{super()}}
+<script src="/static/js/github.js"></script>
 <script src="/static/js/projects.js"></script>
 {% endblock %}
```

### Comparing `runit-server-0.4.1/runit_server/templates/projects/grid.html` & `runit_server-0.4.2/runit_server/templates/projects/grid.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/projects/index.html` & `runit_server-0.4.2/runit_server/templates/projects/index.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/projects/list.html` & `runit_server-0.4.2/runit_server/templates/projects/list.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/projects/modal.html` & `runit_server-0.4.2/runit_server/templates/projects/modal.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/register.html` & `runit_server-0.4.2/runit_server/templates/register.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/templates/setup/index.html` & `runit_server-0.4.2/runit_server/templates/setup/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,29 @@
                             <div id="setupWizard">
                                 <div class="setup-step">
                                     <h6 class="text-center text-danger fs-6">Database Setup</h6>
                                     <div class="form-group mb-1">
                                         <label class="small" for="email">DBMS</label>
                                         <select name="DBMS" id="" class="form-select form-select-sm text-black-50" required onchange="selectDMEngine(this.value)">
                                             <option></option>
-                                            <option value="mongodb">MongoDB</option>
-                                            <option value="mysql">Mysql</option>
-                                            <option value="sqlite">Sqlites</option>
+                                            <option value="sqlite" selected>SQLITE</option>
+                                            <option value="mongodb">MONGODB</option>
+                                            <option value="postgresql">POSTGRESQL</option>
+                                            <option value="mysql" disabled>MYSQL</option>
                                         </select>
                                     </div>
                                     <div class="form-group mb-1">
                                         <label class="small">Host</label>
                                         <input type="text" value="127.0.0.1"
                                             class="form-control form-control-sm text-black-50" name="DATABASE_HOST" required>
                                     </div>
                                     <div class="form-group mb-1">
                                         <label class="small">Port</label>
                                         <input type="text" class="form-control form-control-sm text-black-50"
-                                            name="DATABASE_PORT" required>
+                                            name="DATABASE_PORT">
                                     </div>
                                     <div class="form-group mb-1">
                                         <label class="small">Database Name</label>
                                         <input type="text" name="DATABASE_NAME" value="runit"
                                             class="form-control form-control-sm text-black-50">
                                     </div>
                                     <div class="form-group mb-1">
@@ -76,14 +77,19 @@
                                         <input type="text" class="form-control form-control-sm text-black-50"
                                             value="node" name="RUNTIME_JAVASCRIPT" required>
                                     </div>
                                 </div>
                                 <div class="setup-step">
                                     <h6 class="text-center text-danger fs-6">Administrator Setup</h6>
                                     <div class="form-group mb-3">
+                                        <label class="small font-weight-bold font-roboto">Email Address</label>
+                                        <input type="email" class="form-control form-control-sm text-black-50"
+                                            value="" name="adminemail" required>
+                                    </div>
+                                    <div class="form-group mb-3">
                                         <label class="small font-weight-bold font-roboto">Username</label>
                                         <input type="text" class="form-control form-control-sm text-black-50"
                                             value="admin" name="adminusername" required>
                                     </div>
                                     <div class="form-group mb-3">
                                         <label class="small font-weight-bold font-roboto">Password</label>
                                         <input type="password" class="form-control form-control-sm text-black-50"
```

### Comparing `runit-server-0.4.1/runit_server/templates/sidebar.html` & `runit_server-0.4.2/runit_server/templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server/test.py` & `runit_server-0.4.2/runit_server/test.py`

 * *Files identical despite different names*

### Comparing `runit-server-0.4.1/runit_server.egg-info/PKG-INFO` & `runit_server-0.4.2/runit_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runit-server
-Version: 0.4.1
+Version: 0.4.2
 Summary: Backend for python-runit
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit-server/
 Project-URL: Tracker, https://github.com/theonlyamos/runit-server/issues
 Keywords: python3 runit server backend developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `runit-server-0.4.1/runit_server.egg-info/SOURCES.txt` & `runit_server-0.4.2/runit_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,18 @@
 runit_server/templates/layout.html
 runit_server/templates/login.html
 runit_server/templates/register.html
 runit_server/templates/sidebar.html
 runit_server/templates/account/home.html
 runit_server/templates/account/layout.html
 runit_server/templates/account/profile.html
+runit_server/templates/admin/dashboard.html
 runit_server/templates/admin/index.html
 runit_server/templates/admin/layout.html
 runit_server/templates/admin/login.html
-runit_server/templates/admin/profile.html
 runit_server/templates/admin/sidebar.html
 runit_server/templates/admin/databases/details.html
 runit_server/templates/admin/databases/grid.html
 runit_server/templates/admin/databases/index.html
 runit_server/templates/admin/databases/list.html
 runit_server/templates/admin/databases/modals/database.html
 runit_server/templates/admin/databases/modals/document.html
```

### Comparing `runit-server-0.4.1/setup.py` & `runit_server-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='runit-server',
     version=VERSION,
```

