# Comparing `tmp/djangorestframework-util-0.0.7.tar.gz` & `tmp/djangorestframework-util-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-util-0.0.7.tar", last modified: Wed Apr  3 05:56:05 2024, max compression
+gzip compressed data, was "djangorestframework-util-0.0.8.tar", last modified: Thu Apr 18 03:40:25 2024, max compression
```

## Comparing `djangorestframework-util-0.0.7.tar` & `djangorestframework-util-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.599383 djangorestframework-util-0.0.7/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-12-22 08:49:53.000000 djangorestframework-util-0.0.7/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/MANIFEST.in
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-03 05:56:05.598252 djangorestframework-util-0.0.7/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      443 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/README.md
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.049669 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1911 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/not-zip-safe
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       20 2024-04-03 05:56:04.000000 djangorestframework-util-0.0.7/djangorestframework_util.egg-info/top_level.txt
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.182392 djangorestframework-util-0.0.7/rest_framework_util/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      364 2024-04-03 05:38:52.000000 djangorestframework-util-0.0.7/rest_framework_util/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      448 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/apps.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.195098 djangorestframework-util-0.0.7/rest_framework_util/core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      557 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.203784 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1424 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.260955 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/aes.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/base.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.278568 djangorestframework-util-0.0.7/rest_framework_util/core/storage/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1441 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.345304 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2797 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2596 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/local.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7162 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/minio.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.406530 djangorestframework-util-0.0.7/rest_framework_util/core/upload/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      656 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/backends.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      287 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/configs.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      888 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/core/upload/settings.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.416896 djangorestframework-util-0.0.7/rest_framework_util/db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.486823 djangorestframework-util-0.0.7/rest_framework_util/db/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3013 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      635 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/manager.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      555 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/db/models/query.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1283 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/decorators.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3132 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/exceptions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3183 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/filters.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-03-25 06:44:33.000000 djangorestframework-util-0.0.7/rest_framework_util/log.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 05:56:05.583135 djangorestframework-util-0.0.7/rest_framework_util/middlewares/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      746 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/agent.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      423 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/csrf.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2207 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/exception.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2053 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2902 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/response.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      997 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.7/rest_framework_util/middlewares/trace.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2610 2024-04-03 05:38:40.000000 djangorestframework-util-0.0.7/rest_framework_util/pagination.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      704 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.7/rest_framework_util/response.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3076 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/serializers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/services.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1832 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/settings.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1749 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.7/rest_framework_util/urls.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5198 2024-04-03 05:38:40.000000 djangorestframework-util-0.0.7/rest_framework_util/viewsets.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-03 05:56:05.599383 djangorestframework-util-0.0.7/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3397 2024-03-25 06:05:43.000000 djangorestframework-util-0.0.7/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.793846 djangorestframework-util-0.0.8/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-12-22 08:49:53.000000 djangorestframework-util-0.0.8/LICENSE
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/MANIFEST.in
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-18 03:40:25.793846 djangorestframework-util-0.0.8/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      443 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/README.md
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.070163 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1351 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1972 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/not-zip-safe
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       20 2024-04-18 03:40:24.000000 djangorestframework-util-0.0.8/djangorestframework_util.egg-info/top_level.txt
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.249197 djangorestframework-util-0.0.8/rest_framework_util/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      364 2024-04-18 03:34:54.000000 djangorestframework-util-0.0.8/rest_framework_util/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      448 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/apps.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.266027 djangorestframework-util-0.0.8/rest_framework_util/core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      557 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/core/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.283975 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1424 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.352556 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/aes.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      696 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/base.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.375224 djangorestframework-util-0.0.8/rest_framework_util/core/storage/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1441 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/core/storage/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.482998 djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      178 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2797 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2596 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/local.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7162 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/minio.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.576402 djangorestframework-util-0.0.8/rest_framework_util/core/upload/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      656 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/upload/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/upload/backends.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      287 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/upload/configs.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      888 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/core/upload/settings.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.592677 djangorestframework-util-0.0.8/rest_framework_util/db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/db/__init__.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.663160 djangorestframework-util-0.0.8/rest_framework_util/db/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/db/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3013 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/db/models/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      635 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/db/models/manager.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/db/models/query.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1283 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/decorators.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3132 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/exceptions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3183 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/filters.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-03-25 06:44:33.000000 djangorestframework-util-0.0.8/rest_framework_util/log.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 03:40:25.782675 djangorestframework-util-0.0.8/rest_framework_util/middlewares/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      746 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      673 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/agent.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      423 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/csrf.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2207 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/exception.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2053 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2902 2024-03-25 08:28:04.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/response.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      997 2024-03-25 05:23:25.000000 djangorestframework-util-0.0.8/rest_framework_util/middlewares/trace.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1419 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/mixins.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2610 2024-04-03 05:38:40.000000 djangorestframework-util-0.0.8/rest_framework_util/pagination.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      704 2023-12-25 01:37:43.000000 djangorestframework-util-0.0.8/rest_framework_util/response.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1850 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/routers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3078 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/serializers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      407 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/services.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1832 2024-03-24 11:46:22.000000 djangorestframework-util-0.0.8/rest_framework_util/settings.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1981 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/urls.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5233 2024-04-18 03:25:13.000000 djangorestframework-util-0.0.8/rest_framework_util/viewsets.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-18 03:40:25.793846 djangorestframework-util-0.0.8/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3397 2024-03-25 06:05:43.000000 djangorestframework-util-0.0.8/setup.py
```

### Comparing `djangorestframework-util-0.0.7/LICENSE` & `djangorestframework-util-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/PKG-INFO` & `djangorestframework-util-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-util
-Version: 0.0.7
+Version: 0.0.8
 Summary: Common Utils for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-util
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-util
 Keywords: djangorestframework util
```

### Comparing `djangorestframework-util-0.0.7/djangorestframework_util.egg-info/PKG-INFO` & `djangorestframework-util-0.0.8/djangorestframework_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-util
-Version: 0.0.7
+Version: 0.0.8
 Summary: Common Utils for DjangoRestFramework, made easy.
 Home-page: https://gitee.com/iamfengdy/djangorestframework-util
 Author: fengdy
 Author-email: iamfengdy@126.com
 License: BSD
 Project-URL: Source, https://gitee.com/iamfengdy/djangorestframework-util
 Keywords: djangorestframework util
```

### Comparing `djangorestframework-util-0.0.7/djangorestframework_util.egg-info/SOURCES.txt` & `djangorestframework-util-0.0.8/djangorestframework_util.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 rest_framework_util/__init__.py
 rest_framework_util/apps.py
 rest_framework_util/decorators.py
 rest_framework_util/exceptions.py
 rest_framework_util/fields.py
 rest_framework_util/filters.py
 rest_framework_util/log.py
+rest_framework_util/mixins.py
 rest_framework_util/pagination.py
 rest_framework_util/response.py
+rest_framework_util/routers.py
 rest_framework_util/serializers.py
 rest_framework_util/services.py
 rest_framework_util/settings.py
 rest_framework_util/urls.py
 rest_framework_util/viewsets.py
 rest_framework_util/core/__init__.py
 rest_framework_util/core/cipher/__init__.py
```

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/__init__.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/__init__.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/aes.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/aes.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/cipher/backends/base.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/cipher/backends/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/storage/__init__.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/base.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/local.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/local.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/storage/backends/minio.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/storage/backends/minio.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/upload/__init__.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/upload/backends.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/upload/backends.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/core/upload/settings.py` & `djangorestframework-util-0.0.8/rest_framework_util/core/upload/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/db/models/base.py` & `djangorestframework-util-0.0.8/rest_framework_util/db/models/base.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/db/models/manager.py` & `djangorestframework-util-0.0.8/rest_framework_util/db/models/manager.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/db/models/query.py` & `djangorestframework-util-0.0.8/rest_framework_util/db/models/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,12 +11,14 @@
 
 from django.db.models import QuerySet
 from django.utils import timezone
 
 
 class DeleteQuerySet(QuerySet):
     def delete(self, delete_user_id):
+        """ 逻辑删除 """
         return super(DeleteQuerySet, self).update(
             delete_user_id=delete_user_id, delete_datetime=timezone.now())
 
-    def _delete(self):
+    def raw_delete(self):
+        """ 物理删除 """
         return super(DeleteQuerySet, self).delete()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/decorators.py` & `djangorestframework-util-0.0.8/rest_framework_util/decorators.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/exceptions.py` & `djangorestframework-util-0.0.8/rest_framework_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/fields.py` & `djangorestframework-util-0.0.8/rest_framework_util/fields.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/log.py` & `djangorestframework-util-0.0.8/rest_framework_util/log.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/__init__.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/agent.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/agent.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/exception.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/log.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/log.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/response.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/response.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/middlewares/trace.py` & `djangorestframework-util-0.0.8/rest_framework_util/middlewares/trace.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/pagination.py` & `djangorestframework-util-0.0.8/rest_framework_util/pagination.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/response.py` & `djangorestframework-util-0.0.8/rest_framework_util/response.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/serializers.py` & `djangorestframework-util-0.0.8/rest_framework_util/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     description = serializers.CharField(
         required=False, allow_blank=True, allow_null=True, help_text='描述')
     create_ts = serializers.SerializerMethodField()
     update_ts = serializers.SerializerMethodField()
 
     class Meta:
         fields = BaseRelatedModelSerializer.Meta.fields + (
-            'description',
+            # 'description',
             'create_user',
             'update_user',
             'create_datetime',
             'update_datetime',
             'create_ts',
             'update_ts',
         )
```

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/settings.py` & `djangorestframework-util-0.0.8/rest_framework_util/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/urls.py` & `djangorestframework-util-0.0.8/rest_framework_util/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,37 @@
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
 __all__ = ['load_urlpatterns']
 
 from importlib import import_module
 
+from django.conf import settings
 from django.urls import path, include
 
 
 def load_urlpatterns(installed_apps, with_app_prefix=True, user_prefix=None):
     """ 根据installed_apps加载url
 
     :param list installed_apps: 安装的应用
     :param bool with_app_prefix: 是否以应用名为url前缀
     :param dict user_prefix: 用户自定义url前缀，格式为{‘app名称，即在INSTALL_APP的名称’:'url前缀'}
     :return:
     """
     user_prefix = user_prefix or {}
     _urlpatterns = []
     for no, install_app in enumerate(installed_apps, start=1):
-        _string = f'{install_app}.urls.urlpatterns'
+        if settings.MODE == 'app' and not install_app.startswith('rest_framework_admin.'):
+            _install_app = install_app + '.app'
+        else:
+            _install_app = install_app
+        _string = f'{_install_app}.urls.urlpatterns'
         print(f'[#{no}] import {_string}')
         try:
-            module_path = f'{install_app}.urls'
+            module_path = f'{_install_app}.urls'
             module = import_module(module_path)
             __urlpatterns = getattr(module, 'urlpatterns')
         except ModuleNotFoundError as exc:
             print(f'\t{exc}')
         except ImportError as exc:
             print(f'\t{exc}')
         except BaseException as exc:
```

### Comparing `djangorestframework-util-0.0.7/rest_framework_util/viewsets.py` & `djangorestframework-util-0.0.8/rest_framework_util/viewsets.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,51 @@
 # Email:iamfengdy@126.com
 # DateTime:2023/12/14
 # Tool:PyCharm
 
 """  """
 __version__ = '0.0.1'
 __history__ = """"""
-__all__ = ['BaseRelModelViewSet', 'BaseModeViewSet', 'BaseFileUploadAPIView']
+__all__ = [
+    'BaseRelModelViewSet',
+    'BaseModeViewSet',
+    'BaseFileUploadAPIView',
+    'RetrieveSerializerViewSet']
 
 from abc import ABC, abstractmethod
 
 from django.db.models import Q
 from django.utils import timezone
 from rest_framework import mixins
 from rest_framework.decorators import action
 from rest_framework.views import APIView
 from rest_framework.viewsets import GenericViewSet, ModelViewSet
 
 from rest_framework_util.core.upload.settings import UploadSettings
 from rest_framework_util.core.upload.backends import upload, merge
 from rest_framework_util.exceptions import HTTP404
+from rest_framework_util.mixins import CreateRelModelMixin, DestroyRelModelMixin, UpdateRelModelMixin
 
 
-class BaseRelModelViewSet(mixins.CreateModelMixin,
-                          mixins.DestroyModelMixin,
-                          mixins.ListModelMixin,
-                          GenericViewSet):
+class RetrieveSerializerViewSet:
+    def get_serializer_class(self):
+        """ 根据固定格式获取 """
+        serializer_class = super().get_serializer_class()
+        action_name = ''
+        for _action in self.action.split('_'):
+            action_name += _action.capitalize()
+        serializer_class_name = action_name + serializer_class.__name__
+        serializer_class = getattr(
+            self.serializer_module,
+            serializer_class_name,
+            serializer_class)
+        return serializer_class
 
+
+class GenericRelViewSet(RetrieveSerializerViewSet, GenericViewSet):
     parent_key = None
     parent_model = None
 
     def get_parent_key(self):
         return self.parent_key or f'{self.parent_model.__name__.lower()}_id'
 
     def get_parent_object(self):
@@ -56,72 +72,60 @@
         queryset = super().get_queryset()
         key = self.get_parent_key()
         kwargs = {
             key: self.kwargs[key]
         }
         return queryset.filter(**kwargs)
 
-    def perform_create(self, serializer):
-        key = self.get_parent_key()
-        kwargs = {
-            key: self.kwargs[key]
-        }
-        serializer.save(create_user_id=self.request.user.id, **kwargs)
 
-    def create(self, request, *args, **kwargs):
-        response = super().create(request, *args, **kwargs)
-        response.data = None
-        return response
-
-    def perform_destroy(self, instance):
-        instance.delete(delete_user_id=self.request.user.id)
-
-
-class BaseModeViewSet(ModelViewSet):
+class BaseRelModelViewSet(mixins.ListModelMixin,
+                          CreateRelModelMixin,
+                          UpdateRelModelMixin,
+                          DestroyRelModelMixin,
+                          GenericRelViewSet):
+    pass
+
+
+class BaseModeViewSet(RetrieveSerializerViewSet, ModelViewSet):
+    http_method_names = [
+        "get",
+        "post",
+        # "put",
+        "patch",
+        "delete",
+        "head",
+        "options",
+        "trace",
+    ]
     serializer_module = None
 
     def get_queryset(self):
         queryset = super().get_queryset()
         if self.action == 'selection':
             # 过滤未激活以及过期的
             queryset = queryset.filter(is_active=True)
             model = self.serializer_class.Meta.model
             if hasattr(model, 'expire_datetime'):
                 queryset = queryset.filter(Q(expire_datetime__isnull=True) | Q(
                     expire_datetime__lt=timezone.now()))
         return queryset
 
-    def get_serializer_class(self):
-        """ 根据固定格式获取 """
-        serializer_class = super(
-            BaseModeViewSet,
-            self).get_serializer_class()
-        action_name = ''
-        for _action in self.action.split('_'):
-            action_name += _action.capitalize()
-        serializer_class_name = action_name + serializer_class.__name__
-        serializer_class = getattr(
-            self.serializer_module,
-            serializer_class_name,
-            serializer_class)
-        return serializer_class
-
-    def perform_create(self, serializer):
-        serializer.save(create_user_id=self.request.user.id)
+    def perform_create(self, serializer, **kwargs):
+        serializer.save(create_user_id=self.request.user.id, **kwargs)
 
-    def perform_update(self, serializer):
-        serializer.save(update_user_id=self.request.user.id)
+    def perform_update(self, serializer, **kwargs):
+        serializer.save(update_user_id=self.request.user.id, **kwargs)
 
     @action(detail=True, methods=['PATCH'])
     def switch(self, request, *args, **kwargs):
         """ 启用/禁用 """
         return self.update(request, *args, **kwargs)
 
-    @action(detail=False, methods=['GET'])
-    def selection(self, request, *args, **kwargs):
+    @action(detail=False, methods=['GET'], url_path='selection')
+    def select(self, request, *args, **kwargs):
         """ 下拉选择 """
         return self.list(request, *args, **kwargs)
 
 
 class BaseFileUploadAPIView(APIView, ABC):
     app_settings = None
```

### Comparing `djangorestframework-util-0.0.7/setup.py` & `djangorestframework-util-0.0.8/setup.py`

 * *Files identical despite different names*

