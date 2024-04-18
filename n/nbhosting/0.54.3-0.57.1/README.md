# Comparing `tmp/nbhosting-0.54.3.tar.gz` & `tmp/nbhosting-0.57.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbhosting-0.54.3.tar", last modified: Wed Nov  1 10:56:40 2023, max compression
+gzip compressed data, was "nbhosting-0.57.1.tar", last modified: Thu Apr 18 11:27:53 2024, max compression
```

## Comparing `nbhosting-0.54.3.tar` & `nbhosting-0.57.1.tar`

### file list

```diff
@@ -1,107 +1,116 @@
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.708101 nbhosting-0.54.3/
--rw-r--r--   0 tparment (15010) diana    (200036)      503 2023-11-01 10:56:40.707697 nbhosting-0.54.3/PKG-INFO
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.654013 nbhosting-0.54.3/nbh_main/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:32.000000 nbhosting-0.54.3/nbh_main/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       87 2019-03-16 17:17:32.000000 nbhosting-0.54.3/nbh_main/apps.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1890 2019-11-27 15:58:16.000000 nbhosting-0.54.3/nbh_main/loggers.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.654620 nbhosting-0.54.3/nbh_main/management/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbh_main/management/__init__.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.659124 nbhosting-0.54.3/nbh_main/management/commands/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbh_main/management/commands/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3131 2023-08-28 14:51:13.000000 nbhosting-0.54.3/nbh_main/management/commands/build_images.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     2984 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/management/commands/group_list.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)    14088 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/management/commands/mass_register.py
--rw-r--r--   0 tparment (15010) diana    (200036)     5651 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/management/commands/pull_students.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2136 2019-11-18 12:47:17.000000 nbhosting-0.54.3/nbh_main/management/commands/shell_sitesettings.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1740 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/management/commands/user_list.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4973 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/settings.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4178 2023-09-23 15:27:41.000000 nbhosting-0.54.3/nbh_main/sitesettings.py
--rw-r--r--   0 tparment (15010) diana    (200036)     6052 2023-06-28 11:47:55.000000 nbhosting-0.54.3/nbh_main/urls.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1654 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbh_main/views.py
--rw-r--r--   0 tparment (15010) diana    (200036)      394 2020-11-20 21:56:02.000000 nbhosting-0.54.3/nbh_main/wsgi.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.662051 nbhosting-0.54.3/nbhosting/
--rw-r--r--   0 tparment (15010) diana    (200036)      335 2020-08-02 15:51:31.000000 nbhosting-0.54.3/nbhosting/__init__.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.677231 nbhosting-0.54.3/nbhosting/courses/
--rw-r--r--   0 tparment (15010) diana    (200036)      363 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)      667 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/admin.py
--rw-r--r--   0 tparment (15010) diana    (200036)       99 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/courses/apps.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2506 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/forms.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.678027 nbhosting-0.54.3/nbhosting/courses/management/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/courses/management/__init__.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.686189 nbhosting-0.54.3/nbhosting/courses/management/commands/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1811 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_auto_pull.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1369 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_build_image.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1655 2020-08-02 15:51:31.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_create.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1568 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_delete.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2043 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_group.py
--rw-r--r--   0 tparment (15010) diana    (200036)      715 2023-08-29 07:53:17.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_image_details.py
--rw-r--r--   0 tparment (15010) diana    (200036)     7833 2023-09-24 14:47:23.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_list.py
--rw-r--r--   0 tparment (15010) diana    (200036)      707 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_pull.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1136 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_rename.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1688 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_run_build.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2002 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/management/commands/course_tracks.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.689794 nbhosting-0.54.3/nbhosting/courses/migrations/
--rw-r--r--   0 tparment (15010) diana    (200036)     1022 2019-07-11 13:23:28.000000 nbhosting-0.54.3/nbhosting/courses/migrations/0001_initial.py
--rw-r--r--   0 tparment (15010) diana    (200036)      597 2019-10-31 10:53:08.000000 nbhosting-0.54.3/nbhosting/courses/migrations/0002_registered_groups.py
--rw-r--r--   0 tparment (15010) diana    (200036)      391 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/migrations/0003_coursedir_archived.py
--rw-r--r--   0 tparment (15010) diana    (200036)      393 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/migrations/0004_coursedir_autobuild.py
--rw-r--r--   0 tparment (15010) diana    (200036)      445 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/migrations/0005_alter_coursedir_id.py
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-07-11 13:23:28.000000 nbhosting-0.54.3/nbhosting/courses/migrations/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2901 2023-10-11 13:41:57.000000 nbhosting-0.54.3/nbhosting/courses/model_build.py
--rw-r--r--   0 tparment (15010) diana    (200036)    33660 2023-10-11 13:26:14.000000 nbhosting-0.54.3/nbhosting/courses/model_course.py
--rw-r--r--   0 tparment (15010) diana    (200036)     5250 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/model_dropped.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2205 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/courses/model_mapping.py
--rw-r--r--   0 tparment (15010) diana    (200036)    13826 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/model_track.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3181 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/tests.py
--rw-r--r--   0 tparment (15010) diana    (200036)     5201 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/views_auditor.py
--rw-r--r--   0 tparment (15010) diana    (200036)     6509 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/views_staff.py
--rw-r--r--   0 tparment (15010) diana    (200036)     4535 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/courses/views_teacher.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.693049 nbhosting-0.54.3/nbhosting/edxfront/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       63 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/admin.py
--rw-r--r--   0 tparment (15010) diana    (200036)      142 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/apps.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.694161 nbhosting-0.54.3/nbhosting/edxfront/migrations/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/migrations/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       98 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/models.py
--rw-r--r--   0 tparment (15010) diana    (200036)       60 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/edxfront/tests.py
--rw-r--r--   0 tparment (15010) diana    (200036)    21830 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/edxfront/views.py
--rw-r--r--   0 tparment (15010) diana    (200036)     1301 2019-09-22 09:12:57.000000 nbhosting-0.54.3/nbhosting/matching.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.700230 nbhosting-0.54.3/nbhosting/stats/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/stats/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       63 2017-02-01 15:36:56.000000 nbhosting-0.54.3/nbhosting/stats/admin.py
--rw-r--r--   0 tparment (15010) diana    (200036)       95 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/stats/apps.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.700893 nbhosting-0.54.3/nbhosting/stats/management/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/stats/management/__init__.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.702324 nbhosting-0.54.3/nbhosting/stats/management/commands/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/stats/management/commands/__init__.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     6804 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/stats/management/commands/containers.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1501 2020-05-26 14:19:11.000000 nbhosting-0.54.3/nbhosting/stats/management/commands/monitor.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.703095 nbhosting-0.54.3/nbhosting/stats/migrations/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2017-02-01 15:36:56.000000 nbhosting-0.54.3/nbhosting/stats/migrations/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       57 2017-02-01 15:36:56.000000 nbhosting-0.54.3/nbhosting/stats/models.py
--rwxr-xr-x   0 tparment (15010) diana    (200036)    20668 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/stats/monitor.py
--rw-r--r--   0 tparment (15010) diana    (200036)    19912 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/stats/stats.py
--rw-r--r--   0 tparment (15010) diana    (200036)       60 2017-02-01 15:36:56.000000 nbhosting-0.54.3/nbhosting/stats/tests.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3058 2019-03-16 17:17:33.000000 nbhosting-0.54.3/nbhosting/stats/timebuckets.py
--rw-r--r--   0 tparment (15010) diana    (200036)     3967 2023-06-22 06:30:45.000000 nbhosting-0.54.3/nbhosting/stats/views.py
--rw-r--r--   0 tparment (15010) diana    (200036)      593 2019-02-18 08:08:10.000000 nbhosting-0.54.3/nbhosting/stats/wip-testresults.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.706674 nbhosting-0.54.3/nbhosting/students/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-11-04 18:31:45.000000 nbhosting-0.54.3/nbhosting/students/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)       63 2019-11-04 13:32:12.000000 nbhosting-0.54.3/nbhosting/students/admin.py
--rw-r--r--   0 tparment (15010) diana    (200036)       91 2019-11-04 13:32:12.000000 nbhosting-0.54.3/nbhosting/students/apps.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.707270 nbhosting-0.54.3/nbhosting/students/migrations/
--rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-11-04 13:32:12.000000 nbhosting-0.54.3/nbhosting/students/migrations/__init__.py
--rw-r--r--   0 tparment (15010) diana    (200036)     2036 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/students/models.py
--rw-r--r--   0 tparment (15010) diana    (200036)       60 2019-11-04 13:32:12.000000 nbhosting-0.54.3/nbhosting/students/tests.py
--rw-r--r--   0 tparment (15010) diana    (200036)      116 2019-11-04 13:45:30.000000 nbhosting-0.54.3/nbhosting/students/views.py
--rw-r--r--   0 tparment (15010) diana    (200036)      339 2023-06-22 06:30:18.000000 nbhosting-0.54.3/nbhosting/utils.py
--rw-r--r--   0 tparment (15010) diana    (200036)       23 2023-11-01 10:56:26.000000 nbhosting-0.54.3/nbhosting/version.py
-drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2023-11-01 10:56:40.664095 nbhosting-0.54.3/nbhosting.egg-info/
--rw-r--r--   0 tparment (15010) diana    (200036)      503 2023-11-01 10:56:40.000000 nbhosting-0.54.3/nbhosting.egg-info/PKG-INFO
--rw-r--r--   0 tparment (15010) diana    (200036)     3107 2023-11-01 10:56:40.000000 nbhosting-0.54.3/nbhosting.egg-info/SOURCES.txt
--rw-r--r--   0 tparment (15010) diana    (200036)        1 2023-11-01 10:56:40.000000 nbhosting-0.54.3/nbhosting.egg-info/dependency_links.txt
--rw-r--r--   0 tparment (15010) diana    (200036)      107 2023-11-01 10:56:40.000000 nbhosting-0.54.3/nbhosting.egg-info/requires.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       19 2023-11-01 10:56:40.000000 nbhosting-0.54.3/nbhosting.egg-info/top_level.txt
--rw-r--r--   0 tparment (15010) diana    (200036)       38 2023-11-01 10:56:40.708218 nbhosting-0.54.3/setup.cfg
--rwxr-xr-x   0 tparment (15010) diana    (200036)     1359 2023-11-01 10:54:46.000000 nbhosting-0.54.3/setup.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.039974 nbhosting-0.57.1/
+-rw-r--r--   0 tparment (15010) diana    (200036)      832 2024-04-18 11:27:53.039375 nbhosting-0.57.1/PKG-INFO
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:52.990589 nbhosting-0.57.1/nbh_main/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:32.000000 nbhosting-0.57.1/nbh_main/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       87 2019-03-16 17:17:32.000000 nbhosting-0.57.1/nbh_main/apps.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1388 2023-12-19 12:04:17.000000 nbhosting-0.57.1/nbh_main/loggers.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:52.991088 nbhosting-0.57.1/nbh_main/management/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbh_main/management/__init__.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:52.994382 nbhosting-0.57.1/nbh_main/management/commands/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbh_main/management/commands/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3131 2023-08-28 14:51:13.000000 nbhosting-0.57.1/nbh_main/management/commands/build_images.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     2984 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbh_main/management/commands/group_list.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)    14088 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbh_main/management/commands/mass_register.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     5651 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbh_main/management/commands/pull_students.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2136 2019-11-18 12:47:17.000000 nbhosting-0.57.1/nbh_main/management/commands/shell_sitesettings.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1740 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbh_main/management/commands/user_list.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     5003 2024-04-18 10:55:15.000000 nbhosting-0.57.1/nbh_main/settings.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     4178 2023-09-23 15:27:41.000000 nbhosting-0.57.1/nbh_main/sitesettings.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     6332 2024-04-18 09:13:24.000000 nbhosting-0.57.1/nbh_main/urls.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1654 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbh_main/views.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      394 2020-11-20 21:56:02.000000 nbhosting-0.57.1/nbh_main/wsgi.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:52.996906 nbhosting-0.57.1/nbhosting/
+-rw-r--r--   0 tparment (15010) diana    (200036)      335 2020-08-02 15:51:31.000000 nbhosting-0.57.1/nbhosting/__init__.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.010557 nbhosting-0.57.1/nbhosting/courses/
+-rw-r--r--   0 tparment (15010) diana    (200036)      363 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      667 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/admin.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       99 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/courses/apps.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2506 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/forms.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.011620 nbhosting-0.57.1/nbhosting/courses/management/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/courses/management/__init__.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.017452 nbhosting-0.57.1/nbhosting/courses/management/commands/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1811 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_auto_pull.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1369 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_build_image.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1655 2020-08-02 15:51:31.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_create.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1568 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_delete.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2043 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_group.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      715 2023-08-29 07:53:17.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_image_details.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     7833 2023-09-24 14:47:23.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_list.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      707 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_pull.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1136 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_rename.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1688 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_run_build.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2002 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/management/commands/course_tracks.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.020485 nbhosting-0.57.1/nbhosting/courses/migrations/
+-rw-r--r--   0 tparment (15010) diana    (200036)     1022 2019-07-11 13:23:28.000000 nbhosting-0.57.1/nbhosting/courses/migrations/0001_initial.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      597 2019-10-31 10:53:08.000000 nbhosting-0.57.1/nbhosting/courses/migrations/0002_registered_groups.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      391 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/migrations/0003_coursedir_archived.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      393 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/migrations/0004_coursedir_autobuild.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      445 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/migrations/0005_alter_coursedir_id.py
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-07-11 13:23:28.000000 nbhosting-0.57.1/nbhosting/courses/migrations/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2901 2023-10-11 13:41:57.000000 nbhosting-0.57.1/nbhosting/courses/model_build.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    33660 2024-04-16 13:07:38.000000 nbhosting-0.57.1/nbhosting/courses/model_course.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     5250 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/model_dropped.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2205 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/courses/model_mapping.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    13826 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/model_track.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3181 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/tests.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     5201 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/views_auditor.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     6652 2024-04-18 09:13:24.000000 nbhosting-0.57.1/nbhosting/courses/views_staff.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     4535 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/courses/views_teacher.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.023400 nbhosting-0.57.1/nbhosting/edxfront/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       63 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/admin.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      142 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/apps.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.024005 nbhosting-0.57.1/nbhosting/edxfront/migrations/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/migrations/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       98 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/models.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       60 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/edxfront/tests.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    21830 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/edxfront/views.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     1292 2024-04-17 12:59:14.000000 nbhosting-0.57.1/nbhosting/matching.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.026692 nbhosting-0.57.1/nbhosting/process/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       63 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/admin.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      146 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/apps.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.027543 nbhosting-0.57.1/nbhosting/process/migrations/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/migrations/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       57 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/models.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       60 2024-04-18 09:04:57.000000 nbhosting-0.57.1/nbhosting/process/tests.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3175 2024-04-18 11:17:17.000000 nbhosting-0.57.1/nbhosting/process/views.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.032499 nbhosting-0.57.1/nbhosting/stats/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/stats/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       63 2017-02-01 15:36:56.000000 nbhosting-0.57.1/nbhosting/stats/admin.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       95 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/stats/apps.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.033002 nbhosting-0.57.1/nbhosting/stats/management/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/stats/management/__init__.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.034449 nbhosting-0.57.1/nbhosting/stats/management/commands/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/stats/management/commands/__init__.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     6804 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/stats/management/commands/containers.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1501 2020-05-26 14:19:11.000000 nbhosting-0.57.1/nbhosting/stats/management/commands/monitor.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.035008 nbhosting-0.57.1/nbhosting/stats/migrations/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2017-02-01 15:36:56.000000 nbhosting-0.57.1/nbhosting/stats/migrations/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       57 2017-02-01 15:36:56.000000 nbhosting-0.57.1/nbhosting/stats/models.py
+-rwxr-xr-x   0 tparment (15010) diana    (200036)    20668 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/stats/monitor.py
+-rw-r--r--   0 tparment (15010) diana    (200036)    19912 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/stats/stats.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       60 2017-02-01 15:36:56.000000 nbhosting-0.57.1/nbhosting/stats/tests.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3058 2019-03-16 17:17:33.000000 nbhosting-0.57.1/nbhosting/stats/timebuckets.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     3967 2023-06-22 06:30:45.000000 nbhosting-0.57.1/nbhosting/stats/views.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      593 2019-02-18 08:08:10.000000 nbhosting-0.57.1/nbhosting/stats/wip-testresults.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.037713 nbhosting-0.57.1/nbhosting/students/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-11-04 18:31:45.000000 nbhosting-0.57.1/nbhosting/students/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       63 2019-11-04 13:32:12.000000 nbhosting-0.57.1/nbhosting/students/admin.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       91 2019-11-04 13:32:12.000000 nbhosting-0.57.1/nbhosting/students/apps.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.038181 nbhosting-0.57.1/nbhosting/students/migrations/
+-rw-r--r--   0 tparment (15010) diana    (200036)        0 2019-11-04 13:32:12.000000 nbhosting-0.57.1/nbhosting/students/migrations/__init__.py
+-rw-r--r--   0 tparment (15010) diana    (200036)     2036 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/students/models.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       60 2019-11-04 13:32:12.000000 nbhosting-0.57.1/nbhosting/students/tests.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      116 2019-11-04 13:45:30.000000 nbhosting-0.57.1/nbhosting/students/views.py
+-rw-r--r--   0 tparment (15010) diana    (200036)      339 2023-06-22 06:30:18.000000 nbhosting-0.57.1/nbhosting/utils.py
+-rw-r--r--   0 tparment (15010) diana    (200036)       23 2024-04-18 11:25:34.000000 nbhosting-0.57.1/nbhosting/version.py
+drwxr-xr-x   0 tparment (15010) diana    (200036)        0 2024-04-18 11:27:53.038669 nbhosting-0.57.1/nbhosting.egg-info/
+-rw-r--r--   0 tparment (15010) diana    (200036)      832 2024-04-18 11:27:52.000000 nbhosting-0.57.1/nbhosting.egg-info/PKG-INFO
+-rw-r--r--   0 tparment (15010) diana    (200036)     3313 2024-04-18 11:27:52.000000 nbhosting-0.57.1/nbhosting.egg-info/SOURCES.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)        1 2024-04-18 11:27:52.000000 nbhosting-0.57.1/nbhosting.egg-info/dependency_links.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)      119 2024-04-18 11:27:52.000000 nbhosting-0.57.1/nbhosting.egg-info/requires.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       19 2024-04-18 11:27:52.000000 nbhosting-0.57.1/nbhosting.egg-info/top_level.txt
+-rw-r--r--   0 tparment (15010) diana    (200036)       38 2024-04-18 11:27:53.040119 nbhosting-0.57.1/setup.cfg
+-rwxr-xr-x   0 tparment (15010) diana    (200036)     1557 2024-04-18 10:55:15.000000 nbhosting-0.57.1/setup.py
```

### Comparing `nbhosting-0.54.3/nbh_main/loggers.py` & `nbhosting-0.57.1/nbh_main/loggers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,54 @@
-import sys
+"""
+initialize loggers for nbhosting
+"""
 
-from pathlib import Path
+import sys
 
 import logging
 import logging.config
-from logging.handlers import TimedRotatingFileHandler
+
 
 def init_loggers(debug):
+    """
+    initialize loggers for nbhosting
+    """
 
-    level = 'INFO' if not debug else 'DEBUG'
+    level = 'DEBUG' if debug else 'INFO'
 
     logging.config.dictConfig({
-        'version' : 1,
-        'disable_existing_loggers' : False,
+        'version': 1,
+        'disable_existing_loggers': False,
         'formatters': {
             'standard': {
-                'format': '%(asctime)s.%(msecs)03d %(levelname)s %(filename)s:%(lineno)d %(message)s',
+                'format': (
+                    '%(asctime)s.%(msecs)03d %(levelname)s'
+                    ' %(filename)s:%(lineno)d %(message)s'
+                ),
                 'datefmt': '%m-%d %H:%M:%S'
             },
             'shorter': {
                 'format': '%(asctime)s.%(msecs)03d %(levelname)s %(message)s',
                 'datefmt': '%d %H:%M:%S'
             },
         },
         'handlers': {
-#            'nbhosting': {
-#                'class': 'logging.handlers.TimedRotatingFileHandler',
-#                'when': 'midnight',
-#                'backupCount': 7,
-#                'formatter': 'standard',
-#                'filename' : str(path / 'nbhosting.log'),
-#            },
-#            'monitor': {
-#                'class': 'logging.handlers.TimedRotatingFileHandler',
-#                'when': 'midnight',
-#                'backupCount': 7,
-#                'formatter': 'standard',
-#                'filename' : str(path / 'monitor.log'),
-#            },
             'stdout': {
                 'level': level,
                 'class': 'logging.StreamHandler',
                 'formatter': 'standard',
                 'stream': sys.stdout,
             }
         },
         'loggers': {
             'nbhosting': {
                 'level': level,
-                'handlers': ['stdout'],  # no longer on 'nbhosting'
+                'handlers': ['stdout'],   # logs go to systemd/journal
                 'propagate': False,
             },
             'monitor': {
                 'level': level,
-                'handlers': ['stdout'],  # ditto, logs go to systemd/journal
+                'handlers': ['stdout'],   # logs go to systemd/journal
                 'propagate': False,
             },
         },
     })
```

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/build_images.py` & `nbhosting-0.57.1/nbh_main/management/commands/build_images.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/group_list.py` & `nbhosting-0.57.1/nbh_main/management/commands/group_list.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/mass_register.py` & `nbhosting-0.57.1/nbh_main/management/commands/mass_register.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/pull_students.py` & `nbhosting-0.57.1/nbh_main/management/commands/pull_students.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/shell_sitesettings.py` & `nbhosting-0.57.1/nbh_main/management/commands/shell_sitesettings.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/management/commands/user_list.py` & `nbhosting-0.57.1/nbh_main/management/commands/user_list.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/settings.py` & `nbhosting-0.57.1/nbh_main/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     sitesettings.nbhroot = str(django_root / 'fake-root')
     # .parents[0] is dirname(f)
     # .parents[1] is dirname(dirname(f))
     BASE_DIR = Path(__file__).parents[1]
 
     # have the static files served in devel mode
     STATICFILES_DIRS = (str(BASE_DIR / "assets"), )
+    print("DEVEL MODE IS ON")
     DEVEL = True
 
 NBHROOT = Path(sitesettings.nbhroot).resolve()
 
 init_loggers(DEBUG)
 logger = logging.getLogger('nbhosting')
 monitor_logger = logging.getLogger('monitor')
```

### Comparing `nbhosting-0.54.3/nbh_main/sitesettings.py` & `nbhosting-0.57.1/nbh_main/sitesettings.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbh_main/urls.py` & `nbhosting-0.57.1/nbh_main/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.contrib.auth import views as auth_views
 
 import nbhosting.edxfront.views
 import nbhosting.courses.views_auditor
 import nbhosting.courses.views_staff
 import nbhosting.courses.views_teacher
 import nbhosting.stats.views
+import nbhosting.process.views
 import nbh_main.views                                # pylint: disable=wrong-import-order
 
 TRACK =       r'(?P<track>[^/]*)'
 COURSE =      r'(?P<course>\w[\w\d_.-]*)'
 STUDENT =     r'(?P<student>\w[\w\d_.-]*)'
 GROUP =       r'(?P<group>\w[\w\d_.-]*)'
 DROPAREA =    r'(?P<droparea>\w[\w\d_.-]*)'
@@ -73,14 +74,16 @@
                         nbhosting.courses.views_teacher.teacher_dropped_deploy),
 
     # super user
     re_path(rf'^staff/courses/update-from-git/{COURSE}/?$',
                         nbhosting.courses.views_staff.update_from_git),
     re_path(rf'^staff/courses/build-image/{COURSE}/?$',
                         nbhosting.courses.views_staff.build_image),
+    re_path(rf'^staff/courses/build-image-force/{COURSE}/?$',
+                        nbhosting.courses.views_staff.build_image_force),
     re_path(rf'^staff/courses/destroy-my-container/{COURSE}/?$',
                         nbhosting.courses.views_staff.destroy_my_container),
     re_path(rf'^staff/courses/clear-staff/{COURSE}/?$',
                         nbhosting.courses.views_staff.clear_staff),
     re_path(rf'^staff/courses/show-tracks/{COURSE}/?$',
                         nbhosting.courses.views_staff.show_tracks),
     re_path(rf'^staff/courses.*',
@@ -99,14 +102,16 @@
     re_path(rf'^staff/stats/{COURSE}/?$',
                         nbhosting.stats.views.show_stats),
     re_path(rf'^staff.*',
                         nbh_main.views.welcome),
     # this one is not reachable through nginx, mostly for devel
     re_path(rf'^welcome.*',
                         nbh_main.views.welcome),
+    re_path(rf'^process/run.*',
+                        nbhosting.process.views.run_process_and_stream_outputs),
     # empty url
     re_path(rf'^$',
                         nbh_main.views.welcome),
 
     # various redirects and other django-provided pages
     re_path(rf'^admin/',
                         admin.site.urls),
```

### Comparing `nbhosting-0.54.3/nbh_main/views.py` & `nbhosting-0.57.1/nbh_main/views.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/admin.py` & `nbhosting-0.57.1/nbhosting/courses/admin.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/forms.py` & `nbhosting-0.57.1/nbhosting/courses/forms.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_auto_pull.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_auto_pull.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_build_image.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_build_image.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_create.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_create.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_delete.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_delete.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_group.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_group.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_image_details.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_image_details.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_list.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_list.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_pull.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_pull.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_rename.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_rename.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_run_build.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_run_build.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/management/commands/course_tracks.py` & `nbhosting-0.57.1/nbhosting/courses/management/commands/course_tracks.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/migrations/0001_initial.py` & `nbhosting-0.57.1/nbhosting/courses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/migrations/0002_registered_groups.py` & `nbhosting-0.57.1/nbhosting/courses/migrations/0002_registered_groups.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/model_build.py` & `nbhosting-0.57.1/nbhosting/courses/model_build.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/model_course.py` & `nbhosting-0.57.1/nbhosting/courses/model_course.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/model_dropped.py` & `nbhosting-0.57.1/nbhosting/courses/model_dropped.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/model_mapping.py` & `nbhosting-0.57.1/nbhosting/courses/model_mapping.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/model_track.py` & `nbhosting-0.57.1/nbhosting/courses/model_track.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/tests.py` & `nbhosting-0.57.1/nbhosting/courses/tests.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/views_auditor.py` & `nbhosting-0.57.1/nbhosting/courses/views_auditor.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/courses/views_staff.py` & `nbhosting-0.57.1/nbhosting/courses/views_staff.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # pylint: disable=c0111, w1203, r1705
 
+import json
+
+
 from django.shortcuts import render, get_object_or_404
 
 from django.http import HttpResponse, HttpResponseRedirect, HttpResponseNotFound
 from django.views.decorators.csrf import csrf_protect
 from django.contrib.admin.views.decorators import staff_member_required
 
+from nbh_main.settings import NBHROOT
 # from nbh_main.settings import logger
 
 from nbhosting.courses.model_course import CourseDir
 from nbhosting.courses.forms import UpdateCourseForm
 
 from nbhosting.version import __version__ as nbh_version
 from nbh_main.settings import sitesettings
@@ -74,76 +78,80 @@
         giturl=coursedir.giturl,
         tracks=coursedir.tracks(),
         enriched_groups=enriched_groups,
     )
     return render(request, "staff-course.html", env)
 
 
-def render_subprocess_result(request, course,
-                             subcommand, message, python, *args):
-    """    triggers a subprocess and displays results
-    in a web page with returncode, stdout, stderr
+def render_subprocess_stream(
+        request, course, subcommand, message, python, *args):
+    """
+    returns a HTML page that contains a call to /process/run
+    so that the output gets streamed on the fly
 
     this can be either a call to
-    * plain nbh (for code written in bash) with managed=False
+    * plain nbh (for code written in bash) with python=False
     * or to nbh-manage for code written in python
-
     """
-    coursedir = CourseDir.objects.get(coursename=course)
-    completed = coursedir.nbh_subprocess(subcommand, python, *args)
-    command = " ".join(completed.args)
-    # expose most locals, + the attributes of completed
-    # like stdout and stderr
+    if not python:
+        command = ["nbh", "-d", str(NBHROOT)]
+    else:
+        command = [ "nbh-manage" ]
+    command += [subcommand, course] + list(args)
+
+    command_json = json.dumps(command)
+    command_string = " ".join(command)
+
     env = dict(
         nbh_version=nbh_version,
         favicon_path=sitesettings.favicon_path,
         course=course,
         message=message,
-        command=command,
-        returncode=completed.returncode,
-        stdout=completed.stdout,
-        stderr=completed.stderr,
+        command_json=command_json,
+        command_string=command_string,
     )
-    # the html title
-    template = "course-managed.html"
+    template = "course-process.html"
     return render(request, template, env)
 
 
 @staff_member_required
 @csrf_protect
 def update_from_git(request, course):
-    return render_subprocess_result(
-        request, course,
-        "course-update-from-git", 'updated', False)
+    return render_subprocess_stream(
+        request, course, "course-update-from-git", 'updating git repo', False)
 
 
 @staff_member_required
 @csrf_protect
 def build_image(request, course):
-    return render_subprocess_result(
-        request, course,
-        "course-build-image", 'rebuilt', True)
+    return render_subprocess_stream(
+        request, course, "course-build-image", 'rebuilding image', True)
+
+
+@staff_member_required
+@csrf_protect
+def build_image_force(request, course):
+    return render_subprocess_stream(
+        request, course, "course-build-image", 'rebuilding image', True, "--force")
 
 
 @staff_member_required
 @csrf_protect
 def clear_staff(request, course):
     coursedir = CourseDir.objects.get(coursename=course)
-    return render_subprocess_result(
-        request, course,
-        "course-clear-staff", 'staff files cleared', False,
-        *coursedir.staffs)
+    return render_subprocess_stream(
+        request, course, "course-clear-staff", 'clearing staff files',
+        False, *coursedir.staffs)
 
 
 @staff_member_required
 @csrf_protect
 def show_tracks(request, course):
-    return render_subprocess_result(
-        request, course,
-        "course-tracks", 'tracks recomputed', True)
+    return render_subprocess_stream(
+        request, course, "course-tracks", 'recomputing tracks', True)
 
 
 @staff_member_required
 @csrf_protect
 def destroy_my_container(request, course):
     coursedir = get_object_or_404(CourseDir, coursename=course)
     killed = coursedir.kill_student_container(request.user.username)
```

### Comparing `nbhosting-0.54.3/nbhosting/courses/views_teacher.py` & `nbhosting-0.57.1/nbhosting/courses/views_teacher.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/edxfront/views.py` & `nbhosting-0.57.1/nbhosting/edxfront/views.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/matching.py` & `nbhosting-0.57.1/nbhosting/matching.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import re
 
 def matching_policy(name, patterns):
-    """
+    r"""
     matching policy for course or students is as follows
 
     patterns is an iterable of patterns
     matching means a 'OR' of all patterns
     if patterns is empty, name is a match
-    
+
     if one pattern is empty, name is a match
-    if one pattern starts with a =, name matches 
+    if one pattern starts with a =, name matches
         only if it is an exact match of what is after =
-    if one pattern does not contain a '*', 
+    if one pattern does not contain a '*',
         all names that **contain** the filter match
     if one pattern contains a '*', name needs to match that pattern
         in the re sense, with:
         '*' replaced with '.*'
         '.' replaced by \.
     """
-    
+
     if not patterns:
         return True
     for pattern in patterns:
         # an empty pattern like "" or None means a match
         if not pattern:
             return True
         # exact match
         if pattern[0] == '=':
             if name == pattern[1:]:
                 return True
-        # if '*' is 
+        # if '*' is
         elif '*' in pattern:
             pattern = (pattern
-                .replace('.', '\.')
+                .replace('.', r'\.')
                 .replace('*', '.*'))
             pattern = f"^{pattern}$"
             if re.match(pattern, name):
                 return True
         else:
             if pattern in name:
                 return True
```

### Comparing `nbhosting-0.54.3/nbhosting/stats/management/commands/containers.py` & `nbhosting-0.57.1/nbhosting/stats/management/commands/containers.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/management/commands/monitor.py` & `nbhosting-0.57.1/nbhosting/stats/management/commands/monitor.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/monitor.py` & `nbhosting-0.57.1/nbhosting/stats/monitor.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/stats.py` & `nbhosting-0.57.1/nbhosting/stats/stats.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/timebuckets.py` & `nbhosting-0.57.1/nbhosting/stats/timebuckets.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/views.py` & `nbhosting-0.57.1/nbhosting/stats/views.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/stats/wip-testresults.py` & `nbhosting-0.57.1/nbhosting/stats/wip-testresults.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting/students/models.py` & `nbhosting-0.57.1/nbhosting/students/models.py`

 * *Files identical despite different names*

### Comparing `nbhosting-0.54.3/nbhosting.egg-info/SOURCES.txt` & `nbhosting-0.57.1/nbhosting.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -59,14 +59,21 @@
 nbhosting/edxfront/__init__.py
 nbhosting/edxfront/admin.py
 nbhosting/edxfront/apps.py
 nbhosting/edxfront/models.py
 nbhosting/edxfront/tests.py
 nbhosting/edxfront/views.py
 nbhosting/edxfront/migrations/__init__.py
+nbhosting/process/__init__.py
+nbhosting/process/admin.py
+nbhosting/process/apps.py
+nbhosting/process/models.py
+nbhosting/process/tests.py
+nbhosting/process/views.py
+nbhosting/process/migrations/__init__.py
 nbhosting/stats/__init__.py
 nbhosting/stats/admin.py
 nbhosting/stats/apps.py
 nbhosting/stats/models.py
 nbhosting/stats/monitor.py
 nbhosting/stats/stats.py
 nbhosting/stats/tests.py
```

### Comparing `nbhosting-0.54.3/setup.py` & `nbhosting-0.57.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,50 @@
 __package__ = 'nbhosting'
 from .version import __version__
 
 
 try:
     with open("README.md") as readme:
         long_description = readme.read()
-except Exception as e:
+except Exception as exc:
     long_description = "no description could be found"
 
 setup(
-    name = 'nbhosting',
-    version = __version__,
-    author = "Thierry Parmentelat",
-    author_email = "thierry.parmentelat@inria.fr",
-    packages = find_packages(),
-    url = "https://github.com/parmentelat/nbhosting",
-    license = "See LICENSE",
-    description = "An infrastructure for hosting notebooks behind an open-edX MOOC platform, or for registered students like in a classroom",
-    long_description = long_description,
-    install_requires = [
+    name='nbhosting',
+    version=__version__,
+    author="Thierry Parmentelat",
+    author_email="thierry.parmentelat@inria.fr",
+    packages=find_packages(),
+    url="https://github.com/parmentelat/nbhosting",
+    license="See LICENSE",
+    description=(
+        "An infrastructure for hosting notebooks behind an open-edX"
+        " MOOC platform, or for registered students like in a classroom"
+    ),
+    long_description=long_description,
+    install_requires=[
         'pip',
         'setuptools',
         'wheel',
         'django',
         'django_extensions',
         'jsonpickle',
         'nbformat',
         'jupytext',
         'aiohttp',
         'podman',
+        'rich',        # this is for podman, should not be needed, see also
+                       # https://github.com/containers/podman/issues/20964
         'redis',
-        'nbstripout', # for course-pull
+        'nbstripout',  # for course-pull
+        'pandas',      # for mass-register
     ],
-    setup_requires = [],
-    tests_require = [],
+    setup_requires=[],
+    tests_require=[],
 
     # see https://pypi.python.org/pypi?%3Aaction=list_classifiers
-    classifiers = [
+    classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
 )
```

