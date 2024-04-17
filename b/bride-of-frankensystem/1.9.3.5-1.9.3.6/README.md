# Comparing `tmp/bride-of-frankensystem-1.9.3.5.tar.gz` & `tmp/bride-of-frankensystem-1.9.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-m_s5kw6w\bride-of-frankensystem-1.9.3.5.tar", last modified: Tue Apr 16 06:21:27 2024, max compression
+gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-oxepvw9e\bride-of-frankensystem-1.9.3.6.tar", last modified: Wed Apr 17 23:48:27 2024, max compression
```

## Comparing `bride-of-frankensystem-1.9.3.5.tar` & `bride-of-frankensystem-1.9.3.6.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/BOFS/
--rw-rw-rw-   0        0        0    14964 2024-04-15 21:52:57.000000 bride-of-frankensystem-1.9.3.5/BOFS/BOFSFlask.py
--rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.5/BOFS/BOFSSession.py
--rw-rw-rw-   0        0        0    11139 2024-04-16 04:31:57.000000 bride-of-frankensystem-1.9.3.5/BOFS/JSONQuestionnaire.py
--rw-rw-rw-   0        0        0     6767 2024-04-15 22:35:58.000000 bride-of-frankensystem-1.9.3.5/BOFS/JSONTable.py
--rw-rw-rw-   0        0        0     5672 2024-04-15 21:33:28.000000 bride-of-frankensystem-1.9.3.5/BOFS/PageList.py
--rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.5/BOFS/__init__.py
--rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.5/BOFS/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/
--rw-rw-rw-   0        0        0    20083 2024-04-15 22:10:04.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/BOFSFlask.cpython-311.pyc
--rw-rw-rw-   0        0        0     5318 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/BOFSSession.cpython-311.pyc
--rw-rw-rw-   0        0        0    16499 2024-04-16 04:32:10.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
--rw-rw-rw-   0        0        0     9769 2024-04-15 22:36:04.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/JSONTable.cpython-311.pyc
--rw-rw-rw-   0        0        0     6901 2024-04-15 22:13:05.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/PageList.cpython-311.pyc
--rw-rw-rw-   0        0        0      384 2024-04-05 21:05:42.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      337 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/__main__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1998 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/cli.cpython-311.pyc
--rw-rw-rw-   0        0        0     6116 2024-04-16 05:54:42.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/create_app.cpython-311.pyc
--rw-rw-rw-   0        0        0     3017 2024-04-15 22:14:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/globals.cpython-311.pyc
--rw-rw-rw-   0        0        0    17284 2024-04-16 04:26:24.000000 bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/util.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/
--rw-rw-rw-   0        0        0     7018 2024-04-15 21:41:52.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/QuestionnaireResults.py
--rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/
--rw-rw-rw-   0        0        0     2007 2022-05-19 18:13:22.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc
--rw-rw-rw-   0        0        0     3521 2024-04-15 22:13:05.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc
--rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    11236 2024-04-15 22:13:05.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc
--rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/util.cpython-310.pyc
--rw-rw-rw-   0        0        0     8043 2024-04-15 22:36:04.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/util.cpython-311.pyc
--rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    25204 2024-04-16 04:56:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0    10272 2024-04-15 21:47:02.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/export_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/
--rw-rw-rw-   0        0        0      844 2024-04-07 19:31:03.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/database_delete.html
--rw-rw-rw-   0        0        0     1716 2024-04-08 05:56:48.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/export.html
--rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/export_csv.html
--rw-rw-rw-   0        0        0      877 2024-04-08 06:24:14.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/login_admin.html
--rw-rw-rw-   0        0        0     2490 2024-04-08 04:55:02.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/preview_questionnaire.html
--rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/preview_questionnaire_simple.html
--rw-rw-rw-   0        0        0      606 2024-04-08 05:52:37.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress.html
--rw-rw-rw-   0        0        0     2369 2024-04-08 05:37:40.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress_ajax.html
--rw-rw-rw-   0        0        0     3196 2024-04-07 19:09:11.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress_summary_ajax.html
--rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/questionnaire_results.html
--rw-rw-rw-   0        0        0     1388 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/results.html
--rw-rw-rw-   0        0        0     1366 2024-04-07 05:58:54.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/table_ajax.html
--rw-rw-rw-   0        0        0     1056 2024-04-07 18:32:29.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/table_view.html
--rw-rw-rw-   0        0        0     5018 2024-04-07 19:06:30.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/template_admin.html
--rw-rw-rw-   0        0        0     1056 2024-04-07 19:28:04.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/template_admin_head.html
--rw-rw-rw-   0        0        0     4427 2024-04-15 22:36:03.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/util.py
--rw-rw-rw-   0        0        0    16351 2024-04-16 04:56:38.000000 bride-of-frankensystem-1.9.3.5/BOFS/admin/views.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.5/BOFS/cli.py
--rw-rw-rw-   0        0        0     5177 2024-04-16 05:54:35.000000 bride-of-frankensystem-1.9.3.5/BOFS/create_app.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/
--rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/
--rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/models.cpython-310.pyc
--rw-rw-rw-   0        0        0    14931 2024-04-16 04:30:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/models.cpython-311.pyc
--rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    23422 2024-04-07 18:36:40.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0     9695 2024-04-16 04:16:03.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/models.py
--rw-rw-rw-   0        0        0    17838 2024-04-07 18:36:38.000000 bride-of-frankensystem-1.9.3.5/BOFS/default/views.py
--rw-rw-rw-   0        0        0     2105 2024-04-15 22:13:58.000000 bride-of-frankensystem-1.9.3.5/BOFS/globals.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/
--rw-rw-rw-   0        0        0   103009 2024-04-06 05:46:45.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/all.min.css
--rw-rw-rw-   0        0        0   232803 2024-04-06 05:38:05.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/img/
--rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/img/check.png
--rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/img/spinner32.gif
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/js/
--rw-rw-rw-   0        0        0    80721 2024-04-06 05:35:59.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48036 2024-04-06 05:47:33.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/js/htmx.min.js
--rw-rw-rw-   0        0        0    87533 2024-04-06 05:34:06.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/js/jquery-3.7.1.min.js
--rw-rw-rw-   0        0        0      360 2024-04-06 05:47:54.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/js/json-enc.js
--rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/loading.gif
--rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/logo.png
--rw-rw-rw-   0        0        0     2958 2024-04-07 19:19:18.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/style.css
--rw-rw-rw-   0        0        0     2060 2024-04-16 05:00:17.000000 bride-of-frankensystem-1.9.3.5/BOFS/static/style_admin.css
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/
--rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/consent.html
--rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/end.html
--rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/external_id.html
--rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/instructions.html
--rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questionnaire.html
--rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questionnaire_macro.html
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/
--rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/checklist.html
--rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/drop_down.html
--rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/field.html
--rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/multi_field.html
--rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/num_field.html
--rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/radiogrid.html
--rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/radiolist.html
--rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/slider.html
--rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/textview.html
--rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/simple.html
--rw-rw-rw-   0        0        0     5646 2024-04-07 06:04:14.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/template.html
--rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/unity_webgl.html
--rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.5/BOFS/templates/unity_webgl_fullscreen.html
--rw-rw-rw-   0        0        0    12080 2024-04-16 04:19:29.000000 bride-of-frankensystem-1.9.3.5/BOFS/util.py
--rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.5/LICENSE
--rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-1.9.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12537 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3853 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       99 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-16 06:21:26.000000 bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1042 2024-04-15 23:05:24.000000 bride-of-frankensystem-1.9.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 06:21:27.000000 bride-of-frankensystem-1.9.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/
+-rw-rw-rw-   0        0        0    15040 2024-04-17 22:32:56.000000 bride-of-frankensystem-1.9.3.6/BOFS/BOFSFlask.py
+-rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/BOFSSession.py
+-rw-rw-rw-   0        0        0    11113 2024-04-17 06:38:07.000000 bride-of-frankensystem-1.9.3.6/BOFS/JSONQuestionnaire.py
+-rw-rw-rw-   0        0        0     6858 2024-04-17 02:53:52.000000 bride-of-frankensystem-1.9.3.6/BOFS/JSONTable.py
+-rw-rw-rw-   0        0        0     5672 2024-04-15 21:33:28.000000 bride-of-frankensystem-1.9.3.6/BOFS/PageList.py
+-rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/
+-rw-rw-rw-   0        0        0    20215 2024-04-17 22:47:04.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/BOFSFlask.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5318 2024-04-05 21:05:43.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/BOFSSession.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16496 2024-04-17 06:38:19.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9903 2024-04-17 04:31:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/JSONTable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6901 2024-04-15 22:13:05.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/PageList.cpython-311.pyc
+-rw-rw-rw-   0        0        0      384 2024-04-05 21:05:42.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      337 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/__main__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1998 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/cli.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6150 2024-04-17 21:53:01.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/create_app.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3017 2024-04-15 22:14:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/globals.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17284 2024-04-16 04:26:24.000000 bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/util.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/
+-rw-rw-rw-   0        0        0    11884 2024-04-17 23:36:43.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/Results.py
+-rw-rw-rw-   0        0        0      883 2024-04-17 19:42:01.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/SummaryStats.py
+-rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/
+-rw-rw-rw-   0        0        0    13618 2024-04-17 23:24:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/Results.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2059 2024-04-17 19:44:37.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc
+-rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8043 2024-04-15 22:36:04.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/util.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    27833 2024-04-17 23:35:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/views.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/
+-rw-rw-rw-   0        0        0      844 2024-04-07 19:31:03.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/database_delete.html
+-rw-rw-rw-   0        0        0     1648 2024-04-17 06:00:53.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/export.html
+-rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/export_csv.html
+-rw-rw-rw-   0        0        0      877 2024-04-08 06:24:14.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/login_admin.html
+-rw-rw-rw-   0        0        0     2490 2024-04-08 04:55:02.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/preview_questionnaire.html
+-rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/preview_questionnaire_simple.html
+-rw-rw-rw-   0        0        0      606 2024-04-08 05:52:37.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress.html
+-rw-rw-rw-   0        0        0     2369 2024-04-08 05:37:40.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress_ajax.html
+-rw-rw-rw-   0        0        0     3196 2024-04-07 19:09:11.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress_summary_ajax.html
+-rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/questionnaire_results.html
+-rw-rw-rw-   0        0        0     2020 2024-04-17 23:32:30.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/results.html
+-rw-rw-rw-   0        0        0      572 2024-04-17 23:31:16.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/results_boxplot.html
+-rw-rw-rw-   0        0        0     1366 2024-04-07 05:58:54.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/table_ajax.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 18:32:29.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/table_view.html
+-rw-rw-rw-   0        0        0     5199 2024-04-17 20:52:51.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/template_admin.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 19:28:04.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/template_admin_head.html
+-rw-rw-rw-   0        0        0     4427 2024-04-15 22:36:03.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/util.py
+-rw-rw-rw-   0        0        0    17920 2024-04-17 23:35:11.000000 bride-of-frankensystem-1.9.3.6/BOFS/admin/views.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.6/BOFS/cli.py
+-rw-rw-rw-   0        0        0     5299 2024-04-17 23:43:06.000000 bride-of-frankensystem-1.9.3.6/BOFS/create_app.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/
+-rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/
+-rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/models.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15144 2024-04-17 04:31:32.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    23768 2024-04-16 20:43:42.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9769 2024-04-17 23:42:26.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/models.py
+-rw-rw-rw-   0        0        0    18057 2024-04-16 20:43:36.000000 bride-of-frankensystem-1.9.3.6/BOFS/default/views.py
+-rw-rw-rw-   0        0        0     2105 2024-04-15 22:13:58.000000 bride-of-frankensystem-1.9.3.6/BOFS/globals.py
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/
+-rw-rw-rw-   0        0        0   103009 2024-04-06 05:46:45.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/all.min.css
+-rw-rw-rw-   0        0        0   232803 2024-04-06 05:38:05.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/img/
+-rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/img/check.png
+-rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/img/spinner32.gif
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/js/
+-rw-rw-rw-   0        0        0    80721 2024-04-06 05:35:59.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48036 2024-04-06 05:47:33.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/js/htmx.min.js
+-rw-rw-rw-   0        0        0    87533 2024-04-06 05:34:06.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/js/jquery-3.7.1.min.js
+-rw-rw-rw-   0        0        0      360 2024-04-06 05:47:54.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/js/json-enc.js
+-rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/loading.gif
+-rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/logo.png
+-rw-rw-rw-   0        0        0     2958 2024-04-07 19:19:18.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/style.css
+-rw-rw-rw-   0        0        0     2060 2024-04-16 05:00:17.000000 bride-of-frankensystem-1.9.3.6/BOFS/static/style_admin.css
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/
+-rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/consent.html
+-rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/end.html
+-rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/external_id.html
+-rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/instructions.html
+-rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questionnaire.html
+-rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questionnaire_macro.html
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/
+-rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/checklist.html
+-rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/drop_down.html
+-rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/field.html
+-rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/multi_field.html
+-rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/num_field.html
+-rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/radiogrid.html
+-rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/radiolist.html
+-rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/slider.html
+-rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/textview.html
+-rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/simple.html
+-rw-rw-rw-   0        0        0     5646 2024-04-07 06:04:14.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/template.html
+-rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/unity_webgl.html
+-rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.6/BOFS/templates/unity_webgl_fullscreen.html
+-rw-rw-rw-   0        0        0    12080 2024-04-16 04:19:29.000000 bride-of-frankensystem-1.9.3.6/BOFS/util.py
+-rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.6/LICENSE
+-rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-1.9.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12537 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12537 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2024-04-17 23:48:06.000000 bride-of-frankensystem-1.9.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 23:48:27.000000 bride-of-frankensystem-1.9.3.6/setup.cfg
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/BOFSFlask.py` & `bride-of-frankensystem-1.9.3.6/BOFS/BOFSFlask.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             print(" Do not use this as a production web server. ")
             print("!!!!!!!!!!!!!!!!!!!!!!! WARNING !!!!!!!!!!!!!!!!!!!!!!!!")
             print('\033[0m')  # End the red
 
             if not self.run_with_reloader_off:
                 print('Auto-reloading of project when changes are detected is turned ON.')
 
-            super(BOFSFlask, self).run(host, port, use_reloader=not self.run_with_reloader_off, **options)
+            super(BOFSFlask, self).run(host, port, debug=True, use_reloader=not self.run_with_reloader_off, **options)
         else:
             self.eventlet_run(self, host=host, port=port, **options)
 
     # This method is straight from Flask-SocketIO
     # (https://github.com/miguelgrinberg/Flask-SocketIO/blob/master/flask_socketio/__init__.py)
     # MIT License, Copyright holder Miguel Grinberg
     def eventlet_run(self, app, host=None, port=None, **kwargs) -> None:
@@ -310,19 +310,20 @@
         return "<h1>File not Found (404)</h1>" \
                "<p>Could not load the requested page. If you are just starting out, " \
                "please click <a href=\"/restart\"><b>here</b></a> to reset your cookies for this page. " \
                "If that doesn't work, please clear your cookies or switch web browsers.", 404
 
     def internal_error(self, error):
         if not self.run_with_debugging:
+            log_path = os.path.join(self.root_path, 'error.log')
             open_mode = 'a'
-            if os.path.exists('error.log'):
+            if not os.path.exists(log_path):
                 open_mode = 'w'
 
-            with open('error.log', open_mode) as f:
+            with open(log_path, open_mode) as f:
                 f.write(f"{datetime.now()} - {error}\n")
 
         return f"<h1>Internal Server Error (500)</h1> <p>{error.description}</p><pre>{error.original_exception}</pre>", 500
 
     def inject_jinja_vars(self) -> dict:
         """
         Allows all templates to access several variables/methods used within BOFS.
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/BOFSSession.py` & `bride-of-frankensystem-1.9.3.6/BOFS/BOFSSession.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/JSONQuestionnaire.py` & `bride-of-frankensystem-1.9.3.6/BOFS/JSONQuestionnaire.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import json
 import re
 import pprint
 from flask import current_app, request, session, config
 from datetime import datetime
 from .globals import db
+from BOFS.util import mean, stdev, std, var, variance, median
 
 
 class JSONQuestionnaireColumn(object):
     def __init__(self, definition: dict, question_type: str | None = None):
         self.id = definition['id']
         self.data_type = "string"
         self.default = ""
@@ -82,26 +83,24 @@
         if not self.json_data or 'questions' not in self.json_data:
             print ("ERROR! `%s` questionnaire contains no questions." % self.file_name)
             return
 
         #print "fetchFields() for " + self.fileName
 
         for q in self.json_data['questions']:
-            if not 'id' in list(q.keys()):
-                continue
-
             # Build up the fields list based on the questionnaire
             if 'q_text' in q and 'questions' not in q:
                 q['questions'] = q['q_text']
 
             if 'questions' in q:
                 question_type = q['questiontype']
                 for qt in q['questions']:
                     if 'id' in qt:
                         self.__fields.append(JSONQuestionnaireColumn(qt, question_type))
+
             if 'id' in q:
                 self.__fields.append(JSONQuestionnaireColumn(q))
 
         self.__field_count = len(self.__fields)
         return self.__fields
 
     def create_db_class(self):
@@ -109,15 +108,15 @@
 
         if not self.__fields:  # If list is empty
             self.fetch_fields()
 
         if not self.__calc_fields:
             self.__calc_fields = []
 
-        table_name = str.format(u"questionnaire_{}", self.file_name)
+        table_name = f"questionnaire_{self.file_name}"
 
         table_attr = {
             '__tablename__': table_name,
             str.format(u'{0}ID', self.file_name): db.Column(db.Integer, primary_key=True, autoincrement=True),
             'participantID': db.Column(db.Integer, db.ForeignKey("participant.participantID"), nullable=False),
             #'participantID': db.Column(db.Integer),
             'participant': db.relationship("Participant", backref=table_name),
@@ -159,15 +158,15 @@
 
     def create_blank(self):
         blank = self.db_class()
 
         for column in blank.__table__.c:
             if column.default:
                 setattr(blank, column.name, column.default.arg)
-            if column.data_type == db.DateTime:
+            if column.type == db.DateTime:
                 setattr(blank, column.name, datetime.min)
 
         return blank
 
     def handle_questionnaire(self, tag=""):
         # Check to see if the user has submitted this once already...
         previous = db.session.query(self.db_class).filter(
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/JSONTable.py` & `bride-of-frankensystem-1.9.3.6/BOFS/JSONTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,21 @@
 
         self.db_class = None
 
     def get_columns(self) -> list["JSONTableColumn"]:
         return self.__columns
 
     def create_db_class(self):
-        table_name = self.file_name
+        table_name = "table_" + self.file_name
 
         table_attr = {
             '__tablename__': table_name,
             str.format(u'{0}ID', self.file_name): db.Column(db.Integer, primary_key=True, autoincrement=True),
             'participantID': db.Column(db.Integer, db.ForeignKey("participant.participantID"), nullable=False),
+            'participant': db.relationship("Participant", backref=table_name),
             'timeSubmitted': db.Column(db.DateTime, nullable=False, default=datetime.utcnow)
         }
 
         for column in self.json_data['columns']:
             column_details = self.json_data['columns'][column]
             new_column = JSONTableColumn(column, column_details)
             self.__columns.append(new_column)
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/PageList.py` & `bride-of-frankensystem-1.9.3.6/BOFS/PageList.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/BOFSFlask.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/BOFSFlask.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb9a11d66 (Mon Apr 15 21:52:57 2024 UTC)
-files sz: 14964
+moddate:  0x184e2066 (Wed Apr 17 22:32:56 2024 UTC)
+files sz: 15040
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d005a000100640064026c016d025a020100640064
@@ -305,23 +305,23 @@
                      280 MAKE_FUNCTION            4 (annotations)
                      282 STORE_NAME              28 (page_not_found)
          
          315         284 LOAD_CONST              27 (<code object internal_error, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\BOFSFlask.py", line 315>)
                      286 MAKE_FUNCTION            0
                      288 STORE_NAME              29 (internal_error)
          
-         326         290 LOAD_CONST               4 ('return')
+         327         290 LOAD_CONST               4 ('return')
                      292 LOAD_NAME               13 (dict)
                      294 BUILD_TUPLE              2
-                     296 LOAD_CONST              28 (<code object inject_jinja_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\BOFSFlask.py", line 326>)
+                     296 LOAD_CONST              28 (<code object inject_jinja_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\BOFSFlask.py", line 327>)
                      298 MAKE_FUNCTION            4 (annotations)
                      300 STORE_NAME              30 (inject_jinja_vars)
          
-         340         302 LOAD_CONST              32 (('return', None))
-                     304 LOAD_CONST              29 (<code object before_request_, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\BOFSFlask.py", line 340>)
+         341         302 LOAD_CONST              32 (('return', None))
+                     304 LOAD_CONST              29 (<code object before_request_, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\BOFSFlask.py", line 341>)
                      306 MAKE_FUNCTION            4 (annotations)
                      308 STORE_NAME              31 (before_request_)
                      310 LOAD_CLOSURE             0 (__class__)
                      312 COPY                     1
                      314 STORE_NAME              32 (__classcell__)
                      316 RETURN_VALUE
          consts
@@ -677,27 +677,27 @@
                stacksize : 6
                flags     : 11
                code
                   0x950197007c0281027c026e0164017d047c0181027c016e0164027d0574
                   010000000000000000000064037c059b0064047c049b009d04a6010000ab
                   01000000000000000001007c0564026b0300000000721274010000000000
                   000000000064057c049b009d02a6010000ab01000000000000000001007c
-                  006a010000000000000000729c7401000000000000000000006406a60100
+                  006a010000000000000000729d7401000000000000000000006406a60100
                   00ab01000000000000000001007401000000000000000000006407a60100
                   00ab01000000000000000001007401000000000000000000006408a60100
                   00ab01000000000000000001007401000000000000000000006409a60100
                   00ab01000000000000000001007401000000000000000000006407a60100
                   00ab0100000000000000000100740100000000000000000000640aa60100
                   00ab01000000000000000001007c006a020000000000000000730f740100
                   000000000000000000640ba6010000ab0100000000000000000100020074
                   07000000000000000000007408000000000000000000007c00a6020000ab
                   0200000000000000006a0500000000000000007c017c026602640c7c006a
-                  0200000000000000000c0069017c03a4018e0101006400530002007c006a
-                  0600000000000000007c0066017c017c02640d9c027c03a4018e01010064
-                  005300
+                  0200000000000000000c00640d9c027c03a4018e0101006400530002007c
+                  006a0600000000000000007c0066017c017c02640e9c027c03a4018e0101
+                  0064005300
                              0 COPY_FREE_VARS           1
                
                 81           2 RESUME                   0
                
                 82           4 LOAD_FAST                2 (port)
                              6 POP_JUMP_FORWARD_IF_NONE     2 (to 12)
                              8 LOAD_FAST                2 (port)
@@ -736,15 +736,15 @@
                            100 BUILD_STRING             2
                            102 PRECALL                  1
                            106 CALL                     1
                            116 POP_TOP
                
                 89     >>  118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                1 (run_with_debugging)
-                           130 POP_JUMP_FORWARD_IF_FALSE   156 (to 444)
+                           130 POP_JUMP_FORWARD_IF_FALSE   157 (to 446)
                
                 90         132 LOAD_GLOBAL              1 (NULL + print)
                            144 LOAD_CONST               6 ('\x1b[91m\x1b[1m')
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_TOP
                
@@ -794,66 +794,68 @@
                            382 LOAD_FAST                0 (self)
                            384 PRECALL                  2
                            388 CALL                     2
                            398 LOAD_ATTR                5 (run)
                            408 LOAD_FAST                1 (host)
                            410 LOAD_FAST                2 (port)
                            412 BUILD_TUPLE              2
-                           414 LOAD_CONST              12 ('use_reloader')
+                           414 LOAD_CONST              12 (True)
                            416 LOAD_FAST                0 (self)
                            418 LOAD_ATTR                2 (run_with_reloader_off)
                            428 UNARY_NOT
-                           430 BUILD_MAP                1
-                           432 LOAD_FAST                3 (options)
-                           434 DICT_MERGE               1
-                           436 CALL_FUNCTION_EX         1
-                           438 POP_TOP
-                           440 LOAD_CONST               0 (None)
-                           442 RETURN_VALUE
-               
-               102     >>  444 PUSH_NULL
-                           446 LOAD_FAST                0 (self)
-                           448 LOAD_ATTR                6 (eventlet_run)
-                           458 LOAD_FAST                0 (self)
-                           460 BUILD_TUPLE              1
-                           462 LOAD_FAST                1 (host)
-                           464 LOAD_FAST                2 (port)
-                           466 LOAD_CONST              13 (('host', 'port'))
-                           468 BUILD_CONST_KEY_MAP      2
-                           470 LOAD_FAST                3 (options)
-                           472 DICT_MERGE               1
-                           474 CALL_FUNCTION_EX         1
-                           476 POP_TOP
-                           478 LOAD_CONST               0 (None)
-                           480 RETURN_VALUE
+                           430 LOAD_CONST              13 (('debug', 'use_reloader'))
+                           432 BUILD_CONST_KEY_MAP      2
+                           434 LOAD_FAST                3 (options)
+                           436 DICT_MERGE               1
+                           438 CALL_FUNCTION_EX         1
+                           440 POP_TOP
+                           442 LOAD_CONST               0 (None)
+                           444 RETURN_VALUE
+               
+               102     >>  446 PUSH_NULL
+                           448 LOAD_FAST                0 (self)
+                           450 LOAD_ATTR                6 (eventlet_run)
+                           460 LOAD_FAST                0 (self)
+                           462 BUILD_TUPLE              1
+                           464 LOAD_FAST                1 (host)
+                           466 LOAD_FAST                2 (port)
+                           468 LOAD_CONST              14 (('host', 'port'))
+                           470 BUILD_CONST_KEY_MAP      2
+                           472 LOAD_FAST                3 (options)
+                           474 DICT_MERGE               1
+                           476 CALL_FUNCTION_EX         1
+                           478 POP_TOP
+                           480 LOAD_CONST               0 (None)
+                           482 RETURN_VALUE
                consts
                   None
                   5000
                   '127.0.0.1'
                   'Listening on http://'
                   ':'
                   'Preview locally at http://127.0.0.1:'
                   '\x1b[91m\x1b[1m'
                   '!!!!!!!!!!!!!!!!!!!!!!! WARNING !!!!!!!!!!!!!!!!!!!!!!!!'
                   ' Debugging mode is enabled. '
                   ' Do not use this as a production web server. '
                   '\x1b[0m'
                   'Auto-reloading of project when changes are detected is turned ON.'
-                  'use_reloader'
+                  True
+                  ('debug', 'use_reloader')
                   ('host', 'port')
                names      ('print', 'run_with_debugging', 'run_with_reloader_off', 'super', 'BOFSFlask', 'run', 'eventlet_run')
                varnames   ('self', 'host', 'port', 'options', 'actual_port', 'actual_host')
                freevars   ('__class__',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
                name       'run'
                firstlineno 81
                lnotab
                   0x04010c010c022a010c0124020e011e011e011e011e011e011e020e011e
-                  025802
+                  025a02
             code
                argcount  : 4
                nlocals   : 10
                stacksize : 5
                flags     : 11
                code
                   0x8704870a9700640164006c007d05640164006c017d057c056a02000000
@@ -2362,214 +2364,227 @@
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
                name       'page_not_found'
                firstlineno 309
                lnotab 0x0201
             code
                argcount  : 2
-               nlocals   : 4
+               nlocals   : 5
                stacksize : 7
                flags     : 3
                code
-                  0x97007c006a000000000000000000737764017d02740200000000000000
-                  0000006a020000000000000000a003000000000000000000000000000000
-                  00000000006402a6010000ab010000000000000000720264037d02740900
-                  00000000000000000064027c02a6020000ab02000000000000000035007d
-                  037c03a0050000000000000000000000000000000000000000740d000000
-                  000000000000006a070000000000000000a6000000ab0000000000000000
-                  009b0064047c019b0064059d04a6010000ab010000000000000000010064
-                  0064006400a6020000ab02000000000000000001006e0b23003100730477
-                  02780359007701010059000100010064067c016a0800000000000000009b
-                  0064077c016a0900000000000000009b0064089d05640966025300
+                  0x97007c006a000000000000000000739c7402000000000000000000006a
+                  020000000000000000a00300000000000000000000000000000000000000
+                  007c006a0400000000000000006401a6020000ab0200000000000000007d
+                  0264027d037402000000000000000000006a020000000000000000a00500
+                  000000000000000000000000000000000000007c02a6010000ab01000000
+                  0000000000730264037d03740d000000000000000000007c027c03a60200
+                  00ab02000000000000000035007d047c04a0070000000000000000000000
+                  0000000000000000007411000000000000000000006a0900000000000000
+                  00a6000000ab0000000000000000009b0064047c019b0064059d04a60100
+                  00ab0100000000000000000100640064006400a6020000ab020000000000
+                  00000001006e0b2300310073047702780359007701010059000100010064
+                  067c016a0a00000000000000009b0064077c016a0b00000000000000009b
+                  0064089d05640966025300
                315           0 RESUME                   0
                
                316           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (run_with_debugging)
-                            14 POP_JUMP_FORWARD_IF_TRUE   119 (to 254)
-               
-               317          16 LOAD_CONST               1 ('a')
-                            18 STORE_FAST               2 (open_mode)
+                            14 POP_JUMP_FORWARD_IF_TRUE   156 (to 328)
                
-               318          20 LOAD_GLOBAL              2 (os)
-                            32 LOAD_ATTR                2 (path)
-                            42 LOAD_METHOD              3 (exists)
-                            64 LOAD_CONST               2 ('error.log')
-                            66 PRECALL                  1
-                            70 CALL                     1
-                            80 POP_JUMP_FORWARD_IF_FALSE     2 (to 86)
-               
-               319          82 LOAD_CONST               3 ('w')
-                            84 STORE_FAST               2 (open_mode)
-               
-               321     >>   86 LOAD_GLOBAL              9 (NULL + open)
-                            98 LOAD_CONST               2 ('error.log')
-                           100 LOAD_FAST                2 (open_mode)
-                           102 PRECALL                  2
-                           106 CALL                     2
-                           116 BEFORE_WITH
-                           118 STORE_FAST               3 (f)
-               
-               322         120 LOAD_FAST                3 (f)
-                           122 LOAD_METHOD              5 (write)
-                           144 LOAD_GLOBAL             13 (NULL + datetime)
-                           156 LOAD_ATTR                7 (now)
-                           166 PRECALL                  0
-                           170 CALL                     0
-                           180 FORMAT_VALUE             0
-                           182 LOAD_CONST               4 (' - ')
-                           184 LOAD_FAST                1 (error)
-                           186 FORMAT_VALUE             0
-                           188 LOAD_CONST               5 ('\n')
-                           190 BUILD_STRING             4
-                           192 PRECALL                  1
-                           196 CALL                     1
-                           206 POP_TOP
-               
-               321         208 LOAD_CONST               0 (None)
-                           210 LOAD_CONST               0 (None)
-                           212 LOAD_CONST               0 (None)
-                           214 PRECALL                  2
-                           218 CALL                     2
-                           228 POP_TOP
-                           230 JUMP_FORWARD            11 (to 254)
-                       >>  232 PUSH_EXC_INFO
-                           234 WITH_EXCEPT_START
-                           236 POP_JUMP_FORWARD_IF_TRUE     4 (to 246)
-                           238 RERAISE                  2
-                       >>  240 COPY                     3
-                           242 POP_EXCEPT
-                           244 RERAISE                  1
-                       >>  246 POP_TOP
-                           248 POP_EXCEPT
-                           250 POP_TOP
-                           252 POP_TOP
+               317          16 LOAD_GLOBAL              2 (os)
+                            28 LOAD_ATTR                2 (path)
+                            38 LOAD_METHOD              3 (join)
+                            60 LOAD_FAST                0 (self)
+                            62 LOAD_ATTR                4 (root_path)
+                            72 LOAD_CONST               1 ('error.log')
+                            74 PRECALL                  2
+                            78 CALL                     2
+                            88 STORE_FAST               2 (log_path)
+               
+               318          90 LOAD_CONST               2 ('a')
+                            92 STORE_FAST               3 (open_mode)
+               
+               319          94 LOAD_GLOBAL              2 (os)
+                           106 LOAD_ATTR                2 (path)
+                           116 LOAD_METHOD              5 (exists)
+                           138 LOAD_FAST                2 (log_path)
+                           140 PRECALL                  1
+                           144 CALL                     1
+                           154 POP_JUMP_FORWARD_IF_TRUE     2 (to 160)
+               
+               320         156 LOAD_CONST               3 ('w')
+                           158 STORE_FAST               3 (open_mode)
+               
+               322     >>  160 LOAD_GLOBAL             13 (NULL + open)
+                           172 LOAD_FAST                2 (log_path)
+                           174 LOAD_FAST                3 (open_mode)
+                           176 PRECALL                  2
+                           180 CALL                     2
+                           190 BEFORE_WITH
+                           192 STORE_FAST               4 (f)
+               
+               323         194 LOAD_FAST                4 (f)
+                           196 LOAD_METHOD              7 (write)
+                           218 LOAD_GLOBAL             17 (NULL + datetime)
+                           230 LOAD_ATTR                9 (now)
+                           240 PRECALL                  0
+                           244 CALL                     0
+                           254 FORMAT_VALUE             0
+                           256 LOAD_CONST               4 (' - ')
+                           258 LOAD_FAST                1 (error)
+                           260 FORMAT_VALUE             0
+                           262 LOAD_CONST               5 ('\n')
+                           264 BUILD_STRING             4
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 POP_TOP
                
-               324     >>  254 LOAD_CONST               6 ('<h1>Internal Server Error (500)</h1> <p>')
-                           256 LOAD_FAST                1 (error)
-                           258 LOAD_ATTR                8 (description)
-                           268 FORMAT_VALUE             0
-                           270 LOAD_CONST               7 ('</p><pre>')
-                           272 LOAD_FAST                1 (error)
-                           274 LOAD_ATTR                9 (original_exception)
-                           284 FORMAT_VALUE             0
-                           286 LOAD_CONST               8 ('</pre>')
-                           288 BUILD_STRING             5
-                           290 LOAD_CONST               9 (500)
-                           292 BUILD_TUPLE              2
-                           294 RETURN_VALUE
+               322         282 LOAD_CONST               0 (None)
+                           284 LOAD_CONST               0 (None)
+                           286 LOAD_CONST               0 (None)
+                           288 PRECALL                  2
+                           292 CALL                     2
+                           302 POP_TOP
+                           304 JUMP_FORWARD            11 (to 328)
+                       >>  306 PUSH_EXC_INFO
+                           308 WITH_EXCEPT_START
+                           310 POP_JUMP_FORWARD_IF_TRUE     4 (to 320)
+                           312 RERAISE                  2
+                       >>  314 COPY                     3
+                           316 POP_EXCEPT
+                           318 RERAISE                  1
+                       >>  320 POP_TOP
+                           322 POP_EXCEPT
+                           324 POP_TOP
+                           326 POP_TOP
+               
+               325     >>  328 LOAD_CONST               6 ('<h1>Internal Server Error (500)</h1> <p>')
+                           330 LOAD_FAST                1 (error)
+                           332 LOAD_ATTR               10 (description)
+                           342 FORMAT_VALUE             0
+                           344 LOAD_CONST               7 ('</p><pre>')
+                           346 LOAD_FAST                1 (error)
+                           348 LOAD_ATTR               11 (original_exception)
+                           358 FORMAT_VALUE             0
+                           360 LOAD_CONST               8 ('</pre>')
+                           362 BUILD_STRING             5
+                           364 LOAD_CONST               9 (500)
+                           366 BUILD_TUPLE              2
+                           368 RETURN_VALUE
                ExceptionTable:
-                 118 to 206 -> 232 [1] lasti
-                 232 to 238 -> 240 [3] lasti
-                 246 to 246 -> 240 [3] lasti
+                 192 to 280 -> 306 [1] lasti
+                 306 to 312 -> 314 [3] lasti
+                 320 to 320 -> 314 [3] lasti
                consts
                   None
-                  'a'
                   'error.log'
+                  'a'
                   'w'
                   ' - '
                   '\n'
                   '<h1>Internal Server Error (500)</h1> <p>'
                   '</p><pre>'
                   '</pre>'
                   500
-               names      ('run_with_debugging', 'os', 'path', 'exists', 'open', 'write', 'datetime', 'now', 'description', 'original_exception')
-               varnames   ('self', 'error', 'open_mode', 'f')
+               names      ('run_with_debugging', 'os', 'path', 'join', 'root_path', 'exists', 'open', 'write', 'datetime', 'now', 'description', 'original_exception')
+               varnames   ('self', 'error', 'log_path', 'open_mode', 'f')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
                name       'internal_error'
                firstlineno 315
-               lnotab 0x02010e0104013e010402220158ff2e03
+               lnotab 0x02010e014a0104013e010402220158ff2e03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007c006a0300000000000000007408000000000000000000006a0500
                   00000000000000740d000000000000000000006a070000000000000000a6
                   000000ab0000000000000000007410000000000000000000006a09000000
                   0000000000ac01a6050000ab0500000000000000007d017c015300
-               326           0 RESUME                   0
+               327           0 RESUME                   0
                
-               331           2 LOAD_GLOBAL              1 (NULL + dict)
+               332           2 LOAD_GLOBAL              1 (NULL + dict)
                
-               332          14 LOAD_FAST                0 (self)
+               333          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (page_list)
                             26 LOAD_METHOD              2 (flat_page_list)
                             48 PRECALL                  0
                             52 CALL                     0
                
-               333          62 LOAD_FAST                0 (self)
+               334          62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (run_with_debugging)
                
-               334          74 LOAD_GLOBAL              8 (random)
+               335          74 LOAD_GLOBAL              8 (random)
                             86 LOAD_ATTR                5 (shuffle)
                
-               335          96 LOAD_GLOBAL             13 (NULL + util)
+               336          96 LOAD_GLOBAL             13 (NULL + util)
                            108 LOAD_ATTR                7 (create_breadcrumbs)
                            118 PRECALL                  0
                            122 CALL                     0
                
-               336         132 LOAD_GLOBAL             16 (json)
+               337         132 LOAD_GLOBAL             16 (json)
                            144 LOAD_ATTR                9 (dumps)
                
-               331         154 KW_NAMES                 1
+               332         154 KW_NAMES                 1
                            156 PRECALL                  5
                            160 CALL                     5
                            170 STORE_FAST               1 (template_vars)
                
-               338         172 LOAD_FAST                1 (template_vars)
+               339         172 LOAD_FAST                1 (template_vars)
                            174 RETURN_VALUE
                consts
                   '\n        Allows all templates to access several variables/methods used within BOFS.\n        :return: a dictionary of variables/methods\n        '
                   ('flat_page_list', 'debug', 'shuffle', 'crumbs', 'json_dumps')
                names      ('dict', 'page_list', 'flat_page_list', 'run_with_debugging', 'random', 'shuffle', 'util', 'create_breadcrumbs', 'json', 'dumps')
                varnames   ('self', 'template_vars')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
                name       'inject_jinja_vars'
-               firstlineno 326
+               firstlineno 327
                lnotab 0x02050c0130010c011601240116fb1207
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000720e69007c006a0100000000000000
                   005f0200000000000000006401530064015300
-               340           0 RESUME                   0
+               341           0 RESUME                   0
                
-               344           2 LOAD_FAST                0 (self)
+               345           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (run_with_debugging)
                             14 POP_JUMP_FORWARD_IF_FALSE    14 (to 44)
                
-               345          16 BUILD_MAP                0
+               346          16 BUILD_MAP                0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (jinja_env)
                             30 STORE_ATTR               2 (cache)
                             40 LOAD_CONST               1 (None)
                             42 RETURN_VALUE
                
-               344     >>   44 LOAD_CONST               1 (None)
+               345     >>   44 LOAD_CONST               1 (None)
                             46 RETURN_VALUE
                consts
                   '\n        If running the server in debug mode, turn off Jinja caching.\n        '
                   None
                names      ('run_with_debugging', 'jinja_env', 'cache')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
                name       'before_request_'
-               firstlineno 340
+               firstlineno 341
                lnotab 0x02040e011cff
             (None, False, False)
             (None, None)
             ('return', None)
             (False,)
             (None, True)
             ('.json',)
@@ -2578,15 +2593,15 @@
          freevars   ()
          cellvars   ('__class__',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
          name       'BOFSFlask'
          firstlineno 18
          lnotab
             0x0c010c3e0e1a0a160a0a060b0a1c081a1a16321b08071c110c09080912
-            080c030c031c06060b0c0e
+            080c030c031c06060c0c0e
       'BOFSFlask'
    names      ('datetime', 'crawlerdetect', 'CrawlerDetect', 'jinja2', 'json', 'toml', 'os', 'random', 'flask', 'Flask', 'send_from_directory', 'Response', 'Blueprint', 'flask_sqlalchemy', 'SQLAlchemy', 'flask_compress', 'Compress', 'BOFS', 'util', 'BOFSSession', 'BOFSSessionInterface', 'JSONQuestionnaire', 'JSONTable', 'PageList', 'BOFSFlask')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\BOFSFlask.py'
    name       '<module>'
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/BOFSSession.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/BOFSSession.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x3dff1d66 (Tue Apr 16 04:31:57 2024 UTC)
-files sz: 11139
+moddate:  0x4f6e1f66 (Wed Apr 17 06:38:07 2024 UTC)
+files sz: 11113
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       016c035a03640064026c046d055a056d065a066d075a076d085a08010064
-      0064036c096d095a090100640464056c0a6d0b5a0b010002004700640684
-      006407650ca6030000ab0300000000000000005a0d020047006408840064
-      09650ca6030000ab0300000000000000005a0e64015300
+      0064036c096d095a090100640464056c0a6d0b5a0b0100640064066c0c6d
+      0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d125a1201000200470064
+      07840064086513a6030000ab0300000000000000005a1402004700640984
+      00640a6513a6030000ab0300000000000000005a1564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -57,73 +58,91 @@
      7          70 LOAD_CONST               4 (1)
                 72 LOAD_CONST               5 (('db',))
                 74 IMPORT_NAME             10 (globals)
                 76 IMPORT_FROM             11 (db)
                 78 STORE_NAME              11 (db)
                 80 POP_TOP
    
-    10          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               6 (<code object JSONQuestionnaireColumn, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 10>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               7 ('JSONQuestionnaireColumn')
-                92 LOAD_NAME               12 (object)
-                94 PRECALL                  3
-                98 CALL                     3
-               108 STORE_NAME              13 (JSONQuestionnaireColumn)
+     8          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               6 (('mean', 'stdev', 'std', 'var', 'variance', 'median'))
+                86 IMPORT_NAME             12 (BOFS.util)
+                88 IMPORT_FROM             13 (mean)
+                90 STORE_NAME              13 (mean)
+                92 IMPORT_FROM             14 (stdev)
+                94 STORE_NAME              14 (stdev)
+                96 IMPORT_FROM             15 (std)
+                98 STORE_NAME              15 (std)
+               100 IMPORT_FROM             16 (var)
+               102 STORE_NAME              16 (var)
+               104 IMPORT_FROM             17 (variance)
+               106 STORE_NAME              17 (variance)
+               108 IMPORT_FROM             18 (median)
+               110 STORE_NAME              18 (median)
+               112 POP_TOP
    
-    55         110 PUSH_NULL
-               112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               8 (<code object JSONQuestionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 55>)
-               116 MAKE_FUNCTION            0
-               118 LOAD_CONST               9 ('JSONQuestionnaire')
-               120 LOAD_NAME               12 (object)
-               122 PRECALL                  3
-               126 CALL                     3
-               136 STORE_NAME              14 (JSONQuestionnaire)
-               138 LOAD_CONST               1 (None)
-               140 RETURN_VALUE
+    11         114 PUSH_NULL
+               116 LOAD_BUILD_CLASS
+               118 LOAD_CONST               7 (<code object JSONQuestionnaireColumn, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 11>)
+               120 MAKE_FUNCTION            0
+               122 LOAD_CONST               8 ('JSONQuestionnaireColumn')
+               124 LOAD_NAME               19 (object)
+               126 PRECALL                  3
+               130 CALL                     3
+               140 STORE_NAME              20 (JSONQuestionnaireColumn)
+   
+    56         142 PUSH_NULL
+               144 LOAD_BUILD_CLASS
+               146 LOAD_CONST               9 (<code object JSONQuestionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 56>)
+               148 MAKE_FUNCTION            0
+               150 LOAD_CONST              10 ('JSONQuestionnaire')
+               152 LOAD_NAME               19 (object)
+               154 PRECALL                  3
+               158 CALL                     3
+               168 STORE_NAME              21 (JSONQuestionnaire)
+               170 LOAD_CONST               1 (None)
+               172 RETURN_VALUE
    consts
       0
       None
       ('current_app', 'request', 'session', 'config')
       ('datetime',)
       1
       ('db',)
+      ('mean', 'stdev', 'std', 'var', 'variance', 'median')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026407640265036403650464017a070000660464
             0484055a05640584005a06640684005a0764015300
-          10           0 RESUME                   0
+          11           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('JSONQuestionnaireColumn')
                        8 STORE_NAME               2 (__qualname__)
          
-          11          10 LOAD_CONST               7 ((None,))
+          12          10 LOAD_CONST               7 ((None,))
                       12 LOAD_CONST               2 ('definition')
                       14 LOAD_NAME                3 (dict)
                       16 LOAD_CONST               3 ('question_type')
                       18 LOAD_NAME                4 (str)
                       20 LOAD_CONST               1 (None)
                       22 BINARY_OP                7 (|)
                       26 BUILD_TUPLE              4
-                      28 LOAD_CONST               4 (<code object __init__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 11>)
+                      28 LOAD_CONST               4 (<code object __init__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 12>)
                       30 MAKE_FUNCTION            5 (defaults, annotations)
                       32 STORE_NAME               5 (__init__)
          
-          30          34 LOAD_CONST               5 (<code object get_type_ddl, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 30>)
+          31          34 LOAD_CONST               5 (<code object get_type_ddl, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 31>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (get_type_ddl)
          
-          42          40 LOAD_CONST               6 (<code object generate_db_column, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 42>)
+          43          40 LOAD_CONST               6 (<code object generate_db_column, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 43>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (generate_db_column)
                       46 LOAD_CONST               1 (None)
                       48 RETURN_VALUE
          consts
             'JSONQuestionnaireColumn'
             None
@@ -139,82 +158,82 @@
                   027c005f01000000000000000064037c005f0200000000000000007c0280
                   0d64047c01760072097c016404190000000000000000007d026e0264027d
                   027c02a0030000000000000000000000000000000000000000a6000000ab
                   00000000000000000064057600720764067c005f01000000000000000064
                   077c017600720d7c016407190000000000000000007c005f010000000000
                   0000007c006a01000000000000000064087600720964097c005f02000000
                   00000000006400530064005300
-                11           0 RESUME                   0
+                12           0 RESUME                   0
                
-                12           2 LOAD_FAST                1 (definition)
+                13           2 LOAD_FAST                1 (definition)
                              4 LOAD_CONST               1 ('id')
                              6 BINARY_SUBSCR
                             16 LOAD_FAST                0 (self)
                             18 STORE_ATTR               0 (id)
                
-                13          28 LOAD_CONST               2 ('string')
+                14          28 LOAD_CONST               2 ('string')
                             30 LOAD_FAST                0 (self)
                             32 STORE_ATTR               1 (data_type)
                
-                14          42 LOAD_CONST               3 ('')
+                15          42 LOAD_CONST               3 ('')
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               2 (default)
                
-                16          56 LOAD_FAST                2 (question_type)
+                17          56 LOAD_FAST                2 (question_type)
                             58 POP_JUMP_FORWARD_IF_NOT_NONE    13 (to 86)
                             60 LOAD_CONST               4 ('questiontype')
                             62 LOAD_FAST                1 (definition)
                             64 CONTAINS_OP              0
                             66 POP_JUMP_FORWARD_IF_FALSE     9 (to 86)
                
-                17          68 LOAD_FAST                1 (definition)
+                18          68 LOAD_FAST                1 (definition)
                             70 LOAD_CONST               4 ('questiontype')
                             72 BINARY_SUBSCR
                             82 STORE_FAST               2 (question_type)
                             84 JUMP_FORWARD             2 (to 90)
                
-                19     >>   86 LOAD_CONST               2 ('string')
+                20     >>   86 LOAD_CONST               2 ('string')
                             88 STORE_FAST               2 (question_type)
                
-                21     >>   90 LOAD_FAST                2 (question_type)
+                22     >>   90 LOAD_FAST                2 (question_type)
                             92 LOAD_METHOD              3 (lower)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 LOAD_CONST               5 (('slider', 'num_field'))
                            130 CONTAINS_OP              0
                            132 POP_JUMP_FORWARD_IF_FALSE     7 (to 148)
                
-                22         134 LOAD_CONST               6 ('integer')
+                23         134 LOAD_CONST               6 ('integer')
                            136 LOAD_FAST                0 (self)
                            138 STORE_ATTR               1 (data_type)
                
-                24     >>  148 LOAD_CONST               7 ('datatype')
+                25     >>  148 LOAD_CONST               7 ('datatype')
                            150 LOAD_FAST                1 (definition)
                            152 CONTAINS_OP              0
                            154 POP_JUMP_FORWARD_IF_FALSE    13 (to 182)
                
-                25         156 LOAD_FAST                1 (definition)
+                26         156 LOAD_FAST                1 (definition)
                            158 LOAD_CONST               7 ('datatype')
                            160 BINARY_SUBSCR
                            170 LOAD_FAST                0 (self)
                            172 STORE_ATTR               1 (data_type)
                
-                27     >>  182 LOAD_FAST                0 (self)
+                28     >>  182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                1 (data_type)
                            194 LOAD_CONST               8 (('integer', 'float'))
                            196 CONTAINS_OP              0
                            198 POP_JUMP_FORWARD_IF_FALSE     9 (to 218)
                
-                28         200 LOAD_CONST               9 (0)
+                29         200 LOAD_CONST               9 (0)
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               2 (default)
                            214 LOAD_CONST               0 (None)
                            216 RETURN_VALUE
                
-                27     >>  218 LOAD_CONST               0 (None)
+                28     >>  218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                consts
                   None
                   'id'
                   'string'
                   ''
                   'questiontype'
@@ -225,65 +244,65 @@
                   0
                names      ('id', 'data_type', 'default', 'lower')
                varnames   ('self', 'definition', 'question_type')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       '__init__'
-               firstlineno 11
+               firstlineno 12
                lnotab 0x02011a010e010e020c01120204022c010e0208011a02120112ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b02000000007202640253007c
                   006a00000000000000000064036b02000000007202640453007c006a0000
                   0000000000000064056b02000000007202640653007c006a000000000000
                   00000064076b020000000072026408530064095300
-                30           0 RESUME                   0
+                31           0 RESUME                   0
                
-                31           2 LOAD_FAST                0 (self)
+                32           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (data_type)
                             14 LOAD_CONST               1 ('integer')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-                32          24 LOAD_CONST               2 ('INTEGER')
+                33          24 LOAD_CONST               2 ('INTEGER')
                             26 RETURN_VALUE
                
-                33     >>   28 LOAD_FAST                0 (self)
+                34     >>   28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (data_type)
                             40 LOAD_CONST               3 ('float')
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-                34          50 LOAD_CONST               4 ('NUMERIC')
+                35          50 LOAD_CONST               4 ('NUMERIC')
                             52 RETURN_VALUE
                
-                35     >>   54 LOAD_FAST                0 (self)
+                36     >>   54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (data_type)
                             66 LOAD_CONST               5 ('datetime')
                             68 COMPARE_OP               2 (==)
                             74 POP_JUMP_FORWARD_IF_FALSE     2 (to 80)
                
-                36          76 LOAD_CONST               6 ('DATETIME')
+                37          76 LOAD_CONST               6 ('DATETIME')
                             78 RETURN_VALUE
                
-                37     >>   80 LOAD_FAST                0 (self)
+                38     >>   80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                0 (data_type)
                             92 LOAD_CONST               7 ('boolean')
                             94 COMPARE_OP               2 (==)
                            100 POP_JUMP_FORWARD_IF_FALSE     2 (to 106)
                
-                38         102 LOAD_CONST               8 ('BOOLEAN')
+                39         102 LOAD_CONST               8 ('BOOLEAN')
                            104 RETURN_VALUE
                
-                40     >>  106 LOAD_CONST               9 ('TEXT')
+                41     >>  106 LOAD_CONST               9 ('TEXT')
                            108 RETURN_VALUE
                consts
                   None
                   'integer'
                   'INTEGER'
                   'float'
                   'NUMERIC'
@@ -294,15 +313,15 @@
                   'TEXT'
                names      ('data_type',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'get_type_ddl'
-               firstlineno 30
+               firstlineno 31
                lnotab 0x020116010401160104011601040116010402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
@@ -318,89 +337,89 @@
                   040000000000000000ac03a6030000ab03000000000000000053007c006a
                   00000000000000000064066b020000000072267403000000000000000000
                   006a0200000000000000007402000000000000000000006a070000000000
                   00000064027c006a040000000000000000ac03a6030000ab030000000000
                   00000053007403000000000000000000006a020000000000000000740200
                   0000000000000000006a08000000000000000064027c006a040000000000
                   000000ac03a6030000ab0300000000000000005300
-                42           0 RESUME                   0
+                43           0 RESUME                   0
                
-                43           2 LOAD_FAST                0 (self)
+                44           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (data_type)
                             14 LOAD_CONST               1 ('integer')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE    38 (to 100)
                
-                44          24 LOAD_GLOBAL              3 (NULL + db)
+                45          24 LOAD_GLOBAL              3 (NULL + db)
                             36 LOAD_ATTR                2 (Column)
                             46 LOAD_GLOBAL              2 (db)
                             58 LOAD_ATTR                3 (Integer)
                             68 LOAD_CONST               2 (False)
                             70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                4 (default)
                             82 KW_NAMES                 3
                             84 PRECALL                  3
                             88 CALL                     3
                             98 RETURN_VALUE
                
-                45     >>  100 LOAD_FAST                0 (self)
+                46     >>  100 LOAD_FAST                0 (self)
                            102 LOAD_ATTR                0 (data_type)
                            112 LOAD_CONST               4 ('float')
                            114 COMPARE_OP               2 (==)
                            120 POP_JUMP_FORWARD_IF_FALSE    38 (to 198)
                
-                46         122 LOAD_GLOBAL              3 (NULL + db)
+                47         122 LOAD_GLOBAL              3 (NULL + db)
                            134 LOAD_ATTR                2 (Column)
                            144 LOAD_GLOBAL              2 (db)
                            156 LOAD_ATTR                5 (Float)
                            166 LOAD_CONST               2 (False)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                4 (default)
                            180 KW_NAMES                 3
                            182 PRECALL                  3
                            186 CALL                     3
                            196 RETURN_VALUE
                
-                47     >>  198 LOAD_FAST                0 (self)
+                48     >>  198 LOAD_FAST                0 (self)
                            200 LOAD_ATTR                0 (data_type)
                            210 LOAD_CONST               5 ('datetime')
                            212 COMPARE_OP               2 (==)
                            218 POP_JUMP_FORWARD_IF_FALSE    38 (to 296)
                
-                48         220 LOAD_GLOBAL              3 (NULL + db)
+                49         220 LOAD_GLOBAL              3 (NULL + db)
                            232 LOAD_ATTR                2 (Column)
                            242 LOAD_GLOBAL              2 (db)
                            254 LOAD_ATTR                6 (DateTime)
                            264 LOAD_CONST               2 (False)
                            266 LOAD_FAST                0 (self)
                            268 LOAD_ATTR                4 (default)
                            278 KW_NAMES                 3
                            280 PRECALL                  3
                            284 CALL                     3
                            294 RETURN_VALUE
                
-                49     >>  296 LOAD_FAST                0 (self)
+                50     >>  296 LOAD_FAST                0 (self)
                            298 LOAD_ATTR                0 (data_type)
                            308 LOAD_CONST               6 ('boolean')
                            310 COMPARE_OP               2 (==)
                            316 POP_JUMP_FORWARD_IF_FALSE    38 (to 394)
                
-                50         318 LOAD_GLOBAL              3 (NULL + db)
+                51         318 LOAD_GLOBAL              3 (NULL + db)
                            330 LOAD_ATTR                2 (Column)
                            340 LOAD_GLOBAL              2 (db)
                            352 LOAD_ATTR                7 (Boolean)
                            362 LOAD_CONST               2 (False)
                            364 LOAD_FAST                0 (self)
                            366 LOAD_ATTR                4 (default)
                            376 KW_NAMES                 3
                            378 PRECALL                  3
                            382 CALL                     3
                            392 RETURN_VALUE
                
-                52     >>  394 LOAD_GLOBAL              3 (NULL + db)
+                53     >>  394 LOAD_GLOBAL              3 (NULL + db)
                            406 LOAD_ATTR                2 (Column)
                            416 LOAD_GLOBAL              2 (db)
                            428 LOAD_ATTR                8 (Text)
                            438 LOAD_CONST               2 (False)
                            440 LOAD_FAST                0 (self)
                            442 LOAD_ATTR                4 (default)
                            452 KW_NAMES                 3
@@ -417,105 +436,105 @@
                   'boolean'
                names      ('data_type', 'db', 'Column', 'Integer', 'default', 'Float', 'DateTime', 'Boolean', 'Text')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'generate_db_column'
-               firstlineno 42
+               firstlineno 43
                lnotab 0x020116014c0116014c0116014c0116014c02
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'dict', 'str', '__init__', 'get_type_ddl', 'generate_db_column')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
          name       'JSONQuestionnaireColumn'
-         firstlineno 10
+         firstlineno 11
          lnotab 0x0a011813060c
       'JSONQuestionnaireColumn'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0264016503640265036604640384045a04640484
             005a05640565066503190000000000000000006602640684045a07640565
             066407190000000000000000006602640884045a08640984005a09640a84
             005a0a640b84005a0b6415640d84015a0c640e84005a0d640f84005a0e64
             1084005a0f6416641384015a1064145300
-          55           0 RESUME                   0
+          56           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('JSONQuestionnaire')
                        8 STORE_NAME               2 (__qualname__)
          
-          56          10 LOAD_CONST               1 ('directory')
+          57          10 LOAD_CONST               1 ('directory')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('file_name')
                       16 LOAD_NAME                3 (str)
                       18 BUILD_TUPLE              4
-                      20 LOAD_CONST               3 (<code object __init__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 56>)
+                      20 LOAD_CONST               3 (<code object __init__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 57>)
                       22 MAKE_FUNCTION            4 (annotations)
                       24 STORE_NAME               4 (__init__)
          
-          73          26 LOAD_CONST               4 (<code object get_table_name, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 73>)
+          74          26 LOAD_CONST               4 (<code object get_table_name, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 74>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (get_table_name)
          
-          76          32 LOAD_CONST               5 ('return')
+          77          32 LOAD_CONST               5 ('return')
                       34 LOAD_NAME                6 (list)
                       36 LOAD_NAME                3 (str)
                       38 BINARY_SUBSCR
                       48 BUILD_TUPLE              2
-                      50 LOAD_CONST               6 (<code object get_calculated_fields, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 76>)
+                      50 LOAD_CONST               6 (<code object get_calculated_fields, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 77>)
                       52 MAKE_FUNCTION            4 (annotations)
                       54 STORE_NAME               7 (get_calculated_fields)
          
-          79          56 LOAD_CONST               5 ('return')
+          80          56 LOAD_CONST               5 ('return')
                       58 LOAD_NAME                6 (list)
                       60 LOAD_CONST               7 ('JSONQuestionnaireColumn')
                       62 BINARY_SUBSCR
                       72 BUILD_TUPLE              2
-                      74 LOAD_CONST               8 (<code object fetch_fields, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 79>)
+                      74 LOAD_CONST               8 (<code object fetch_fields, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 80>)
                       76 MAKE_FUNCTION            4 (annotations)
                       78 STORE_NAME               8 (fetch_fields)
          
-         107          80 LOAD_CONST               9 (<code object create_db_class, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 107>)
+         106          80 LOAD_CONST               9 (<code object create_db_class, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 106>)
                       82 MAKE_FUNCTION            0
                       84 STORE_NAME               9 (create_db_class)
          
-         153          86 LOAD_CONST              10 (<code object preprocess_calculation_string, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 153>)
+         152          86 LOAD_CONST              10 (<code object preprocess_calculation_string, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 152>)
                       88 MAKE_FUNCTION            0
                       90 STORE_NAME              10 (preprocess_calculation_string)
          
-         160          92 LOAD_CONST              11 (<code object create_blank, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 160>)
+         159          92 LOAD_CONST              11 (<code object create_blank, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 159>)
                       94 MAKE_FUNCTION            0
                       96 STORE_NAME              11 (create_blank)
          
-         171          98 LOAD_CONST              21 (('',))
-                     100 LOAD_CONST              13 (<code object handle_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 171>)
+         170          98 LOAD_CONST              21 (('',))
+                     100 LOAD_CONST              13 (<code object handle_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 170>)
                      102 MAKE_FUNCTION            1 (defaults)
                      104 STORE_NAME              12 (handle_questionnaire)
          
-         253         106 LOAD_CONST              14 (<code object get_field, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 253>)
+         252         106 LOAD_CONST              14 (<code object get_field, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 252>)
                      108 MAKE_FUNCTION            0
                      110 STORE_NAME              13 (get_field)
          
-         259         112 LOAD_CONST              15 (<code object fetch_all_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 259>)
+         258         112 LOAD_CONST              15 (<code object fetch_all_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 258>)
                      114 MAKE_FUNCTION            0
                      116 STORE_NAME              14 (fetch_all_data)
          
-         262         118 LOAD_CONST              16 (<code object fetch_finished_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 262>)
+         261         118 LOAD_CONST              16 (<code object fetch_finished_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 261>)
                      120 MAKE_FUNCTION            0
                      122 STORE_NAME              15 (fetch_finished_data)
          
-         266         124 LOAD_CONST              22 ((0, True))
-                     126 LOAD_CONST              19 (<code object fetch_column_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 266>)
+         265         124 LOAD_CONST              22 ((0, True))
+                     126 LOAD_CONST              19 (<code object fetch_column_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 265>)
                      128 MAKE_FUNCTION            1 (defaults)
                      130 STORE_NAME              16 (fetch_column_data)
                      132 LOAD_CONST              20 (None)
                      134 RETURN_VALUE
          consts
             'JSONQuestionnaire'
             'directory'
@@ -534,49 +553,49 @@
                   0100000000000000007c005f070000000000000000640064006400a60200
                   00ab02000000000000000001006e0b230031007304770278035900770101
                   005900010001006e2823007410000000000000000000002400721b7d0574
                   130000000000000000000064027c029b0164037c059b0164049d05a60100
                   00ab010000000000000000820164007d057e057701770078035900770167
                   007c005f0a000000000000000067007c005f0b000000000000000064057c
                   005f0c000000000000000064007c005f0d000000000000000064005300
-                56           0 RESUME                   0
+                57           0 RESUME                   0
                
-                57           2 LOAD_FAST                2 (file_name)
+                58           2 LOAD_FAST                2 (file_name)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (file_name)
                
-                58          16 LOAD_GLOBAL              2 (os)
+                59          16 LOAD_GLOBAL              2 (os)
                             28 LOAD_ATTR                2 (path)
                             38 LOAD_METHOD              3 (join)
                             60 LOAD_FAST                1 (directory)
                             62 LOAD_FAST                2 (file_name)
                             64 LOAD_CONST               1 ('.json')
                             66 BINARY_OP                0 (+)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 STORE_FAST               3 (fullPath)
                
-                60          86 NOP
+                61          86 NOP
                
-                61          88 LOAD_GLOBAL              9 (NULL + open)
+                62          88 LOAD_GLOBAL              9 (NULL + open)
                            100 LOAD_FAST                3 (fullPath)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 BEFORE_WITH
                            118 STORE_FAST               4 (f)
                
-                62         120 LOAD_GLOBAL             11 (NULL + json)
+                63         120 LOAD_GLOBAL             11 (NULL + json)
                            132 LOAD_ATTR                6 (load)
                            142 LOAD_FAST                4 (f)
                            144 PRECALL                  1
                            148 CALL                     1
                            158 LOAD_FAST                0 (self)
                            160 STORE_ATTR               7 (json_data)
                
-                61         170 LOAD_CONST               0 (None)
+                62         170 LOAD_CONST               0 (None)
                            172 LOAD_CONST               0 (None)
                            174 LOAD_CONST               0 (None)
                            176 PRECALL                  2
                            180 CALL                     2
                            190 POP_TOP
                            192 JUMP_FORWARD            11 (to 216)
                        >>  194 PUSH_EXC_INFO
@@ -589,56 +608,56 @@
                        >>  208 POP_TOP
                            210 POP_EXCEPT
                            212 POP_TOP
                            214 POP_TOP
                        >>  216 JUMP_FORWARD            40 (to 298)
                        >>  218 PUSH_EXC_INFO
                
-                63         220 LOAD_GLOBAL             16 (ValueError)
+                64         220 LOAD_GLOBAL             16 (ValueError)
                            232 CHECK_EXC_MATCH
                            234 POP_JUMP_FORWARD_IF_FALSE    27 (to 290)
                            236 STORE_FAST               5 (error)
                
-                64         238 LOAD_GLOBAL             19 (NULL + SyntaxError)
+                65         238 LOAD_GLOBAL             19 (NULL + SyntaxError)
                            250 LOAD_CONST               2 ('ERROR! Unable to parse `')
                
-                65         252 LOAD_FAST                2 (file_name)
+                66         252 LOAD_FAST                2 (file_name)
                            254 FORMAT_VALUE             1 (str)
                            256 LOAD_CONST               3 ('` questionnaire. Please check that the file contains valid JSON syntax. Python reports the following error: `')
                            258 LOAD_FAST                5 (error)
                            260 FORMAT_VALUE             1 (str)
                            262 LOAD_CONST               4 ('`')
                
-                64         264 BUILD_STRING             5
+                65         264 BUILD_STRING             5
                            266 PRECALL                  1
                            270 CALL                     1
                            280 RAISE_VARARGS            1
                        >>  282 LOAD_CONST               0 (None)
                            284 STORE_FAST               5 (error)
                            286 DELETE_FAST              5 (error)
                            288 RERAISE                  1
                
-                63     >>  290 RERAISE                  0
+                64     >>  290 RERAISE                  0
                        >>  292 COPY                     3
                            294 POP_EXCEPT
                            296 RERAISE                  1
                
-                68     >>  298 BUILD_LIST               0
+                69     >>  298 BUILD_LIST               0
                            300 LOAD_FAST                0 (self)
                            302 STORE_ATTR              10 (_JSONQuestionnaire__fields)
                
-                69         312 BUILD_LIST               0
+                70         312 BUILD_LIST               0
                            314 LOAD_FAST                0 (self)
                            316 STORE_ATTR              11 (_JSONQuestionnaire__calc_fields)
                
-                70         326 LOAD_CONST               5 (0)
+                71         326 LOAD_CONST               5 (0)
                            328 LOAD_FAST                0 (self)
                            330 STORE_ATTR              12 (_JSONQuestionnaire__field_count)
                
-                71         340 LOAD_CONST               0 (None)
+                72         340 LOAD_CONST               0 (None)
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR              13 (db_class)
                            354 LOAD_CONST               0 (None)
                            356 RETURN_VALUE
                ExceptionTable:
                  88 to 116 -> 218 [0]
                  118 to 168 -> 194 [1] lasti
@@ -659,482 +678,463 @@
                   0
                names      ('file_name', 'os', 'path', 'join', 'open', 'json', 'load', 'json_data', 'ValueError', 'SyntaxError', '_JSONQuestionnaire__fields', '_JSONQuestionnaire__calc_fields', '_JSONQuestionnaire__field_count', 'db_class')
                varnames   ('self', 'directory', 'file_name', 'fullPath', 'f', 'error')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       '__init__'
-               firstlineno 56
+               firstlineno 57
                lnotab
                   0x02010e0146020201200132ff320212010e010cff1aff08050e010e010e
                   01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000006a0100000000000000005300
-                73           0 RESUME                   0
+                74           0 RESUME                   0
                
-                74           2 LOAD_FAST                0 (self)
+                75           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (db_class)
                             14 LOAD_ATTR                1 (__tablename__)
                             24 RETURN_VALUE
                consts
                   None
                names      ('db_class', '__tablename__')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'get_table_name'
-               firstlineno 73
+               firstlineno 74
                lnotab 0x0201
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-                76           0 RESUME                   0
+                77           0 RESUME                   0
                
-                77           2 LOAD_FAST                0 (self)
+                78           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_JSONQuestionnaire__calc_fields)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_JSONQuestionnaire__calc_fields',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'get_calculated_fields'
-               firstlineno 76
+               firstlineno 77
                lnotab 0x0201
             'JSONQuestionnaireColumn'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
                   0x970067007c005f0000000000000000007c006a01000000000000000072
                   0964017c006a010000000000000000760172197405000000000000000000
                   0064027c006a0300000000000000007a060000a6010000ab010000000000
                   0000000100640053007c006a010000000000000000640119000000000000
-                  00000044005da77d0164037409000000000000000000007c01a005000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00a6010000ab010000000000000000760172018c2664047c017600720f64
-                  017c017601720b7c016404190000000000000000007c0164013c00000064
-                  017c017600723f7c016405190000000000000000007d027c016401190000
-                  0000000000000044005d2e7d0364037c03760072287c006a000000000000
-                  000000a0060000000000000000000000000000000000000000740f000000
-                  000000000000007c037c02a6020000ab020000000000000000a6010000ab
-                  01000000000000000001008c2f64037c01760072277c006a000000000000
-                  000000a0060000000000000000000000000000000000000000740f000000
-                  000000000000007c01a6010000ab010000000000000000a6010000ab0100
-                  0000000000000001008ca87411000000000000000000007c006a00000000
-                  0000000000a6010000ab0100000000000000007c005f0900000000000000
-                  007c006a0000000000000000005300
-                79           0 RESUME                   0
+                  00000044005d837d0164037c017600720f64017c017601720b7c01640319
+                  0000000000000000007c0164013c00000064017c017600723f7c01640419
+                  0000000000000000007d027c0164011900000000000000000044005d2e7d
+                  0364057c03760072287c006a000000000000000000a00400000000000000
+                  00000000000000000000000000740b000000000000000000007c037c02a6
+                  020000ab020000000000000000a6010000ab01000000000000000001008c
+                  2f64057c01760072277c006a000000000000000000a00400000000000000
+                  00000000000000000000000000740b000000000000000000007c01a60100
+                  00ab010000000000000000a6010000ab01000000000000000001008c8474
+                  0d000000000000000000007c006a000000000000000000a6010000ab0100
+                  000000000000007c005f0700000000000000007c006a0000000000000000
+                  005300
+                80           0 RESUME                   0
                
-                80           2 BUILD_LIST               0
+                81           2 BUILD_LIST               0
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (_JSONQuestionnaire__fields)
                
-                82          16 LOAD_FAST                0 (self)
+                83          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (json_data)
                             28 POP_JUMP_FORWARD_IF_FALSE     9 (to 48)
                             30 LOAD_CONST               1 ('questions')
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                1 (json_data)
                             44 CONTAINS_OP              1
                             46 POP_JUMP_FORWARD_IF_FALSE    25 (to 98)
                
-                83     >>   48 LOAD_GLOBAL              5 (NULL + print)
+                84     >>   48 LOAD_GLOBAL              5 (NULL + print)
                             60 LOAD_CONST               2 ('ERROR! `%s` questionnaire contains no questions.')
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (file_name)
                             74 BINARY_OP                6 (%)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 POP_TOP
                
-                84          94 LOAD_CONST               0 (None)
+                85          94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                
-                88     >>   98 LOAD_FAST                0 (self)
+                89     >>   98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                1 (json_data)
                            110 LOAD_CONST               1 ('questions')
                            112 BINARY_SUBSCR
                            122 GET_ITER
-                       >>  124 FOR_ITER               167 (to 460)
+                       >>  124 FOR_ITER               131 (to 388)
                            126 STORE_FAST               1 (q)
                
-                89         128 LOAD_CONST               3 ('id')
-                           130 LOAD_GLOBAL              9 (NULL + list)
-                           142 LOAD_FAST                1 (q)
-                           144 LOAD_METHOD              5 (keys)
-                           166 PRECALL                  0
-                           170 CALL                     0
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 CONTAINS_OP              1
-                           196 POP_JUMP_FORWARD_IF_FALSE     1 (to 200)
-               
-                90         198 JUMP_BACKWARD           38 (to 124)
-               
-                93     >>  200 LOAD_CONST               4 ('q_text')
-                           202 LOAD_FAST                1 (q)
-                           204 CONTAINS_OP              0
-                           206 POP_JUMP_FORWARD_IF_FALSE    15 (to 238)
-                           208 LOAD_CONST               1 ('questions')
-                           210 LOAD_FAST                1 (q)
-                           212 CONTAINS_OP              1
-                           214 POP_JUMP_FORWARD_IF_FALSE    11 (to 238)
-               
-                94         216 LOAD_FAST                1 (q)
-                           218 LOAD_CONST               4 ('q_text')
-                           220 BINARY_SUBSCR
-                           230 LOAD_FAST                1 (q)
-                           232 LOAD_CONST               1 ('questions')
-                           234 STORE_SUBSCR
-               
-                96     >>  238 LOAD_CONST               1 ('questions')
-                           240 LOAD_FAST                1 (q)
-                           242 CONTAINS_OP              0
-                           244 POP_JUMP_FORWARD_IF_FALSE    63 (to 372)
-               
-                97         246 LOAD_FAST                1 (q)
-                           248 LOAD_CONST               5 ('questiontype')
-                           250 BINARY_SUBSCR
-                           260 STORE_FAST               2 (question_type)
-               
-                98         262 LOAD_FAST                1 (q)
-                           264 LOAD_CONST               1 ('questions')
-                           266 BINARY_SUBSCR
-                           276 GET_ITER
-                       >>  278 FOR_ITER                46 (to 372)
-                           280 STORE_FAST               3 (qt)
-               
-                99         282 LOAD_CONST               3 ('id')
-                           284 LOAD_FAST                3 (qt)
-                           286 CONTAINS_OP              0
-                           288 POP_JUMP_FORWARD_IF_FALSE    40 (to 370)
-               
-               100         290 LOAD_FAST                0 (self)
-                           292 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
-                           302 LOAD_METHOD              6 (append)
-                           324 LOAD_GLOBAL             15 (NULL + JSONQuestionnaireColumn)
-                           336 LOAD_FAST                3 (qt)
-                           338 LOAD_FAST                2 (question_type)
-                           340 PRECALL                  2
-                           344 CALL                     2
-                           354 PRECALL                  1
-                           358 CALL                     1
-                           368 POP_TOP
-                       >>  370 JUMP_BACKWARD           47 (to 278)
-               
-               101     >>  372 LOAD_CONST               3 ('id')
-                           374 LOAD_FAST                1 (q)
-                           376 CONTAINS_OP              0
-                           378 POP_JUMP_FORWARD_IF_FALSE    39 (to 458)
-               
-               102         380 LOAD_FAST                0 (self)
-                           382 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
-                           392 LOAD_METHOD              6 (append)
-                           414 LOAD_GLOBAL             15 (NULL + JSONQuestionnaireColumn)
-                           426 LOAD_FAST                1 (q)
-                           428 PRECALL                  1
-                           432 CALL                     1
-                           442 PRECALL                  1
-                           446 CALL                     1
-                           456 POP_TOP
-                       >>  458 JUMP_BACKWARD          168 (to 124)
-               
-               104     >>  460 LOAD_GLOBAL             17 (NULL + len)
-                           472 LOAD_FAST                0 (self)
-                           474 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
-                           484 PRECALL                  1
-                           488 CALL                     1
-                           498 LOAD_FAST                0 (self)
-                           500 STORE_ATTR               9 (_JSONQuestionnaire__field_count)
-               
-               105         510 LOAD_FAST                0 (self)
-                           512 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
-                           522 RETURN_VALUE
+                91         128 LOAD_CONST               3 ('q_text')
+                           130 LOAD_FAST                1 (q)
+                           132 CONTAINS_OP              0
+                           134 POP_JUMP_FORWARD_IF_FALSE    15 (to 166)
+                           136 LOAD_CONST               1 ('questions')
+                           138 LOAD_FAST                1 (q)
+                           140 CONTAINS_OP              1
+                           142 POP_JUMP_FORWARD_IF_FALSE    11 (to 166)
+               
+                92         144 LOAD_FAST                1 (q)
+                           146 LOAD_CONST               3 ('q_text')
+                           148 BINARY_SUBSCR
+                           158 LOAD_FAST                1 (q)
+                           160 LOAD_CONST               1 ('questions')
+                           162 STORE_SUBSCR
+               
+                94     >>  166 LOAD_CONST               1 ('questions')
+                           168 LOAD_FAST                1 (q)
+                           170 CONTAINS_OP              0
+                           172 POP_JUMP_FORWARD_IF_FALSE    63 (to 300)
+               
+                95         174 LOAD_FAST                1 (q)
+                           176 LOAD_CONST               4 ('questiontype')
+                           178 BINARY_SUBSCR
+                           188 STORE_FAST               2 (question_type)
+               
+                96         190 LOAD_FAST                1 (q)
+                           192 LOAD_CONST               1 ('questions')
+                           194 BINARY_SUBSCR
+                           204 GET_ITER
+                       >>  206 FOR_ITER                46 (to 300)
+                           208 STORE_FAST               3 (qt)
+               
+                97         210 LOAD_CONST               5 ('id')
+                           212 LOAD_FAST                3 (qt)
+                           214 CONTAINS_OP              0
+                           216 POP_JUMP_FORWARD_IF_FALSE    40 (to 298)
+               
+                98         218 LOAD_FAST                0 (self)
+                           220 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
+                           230 LOAD_METHOD              4 (append)
+                           252 LOAD_GLOBAL             11 (NULL + JSONQuestionnaireColumn)
+                           264 LOAD_FAST                3 (qt)
+                           266 LOAD_FAST                2 (question_type)
+                           268 PRECALL                  2
+                           272 CALL                     2
+                           282 PRECALL                  1
+                           286 CALL                     1
+                           296 POP_TOP
+                       >>  298 JUMP_BACKWARD           47 (to 206)
+               
+               100     >>  300 LOAD_CONST               5 ('id')
+                           302 LOAD_FAST                1 (q)
+                           304 CONTAINS_OP              0
+                           306 POP_JUMP_FORWARD_IF_FALSE    39 (to 386)
+               
+               101         308 LOAD_FAST                0 (self)
+                           310 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
+                           320 LOAD_METHOD              4 (append)
+                           342 LOAD_GLOBAL             11 (NULL + JSONQuestionnaireColumn)
+                           354 LOAD_FAST                1 (q)
+                           356 PRECALL                  1
+                           360 CALL                     1
+                           370 PRECALL                  1
+                           374 CALL                     1
+                           384 POP_TOP
+                       >>  386 JUMP_BACKWARD          132 (to 124)
+               
+               103     >>  388 LOAD_GLOBAL             13 (NULL + len)
+                           400 LOAD_FAST                0 (self)
+                           402 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 LOAD_FAST                0 (self)
+                           428 STORE_ATTR               7 (_JSONQuestionnaire__field_count)
+               
+               104         438 LOAD_FAST                0 (self)
+                           440 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
+                           450 RETURN_VALUE
                consts
                   None
                   'questions'
                   'ERROR! `%s` questionnaire contains no questions.'
-                  'id'
                   'q_text'
                   'questiontype'
-               names      ('_JSONQuestionnaire__fields', 'json_data', 'print', 'file_name', 'list', 'keys', 'append', 'JSONQuestionnaireColumn', 'len', '_JSONQuestionnaire__field_count')
+                  'id'
+               names      ('_JSONQuestionnaire__fields', 'json_data', 'print', 'file_name', 'append', 'JSONQuestionnaireColumn', 'len', '_JSONQuestionnaire__field_count')
                varnames   ('self', 'q', 'question_type', 'qt')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'fetch_fields'
-               firstlineno 79
+               firstlineno 80
                lnotab
-                  0x02010e0220012e0104041e014601020310011602080110011401080152
-                  01080150023201
+                  0x02010e0220012e0104041e021001160208011001140108015202080150
+                  023201
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 19
                flags     : 3
                code
                   0x8705870697007c006a00000000000000000073147c00a0010000000000
                   000000000000000000000000000000a6000000ab00000000000000000001
-                  007c006a020000000000000000730767007c005f02000000000000000074
-                  0600000000000000000000a0040000000000000000000000000000000000
-                  00000064017c006a050000000000000000a6020000ab0200000000000000
-                  007d0164027c01740600000000000000000000a004000000000000000000
-                  000000000000000000000064037c006a050000000000000000a6020000ab
-                  020000000000000000740d000000000000000000006a0700000000000000
-                  00740c000000000000000000006a08000000000000000064046404ac05a6
-                  030000ab0300000000000000006406740d000000000000000000006a0700
-                  00000000000000740c000000000000000000006a08000000000000000074
-                  0d000000000000000000006a0900000000000000006407a6010000ab0100
-                  000000000000006408ac09a6030000ab030000000000000000640a740d00
-                  0000000000000000006a0a0000000000000000640b7c01ac0ca6020000ab
-                  020000000000000000640d740d000000000000000000006a070000000000
-                  000000740c000000000000000000006a0b00000000000000006408640eac
-                  0fa6030000ab0300000000000000006410740d000000000000000000006a
-                  070000000000000000740c000000000000000000006a0c00000000000000
-                  006408740c000000000000000000006a0d0000000000000000a00e000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00ac0fa6030000ab0300000000000000006411740d000000000000000000
-                  006a070000000000000000740c000000000000000000006a0c0000000000
-                  0000006408740c000000000000000000006a0d0000000000000000a00e00
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  000000ac0fa6030000ab03000000000000000064126413840069087d027c
-                  006a00000000000000000044005d1e7d037c03a00f000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000007c027c036a
-                  1000000000000000003c0000008c1f64147c006a11000000000000000076
-                  00726388066601641584088a057c006a1100000000000000006414190000
-                  00000000000000a0120000000000000000000000000000000000000000a6
-                  000000ab00000000000000000044005d3e5c0200008a067d047c006a0200
-                  00000000000000a013000000000000000000000000000000000000000089
-                  06a6010000ab01000000000000000001007c00a014000000000000000000
-                  00000000000000000000007c04a6010000ab0100000000000000007d047c
-                  04660188056601641684097c0289063c0000008c3f742b00000000000000
-                  0000007c006a050000000000000000740c000000000000000000006a1600
-                  0000000000000066017c02a6030000ab0300000000000000007c005f1700
-                  0000000000000064005300
+                  007c006a020000000000000000730767007c005f02000000000000000064
+                  017c006a0300000000000000009b009d027d0164027c0174080000000000
+                  0000000000a005000000000000000000000000000000000000000064037c
+                  006a030000000000000000a6020000ab020000000000000000740d000000
+                  000000000000006a070000000000000000740c000000000000000000006a
+                  08000000000000000064046404ac05a6030000ab03000000000000000064
+                  06740d000000000000000000006a070000000000000000740c0000000000
+                  00000000006a080000000000000000740d000000000000000000006a0900
+                  000000000000006407a6010000ab0100000000000000006408ac09a60300
+                  00ab030000000000000000640a740d000000000000000000006a0a000000
+                  0000000000640b7c01ac0ca6020000ab020000000000000000640d740d00
+                  0000000000000000006a070000000000000000740c000000000000000000
+                  006a0b00000000000000006408640eac0fa6030000ab0300000000000000
+                  006410740d000000000000000000006a070000000000000000740c000000
+                  000000000000006a0c00000000000000006408740c000000000000000000
+                  006a0d0000000000000000a00e0000000000000000000000000000000000
+                  000000a6000000ab000000000000000000ac0fa6030000ab030000000000
+                  0000006411740d000000000000000000006a070000000000000000740c00
+                  0000000000000000006a0c00000000000000006408740c00000000000000
+                  0000006a0d0000000000000000a00e000000000000000000000000000000
+                  0000000000a6000000ab000000000000000000ac0fa6030000ab03000000
+                  000000000064126413840069087d027c006a00000000000000000044005d
+                  1e7d037c03a00f0000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007c027c036a1000000000000000003c0000008c
+                  1f64147c006a1100000000000000007600726388066601641584088a057c
+                  006a110000000000000000641419000000000000000000a0120000000000
+                  000000000000000000000000000000a6000000ab00000000000000000044
+                  005d3e5c0200008a067d047c006a020000000000000000a0130000000000
+                  0000000000000000000000000000008906a6010000ab0100000000000000
+                  0001007c00a01400000000000000000000000000000000000000007c04a6
+                  010000ab0100000000000000007d047c04660188056601641684097c0289
+                  063c0000008c3f742b000000000000000000007c006a0300000000000000
+                  00740c000000000000000000006a16000000000000000066017c02a60300
+                  00ab0300000000000000007c005f17000000000000000064005300
                              0 MAKE_CELL                5 (execute_calculation)
                              2 MAKE_CELL                6 (field_name)
                
-               107           4 RESUME                   0
+               106           4 RESUME                   0
                
-               110           6 LOAD_FAST                0 (self)
+               109           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
                             18 POP_JUMP_FORWARD_IF_TRUE    20 (to 60)
                
-               111          20 LOAD_FAST                0 (self)
+               110          20 LOAD_FAST                0 (self)
                             22 LOAD_METHOD              1 (fetch_fields)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 POP_TOP
                
-               113     >>   60 LOAD_FAST                0 (self)
+               112     >>   60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                2 (_JSONQuestionnaire__calc_fields)
                             72 POP_JUMP_FORWARD_IF_TRUE     7 (to 88)
                
-               114          74 BUILD_LIST               0
+               113          74 BUILD_LIST               0
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               2 (_JSONQuestionnaire__calc_fields)
                
-               116     >>   88 LOAD_GLOBAL              6 (str)
-                           100 LOAD_METHOD              4 (format)
-                           122 LOAD_CONST               1 ('questionnaire_{}')
-                           124 LOAD_FAST                0 (self)
-                           126 LOAD_ATTR                5 (file_name)
-                           136 PRECALL                  2
-                           140 CALL                     2
-                           150 STORE_FAST               1 (table_name)
-               
-               119         152 LOAD_CONST               2 ('__tablename__')
-                           154 LOAD_FAST                1 (table_name)
-               
-               120         156 LOAD_GLOBAL              6 (str)
-                           168 LOAD_METHOD              4 (format)
-                           190 LOAD_CONST               3 ('{0}ID')
-                           192 LOAD_FAST                0 (self)
-                           194 LOAD_ATTR                5 (file_name)
-                           204 PRECALL                  2
-                           208 CALL                     2
-                           218 LOAD_GLOBAL             13 (NULL + db)
-                           230 LOAD_ATTR                7 (Column)
-                           240 LOAD_GLOBAL             12 (db)
-                           252 LOAD_ATTR                8 (Integer)
-                           262 LOAD_CONST               4 (True)
-                           264 LOAD_CONST               4 (True)
-                           266 KW_NAMES                 5
-                           268 PRECALL                  3
-                           272 CALL                     3
-               
-               121         282 LOAD_CONST               6 ('participantID')
+               115     >>   88 LOAD_CONST               1 ('questionnaire_')
+                            90 LOAD_FAST                0 (self)
+                            92 LOAD_ATTR                3 (file_name)
+                           102 FORMAT_VALUE             0
+                           104 BUILD_STRING             2
+                           106 STORE_FAST               1 (table_name)
+               
+               118         108 LOAD_CONST               2 ('__tablename__')
+                           110 LOAD_FAST                1 (table_name)
+               
+               119         112 LOAD_GLOBAL              8 (str)
+                           124 LOAD_METHOD              5 (format)
+                           146 LOAD_CONST               3 ('{0}ID')
+                           148 LOAD_FAST                0 (self)
+                           150 LOAD_ATTR                3 (file_name)
+                           160 PRECALL                  2
+                           164 CALL                     2
+                           174 LOAD_GLOBAL             13 (NULL + db)
+                           186 LOAD_ATTR                7 (Column)
+                           196 LOAD_GLOBAL             12 (db)
+                           208 LOAD_ATTR                8 (Integer)
+                           218 LOAD_CONST               4 (True)
+                           220 LOAD_CONST               4 (True)
+                           222 KW_NAMES                 5
+                           224 PRECALL                  3
+                           228 CALL                     3
+               
+               120         238 LOAD_CONST               6 ('participantID')
+                           240 LOAD_GLOBAL             13 (NULL + db)
+                           252 LOAD_ATTR                7 (Column)
+                           262 LOAD_GLOBAL             12 (db)
+                           274 LOAD_ATTR                8 (Integer)
                            284 LOAD_GLOBAL             13 (NULL + db)
-                           296 LOAD_ATTR                7 (Column)
-                           306 LOAD_GLOBAL             12 (db)
-                           318 LOAD_ATTR                8 (Integer)
-                           328 LOAD_GLOBAL             13 (NULL + db)
-                           340 LOAD_ATTR                9 (ForeignKey)
-                           350 LOAD_CONST               7 ('participant.participantID')
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 LOAD_CONST               8 (False)
-                           368 KW_NAMES                 9
-                           370 PRECALL                  3
-                           374 CALL                     3
+                           296 LOAD_ATTR                9 (ForeignKey)
+                           306 LOAD_CONST               7 ('participant.participantID')
+                           308 PRECALL                  1
+                           312 CALL                     1
+                           322 LOAD_CONST               8 (False)
+                           324 KW_NAMES                 9
+                           326 PRECALL                  3
+                           330 CALL                     3
+               
+               122         340 LOAD_CONST              10 ('participant')
+                           342 LOAD_GLOBAL             13 (NULL + db)
+                           354 LOAD_ATTR               10 (relationship)
+                           364 LOAD_CONST              11 ('Participant')
+                           366 LOAD_FAST                1 (table_name)
+                           368 KW_NAMES                12
+                           370 PRECALL                  2
+                           374 CALL                     2
                
-               123         384 LOAD_CONST              10 ('participant')
+               123         384 LOAD_CONST              13 ('tag')
                            386 LOAD_GLOBAL             13 (NULL + db)
-                           398 LOAD_ATTR               10 (relationship)
-                           408 LOAD_CONST              11 ('Participant')
-                           410 LOAD_FAST                1 (table_name)
-                           412 KW_NAMES                12
-                           414 PRECALL                  2
-                           418 CALL                     2
-               
-               124         428 LOAD_CONST              13 ('tag')
-                           430 LOAD_GLOBAL             13 (NULL + db)
-                           442 LOAD_ATTR                7 (Column)
-                           452 LOAD_GLOBAL             12 (db)
-                           464 LOAD_ATTR               11 (String)
-                           474 LOAD_CONST               8 (False)
-                           476 LOAD_CONST              14 ('')
-                           478 KW_NAMES                15
-                           480 PRECALL                  3
-                           484 CALL                     3
-               
-               125         494 LOAD_CONST              16 ('timeStarted')
-                           496 LOAD_GLOBAL             13 (NULL + db)
-                           508 LOAD_ATTR                7 (Column)
-                           518 LOAD_GLOBAL             12 (db)
-                           530 LOAD_ATTR               12 (DateTime)
-                           540 LOAD_CONST               8 (False)
-                           542 LOAD_GLOBAL             12 (db)
-                           554 LOAD_ATTR               13 (func)
-                           564 LOAD_METHOD             14 (now)
-                           586 PRECALL                  0
-                           590 CALL                     0
-                           600 KW_NAMES                15
-                           602 PRECALL                  3
-                           606 CALL                     3
-               
-               126         616 LOAD_CONST              17 ('timeEnded')
-                           618 LOAD_GLOBAL             13 (NULL + db)
-                           630 LOAD_ATTR                7 (Column)
-                           640 LOAD_GLOBAL             12 (db)
-                           652 LOAD_ATTR               12 (DateTime)
-                           662 LOAD_CONST               8 (False)
-                           664 LOAD_GLOBAL             12 (db)
-                           676 LOAD_ATTR               13 (func)
-                           686 LOAD_METHOD             14 (now)
-                           708 PRECALL                  0
-                           712 CALL                     0
-                           722 KW_NAMES                15
-                           724 PRECALL                  3
-                           728 CALL                     3
-               
-               127         738 LOAD_CONST              18 ('duration')
-                           740 LOAD_CONST              19 (<code object <lambda>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 127>)
-                           742 MAKE_FUNCTION            0
-               
-               118         744 BUILD_MAP                8
-                           746 STORE_FAST               2 (table_attr)
-               
-               130         748 LOAD_FAST                0 (self)
-                           750 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
-                           760 GET_ITER
-                       >>  762 FOR_ITER                30 (to 824)
-                           764 STORE_FAST               3 (field)
-               
-               131         766 LOAD_FAST                3 (field)
-                           768 LOAD_METHOD             15 (generate_db_column)
-                           790 PRECALL                  0
-                           794 CALL                     0
-                           804 LOAD_FAST                2 (table_attr)
-                           806 LOAD_FAST                3 (field)
-                           808 LOAD_ATTR               16 (id)
-                           818 STORE_SUBSCR
-                           822 JUMP_BACKWARD           31 (to 762)
-               
-               133     >>  824 LOAD_CONST              20 ('participant_calculations')
-                           826 LOAD_FAST                0 (self)
-                           828 LOAD_ATTR               17 (json_data)
-                           838 CONTAINS_OP              0
-                           840 POP_JUMP_FORWARD_IF_FALSE    99 (to 1040)
-               
-               134         842 LOAD_CLOSURE             6 (field_name)
-                           844 BUILD_TUPLE              1
-                           846 LOAD_CONST              21 (<code object execute_calculation, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 134>)
-                           848 MAKE_FUNCTION            8 (closure)
-                           850 STORE_DEREF              5 (execute_calculation)
-               
-               144         852 LOAD_FAST                0 (self)
-                           854 LOAD_ATTR               17 (json_data)
-                           864 LOAD_CONST              20 ('participant_calculations')
-                           866 BINARY_SUBSCR
-                           876 LOAD_METHOD             18 (items)
-                           898 PRECALL                  0
-                           902 CALL                     0
-                           912 GET_ITER
-                       >>  914 FOR_ITER                62 (to 1040)
-                           916 UNPACK_SEQUENCE          2
-                           920 STORE_DEREF              6 (field_name)
-                           922 STORE_FAST               4 (calculation)
-               
-               145         924 LOAD_FAST                0 (self)
-                           926 LOAD_ATTR                2 (_JSONQuestionnaire__calc_fields)
-                           936 LOAD_METHOD             19 (append)
-                           958 LOAD_DEREF               6 (field_name)
-                           960 PRECALL                  1
-                           964 CALL                     1
-                           974 POP_TOP
-               
-               146         976 LOAD_FAST                0 (self)
-                           978 LOAD_METHOD             20 (preprocess_calculation_string)
-                          1000 LOAD_FAST                4 (calculation)
-                          1002 PRECALL                  1
-                          1006 CALL                     1
-                          1016 STORE_FAST               4 (calculation)
-               
-               148        1018 LOAD_FAST                4 (calculation)
-                          1020 BUILD_TUPLE              1
-                          1022 LOAD_CLOSURE             5 (execute_calculation)
-                          1024 BUILD_TUPLE              1
-                          1026 LOAD_CONST              22 (<code object <lambda>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 148>)
-                          1028 MAKE_FUNCTION            9 (defaults, closure)
-                          1030 LOAD_FAST                2 (table_attr)
-                          1032 LOAD_DEREF               6 (field_name)
-                          1034 STORE_SUBSCR
-                          1038 JUMP_BACKWARD           63 (to 914)
-               
-               150     >> 1040 LOAD_GLOBAL             43 (NULL + type)
-                          1052 LOAD_FAST                0 (self)
-                          1054 LOAD_ATTR                5 (file_name)
-                          1064 LOAD_GLOBAL             12 (db)
-                          1076 LOAD_ATTR               22 (Model)
-                          1086 BUILD_TUPLE              1
-                          1088 LOAD_FAST                2 (table_attr)
-                          1090 PRECALL                  3
-                          1094 CALL                     3
-                          1104 LOAD_FAST                0 (self)
-                          1106 STORE_ATTR              23 (db_class)
-                          1116 LOAD_CONST               0 (None)
-                          1118 RETURN_VALUE
+                           398 LOAD_ATTR                7 (Column)
+                           408 LOAD_GLOBAL             12 (db)
+                           420 LOAD_ATTR               11 (String)
+                           430 LOAD_CONST               8 (False)
+                           432 LOAD_CONST              14 ('')
+                           434 KW_NAMES                15
+                           436 PRECALL                  3
+                           440 CALL                     3
+               
+               124         450 LOAD_CONST              16 ('timeStarted')
+                           452 LOAD_GLOBAL             13 (NULL + db)
+                           464 LOAD_ATTR                7 (Column)
+                           474 LOAD_GLOBAL             12 (db)
+                           486 LOAD_ATTR               12 (DateTime)
+                           496 LOAD_CONST               8 (False)
+                           498 LOAD_GLOBAL             12 (db)
+                           510 LOAD_ATTR               13 (func)
+                           520 LOAD_METHOD             14 (now)
+                           542 PRECALL                  0
+                           546 CALL                     0
+                           556 KW_NAMES                15
+                           558 PRECALL                  3
+                           562 CALL                     3
+               
+               125         572 LOAD_CONST              17 ('timeEnded')
+                           574 LOAD_GLOBAL             13 (NULL + db)
+                           586 LOAD_ATTR                7 (Column)
+                           596 LOAD_GLOBAL             12 (db)
+                           608 LOAD_ATTR               12 (DateTime)
+                           618 LOAD_CONST               8 (False)
+                           620 LOAD_GLOBAL             12 (db)
+                           632 LOAD_ATTR               13 (func)
+                           642 LOAD_METHOD             14 (now)
+                           664 PRECALL                  0
+                           668 CALL                     0
+                           678 KW_NAMES                15
+                           680 PRECALL                  3
+                           684 CALL                     3
+               
+               126         694 LOAD_CONST              18 ('duration')
+                           696 LOAD_CONST              19 (<code object <lambda>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 126>)
+                           698 MAKE_FUNCTION            0
+               
+               117         700 BUILD_MAP                8
+                           702 STORE_FAST               2 (table_attr)
+               
+               129         704 LOAD_FAST                0 (self)
+                           706 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
+                           716 GET_ITER
+                       >>  718 FOR_ITER                30 (to 780)
+                           720 STORE_FAST               3 (field)
+               
+               130         722 LOAD_FAST                3 (field)
+                           724 LOAD_METHOD             15 (generate_db_column)
+                           746 PRECALL                  0
+                           750 CALL                     0
+                           760 LOAD_FAST                2 (table_attr)
+                           762 LOAD_FAST                3 (field)
+                           764 LOAD_ATTR               16 (id)
+                           774 STORE_SUBSCR
+                           778 JUMP_BACKWARD           31 (to 718)
+               
+               132     >>  780 LOAD_CONST              20 ('participant_calculations')
+                           782 LOAD_FAST                0 (self)
+                           784 LOAD_ATTR               17 (json_data)
+                           794 CONTAINS_OP              0
+                           796 POP_JUMP_FORWARD_IF_FALSE    99 (to 996)
+               
+               133         798 LOAD_CLOSURE             6 (field_name)
+                           800 BUILD_TUPLE              1
+                           802 LOAD_CONST              21 (<code object execute_calculation, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 133>)
+                           804 MAKE_FUNCTION            8 (closure)
+                           806 STORE_DEREF              5 (execute_calculation)
+               
+               143         808 LOAD_FAST                0 (self)
+                           810 LOAD_ATTR               17 (json_data)
+                           820 LOAD_CONST              20 ('participant_calculations')
+                           822 BINARY_SUBSCR
+                           832 LOAD_METHOD             18 (items)
+                           854 PRECALL                  0
+                           858 CALL                     0
+                           868 GET_ITER
+                       >>  870 FOR_ITER                62 (to 996)
+                           872 UNPACK_SEQUENCE          2
+                           876 STORE_DEREF              6 (field_name)
+                           878 STORE_FAST               4 (calculation)
+               
+               144         880 LOAD_FAST                0 (self)
+                           882 LOAD_ATTR                2 (_JSONQuestionnaire__calc_fields)
+                           892 LOAD_METHOD             19 (append)
+                           914 LOAD_DEREF               6 (field_name)
+                           916 PRECALL                  1
+                           920 CALL                     1
+                           930 POP_TOP
+               
+               145         932 LOAD_FAST                0 (self)
+                           934 LOAD_METHOD             20 (preprocess_calculation_string)
+                           956 LOAD_FAST                4 (calculation)
+                           958 PRECALL                  1
+                           962 CALL                     1
+                           972 STORE_FAST               4 (calculation)
+               
+               147         974 LOAD_FAST                4 (calculation)
+                           976 BUILD_TUPLE              1
+                           978 LOAD_CLOSURE             5 (execute_calculation)
+                           980 BUILD_TUPLE              1
+                           982 LOAD_CONST              22 (<code object <lambda>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONQuestionnaire.py", line 147>)
+                           984 MAKE_FUNCTION            9 (defaults, closure)
+                           986 LOAD_FAST                2 (table_attr)
+                           988 LOAD_DEREF               6 (field_name)
+                           990 STORE_SUBSCR
+                           994 JUMP_BACKWARD           63 (to 870)
+               
+               149     >>  996 LOAD_GLOBAL             43 (NULL + type)
+                          1008 LOAD_FAST                0 (self)
+                          1010 LOAD_ATTR                3 (file_name)
+                          1020 LOAD_GLOBAL             12 (db)
+                          1032 LOAD_ATTR               22 (Model)
+                          1042 BUILD_TUPLE              1
+                          1044 LOAD_FAST                2 (table_attr)
+                          1046 PRECALL                  3
+                          1050 CALL                     3
+                          1060 LOAD_FAST                0 (self)
+                          1062 STORE_ATTR              23 (db_class)
+                          1072 LOAD_CONST               0 (None)
+                          1074 RETURN_VALUE
                consts
                   None
-                  'questionnaire_{}'
+                  'questionnaire_'
                   '__tablename__'
                   '{0}ID'
                   True
                   ('primary_key', 'autoincrement')
                   'participantID'
                   'participant.participantID'
                   False
@@ -1153,15 +1153,15 @@
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x97007c006a0000000000000000007c006a0100000000000000007a0a00
                         00a0020000000000000000000000000000000000000000a6000000ab0000
                         000000000000005300
-                     127           0 RESUME                   0
+                     126           0 RESUME                   0
                                    2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (timeEnded)
                                   14 LOAD_FAST                0 (self)
                                   16 LOAD_ATTR                1 (timeStarted)
                                   26 BINARY_OP               10 (-)
                                   30 LOAD_METHOD              2 (total_seconds)
                                   52 PRECALL                  0
@@ -1171,15 +1171,15 @@
                         None
                      names      ('timeEnded', 'timeStarted', 'total_seconds')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                      name       '<lambda>'
-                     firstlineno 127
+                     firstlineno 126
                      lnotab 0x
                   'participant_calculations'
                   code
                      argcount  : 2
                      nlocals   : 4
                      stacksize : 7
                      flags     : 19
@@ -1189,60 +1189,60 @@
                         02000000000000000000000000000000000000000089047c006a03000000
                         00000000007c017c02a6040000ab0400000000000000007d037409000000
                         000000000000007c03a6010000ab01000000000000000001007403000000
                         000000000000007c03a6010000ab010000000000000000820164007d027e
                         0277017700780359007701
                                    0 COPY_FREE_VARS           1
                      
-                     134           2 RESUME                   0
+                     133           2 RESUME                   0
                      
-                     135           4 NOP
+                     134           4 NOP
                      
-                     136           6 LOAD_GLOBAL              1 (NULL + eval)
+                     135           6 LOAD_GLOBAL              1 (NULL + eval)
                                   18 LOAD_FAST                1 (calculation)
                                   20 PRECALL                  1
                                   24 CALL                     1
                                   34 RETURN_VALUE
                              >>   36 PUSH_EXC_INFO
                      
-                     137          38 LOAD_GLOBAL              2 (Exception)
+                     136          38 LOAD_GLOBAL              2 (Exception)
                                   50 CHECK_EXC_MATCH
                                   52 POP_JUMP_FORWARD_IF_FALSE    64 (to 182)
                                   54 STORE_FAST               2 (e)
                      
-                     138          56 LOAD_CONST               1 ('Unable to add calculated field `{0}` to the export of questionnaire `{1}`. \nThe preprocessed calculation string was: `{2}`\nThe thrown exception was: {3}')
+                     137          56 LOAD_CONST               1 ('Unable to add calculated field `{0}` to the export of questionnaire `{1}`. \nThe preprocessed calculation string was: `{2}`\nThe thrown exception was: {3}')
                      
-                     140          58 LOAD_METHOD              2 (format)
+                     139          58 LOAD_METHOD              2 (format)
                                   80 LOAD_DEREF               4 (field_name)
                                   82 LOAD_FAST                0 (self)
                                   84 LOAD_ATTR                3 (__tablename__)
                                   94 LOAD_FAST                1 (calculation)
                                   96 LOAD_FAST                2 (e)
                                   98 PRECALL                  4
                                  102 CALL                     4
                      
-                     138         112 STORE_FAST               3 (error)
+                     137         112 STORE_FAST               3 (error)
                      
-                     141         114 LOAD_GLOBAL              9 (NULL + print)
+                     140         114 LOAD_GLOBAL              9 (NULL + print)
                                  126 LOAD_FAST                3 (error)
                                  128 PRECALL                  1
                                  132 CALL                     1
                                  142 POP_TOP
                      
-                     142         144 LOAD_GLOBAL              3 (NULL + Exception)
+                     141         144 LOAD_GLOBAL              3 (NULL + Exception)
                                  156 LOAD_FAST                3 (error)
                                  158 PRECALL                  1
                                  162 CALL                     1
                                  172 RAISE_VARARGS            1
                              >>  174 LOAD_CONST               0 (None)
                                  176 STORE_FAST               2 (e)
                                  178 DELETE_FAST              2 (e)
                                  180 RERAISE                  1
                      
-                     137     >>  182 RERAISE                  0
+                     136     >>  182 RERAISE                  0
                              >>  184 COPY                     3
                                  186 POP_EXCEPT
                                  188 RERAISE                  1
                      ExceptionTable:
                        6 to 32 -> 36 [0]
                        36 to 54 -> 184 [1] lasti
                        56 to 172 -> 174 [1] lasti
@@ -1252,25 +1252,25 @@
                         'Unable to add calculated field `{0}` to the export of questionnaire `{1}`. \nThe preprocessed calculation string was: `{2}`\nThe thrown exception was: {3}'
                      names      ('eval', 'Exception', 'format', '__tablename__', 'print')
                      varnames   ('self', 'calculation', 'e', 'error')
                      freevars   ('field_name',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                      name       'execute_calculation'
-                     firstlineno 134
+                     firstlineno 133
                      lnotab 0x0401020120011201020236fe02031e0126fb
                   code
                      argcount  : 2
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code 0x95019700020089027c007c01a6020000ab0200000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     148           2 RESUME                   0
+                     147           2 RESUME                   0
                                    4 PUSH_NULL
                                    6 LOAD_DEREF               2 (execute_calculation)
                                    8 LOAD_FAST                0 (self)
                                   10 LOAD_FAST                1 (calculation)
                                   12 PRECALL                  2
                                   16 CALL                     2
                                   26 RETURN_VALUE
@@ -1278,81 +1278,81 @@
                         None
                      names      ()
                      varnames   ('self', 'calculation')
                      freevars   ('execute_calculation',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                      name       '<lambda>'
-                     firstlineno 148
+                     firstlineno 147
                      lnotab 0x
-               names      ('_JSONQuestionnaire__fields', 'fetch_fields', '_JSONQuestionnaire__calc_fields', 'str', 'format', 'file_name', 'db', 'Column', 'Integer', 'ForeignKey', 'relationship', 'String', 'DateTime', 'func', 'now', 'generate_db_column', 'id', 'json_data', 'items', 'append', 'preprocess_calculation_string', 'type', 'Model', 'db_class')
+               names      ('_JSONQuestionnaire__fields', 'fetch_fields', '_JSONQuestionnaire__calc_fields', 'file_name', 'str', 'format', 'db', 'Column', 'Integer', 'ForeignKey', 'relationship', 'String', 'DateTime', 'func', 'now', 'generate_db_column', 'id', 'json_data', 'items', 'append', 'preprocess_calculation_string', 'type', 'Model', 'db_class')
                varnames   ('self', 'table_name', 'table_attr', 'field', 'calculation')
                freevars   ()
                cellvars   ('execute_calculation', 'field_name')
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'create_db_class'
-               firstlineno 107
+               firstlineno 106
                lnotab
-                  0x06030e0128020e010e02400304017e0166022c0142017a017a0106f704
+                  0x06030e0128020e010e02140304017e0166022c0142017a017a0106f704
                   0c12013a0212010a0a480134012a021602
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d487d02740300000000000000
                   0000006a0200000000000000006401a00300000000000000000000000000
                   000000000000007c026a040000000000000000a6010000ab010000000000
                   0000006402a00300000000000000000000000000000000000000007c026a
                   040000000000000000a6010000ab0100000000000000007c01a6030000ab
                   0300000000000000007d018c497c015300
-               153           0 RESUME                   0
+               152           0 RESUME                   0
                
-               154           2 LOAD_FAST                0 (self)
+               153           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
                             14 GET_ITER
                        >>   16 FOR_ITER                72 (to 162)
                             18 STORE_FAST               2 (field)
                
-               155          20 LOAD_GLOBAL              3 (NULL + re)
+               154          20 LOAD_GLOBAL              3 (NULL + re)
                             32 LOAD_ATTR                2 (sub)
                             42 LOAD_CONST               1 ('{}(?=,|\\]|\\)|-|\\+|/|\\*| |$)')
                
-               156          44 LOAD_METHOD              3 (format)
+               155          44 LOAD_METHOD              3 (format)
                             66 LOAD_FAST                2 (field)
                             68 LOAD_ATTR                4 (id)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 LOAD_CONST               2 ("float(getattr(self, '{}'))")
                             94 LOAD_METHOD              3 (format)
                            116 LOAD_FAST                2 (field)
                            118 LOAD_ATTR                4 (id)
                            128 PRECALL                  1
                            132 CALL                     1
                            142 LOAD_FAST                1 (calculationString)
                
-               155         144 PRECALL                  3
+               154         144 PRECALL                  3
                            148 CALL                     3
                            158 STORE_FAST               1 (calculationString)
                            160 JUMP_BACKWARD           73 (to 16)
                
-               158     >>  162 LOAD_FAST                1 (calculationString)
+               157     >>  162 LOAD_FAST                1 (calculationString)
                            164 RETURN_VALUE
                consts
                   None
                   '{}(?=,|\\]|\\)|-|\\+|/|\\*| |$)'
                   "float(getattr(self, '{}'))"
                names      ('_JSONQuestionnaire__fields', 're', 'sub', 'format', 'id')
                varnames   ('self', 'calculationString', 'field')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'preprocess_calculation_string'
-               firstlineno 153
+               firstlineno 152
                lnotab 0x02011201180164ff1203
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -1361,73 +1361,73 @@
                   000000000044005d5e7d027c026a03000000000000000072207409000000
                   000000000000007c017c026a0500000000000000007c026a030000000000
                   0000006a060000000000000000a6030000ab03000000000000000001007c
                   026a0700000000000000007410000000000000000000006a090000000000
                   0000006b020000000072207409000000000000000000007c017c026a0500
                   000000000000007414000000000000000000006a0b0000000000000000a6
                   030000ab03000000000000000001008c5f7c015300
-               160           0 RESUME                   0
+               159           0 RESUME                   0
                
-               161           2 LOAD_FAST                0 (self)
+               160           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (db_class)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (blank)
                
-               163          42 LOAD_FAST                1 (blank)
+               162          42 LOAD_FAST                1 (blank)
                             44 LOAD_ATTR                1 (__table__)
                             54 LOAD_ATTR                2 (c)
                             64 GET_ITER
                        >>   66 FOR_ITER                94 (to 256)
                             68 STORE_FAST               2 (column)
                
-               164          70 LOAD_FAST                2 (column)
+               163          70 LOAD_FAST                2 (column)
                             72 LOAD_ATTR                3 (default)
                             82 POP_JUMP_FORWARD_IF_FALSE    32 (to 148)
                
-               165          84 LOAD_GLOBAL              9 (NULL + setattr)
+               164          84 LOAD_GLOBAL              9 (NULL + setattr)
                             96 LOAD_FAST                1 (blank)
                             98 LOAD_FAST                2 (column)
                            100 LOAD_ATTR                5 (name)
                            110 LOAD_FAST                2 (column)
                            112 LOAD_ATTR                3 (default)
                            122 LOAD_ATTR                6 (arg)
                            132 PRECALL                  3
                            136 CALL                     3
                            146 POP_TOP
                
-               166     >>  148 LOAD_FAST                2 (column)
-                           150 LOAD_ATTR                7 (data_type)
+               165     >>  148 LOAD_FAST                2 (column)
+                           150 LOAD_ATTR                7 (type)
                            160 LOAD_GLOBAL             16 (db)
                            172 LOAD_ATTR                9 (DateTime)
                            182 COMPARE_OP               2 (==)
                            188 POP_JUMP_FORWARD_IF_FALSE    32 (to 254)
                
-               167         190 LOAD_GLOBAL              9 (NULL + setattr)
+               166         190 LOAD_GLOBAL              9 (NULL + setattr)
                            202 LOAD_FAST                1 (blank)
                            204 LOAD_FAST                2 (column)
                            206 LOAD_ATTR                5 (name)
                            216 LOAD_GLOBAL             20 (datetime)
                            228 LOAD_ATTR               11 (min)
                            238 PRECALL                  3
                            242 CALL                     3
                            252 POP_TOP
                        >>  254 JUMP_BACKWARD           95 (to 66)
                
-               169     >>  256 LOAD_FAST                1 (blank)
+               168     >>  256 LOAD_FAST                1 (blank)
                            258 RETURN_VALUE
                consts
                   None
-               names      ('db_class', '__table__', 'c', 'default', 'setattr', 'name', 'arg', 'data_type', 'db', 'DateTime', 'datetime', 'min')
+               names      ('db_class', '__table__', 'c', 'default', 'setattr', 'name', 'arg', 'type', 'db', 'DateTime', 'datetime', 'min')
                varnames   ('self', 'blank', 'column')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'create_blank'
-               firstlineno 160
+               firstlineno 159
                lnotab 0x020128021c010e0140012a014202
             ''
             code
                argcount  : 2
                nlocals   : 14
                stacksize : 8
                flags     : 3
@@ -1509,88 +1509,88 @@
                   0000007c04a6010000ab0100000000000000007a00000064187a00000074
                   210000000000000000000074020000000000000000000064011900000000
                   0000000000a6010000ab0100000000000000007a00000064197a00000074
                   61000000000000000000006a310000000000000000741600000000000000
                   0000006a0c0000000000000000a6010000ab0100000000000000007a0000
                   00641a7a000000a6010000ab010000000000000000010064005300640053
                   0064005300
-               171           0 RESUME                   0
+               170           0 RESUME                   0
                
-               173           2 LOAD_GLOBAL              0 (db)
+               172           2 LOAD_GLOBAL              0 (db)
                             14 LOAD_ATTR                1 (session)
                             24 LOAD_METHOD              2 (query)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (db_class)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (filter)
                
-               174          94 LOAD_FAST                0 (self)
+               173          94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (db_class)
                            106 LOAD_ATTR                5 (participantID)
                            116 LOAD_GLOBAL              2 (session)
                            128 LOAD_CONST               1 ('participantID')
                            130 BINARY_SUBSCR
                            140 COMPARE_OP               2 (==)
                
-               175         146 LOAD_FAST                0 (self)
+               174         146 LOAD_FAST                0 (self)
                            148 LOAD_ATTR                3 (db_class)
                            158 LOAD_ATTR                6 (tag)
                            168 LOAD_FAST                1 (tag)
                            170 COMPARE_OP               2 (==)
                
-               173         176 PRECALL                  2
+               172         176 PRECALL                  2
                            180 CALL                     2
                
-               176         190 LOAD_METHOD              7 (all)
+               175         190 LOAD_METHOD              7 (all)
                            212 PRECALL                  0
                            216 CALL                     0
                
-               173         226 STORE_FAST               2 (previous)
+               172         226 STORE_FAST               2 (previous)
                
-               178         228 LOAD_FAST                2 (previous)
+               177         228 LOAD_FAST                2 (previous)
                            230 POP_JUMP_FORWARD_IF_FALSE    28 (to 288)
                            232 LOAD_GLOBAL             17 (NULL + len)
                            244 LOAD_FAST                2 (previous)
                            246 PRECALL                  1
                            250 CALL                     1
                            260 LOAD_CONST               2 (1)
                            262 COMPARE_OP               2 (==)
                            268 POP_JUMP_FORWARD_IF_FALSE     9 (to 288)
                
-               179         270 LOAD_FAST                2 (previous)
+               178         270 LOAD_FAST                2 (previous)
                            272 LOAD_CONST               3 (0)
                            274 BINARY_SUBSCR
                            284 STORE_FAST               3 (new_object)
                            286 JUMP_FORWARD            20 (to 328)
                
-               181     >>  288 LOAD_FAST                0 (self)
+               180     >>  288 LOAD_FAST                0 (self)
                            290 LOAD_METHOD              3 (db_class)
                            312 PRECALL                  0
                            316 CALL                     0
                            326 STORE_FAST               3 (new_object)
                
-               185     >>  328 NOP
+               184     >>  328 NOP
                
-               186         330 LOAD_GLOBAL             19 (NULL + datetime)
+               185         330 LOAD_GLOBAL             19 (NULL + datetime)
                            342 LOAD_ATTR               10 (strptime)
                            352 LOAD_GLOBAL             22 (request)
                            364 LOAD_ATTR               12 (form)
                            374 LOAD_CONST               4 ('timeStarted')
                            376 BINARY_SUBSCR
                            386 LOAD_CONST               5 ('%Y-%m-%d %H:%M:%S.%f')
                            388 PRECALL                  2
                            392 CALL                     2
                            402 STORE_FAST               4 (timeStarted)
                            404 JUMP_FORWARD            44 (to 494)
                        >>  406 PUSH_EXC_INFO
                
-               187         408 POP_TOP
+               186         408 POP_TOP
                
-               188         410 LOAD_GLOBAL             19 (NULL + datetime)
+               187         410 LOAD_GLOBAL             19 (NULL + datetime)
                            422 LOAD_ATTR               10 (strptime)
                            432 LOAD_GLOBAL             22 (request)
                            444 LOAD_ATTR               12 (form)
                            454 LOAD_CONST               4 ('timeStarted')
                            456 BINARY_SUBSCR
                            466 LOAD_CONST               6 ('%Y-%m-%d %H:%M:%S')
                            468 PRECALL                  2
@@ -1598,15 +1598,15 @@
                            482 STORE_FAST               4 (timeStarted)
                            484 POP_EXCEPT
                            486 JUMP_FORWARD             3 (to 494)
                        >>  488 COPY                     3
                            490 POP_EXCEPT
                            492 RERAISE                  1
                
-               191     >>  494 LOAD_FAST                0 (self)
+               190     >>  494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               13 (_JSONQuestionnaire__fields)
                            506 POP_JUMP_FORWARD_IF_FALSE    53 (to 614)
                            508 LOAD_GLOBAL             17 (NULL + len)
                            520 LOAD_FAST                0 (self)
                            522 LOAD_ATTR               13 (_JSONQuestionnaire__fields)
                            532 PRECALL                  1
                            536 CALL                     1
@@ -1619,197 +1619,197 @@
                            580 PRECALL                  1
                            584 CALL                     1
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR               14 (_JSONQuestionnaire__field_count)
                            606 COMPARE_OP               3 (!=)
                            612 POP_JUMP_FORWARD_IF_FALSE    20 (to 654)
                
-               192     >>  614 LOAD_FAST                0 (self)
+               191     >>  614 LOAD_FAST                0 (self)
                            616 LOAD_METHOD             15 (fetch_fields)
                            638 PRECALL                  0
                            642 CALL                     0
                            652 POP_TOP
                
-               198     >>  654 NOP
+               197     >>  654 NOP
                
-               199         656 LOAD_GLOBAL             33 (NULL + str)
+               198         656 LOAD_GLOBAL             33 (NULL + str)
                            668 LOAD_GLOBAL             22 (request)
                            680 LOAD_ATTR               12 (form)
                            690 LOAD_CONST               7 ('gridItemClicks')
                            692 BINARY_SUBSCR
                            702 PRECALL                  1
                            706 CALL                     1
                            716 LOAD_METHOD             17 (split)
                            738 LOAD_CONST               8 (';')
                            740 PRECALL                  1
                            744 CALL                     1
                            754 GET_ITER
                        >>  756 FOR_ITER               223 (to 1204)
                            758 STORE_FAST               5 (click_event)
                
-               200         760 LOAD_GLOBAL             17 (NULL + len)
+               199         760 LOAD_GLOBAL             17 (NULL + len)
                            772 LOAD_FAST                5 (click_event)
                            774 PRECALL                  1
                            778 CALL                     1
                            788 LOAD_CONST               3 (0)
                            790 COMPARE_OP               2 (==)
                            796 POP_JUMP_FORWARD_IF_FALSE     1 (to 800)
                
-               201         798 JUMP_BACKWARD           22 (to 756)
+               200         798 JUMP_BACKWARD           22 (to 756)
                
-               203     >>  800 LOAD_FAST                5 (click_event)
+               202     >>  800 LOAD_FAST                5 (click_event)
                            802 LOAD_METHOD             18 (replace)
                            824 LOAD_CONST               9 ('\\')
                            826 LOAD_CONST              10 ('')
                            828 PRECALL                  2
                            832 CALL                     2
                            842 STORE_FAST               5 (click_event)
                
-               204         844 LOAD_GLOBAL             39 (NULL + json)
+               203         844 LOAD_GLOBAL             39 (NULL + json)
                            856 LOAD_ATTR               20 (loads)
                            866 LOAD_FAST                5 (click_event)
                            868 PRECALL                  1
                            872 CALL                     1
                            882 STORE_FAST               6 (click_event_dict)
                
-               206         884 LOAD_GLOBAL             19 (NULL + datetime)
+               205         884 LOAD_GLOBAL             19 (NULL + datetime)
                            896 LOAD_ATTR               21 (fromtimestamp)
                            906 LOAD_GLOBAL             45 (NULL + float)
                            918 LOAD_FAST                6 (click_event_dict)
                            920 LOAD_CONST              11 ('time')
                            922 BINARY_SUBSCR
                            932 PRECALL                  1
                            936 CALL                     1
                            946 PRECALL                  1
                            950 CALL                     1
                            960 STORE_FAST               7 (parsed_time)
                
-               208         962 LOAD_GLOBAL              1 (NULL + db)
+               207         962 LOAD_GLOBAL              1 (NULL + db)
                            974 LOAD_ATTR               23 (RadioGridLog)
                            984 PRECALL                  0
                            988 CALL                     0
                            998 STORE_FAST               8 (new_log)
                
-               209        1000 LOAD_GLOBAL              2 (session)
+               208        1000 LOAD_GLOBAL              2 (session)
                           1012 LOAD_CONST               1 ('participantID')
                           1014 BINARY_SUBSCR
                           1024 LOAD_FAST                8 (new_log)
                           1026 STORE_ATTR               5 (participantID)
                
-               210        1036 LOAD_FAST                0 (self)
+               209        1036 LOAD_FAST                0 (self)
                           1038 LOAD_ATTR               24 (file_name)
                           1048 LOAD_FAST                8 (new_log)
                           1050 STORE_ATTR              25 (questionnaire)
                
-               211        1060 LOAD_FAST                1 (tag)
+               210        1060 LOAD_FAST                1 (tag)
                           1062 LOAD_FAST                8 (new_log)
                           1064 STORE_ATTR               6 (tag)
                
-               212        1074 LOAD_FAST                6 (click_event_dict)
+               211        1074 LOAD_FAST                6 (click_event_dict)
                           1076 LOAD_CONST              12 ('id')
                           1078 BINARY_SUBSCR
                           1088 LOAD_FAST                8 (new_log)
                           1090 STORE_ATTR              26 (questionID)
                
-               213        1100 LOAD_FAST                7 (parsed_time)
+               212        1100 LOAD_FAST                7 (parsed_time)
                           1102 LOAD_FAST                8 (new_log)
                           1104 STORE_ATTR              27 (timeClicked)
                
-               214        1114 LOAD_FAST                6 (click_event_dict)
+               213        1114 LOAD_FAST                6 (click_event_dict)
                           1116 LOAD_CONST              13 ('value')
                           1118 BINARY_SUBSCR
                           1128 LOAD_FAST                8 (new_log)
                           1130 STORE_ATTR              28 (value)
                
-               216        1140 LOAD_GLOBAL              0 (db)
+               215        1140 LOAD_GLOBAL              0 (db)
                           1152 LOAD_ATTR                1 (session)
                           1162 LOAD_METHOD             29 (add)
                           1184 LOAD_FAST                8 (new_log)
                           1186 PRECALL                  1
                           1190 CALL                     1
                           1200 POP_TOP
                           1202 JUMP_BACKWARD          224 (to 756)
                
-               218     >> 1204 LOAD_GLOBAL              0 (db)
+               217     >> 1204 LOAD_GLOBAL              0 (db)
                           1216 LOAD_ATTR                1 (session)
                           1226 LOAD_METHOD             30 (commit)
                           1248 PRECALL                  0
                           1252 CALL                     0
                           1262 POP_TOP
                           1264 JUMP_FORWARD             7 (to 1280)
                        >> 1266 PUSH_EXC_INFO
                
-               220        1268 POP_TOP
+               219        1268 POP_TOP
                
-               221        1270 POP_EXCEPT
+               220        1270 POP_EXCEPT
                           1272 JUMP_FORWARD             3 (to 1280)
                        >> 1274 COPY                     3
                           1276 POP_EXCEPT
                           1278 RERAISE                  1
                
-               223     >> 1280 LOAD_FAST                0 (self)
+               222     >> 1280 LOAD_FAST                0 (self)
                           1282 LOAD_ATTR               13 (_JSONQuestionnaire__fields)
                           1292 GET_ITER
                        >> 1294 FOR_ITER               173 (to 1642)
                           1296 STORE_FAST               9 (field)
                
-               226        1298 NOP
+               225        1298 NOP
                
-               227        1300 LOAD_GLOBAL             22 (request)
+               226        1300 LOAD_GLOBAL             22 (request)
                           1312 LOAD_ATTR               12 (form)
                           1322 LOAD_METHOD             31 (get)
                           1344 LOAD_FAST                9 (field)
                           1346 LOAD_ATTR               32 (id)
                           1356 LOAD_CONST               0 (None)
                           1358 PRECALL                  2
                           1362 CALL                     2
                           1372 STORE_FAST              10 (value)
                
-               228        1374 LOAD_FAST               10 (value)
+               227        1374 LOAD_FAST               10 (value)
                           1376 POP_JUMP_FORWARD_IF_NONE    23 (to 1424)
                
-               229        1378 LOAD_GLOBAL             67 (NULL + setattr)
+               228        1378 LOAD_GLOBAL             67 (NULL + setattr)
                           1390 LOAD_FAST                3 (new_object)
                           1392 LOAD_FAST                9 (field)
                           1394 LOAD_ATTR               32 (id)
                           1404 LOAD_FAST               10 (value)
                           1406 PRECALL                  3
                           1410 CALL                     3
                           1420 POP_TOP
                           1422 JUMP_FORWARD            65 (to 1554)
                
-               231     >> 1424 LOAD_GLOBAL             69 (NULL + getattr)
+               230     >> 1424 LOAD_GLOBAL             69 (NULL + getattr)
                           1436 LOAD_FAST                0 (self)
                           1438 LOAD_ATTR                3 (db_class)
                           1448 LOAD_FAST                9 (field)
                           1450 LOAD_ATTR               32 (id)
                           1460 PRECALL                  2
                           1464 CALL                     2
                           1474 STORE_FAST              11 (attr)
                
-               232        1476 LOAD_FAST               11 (attr)
+               231        1476 LOAD_FAST               11 (attr)
                           1478 LOAD_ATTR               35 (expression)
                           1488 LOAD_ATTR               36 (default)
                           1498 LOAD_ATTR               37 (arg)
                           1508 STORE_FAST              12 (default)
                
-               233        1510 LOAD_GLOBAL             67 (NULL + setattr)
+               232        1510 LOAD_GLOBAL             67 (NULL + setattr)
                           1522 LOAD_FAST                3 (new_object)
                           1524 LOAD_FAST                9 (field)
                           1526 LOAD_ATTR               32 (id)
                           1536 LOAD_FAST               12 (default)
                           1538 PRECALL                  3
                           1542 CALL                     3
                           1552 POP_TOP
                        >> 1554 JUMP_BACKWARD          131 (to 1294)
                        >> 1556 PUSH_EXC_INFO
                
-               234        1558 POP_TOP
+               233        1558 POP_TOP
                
-               235        1560 LOAD_GLOBAL             77 (NULL + print)
+               234        1560 LOAD_GLOBAL             77 (NULL + print)
                           1572 LOAD_CONST              14 ('Could not write field ')
                           1574 LOAD_GLOBAL             33 (NULL + str)
                           1586 LOAD_FAST                9 (field)
                           1588 LOAD_ATTR               32 (id)
                           1598 PRECALL                  1
                           1602 CALL                     1
                           1612 BINARY_OP                0 (+)
@@ -1818,107 +1818,107 @@
                           1630 POP_TOP
                           1632 POP_EXCEPT
                           1634 JUMP_BACKWARD          171 (to 1294)
                        >> 1636 COPY                     3
                           1638 POP_EXCEPT
                           1640 RERAISE                  1
                
-               238     >> 1642 LOAD_GLOBAL             67 (NULL + setattr)
+               237     >> 1642 LOAD_GLOBAL             67 (NULL + setattr)
                           1654 LOAD_FAST                3 (new_object)
                           1656 LOAD_CONST               1 ('participantID')
                           1658 LOAD_GLOBAL              2 (session)
                           1670 LOAD_CONST               1 ('participantID')
                           1672 BINARY_SUBSCR
                           1682 PRECALL                  3
                           1686 CALL                     3
                           1696 POP_TOP
                
-               239        1698 LOAD_GLOBAL             67 (NULL + setattr)
+               238        1698 LOAD_GLOBAL             67 (NULL + setattr)
                           1710 LOAD_FAST                3 (new_object)
                           1712 LOAD_CONST               4 ('timeStarted')
                           1714 LOAD_FAST                4 (timeStarted)
                           1716 PRECALL                  3
                           1720 CALL                     3
                           1730 POP_TOP
                
-               240        1732 LOAD_GLOBAL             67 (NULL + setattr)
+               239        1732 LOAD_GLOBAL             67 (NULL + setattr)
                           1744 LOAD_FAST                3 (new_object)
                           1746 LOAD_CONST              15 ('timeEnded')
                           1748 LOAD_GLOBAL             19 (NULL + datetime)
                           1760 LOAD_ATTR               39 (utcnow)
                           1770 PRECALL                  0
                           1774 CALL                     0
                           1784 PRECALL                  3
                           1788 CALL                     3
                           1798 POP_TOP
                
-               241        1800 LOAD_GLOBAL             67 (NULL + setattr)
+               240        1800 LOAD_GLOBAL             67 (NULL + setattr)
                           1812 LOAD_FAST                3 (new_object)
                           1814 LOAD_CONST              16 ('tag')
                           1816 LOAD_FAST                1 (tag)
                           1818 PRECALL                  3
                           1822 CALL                     3
                           1832 POP_TOP
                
-               243        1834 LOAD_GLOBAL              0 (db)
+               242        1834 LOAD_GLOBAL              0 (db)
                           1846 LOAD_ATTR                1 (session)
                           1856 LOAD_METHOD             29 (add)
                           1878 LOAD_FAST                3 (new_object)
                           1880 PRECALL                  1
                           1884 CALL                     1
                           1894 POP_TOP
                
-               244        1896 LOAD_GLOBAL              0 (db)
+               243        1896 LOAD_GLOBAL              0 (db)
                           1908 LOAD_ATTR                1 (session)
                           1918 LOAD_METHOD             30 (commit)
                           1940 PRECALL                  0
                           1944 CALL                     0
                           1954 POP_TOP
                
-               246        1956 LOAD_CONST              17 ('ENABLE_LOGGING')
+               245        1956 LOAD_CONST              17 ('ENABLE_LOGGING')
                           1958 LOAD_GLOBAL             80 (current_app)
                           1970 LOAD_ATTR               41 (config)
                           1980 CONTAINS_OP              0
                           1982 POP_JUMP_FORWARD_IF_FALSE   206 (to 2396)
                           1984 LOAD_GLOBAL             80 (current_app)
                           1996 LOAD_ATTR               41 (config)
                           2006 LOAD_CONST              17 ('ENABLE_LOGGING')
                           2008 BINARY_SUBSCR
                           2018 LOAD_CONST              18 (True)
                           2020 COMPARE_OP               2 (==)
                           2026 POP_JUMP_FORWARD_IF_FALSE   186 (to 2400)
                
-               247        2028 LOAD_GLOBAL             84 (os)
+               246        2028 LOAD_GLOBAL             84 (os)
                           2040 LOAD_ATTR               43 (path)
                           2050 LOAD_METHOD             44 (exists)
                           2072 LOAD_CONST              19 ('logs')
                           2074 PRECALL                  1
                           2078 CALL                     1
                           2088 POP_JUMP_FORWARD_IF_TRUE    20 (to 2130)
                
-               248        2090 LOAD_GLOBAL             85 (NULL + os)
+               247        2090 LOAD_GLOBAL             85 (NULL + os)
                           2102 LOAD_ATTR               45 (makedirs)
                           2112 LOAD_CONST              19 ('logs')
                           2114 PRECALL                  1
                           2118 CALL                     1
                           2128 POP_TOP
                
-               250     >> 2130 LOAD_GLOBAL             93 (NULL + open)
+               249     >> 2130 LOAD_GLOBAL             93 (NULL + open)
                           2142 LOAD_CONST              20 ('logs/')
                           2144 LOAD_FAST                0 (self)
                           2146 LOAD_ATTR               24 (file_name)
                           2156 BINARY_OP                0 (+)
                           2160 LOAD_CONST              21 ('.txt')
                           2162 BINARY_OP                0 (+)
                           2166 LOAD_CONST              22 ('a+')
                           2168 PRECALL                  2
                           2172 CALL                     2
                           2182 STORE_FAST              13 (f)
                
-               251        2184 LOAD_FAST               13 (f)
+               250        2184 LOAD_FAST               13 (f)
                           2186 LOAD_METHOD             47 (write)
                           2208 LOAD_CONST              23 ('Time = ')
                           2210 LOAD_GLOBAL             33 (NULL + str)
                           2222 LOAD_FAST                4 (timeStarted)
                           2224 PRECALL                  1
                           2228 CALL                     1
                           2238 BINARY_OP                0 (+)
@@ -1944,15 +1944,15 @@
                           2372 BINARY_OP                0 (+)
                           2376 PRECALL                  1
                           2380 CALL                     1
                           2390 POP_TOP
                           2392 LOAD_CONST               0 (None)
                           2394 RETURN_VALUE
                
-               246     >> 2396 LOAD_CONST               0 (None)
+               245     >> 2396 LOAD_CONST               0 (None)
                           2398 RETURN_VALUE
                        >> 2400 LOAD_CONST               0 (None)
                           2402 RETURN_VALUE
                ExceptionTable:
                  330 to 402 -> 406 [0]
                  406 to 482 -> 488 [1] lasti
                  656 to 1262 -> 1266 [0]
@@ -1989,74 +1989,74 @@
                   '\n\n'
                names      ('db', 'session', 'query', 'db_class', 'filter', 'participantID', 'tag', 'all', 'len', 'datetime', 'strptime', 'request', 'form', '_JSONQuestionnaire__fields', '_JSONQuestionnaire__field_count', 'fetch_fields', 'str', 'split', 'replace', 'json', 'loads', 'fromtimestamp', 'float', 'RadioGridLog', 'file_name', 'questionnaire', 'questionID', 'timeClicked', 'value', 'add', 'commit', 'get', 'id', 'setattr', 'getattr', 'expression', 'default', 'arg', 'print', 'utcnow', 'current_app', 'config', 'os', 'path', 'exists', 'makedirs', 'open', 'write', 'pprint', 'pformat')
                varnames   ('self', 'tag', 'previous', 'new_object', 'timeStarted', 'click_event', 'click_event_dict', 'parsed_time', 'new_log', 'field', 'value', 'attr', 'default', 'f')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'handle_questionnaire'
-               firstlineno 171
+               firstlineno 170
                lnotab
                   0x02025c0134011efe0e0324fd02052a011202280402014e010201540378
                   01280602016801260102022c0128024e022601240118010e011a010e011a
                   024002400202010a02120302014a0104012e023401220130010201520338
                   012201440122023e013c0248013e0128023601d4fb
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d117d027c026a010000000000
                   0000007c016b020000000072047c026302010053008c1264005300
-               253           0 RESUME                   0
+               252           0 RESUME                   0
                
-               254           2 LOAD_FAST                0 (self)
+               253           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_JSONQuestionnaire__fields)
                             14 GET_ITER
                        >>   16 FOR_ITER                17 (to 52)
                             18 STORE_FAST               2 (f)
                
-               255          20 LOAD_FAST                2 (f)
+               254          20 LOAD_FAST                2 (f)
                             22 LOAD_ATTR                1 (id)
                             32 LOAD_FAST                1 (id)
                             34 COMPARE_OP               2 (==)
                             40 POP_JUMP_FORWARD_IF_FALSE     4 (to 50)
                
-               256          42 LOAD_FAST                2 (f)
+               255          42 LOAD_FAST                2 (f)
                             44 SWAP                     2
                             46 POP_TOP
                             48 RETURN_VALUE
                
-               255     >>   50 JUMP_BACKWARD           18 (to 16)
+               254     >>   50 JUMP_BACKWARD           18 (to 16)
                
-               257     >>   52 LOAD_CONST               0 (None)
+               256     >>   52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
                consts
                   None
                names      ('_JSONQuestionnaire__fields', 'id')
                varnames   ('self', 'id', 'f')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'get_field'
-               firstlineno 253
+               firstlineno 252
                lnotab 0x02011201160108ff0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   0000000000a6000000ab0000000000000000005300
-               259           0 RESUME                   0
+               258           0 RESUME                   0
                
-               260           2 LOAD_GLOBAL              0 (db)
+               259           2 LOAD_GLOBAL              0 (db)
                             14 LOAD_ATTR                1 (session)
                             24 LOAD_METHOD              2 (query)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (db_class)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (all)
@@ -2067,32 +2067,32 @@
                   None
                names      ('db', 'session', 'query', 'db_class', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'fetch_all_data'
-               firstlineno 259
+               firstlineno 258
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007400000000000000000000006a0500000000000000006a0600
                   0000000000000064016b0200000000a6010000ab010000000000000000a0
                   070000000000000000000000000000000000000000a6000000ab00000000
                   00000000005300
-               262           0 RESUME                   0
+               261           0 RESUME                   0
                
-               263           2 LOAD_GLOBAL              0 (db)
+               262           2 LOAD_GLOBAL              0 (db)
                             14 LOAD_ATTR                1 (session)
                             24 LOAD_METHOD              2 (query)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (db_class)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (filter)
@@ -2112,15 +2112,15 @@
                   True
                names      ('db', 'session', 'query', 'db_class', 'filter', 'Participant', 'finished', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'fetch_finished_data'
-               firstlineno 262
+               firstlineno 261
                lnotab 0x0201
             0
             True
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 9
@@ -2134,89 +2134,89 @@
                   000000000000006a0700000000000000007407000000000000000000007c
                   006a0400000000000000006401a6020000ab020000000000000000740000
                   0000000000000000006a0600000000000000006a0800000000000000006b
                   02000000007400000000000000000000006a0600000000000000006a0900
                   000000000000007c026b0200000000a6020000ab020000000000000000a6
                   020000ab0200000000000000007d047c04a00a0000000000000000000000
                   000000000000000000a6000000ab0000000000000000005300
-               266           0 RESUME                   0
+               265           0 RESUME                   0
                
-               273           2 LOAD_GLOBAL              0 (db)
+               272           2 LOAD_GLOBAL              0 (db)
                             14 LOAD_ATTR                1 (session)
                             24 LOAD_METHOD              2 (query)
                             46 LOAD_GLOBAL              7 (NULL + getattr)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                4 (db_class)
                             70 LOAD_FAST                1 (column)
                             72 PRECALL                  2
                             76 CALL                     2
                             86 PRECALL                  1
                             90 CALL                     1
                
-               274         100 LOAD_METHOD              5 (join)
+               273         100 LOAD_METHOD              5 (join)
                            122 LOAD_GLOBAL              0 (db)
                            134 LOAD_ATTR                6 (Participant)
                
-               275         144 LOAD_GLOBAL              1 (NULL + db)
+               274         144 LOAD_GLOBAL              1 (NULL + db)
                            156 LOAD_ATTR                7 (and_)
                
-               276         166 LOAD_GLOBAL              7 (NULL + getattr)
+               275         166 LOAD_GLOBAL              7 (NULL + getattr)
                            178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                4 (db_class)
                            190 LOAD_CONST               1 ('participantID')
                            192 PRECALL                  2
                            196 CALL                     2
                            206 LOAD_GLOBAL              0 (db)
                            218 LOAD_ATTR                6 (Participant)
                            228 LOAD_ATTR                8 (participantID)
                            238 COMPARE_OP               2 (==)
                
-               277         244 LOAD_GLOBAL              0 (db)
+               276         244 LOAD_GLOBAL              0 (db)
                            256 LOAD_ATTR                6 (Participant)
                            266 LOAD_ATTR                9 (condition)
                            276 LOAD_FAST                2 (condition)
                            278 COMPARE_OP               2 (==)
                
-               275         284 PRECALL                  2
+               274         284 PRECALL                  2
                            288 CALL                     2
                
-               274         298 PRECALL                  2
+               273         298 PRECALL                  2
                            302 CALL                     2
                
-               273         312 STORE_FAST               4 (q)
+               272         312 STORE_FAST               4 (q)
                
-               280         314 LOAD_FAST                4 (q)
+               279         314 LOAD_FAST                4 (q)
                            316 LOAD_METHOD             10 (all)
                            338 PRECALL                  0
                            342 CALL                     0
                            352 RETURN_VALUE
                consts
                   None
                   'participantID'
                names      ('db', 'session', 'query', 'getattr', 'db_class', 'join', 'Participant', 'and_', 'participantID', 'condition', 'all')
                varnames   ('self', 'column', 'condition', 'finishedOnly', 'q')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
                name       'fetch_column_data'
-               firstlineno 266
+               firstlineno 265
                lnotab 0x020762012c0116014e0128fe0eff0eff0207
             None
             ('',)
             (0, True)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'get_table_name', 'list', 'get_calculated_fields', 'fetch_fields', 'create_db_class', 'preprocess_calculation_string', 'create_blank', 'handle_questionnaire', 'get_field', 'fetch_all_data', 'fetch_finished_data', 'fetch_column_data')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
          name       'JSONQuestionnaire'
-         firstlineno 55
-         lnotab 0x0a01101106031803181c062e0607060b0852060606030604
+         firstlineno 56
+         lnotab 0x0a01101106031803181a062e0607060b0852060606030604
       'JSONQuestionnaire'
-   names      ('os', 'json', 're', 'pprint', 'flask', 'current_app', 'request', 'session', 'config', 'datetime', 'globals', 'db', 'object', 'JSONQuestionnaireColumn', 'JSONQuestionnaire')
+   names      ('os', 'json', 're', 'pprint', 'flask', 'current_app', 'request', 'session', 'config', 'datetime', 'globals', 'db', 'BOFS.util', 'mean', 'stdev', 'std', 'var', 'variance', 'median', 'object', 'JSONQuestionnaireColumn', 'JSONQuestionnaire')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONQuestionnaire.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080108010801080118010c010c031c2d
+   lnotab 0x00ff0201080108010801080118010c010c0120031c2d
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/JSONTable.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/JSONTable.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xceab1d66 (Mon Apr 15 22:35:58 2024 UTC)
-files sz: 6767
+moddate:  0xc0391f66 (Wed Apr 17 02:53:52 2024 UTC)
+files sz: 6858
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d025a0201
@@ -528,27 +528,27 @@
                       46 MAKE_FUNCTION            4 (annotations)
                       48 STORE_NAME               6 (get_columns)
          
           78          50 LOAD_CONST               7 (<code object create_db_class, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 78>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               7 (create_db_class)
          
-          97          56 LOAD_CONST               8 (<code object create_exports_dict, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 97>)
+          98          56 LOAD_CONST               8 (<code object create_exports_dict, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 98>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               8 (create_exports_dict)
          
-         109          62 LOAD_CONST               9 (<code object row_to_dict, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 109>)
+         110          62 LOAD_CONST               9 (<code object row_to_dict, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 110>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME               9 (row_to_dict)
          
-         130          68 LOAD_CONST              10 (<code object handle_post, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 130>)
+         131          68 LOAD_CONST              10 (<code object handle_post, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 131>)
                       70 MAKE_FUNCTION            0
                       72 STORE_NAME              10 (handle_post)
          
-         161          74 LOAD_CONST              11 (<code object handle_get, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 161>)
+         162          74 LOAD_CONST              11 (<code object handle_get, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 162>)
                       76 MAKE_FUNCTION            0
                       78 STORE_NAME              11 (handle_get)
                       80 LOAD_CONST              12 (None)
                       82 RETURN_VALUE
          consts
             'JSONTable'
             'directory'
@@ -731,242 +731,259 @@
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'get_columns'
                firstlineno 75
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 6
-               stacksize : 12
+               stacksize : 14
                flags     : 3
                code
-                  0x97007c006a0000000000000000007d0164017c01740200000000000000
-                  000000a002000000000000000000000000000000000000000064027c006a
-                  000000000000000000a6020000ab02000000000000000074070000000000
-                  00000000006a0400000000000000007406000000000000000000006a0500
-                  0000000000000064036403ac04a6030000ab030000000000000000640574
+                  0x970064017c006a0000000000000000007a0000007d0164027c01740200
+                  000000000000000000a00200000000000000000000000000000000000000
+                  0064037c006a000000000000000000a6020000ab02000000000000000074
                   07000000000000000000006a040000000000000000740600000000000000
-                  0000006a0500000000000000007407000000000000000000006a06000000
-                  00000000006406a6010000ab0100000000000000006407ac08a6030000ab
-                  03000000000000000064097407000000000000000000006a040000000000
-                  0000007406000000000000000000006a0700000000000000006407741000
-                  0000000000000000006a090000000000000000ac0aa6030000ab03000000
-                  000000000069047d027c006a0a0000000000000000640b19000000000000
-                  00000044005d567d037c006a0a0000000000000000640b19000000000000
-                  0000007c03190000000000000000007d047417000000000000000000007c
-                  037c04a6020000ab0200000000000000007d057c006a0c00000000000000
-                  00a00d00000000000000000000000000000000000000007c05a6010000ab
-                  01000000000000000001007c05a00e000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007c027c033c0000008c5774
-                  1f000000000000000000007c006a00000000000000000074060000000000
-                  00000000006a10000000000000000066017c02a6030000ab030000000000
-                  0000007c005f11000000000000000064005300
+                  0000006a05000000000000000064046404ac05a6030000ab030000000000
+                  00000064067407000000000000000000006a040000000000000000740600
+                  0000000000000000006a0500000000000000007407000000000000000000
+                  006a0600000000000000006407a6010000ab0100000000000000006408ac
+                  09a6030000ab030000000000000000640a7407000000000000000000006a
+                  070000000000000000640b7c01ac0ca6020000ab02000000000000000064
+                  0d7407000000000000000000006a04000000000000000074060000000000
+                  00000000006a08000000000000000064087412000000000000000000006a
+                  0a0000000000000000ac0ea6030000ab03000000000000000069057d027c
+                  006a0b0000000000000000640f1900000000000000000044005d567d037c
+                  006a0b0000000000000000640f190000000000000000007c031900000000
+                  00000000007d047419000000000000000000007c037c04a6020000ab0200
+                  000000000000007d057c006a0d0000000000000000a00e00000000000000
+                  000000000000000000000000007c05a6010000ab01000000000000000001
+                  007c05a00f0000000000000000000000000000000000000000a6000000ab
+                  0000000000000000007c027c033c0000008c577421000000000000000000
+                  007c006a0000000000000000007406000000000000000000006a11000000
+                  000000000066017c02a6030000ab0300000000000000007c005f12000000
+                  000000000064005300
                 78           0 RESUME                   0
                
-                79           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (file_name)
-                            14 STORE_FAST               1 (table_name)
-               
-                82          16 LOAD_CONST               1 ('__tablename__')
-                            18 LOAD_FAST                1 (table_name)
-               
-                83          20 LOAD_GLOBAL              2 (str)
-                            32 LOAD_METHOD              2 (format)
-                            54 LOAD_CONST               2 ('{0}ID')
-                            56 LOAD_FAST                0 (self)
-                            58 LOAD_ATTR                0 (file_name)
-                            68 PRECALL                  2
-                            72 CALL                     2
-                            82 LOAD_GLOBAL              7 (NULL + db)
-                            94 LOAD_ATTR                4 (Column)
-                           104 LOAD_GLOBAL              6 (db)
-                           116 LOAD_ATTR                5 (Integer)
-                           126 LOAD_CONST               3 (True)
-                           128 LOAD_CONST               3 (True)
-                           130 KW_NAMES                 4
-                           132 PRECALL                  3
-                           136 CALL                     3
-               
-                84         146 LOAD_CONST               5 ('participantID')
-                           148 LOAD_GLOBAL              7 (NULL + db)
-                           160 LOAD_ATTR                4 (Column)
-                           170 LOAD_GLOBAL              6 (db)
-                           182 LOAD_ATTR                5 (Integer)
-                           192 LOAD_GLOBAL              7 (NULL + db)
-                           204 LOAD_ATTR                6 (ForeignKey)
-                           214 LOAD_CONST               6 ('participant.participantID')
-                           216 PRECALL                  1
-                           220 CALL                     1
-                           230 LOAD_CONST               7 (False)
-                           232 KW_NAMES                 8
-                           234 PRECALL                  3
-                           238 CALL                     3
-               
-                85         248 LOAD_CONST               9 ('timeSubmitted')
-                           250 LOAD_GLOBAL              7 (NULL + db)
-                           262 LOAD_ATTR                4 (Column)
-                           272 LOAD_GLOBAL              6 (db)
-                           284 LOAD_ATTR                7 (DateTime)
-                           294 LOAD_CONST               7 (False)
-                           296 LOAD_GLOBAL             16 (datetime)
-                           308 LOAD_ATTR                9 (utcnow)
-                           318 KW_NAMES                10
-                           320 PRECALL                  3
-                           324 CALL                     3
-               
-                81         334 BUILD_MAP                4
-                           336 STORE_FAST               2 (table_attr)
-               
-                88         338 LOAD_FAST                0 (self)
-                           340 LOAD_ATTR               10 (json_data)
-                           350 LOAD_CONST              11 ('columns')
-                           352 BINARY_SUBSCR
-                           362 GET_ITER
-                       >>  364 FOR_ITER                86 (to 538)
-                           366 STORE_FAST               3 (column)
-               
-                89         368 LOAD_FAST                0 (self)
-                           370 LOAD_ATTR               10 (json_data)
-                           380 LOAD_CONST              11 ('columns')
-                           382 BINARY_SUBSCR
-                           392 LOAD_FAST                3 (column)
-                           394 BINARY_SUBSCR
-                           404 STORE_FAST               4 (column_details)
-               
-                90         406 LOAD_GLOBAL             23 (NULL + JSONTableColumn)
-                           418 LOAD_FAST                3 (column)
-                           420 LOAD_FAST                4 (column_details)
-                           422 PRECALL                  2
-                           426 CALL                     2
-                           436 STORE_FAST               5 (new_column)
-               
-                91         438 LOAD_FAST                0 (self)
-                           440 LOAD_ATTR               12 (_JSONTable__columns)
-                           450 LOAD_METHOD             13 (append)
-                           472 LOAD_FAST                5 (new_column)
-                           474 PRECALL                  1
-                           478 CALL                     1
-                           488 POP_TOP
-               
-                93         490 LOAD_FAST                5 (new_column)
-                           492 LOAD_METHOD             14 (generate_db_column)
-                           514 PRECALL                  0
-                           518 CALL                     0
-                           528 LOAD_FAST                2 (table_attr)
-                           530 LOAD_FAST                3 (column)
-                           532 STORE_SUBSCR
-                           536 JUMP_BACKWARD           87 (to 364)
-               
-                95     >>  538 LOAD_GLOBAL             31 (NULL + type)
-                           550 LOAD_FAST                0 (self)
-                           552 LOAD_ATTR                0 (file_name)
-                           562 LOAD_GLOBAL              6 (db)
-                           574 LOAD_ATTR               16 (Model)
-                           584 BUILD_TUPLE              1
-                           586 LOAD_FAST                2 (table_attr)
-                           588 PRECALL                  3
-                           592 CALL                     3
-                           602 LOAD_FAST                0 (self)
-                           604 STORE_ATTR              17 (db_class)
-                           614 LOAD_CONST               0 (None)
-                           616 RETURN_VALUE
+                79           2 LOAD_CONST               1 ('table_')
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (file_name)
+                            16 BINARY_OP                0 (+)
+                            20 STORE_FAST               1 (table_name)
+               
+                82          22 LOAD_CONST               2 ('__tablename__')
+                            24 LOAD_FAST                1 (table_name)
+               
+                83          26 LOAD_GLOBAL              2 (str)
+                            38 LOAD_METHOD              2 (format)
+                            60 LOAD_CONST               3 ('{0}ID')
+                            62 LOAD_FAST                0 (self)
+                            64 LOAD_ATTR                0 (file_name)
+                            74 PRECALL                  2
+                            78 CALL                     2
+                            88 LOAD_GLOBAL              7 (NULL + db)
+                           100 LOAD_ATTR                4 (Column)
+                           110 LOAD_GLOBAL              6 (db)
+                           122 LOAD_ATTR                5 (Integer)
+                           132 LOAD_CONST               4 (True)
+                           134 LOAD_CONST               4 (True)
+                           136 KW_NAMES                 5
+                           138 PRECALL                  3
+                           142 CALL                     3
+               
+                84         152 LOAD_CONST               6 ('participantID')
+                           154 LOAD_GLOBAL              7 (NULL + db)
+                           166 LOAD_ATTR                4 (Column)
+                           176 LOAD_GLOBAL              6 (db)
+                           188 LOAD_ATTR                5 (Integer)
+                           198 LOAD_GLOBAL              7 (NULL + db)
+                           210 LOAD_ATTR                6 (ForeignKey)
+                           220 LOAD_CONST               7 ('participant.participantID')
+                           222 PRECALL                  1
+                           226 CALL                     1
+                           236 LOAD_CONST               8 (False)
+                           238 KW_NAMES                 9
+                           240 PRECALL                  3
+                           244 CALL                     3
+               
+                85         254 LOAD_CONST              10 ('participant')
+                           256 LOAD_GLOBAL              7 (NULL + db)
+                           268 LOAD_ATTR                7 (relationship)
+                           278 LOAD_CONST              11 ('Participant')
+                           280 LOAD_FAST                1 (table_name)
+                           282 KW_NAMES                12
+                           284 PRECALL                  2
+                           288 CALL                     2
+               
+                86         298 LOAD_CONST              13 ('timeSubmitted')
+                           300 LOAD_GLOBAL              7 (NULL + db)
+                           312 LOAD_ATTR                4 (Column)
+                           322 LOAD_GLOBAL              6 (db)
+                           334 LOAD_ATTR                8 (DateTime)
+                           344 LOAD_CONST               8 (False)
+                           346 LOAD_GLOBAL             18 (datetime)
+                           358 LOAD_ATTR               10 (utcnow)
+                           368 KW_NAMES                14
+                           370 PRECALL                  3
+                           374 CALL                     3
+               
+                81         384 BUILD_MAP                5
+                           386 STORE_FAST               2 (table_attr)
+               
+                89         388 LOAD_FAST                0 (self)
+                           390 LOAD_ATTR               11 (json_data)
+                           400 LOAD_CONST              15 ('columns')
+                           402 BINARY_SUBSCR
+                           412 GET_ITER
+                       >>  414 FOR_ITER                86 (to 588)
+                           416 STORE_FAST               3 (column)
+               
+                90         418 LOAD_FAST                0 (self)
+                           420 LOAD_ATTR               11 (json_data)
+                           430 LOAD_CONST              15 ('columns')
+                           432 BINARY_SUBSCR
+                           442 LOAD_FAST                3 (column)
+                           444 BINARY_SUBSCR
+                           454 STORE_FAST               4 (column_details)
+               
+                91         456 LOAD_GLOBAL             25 (NULL + JSONTableColumn)
+                           468 LOAD_FAST                3 (column)
+                           470 LOAD_FAST                4 (column_details)
+                           472 PRECALL                  2
+                           476 CALL                     2
+                           486 STORE_FAST               5 (new_column)
+               
+                92         488 LOAD_FAST                0 (self)
+                           490 LOAD_ATTR               13 (_JSONTable__columns)
+                           500 LOAD_METHOD             14 (append)
+                           522 LOAD_FAST                5 (new_column)
+                           524 PRECALL                  1
+                           528 CALL                     1
+                           538 POP_TOP
+               
+                94         540 LOAD_FAST                5 (new_column)
+                           542 LOAD_METHOD             15 (generate_db_column)
+                           564 PRECALL                  0
+                           568 CALL                     0
+                           578 LOAD_FAST                2 (table_attr)
+                           580 LOAD_FAST                3 (column)
+                           582 STORE_SUBSCR
+                           586 JUMP_BACKWARD           87 (to 414)
+               
+                96     >>  588 LOAD_GLOBAL             33 (NULL + type)
+                           600 LOAD_FAST                0 (self)
+                           602 LOAD_ATTR                0 (file_name)
+                           612 LOAD_GLOBAL              6 (db)
+                           624 LOAD_ATTR               17 (Model)
+                           634 BUILD_TUPLE              1
+                           636 LOAD_FAST                2 (table_attr)
+                           638 PRECALL                  3
+                           642 CALL                     3
+                           652 LOAD_FAST                0 (self)
+                           654 STORE_ATTR              18 (db_class)
+                           664 LOAD_CONST               0 (None)
+                           666 RETURN_VALUE
                consts
                   None
+                  'table_'
                   '__tablename__'
                   '{0}ID'
                   True
                   ('primary_key', 'autoincrement')
                   'participantID'
                   'participant.participantID'
                   False
                   ('nullable',)
+                  'participant'
+                  'Participant'
+                  ('backref',)
                   'timeSubmitted'
                   ('nullable', 'default')
                   'columns'
-               names      ('file_name', 'str', 'format', 'db', 'Column', 'Integer', 'ForeignKey', 'DateTime', 'datetime', 'utcnow', 'json_data', 'JSONTableColumn', '_JSONTable__columns', 'append', 'generate_db_column', 'type', 'Model', 'db_class')
+               names      ('file_name', 'str', 'format', 'db', 'Column', 'Integer', 'ForeignKey', 'relationship', 'DateTime', 'datetime', 'utcnow', 'json_data', 'JSONTableColumn', '_JSONTable__columns', 'append', 'generate_db_column', 'type', 'Model', 'db_class')
                varnames   ('self', 'table_name', 'table_attr', 'column', 'column_details', 'new_column')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'create_db_class'
                firstlineno 78
-               lnotab 0x02010e0304017e01660156fc04071e012601200134023002
+               lnotab 0x0201140304017e0166012c0156fb04081e012601200134023002
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x970064017c006a000000000000000000760172026400530067007d0174
                   03000000000000000000007c006a00000000000000000064011900000000
                   0000000000a6010000ab01000000000000000064026b0400000000722f7c
                   006a00000000000000000064011900000000000000000044005d217d027c
                   006a0200000000000000007c0264033c0000007c01a00300000000000000
                   000000000000000000000000007c02a6010000ab01000000000000000001
                   008c227c015300
-                97           0 RESUME                   0
+                98           0 RESUME                   0
                
-                98           2 LOAD_CONST               1 ('exports')
+                99           2 LOAD_CONST               1 ('exports')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (json_data)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE     2 (to 24)
                
-                99          20 LOAD_CONST               0 (None)
+               100          20 LOAD_CONST               0 (None)
                             22 RETURN_VALUE
                
-               101     >>   24 BUILD_LIST               0
+               102     >>   24 BUILD_LIST               0
                             26 STORE_FAST               1 (exports_dict)
                
-               102          28 LOAD_GLOBAL              3 (NULL + len)
+               103          28 LOAD_GLOBAL              3 (NULL + len)
                             40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                0 (json_data)
                             52 LOAD_CONST               1 ('exports')
                             54 BINARY_SUBSCR
                             64 PRECALL                  1
                             68 CALL                     1
                             78 LOAD_CONST               2 (0)
                             80 COMPARE_OP               4 (>)
                             86 POP_JUMP_FORWARD_IF_FALSE    47 (to 182)
                
-               103          88 LOAD_FAST                0 (self)
+               104          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                0 (json_data)
                            100 LOAD_CONST               1 ('exports')
                            102 BINARY_SUBSCR
                            112 GET_ITER
                        >>  114 FOR_ITER                33 (to 182)
                            116 STORE_FAST               2 (export_definition)
                
-               104         118 LOAD_FAST                0 (self)
+               105         118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                2 (file_name)
                            130 LOAD_FAST                2 (export_definition)
                            132 LOAD_CONST               3 ('table')
                            134 STORE_SUBSCR
                
-               105         138 LOAD_FAST                1 (exports_dict)
+               106         138 LOAD_FAST                1 (exports_dict)
                            140 LOAD_METHOD              3 (append)
                            162 LOAD_FAST                2 (export_definition)
                            164 PRECALL                  1
                            168 CALL                     1
                            178 POP_TOP
                            180 JUMP_BACKWARD           34 (to 114)
                
-               107     >>  182 LOAD_FAST                1 (exports_dict)
+               108     >>  182 LOAD_FAST                1 (exports_dict)
                            184 RETURN_VALUE
                consts
                   None
                   'exports'
                   0
                   'table'
                names      ('json_data', 'len', 'file_name', 'append')
                varnames   ('self', 'exports_dict', 'export_definition')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'create_exports_dict'
-               firstlineno 97
+               firstlineno 98
                lnotab 0x02011201040204013c011e0114012c02
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 5
                flags     : 3
                code
@@ -979,129 +996,129 @@
                   021900000000000000000064046b02000000007213740700000000000000
                   0000007c05a6010000ab0100000000000000007c027c033c0000008c677c
                   0464021900000000000000000064056b0200000000721374090000000000
                   00000000007c05a6010000ab0100000000000000007c027c033c0000008c
                   86740b000000000000000000007c05a6010000ab0100000000000000007c
                   027c033c0000008c99740b000000000000000000007c05a6010000ab0100
                   000000000000007c027c033c0000008cac7c025300
-               109           0 RESUME                   0
+               110           0 RESUME                   0
                
-               110           2 BUILD_MAP                0
+               111           2 BUILD_MAP                0
                              4 STORE_FAST               2 (result)
                
-               112           6 LOAD_FAST                0 (self)
+               113           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (json_data)
                             18 LOAD_CONST               1 ('columns')
                             20 BINARY_SUBSCR
                             30 GET_ITER
                        >>   32 FOR_ITER               171 (to 376)
                             34 STORE_FAST               3 (column)
                
-               113          36 LOAD_FAST                0 (self)
+               114          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                0 (json_data)
                             48 LOAD_CONST               1 ('columns')
                             50 BINARY_SUBSCR
                             60 LOAD_FAST                3 (column)
                             62 BINARY_SUBSCR
                             72 STORE_FAST               4 (column_details)
                
-               114          74 LOAD_GLOBAL              3 (NULL + getattr)
+               115          74 LOAD_GLOBAL              3 (NULL + getattr)
                             86 LOAD_FAST                1 (row)
                             88 LOAD_FAST                3 (column)
                             90 PRECALL                  2
                             94 CALL                     2
                            104 STORE_FAST               5 (value)
                
-               116         106 LOAD_CONST               2 ('type')
+               117         106 LOAD_CONST               2 ('type')
                            108 LOAD_FAST                4 (column_details)
                            110 CONTAINS_OP              0
                            112 POP_JUMP_FORWARD_IF_FALSE   112 (to 338)
                
-               117         114 LOAD_FAST                4 (column_details)
+               118         114 LOAD_FAST                4 (column_details)
                            116 LOAD_CONST               2 ('type')
                            118 BINARY_SUBSCR
                            128 LOAD_CONST               3 ('integer')
                            130 COMPARE_OP               2 (==)
                            136 POP_JUMP_FORWARD_IF_FALSE    19 (to 176)
                
-               118         138 LOAD_GLOBAL              5 (NULL + int)
+               119         138 LOAD_GLOBAL              5 (NULL + int)
                            150 LOAD_FAST                5 (value)
                            152 PRECALL                  1
                            156 CALL                     1
                            166 LOAD_FAST                2 (result)
                            168 LOAD_FAST                3 (column)
                            170 STORE_SUBSCR
                            174 JUMP_BACKWARD           72 (to 32)
                
-               119     >>  176 LOAD_FAST                4 (column_details)
+               120     >>  176 LOAD_FAST                4 (column_details)
                            178 LOAD_CONST               2 ('type')
                            180 BINARY_SUBSCR
                            190 LOAD_CONST               4 ('float')
                            192 COMPARE_OP               2 (==)
                            198 POP_JUMP_FORWARD_IF_FALSE    19 (to 238)
                
-               120         200 LOAD_GLOBAL              7 (NULL + float)
+               121         200 LOAD_GLOBAL              7 (NULL + float)
                            212 LOAD_FAST                5 (value)
                            214 PRECALL                  1
                            218 CALL                     1
                            228 LOAD_FAST                2 (result)
                            230 LOAD_FAST                3 (column)
                            232 STORE_SUBSCR
                            236 JUMP_BACKWARD          103 (to 32)
                
-               121     >>  238 LOAD_FAST                4 (column_details)
+               122     >>  238 LOAD_FAST                4 (column_details)
                            240 LOAD_CONST               2 ('type')
                            242 BINARY_SUBSCR
                            252 LOAD_CONST               5 ('boolean')
                            254 COMPARE_OP               2 (==)
                            260 POP_JUMP_FORWARD_IF_FALSE    19 (to 300)
                
-               122         262 LOAD_GLOBAL              9 (NULL + bool)
+               123         262 LOAD_GLOBAL              9 (NULL + bool)
                            274 LOAD_FAST                5 (value)
                            276 PRECALL                  1
                            280 CALL                     1
                            290 LOAD_FAST                2 (result)
                            292 LOAD_FAST                3 (column)
                            294 STORE_SUBSCR
                            298 JUMP_BACKWARD          134 (to 32)
                
-               124     >>  300 LOAD_GLOBAL             11 (NULL + str)
+               125     >>  300 LOAD_GLOBAL             11 (NULL + str)
                            312 LOAD_FAST                5 (value)
                            314 PRECALL                  1
                            318 CALL                     1
                            328 LOAD_FAST                2 (result)
                            330 LOAD_FAST                3 (column)
                            332 STORE_SUBSCR
                            336 JUMP_BACKWARD          153 (to 32)
                
-               126     >>  338 LOAD_GLOBAL             11 (NULL + str)
+               127     >>  338 LOAD_GLOBAL             11 (NULL + str)
                            350 LOAD_FAST                5 (value)
                            352 PRECALL                  1
                            356 CALL                     1
                            366 LOAD_FAST                2 (result)
                            368 LOAD_FAST                3 (column)
                            370 STORE_SUBSCR
                            374 JUMP_BACKWARD          172 (to 32)
                
-               128     >>  376 LOAD_FAST                2 (result)
+               129     >>  376 LOAD_FAST                2 (result)
                            378 RETURN_VALUE
                consts
                   None
                   'columns'
                   'type'
                   'integer'
                   'float'
                   'boolean'
                names      ('json_data', 'getattr', 'int', 'float', 'bool', 'str')
                varnames   ('self', 'row', 'result', 'column', 'column_details', 'value')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'row_to_dict'
-               firstlineno 109
+               firstlineno 110
                lnotab 0x020104021e0126012002080118012601180126011801260226022602
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 8
                flags     : 3
                code
@@ -1125,169 +1142,169 @@
                   00000000007c017c037c05a6030000ab03000000000000000001008cb874
                   0f000000000000000000007c017c037c05a6030000ab0300000000000000
                   0001008cca7416000000000000000000006a010000000000000000a00c00
                   000000000000000000000000000000000000007c01a6010000ab01000000
                   000000000001007416000000000000000000006a010000000000000000a0
                   0d0000000000000000000000000000000000000000a6000000ab00000000
                   0000000000010064075300
-               130           0 RESUME                   0
+               131           0 RESUME                   0
                
-               131           2 LOAD_FAST                0 (self)
+               132           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (db_class)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (entry)
                
-               132          42 LOAD_GLOBAL              2 (session)
+               133          42 LOAD_GLOBAL              2 (session)
                             54 LOAD_CONST               1 ('participantID')
                             56 BINARY_SUBSCR
                             66 LOAD_FAST                1 (entry)
                             68 STORE_ATTR               2 (participantID)
                
-               134          78 NOP
+               135          78 NOP
                
-               135          80 LOAD_GLOBAL              6 (request)
+               136          80 LOAD_GLOBAL              6 (request)
                             92 LOAD_ATTR                4 (json)
                            102 STORE_FAST               2 (data)
                            104 JUMP_FORWARD            19 (to 144)
                        >>  106 PUSH_EXC_INFO
                
-               136         108 POP_TOP
+               137         108 POP_TOP
                
-               137         110 LOAD_GLOBAL              6 (request)
+               138         110 LOAD_GLOBAL              6 (request)
                            122 LOAD_ATTR                5 (form)
                            132 STORE_FAST               2 (data)
                            134 POP_EXCEPT
                            136 JUMP_FORWARD             3 (to 144)
                        >>  138 COPY                     3
                            140 POP_EXCEPT
                            142 RERAISE                  1
                
-               139     >>  144 LOAD_FAST                0 (self)
+               140     >>  144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                6 (json_data)
                            156 LOAD_CONST               2 ('columns')
                            158 BINARY_SUBSCR
                            168 GET_ITER
                        >>  170 FOR_ITER               201 (to 574)
                            172 STORE_FAST               3 (column)
                
-               140         174 LOAD_FAST                3 (column)
+               141         174 LOAD_FAST                3 (column)
                            176 LOAD_FAST                2 (data)
                            178 CONTAINS_OP              0
                            180 POP_JUMP_FORWARD_IF_FALSE   195 (to 572)
                
-               141         182 LOAD_FAST                0 (self)
+               142         182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                6 (json_data)
                            194 LOAD_CONST               2 ('columns')
                            196 BINARY_SUBSCR
                            206 LOAD_FAST                3 (column)
                            208 BINARY_SUBSCR
                            218 STORE_FAST               4 (columnDetails)
                
-               142         220 LOAD_FAST                2 (data)
+               143         220 LOAD_FAST                2 (data)
                            222 LOAD_FAST                3 (column)
                            224 BINARY_SUBSCR
                            234 STORE_FAST               5 (value)
                
-               144         236 LOAD_CONST               3 ('type')
+               145         236 LOAD_CONST               3 ('type')
                            238 LOAD_FAST                4 (columnDetails)
                            240 CONTAINS_OP              0
                            242 POP_JUMP_FORWARD_IF_FALSE   147 (to 538)
                
-               145         244 LOAD_FAST                4 (columnDetails)
+               146         244 LOAD_FAST                4 (columnDetails)
                            246 LOAD_CONST               3 ('type')
                            248 BINARY_SUBSCR
                            258 LOAD_CONST               4 ('integer')
                            260 COMPARE_OP               2 (==)
                            266 POP_JUMP_FORWARD_IF_FALSE    31 (to 330)
                
-               146         268 LOAD_GLOBAL             15 (NULL + setattr)
+               147         268 LOAD_GLOBAL             15 (NULL + setattr)
                            280 LOAD_FAST                1 (entry)
                            282 LOAD_FAST                3 (column)
                            284 LOAD_GLOBAL             17 (NULL + int)
                            296 LOAD_FAST                5 (value)
                            298 PRECALL                  1
                            302 CALL                     1
                            312 PRECALL                  3
                            316 CALL                     3
                            326 POP_TOP
                            328 JUMP_BACKWARD           80 (to 170)
                
-               147     >>  330 LOAD_FAST                4 (columnDetails)
+               148     >>  330 LOAD_FAST                4 (columnDetails)
                            332 LOAD_CONST               3 ('type')
                            334 BINARY_SUBSCR
                            344 LOAD_CONST               5 ('float')
                            346 COMPARE_OP               2 (==)
                            352 POP_JUMP_FORWARD_IF_FALSE    31 (to 416)
                
-               148         354 LOAD_GLOBAL             15 (NULL + setattr)
+               149         354 LOAD_GLOBAL             15 (NULL + setattr)
                            366 LOAD_FAST                1 (entry)
                            368 LOAD_FAST                3 (column)
                            370 LOAD_GLOBAL             19 (NULL + float)
                            382 LOAD_FAST                5 (value)
                            384 PRECALL                  1
                            388 CALL                     1
                            398 PRECALL                  3
                            402 CALL                     3
                            412 POP_TOP
                            414 JUMP_BACKWARD          123 (to 170)
                
-               149     >>  416 LOAD_FAST                4 (columnDetails)
+               150     >>  416 LOAD_FAST                4 (columnDetails)
                            418 LOAD_CONST               3 ('type')
                            420 BINARY_SUBSCR
                            430 LOAD_CONST               6 ('boolean')
                            432 COMPARE_OP               2 (==)
                            438 POP_JUMP_FORWARD_IF_FALSE    31 (to 502)
                
-               150         440 LOAD_GLOBAL             15 (NULL + setattr)
+               151         440 LOAD_GLOBAL             15 (NULL + setattr)
                            452 LOAD_FAST                1 (entry)
                            454 LOAD_FAST                3 (column)
                            456 LOAD_GLOBAL             21 (NULL + bool)
                            468 LOAD_FAST                5 (value)
                            470 PRECALL                  1
                            474 CALL                     1
                            484 PRECALL                  3
                            488 CALL                     3
                            498 POP_TOP
                            500 JUMP_BACKWARD          166 (to 170)
                
-               152     >>  502 LOAD_GLOBAL             15 (NULL + setattr)
+               153     >>  502 LOAD_GLOBAL             15 (NULL + setattr)
                            514 LOAD_FAST                1 (entry)
                            516 LOAD_FAST                3 (column)
                            518 LOAD_FAST                5 (value)
                            520 PRECALL                  3
                            524 CALL                     3
                            534 POP_TOP
                            536 JUMP_BACKWARD          184 (to 170)
                
-               154     >>  538 LOAD_GLOBAL             15 (NULL + setattr)
+               155     >>  538 LOAD_GLOBAL             15 (NULL + setattr)
                            550 LOAD_FAST                1 (entry)
                            552 LOAD_FAST                3 (column)
                            554 LOAD_FAST                5 (value)
                            556 PRECALL                  3
                            560 CALL                     3
                            570 POP_TOP
                        >>  572 JUMP_BACKWARD          202 (to 170)
                
-               156     >>  574 LOAD_GLOBAL             22 (db)
+               157     >>  574 LOAD_GLOBAL             22 (db)
                            586 LOAD_ATTR                1 (session)
                            596 LOAD_METHOD             12 (add)
                            618 LOAD_FAST                1 (entry)
                            620 PRECALL                  1
                            624 CALL                     1
                            634 POP_TOP
                
-               157         636 LOAD_GLOBAL             22 (db)
+               158         636 LOAD_GLOBAL             22 (db)
                            648 LOAD_ATTR                1 (session)
                            658 LOAD_METHOD             13 (commit)
                            680 PRECALL                  0
                            684 CALL                     0
                            694 POP_TOP
                
-               159         696 LOAD_CONST               7 ('')
+               160         696 LOAD_CONST               7 ('')
                            698 RETURN_VALUE
                ExceptionTable:
                  80 to 102 -> 106 [0]
                  106 to 132 -> 138 [1] lasti
                consts
                   None
                   'participantID'
@@ -1299,15 +1316,15 @@
                   ''
                names      ('db_class', 'session', 'participantID', 'request', 'json', 'form', 'json_data', 'setattr', 'int', 'float', 'bool', 'db', 'add', 'commit')
                varnames   ('self', 'entry', 'data', 'column', 'columnDetails', 'value')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'handle_post'
-               firstlineno 130
+               firstlineno 131
                lnotab
                   0x02012801240202011c01020122021e01080126011002080118013e0118
                   013e0118013e02240224023e013c02
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 7
@@ -1327,52 +1344,52 @@
                   006a0700000000000000007c02190000000000000000006b0200000000a6
                   010000ab0100000000000000007d018c5e7c01a00b000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d04880066
                   01640284087c044400a6000000ab0000000000000000007d057419000000
                   000000000000007c05a6010000ab0100000000000000005300
                              0 MAKE_CELL                0 (self)
                
-               161           2 RESUME                   0
+               162           2 RESUME                   0
                
-               162           4 LOAD_GLOBAL              0 (db)
+               163           4 LOAD_GLOBAL              0 (db)
                             16 LOAD_ATTR                1 (session)
                             26 LOAD_METHOD              2 (query)
                             48 LOAD_DEREF               0 (self)
                             50 LOAD_ATTR                3 (db_class)
                             60 PRECALL                  1
                             64 CALL                     1
                
-               163          74 LOAD_METHOD              4 (filter)
+               164          74 LOAD_METHOD              4 (filter)
                             96 LOAD_DEREF               0 (self)
                             98 LOAD_ATTR                3 (db_class)
                            108 LOAD_ATTR                5 (participantID)
                            118 LOAD_GLOBAL              2 (session)
                            130 LOAD_CONST               1 ('participantID')
                            132 BINARY_SUBSCR
                            142 COMPARE_OP               2 (==)
                            148 PRECALL                  1
                            152 CALL                     1
                
-               162         162 STORE_FAST               1 (q)
+               163         162 STORE_FAST               1 (q)
                
-               166         164 LOAD_GLOBAL             12 (request)
+               167         164 LOAD_GLOBAL             12 (request)
                            176 LOAD_ATTR                7 (args)
                            186 GET_ITER
                        >>  188 FOR_ITER                93 (to 376)
                            190 STORE_FAST               2 (arg)
                
-               167         192 LOAD_GLOBAL             17 (NULL + getattr)
+               168         192 LOAD_GLOBAL             17 (NULL + getattr)
                            204 LOAD_DEREF               0 (self)
                            206 LOAD_ATTR                3 (db_class)
                            216 LOAD_FAST                2 (arg)
                            218 PRECALL                  2
                            222 CALL                     2
                            232 STORE_FAST               3 (column)
                
-               168         234 LOAD_FAST                1 (q)
+               169         234 LOAD_FAST                1 (q)
                            236 LOAD_METHOD              4 (filter)
                            258 LOAD_GLOBAL              1 (NULL + db)
                            270 LOAD_ATTR                9 (cast)
                            280 LOAD_FAST                3 (column)
                            282 LOAD_GLOBAL              0 (db)
                            294 LOAD_ATTR               10 (Text)
                            304 PRECALL                  2
@@ -1383,31 +1400,31 @@
                            342 BINARY_SUBSCR
                            352 COMPARE_OP               2 (==)
                            358 PRECALL                  1
                            362 CALL                     1
                            372 STORE_FAST               1 (q)
                            374 JUMP_BACKWARD           94 (to 188)
                
-               170     >>  376 LOAD_FAST                1 (q)
+               171     >>  376 LOAD_FAST                1 (q)
                            378 LOAD_METHOD             11 (all)
                            400 PRECALL                  0
                            404 CALL                     0
                            414 STORE_FAST               4 (results)
                
-               173         416 LOAD_CLOSURE             0 (self)
+               174         416 LOAD_CLOSURE             0 (self)
                            418 BUILD_TUPLE              1
-                           420 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 173>)
+                           420 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\JSONTable.py", line 174>)
                            422 MAKE_FUNCTION            8 (closure)
                            424 LOAD_FAST                4 (results)
                            426 GET_ITER
                            428 PRECALL                  0
                            432 CALL                     0
                            442 STORE_FAST               5 (out)
                
-               175         444 LOAD_GLOBAL             25 (NULL + jsonify)
+               176         444 LOAD_GLOBAL             25 (NULL + jsonify)
                            456 LOAD_FAST                5 (out)
                            458 PRECALL                  1
                            462 CALL                     1
                            472 RETURN_VALUE
                consts
                   None
                   'participantID'
@@ -1417,15 +1434,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     173           2 RESUME                   0
+                     174           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (row)
                                   12 LOAD_DEREF               2 (self)
                                   14 LOAD_METHOD              0 (row_to_dict)
                                   36 LOAD_FAST                1 (row)
@@ -1437,33 +1454,33 @@
                      consts
                      names      ('row_to_dict',)
                      varnames   ('.0', 'row')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                      name       '<listcomp>'
-                     firstlineno 173
+                     firstlineno 174
                      lnotab 0x
                names      ('db', 'session', 'query', 'db_class', 'filter', 'participantID', 'request', 'args', 'getattr', 'cast', 'Text', 'all', 'jsonify')
                varnames   ('self', 'q', 'arg', 'column', 'results', 'out')
                freevars   ()
                cellvars   ('self',)
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
                name       'handle_get'
-               firstlineno 161
+               firstlineno 162
                lnotab 0x0401460158ff02041c012a018e0228031c02
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'list', 'get_columns', 'create_db_class', 'create_exports_dict', 'row_to_dict', 'handle_post', 'handle_get')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
          name       'JSONTable'
          firstlineno 56
-         lnotab 0x0a01101218030613060c0615061f
+         lnotab 0x0a01101218030614060c0615061f
       'JSONTable'
    names      ('os', 'json', 'datetime', 'globals', 'db', 'flask', 'current_app', 'request', 'session', 'config', 'jsonify', 'JSONTableColumn', 'object', 'JSONTable')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\JSONTable.py'
    name       '<module>'
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/PageList.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/PageList.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/cli.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/create_app.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/create_app.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9b121e66 (Tue Apr 16 05:54:35 2024 UTC)
-files sz: 5177
+moddate:  0xbb442066 (Wed Apr 17 21:52:59 2024 UTC)
+files sz: 5233
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d025a0201
@@ -125,24 +125,25 @@
             000000000000000000a6000000ab0000000000000000007d0d7c0c6a2000
             000000000000006a2100000000000000007d0e7c0d44005d4a7d0f742f00
             0000000000000000007c0e7c0f6a2200000000000000007c0fa023000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             007c0f6a240000000000000000a6040000ab040000000000000000721a74
             250000000000000000000064297c0e9b00642a7c0f6a2200000000000000
             009b009d04a6010000ab01000000000000000001008c4b8c7d7c046a2500
-            0000000000000044005d707d107c046a2500000000000000007c10190000
+            0000000000000044005d7c7d107c046a2500000000000000007c10190000
             000000000000007d117c11a0260000000000000000000000000000000000
-            000000a6000000ab0000000000000000007d127c1244005d4a7d13742f00
-            0000000000000000007c107c136a2700000000000000007c13a023000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            007c136a240000000000000000a6040000ab040000000000000000721a74
-            250000000000000000000064297c109b00642a7c136a2700000000000000
-            009b009d04a6010000ab01000000000000000001008c4b8c710900640064
-            006400a6020000ab02000000000000000001006e0b230031007304770278
-            035900770101005900010001007c045300
+            000000a6000000ab0000000000000000007d127c116a2000000000000000
+            006a2100000000000000007d0e7c1244005d4a7d13742f00000000000000
+            0000007c0e7c136a2700000000000000007c13a023000000000000000000
+            0000000000000000000000a6000000ab0000000000000000007c136a2400
+            00000000000000a6040000ab040000000000000000721a74250000000000
+            000000000064297c109b00642a7c136a2700000000000000009b009d04a6
+            010000ab01000000000000000001008c4b8c7d0900640064006400a60200
+            00ab02000000000000000001006e0b230031007304770278035900770101
+            005900010001007c045300
            7           0 RESUME                   0
          
            8           2 LOAD_GLOBAL              1 (NULL + os)
                       14 LOAD_ATTR                1 (chdir)
                       24 LOAD_FAST                0 (path)
                       26 PRECALL                  1
                       30 CALL                     1
@@ -658,92 +659,97 @@
                  >> 2240 JUMP_BACKWARD           75 (to 2092)
          
          119     >> 2242 JUMP_BACKWARD          125 (to 1994)
          
          123     >> 2244 LOAD_FAST                4 (app)
                     2246 LOAD_ATTR               37 (tables)
                     2256 GET_ITER
-                 >> 2258 FOR_ITER               112 (to 2484)
+                 >> 2258 FOR_ITER               124 (to 2508)
                     2260 STORE_FAST              16 (t_key)
          
          124        2262 LOAD_FAST                4 (app)
                     2264 LOAD_ATTR               37 (tables)
                     2274 LOAD_FAST               16 (t_key)
                     2276 BINARY_SUBSCR
                     2286 STORE_FAST              17 (t)
          
          125        2288 LOAD_FAST               17 (t)
                     2290 LOAD_METHOD             38 (get_columns)
                     2312 PRECALL                  0
                     2316 CALL                     0
                     2326 STORE_FAST              18 (columns)
          
-         127        2328 LOAD_FAST               18 (columns)
-                    2330 GET_ITER
-                 >> 2332 FOR_ITER                74 (to 2482)
-                    2334 STORE_FAST              19 (column)
-         
-         128        2336 LOAD_GLOBAL             47 (NULL + check_and_add_column)
-                    2348 LOAD_FAST               16 (t_key)
-                    2350 LOAD_FAST               19 (column)
-                    2352 LOAD_ATTR               39 (name)
-                    2362 LOAD_FAST               19 (column)
-                    2364 LOAD_METHOD             35 (get_type_ddl)
-                    2386 PRECALL                  0
-                    2390 CALL                     0
-                    2400 LOAD_FAST               19 (column)
-                    2402 LOAD_ATTR               36 (default)
-                    2412 PRECALL                  4
-                    2416 CALL                     4
-                    2426 POP_JUMP_FORWARD_IF_FALSE    26 (to 2480)
-         
-         129        2428 LOAD_GLOBAL             37 (NULL + print)
-                    2440 LOAD_CONST              41 ('Added new column to ')
-                    2442 LOAD_FAST               16 (t_key)
-                    2444 FORMAT_VALUE             0
-                    2446 LOAD_CONST              42 (': ')
-                    2448 LOAD_FAST               19 (column)
-                    2450 LOAD_ATTR               39 (name)
-                    2460 FORMAT_VALUE             0
-                    2462 BUILD_STRING             4
-                    2464 PRECALL                  1
-                    2468 CALL                     1
-                    2478 POP_TOP
-                 >> 2480 JUMP_BACKWARD           75 (to 2332)
-         
-         127     >> 2482 JUMP_BACKWARD          113 (to 2258)
-         
-         123     >> 2484 NOP
-         
-          91        2486 LOAD_CONST               0 (None)
-                    2488 LOAD_CONST               0 (None)
-                    2490 LOAD_CONST               0 (None)
-                    2492 PRECALL                  2
-                    2496 CALL                     2
-                    2506 POP_TOP
-                    2508 JUMP_FORWARD            11 (to 2532)
-                 >> 2510 PUSH_EXC_INFO
-                    2512 WITH_EXCEPT_START
-                    2514 POP_JUMP_FORWARD_IF_TRUE     4 (to 2524)
-                    2516 RERAISE                  2
-                 >> 2518 COPY                     3
-                    2520 POP_EXCEPT
-                    2522 RERAISE                  1
-                 >> 2524 POP_TOP
-                    2526 POP_EXCEPT
-                    2528 POP_TOP
+         126        2328 LOAD_FAST               17 (t)
+                    2330 LOAD_ATTR               32 (db_class)
+                    2340 LOAD_ATTR               33 (__tablename__)
+                    2350 STORE_FAST              14 (table_name)
+         
+         128        2352 LOAD_FAST               18 (columns)
+                    2354 GET_ITER
+                 >> 2356 FOR_ITER                74 (to 2506)
+                    2358 STORE_FAST              19 (column)
+         
+         129        2360 LOAD_GLOBAL             47 (NULL + check_and_add_column)
+                    2372 LOAD_FAST               14 (table_name)
+                    2374 LOAD_FAST               19 (column)
+                    2376 LOAD_ATTR               39 (name)
+                    2386 LOAD_FAST               19 (column)
+                    2388 LOAD_METHOD             35 (get_type_ddl)
+                    2410 PRECALL                  0
+                    2414 CALL                     0
+                    2424 LOAD_FAST               19 (column)
+                    2426 LOAD_ATTR               36 (default)
+                    2436 PRECALL                  4
+                    2440 CALL                     4
+                    2450 POP_JUMP_FORWARD_IF_FALSE    26 (to 2504)
+         
+         130        2452 LOAD_GLOBAL             37 (NULL + print)
+                    2464 LOAD_CONST              41 ('Added new column to ')
+                    2466 LOAD_FAST               16 (t_key)
+                    2468 FORMAT_VALUE             0
+                    2470 LOAD_CONST              42 (': ')
+                    2472 LOAD_FAST               19 (column)
+                    2474 LOAD_ATTR               39 (name)
+                    2484 FORMAT_VALUE             0
+                    2486 BUILD_STRING             4
+                    2488 PRECALL                  1
+                    2492 CALL                     1
+                    2502 POP_TOP
+                 >> 2504 JUMP_BACKWARD           75 (to 2356)
+         
+         128     >> 2506 JUMP_BACKWARD          125 (to 2258)
+         
+         123     >> 2508 NOP
+         
+          91        2510 LOAD_CONST               0 (None)
+                    2512 LOAD_CONST               0 (None)
+                    2514 LOAD_CONST               0 (None)
+                    2516 PRECALL                  2
+                    2520 CALL                     2
                     2530 POP_TOP
+                    2532 JUMP_FORWARD            11 (to 2556)
+                 >> 2534 PUSH_EXC_INFO
+                    2536 WITH_EXCEPT_START
+                    2538 POP_JUMP_FORWARD_IF_TRUE     4 (to 2548)
+                    2540 RERAISE                  2
+                 >> 2542 COPY                     3
+                    2544 POP_EXCEPT
+                    2546 RERAISE                  1
+                 >> 2548 POP_TOP
+                    2550 POP_EXCEPT
+                    2552 POP_TOP
+                    2554 POP_TOP
          
-         131     >> 2532 LOAD_FAST                4 (app)
-                    2534 RETURN_VALUE
+         132     >> 2556 LOAD_FAST                4 (app)
+                    2558 RETURN_VALUE
          ExceptionTable:
-           1420 to 1492 -> 2510 [1] lasti
-           1520 to 2482 -> 2510 [1] lasti
-           2510 to 2516 -> 2518 [3] lasti
-           2524 to 2524 -> 2518 [3] lasti
+           1420 to 1492 -> 2534 [1] lasti
+           1520 to 2506 -> 2534 [1] lasti
+           2534 to 2540 -> 2542 [3] lasti
+           2548 to 2548 -> 2542 [3] lasti
          consts
             None
             ('config_name', 'root_path', 'run_with_debugging', 'run_with_reloader_off')
             False
             ('silent',)
             'USE_ADMIN'
             True
@@ -793,16 +799,16 @@
          firstlineno 7
          lnotab
             0x020128013e02180102010201020102fc12052e0230012c031201140212
             011402120114021201140212011402120114021201140212011402120114
             02120114021201140212011402120114021201140212011402120114022c
             01080102024002680104022c010c012e0104010c012c0204012c022c022a
             0128011e0202fc1a0628012801320424022402760108012a013c011e0312
-            011a012801180208015c0136fe020412011a01280208015c0136fe02fc02
-            e02e28
+            011a012801180208015c0136fe020412011a012801180208015c0136fe02
+            fb02e02e29
       (False, False)
    names      ('os', 'sys', 'BOFSFlask', 'admin.util', 'check_and_add_column', 'create_app')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\create_app.py'
    name       '<module>'
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/globals.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/globals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/__pycache__/util.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/export_helpers.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/Results.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,1516 +1,1790 @@
 magic:    0xa70d0d0a
-moddate:  0x56a01d66 (Mon Apr 15 21:47:02 2024 UTC)
-files sz: 10272
+moddate:  0x215a2066 (Wed Apr 17 23:24:17 2024 UTC)
+files sz: 11881
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 9
+   stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a030100640064026c045a
-      04640364046c056d065a066d075a076d085a080100640064056c096d0a5a
-      0a01006406650b6602640784045a0c0900090064116409650d650e190000
-      00000000000000640a650b640b65046a0f00000000000000006a10000000
-      00000000006606640c84055a11090064126409650d650e19000000000000
-      000000640a650b640d65046a0f00000000000000006a1000000000000000
-      00640b64026608640e84055a12090064126409650d650e19000000000000
-      000000640a650b640d65046a0f00000000000000006a1000000000000000
-      00640b64026608640f84055a136409650d650e1900000000000000000064
-      0a650b640b650e6606641084045a1464025300
+      0x9700640064016c006d015a010100640064026c026d035a036d045a046d
+      055a050100640064036c065a06640464056c076d085a086d095a096d0a5a
+      0a0100640064066c0b6d0c5a0c0100640064036c0d5a0e640064036c0f5a
+      0f640064076c106d105a10010064085a110200470064098400640a6512a6
+      030000ab0300000000000000005a1364035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('db', 'questionnaires', 'page_list'))
-                 6 IMPORT_NAME              0 (BOFS.globals)
-                 8 IMPORT_FROM              1 (db)
-                10 STORE_NAME               1 (db)
-                12 IMPORT_FROM              2 (questionnaires)
-                14 STORE_NAME               2 (questionnaires)
-                16 IMPORT_FROM              3 (page_list)
-                18 STORE_NAME               3 (page_list)
-                20 POP_TOP
-   
-     2          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (None)
-                26 IMPORT_NAME              4 (sqlalchemy)
-                28 STORE_NAME               4 (sqlalchemy)
-   
-     3          30 LOAD_CONST               3 (1)
-                32 LOAD_CONST               4 (('escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
-                34 IMPORT_NAME              5 (util)
-                36 IMPORT_FROM              6 (escape_csv)
-                38 STORE_NAME               6 (escape_csv)
-                40 IMPORT_FROM              7 (questionnaire_name_and_tag)
-                42 STORE_NAME               7 (questionnaire_name_and_tag)
-                44 IMPORT_FROM              8 (condition_num_to_label)
-                46 STORE_NAME               8 (condition_num_to_label)
-                48 POP_TOP
-   
-     4          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               5 (('current_app',))
-                54 IMPORT_NAME              9 (flask)
-                56 IMPORT_FROM             10 (current_app)
-                58 STORE_NAME              10 (current_app)
+                 4 LOAD_CONST               1 (('Query',))
+                 6 IMPORT_NAME              0 (sqlalchemy.orm)
+                 8 IMPORT_FROM              1 (Query)
+                10 STORE_NAME               1 (Query)
+                12 POP_TOP
+   
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('db', 'questionnaires', 'page_list'))
+                18 IMPORT_NAME              2 (BOFS.globals)
+                20 IMPORT_FROM              3 (db)
+                22 STORE_NAME               3 (db)
+                24 IMPORT_FROM              4 (questionnaires)
+                26 STORE_NAME               4 (questionnaires)
+                28 IMPORT_FROM              5 (page_list)
+                30 STORE_NAME               5 (page_list)
+                32 POP_TOP
+   
+     3          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (None)
+                38 IMPORT_NAME              6 (sqlalchemy)
+                40 STORE_NAME               6 (sqlalchemy)
+   
+     4          42 LOAD_CONST               4 (1)
+                44 LOAD_CONST               5 (('escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
+                46 IMPORT_NAME              7 (util)
+                48 IMPORT_FROM              8 (escape_csv)
+                50 STORE_NAME               8 (escape_csv)
+                52 IMPORT_FROM              9 (questionnaire_name_and_tag)
+                54 STORE_NAME               9 (questionnaire_name_and_tag)
+                56 IMPORT_FROM             10 (condition_num_to_label)
+                58 STORE_NAME              10 (condition_num_to_label)
                 60 POP_TOP
    
-     7          62 LOAD_CONST               6 ('export_dict')
-                64 LOAD_NAME               11 (dict)
-                66 BUILD_TUPLE              2
-                68 LOAD_CONST               7 (<code object create_export_base_query, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 7>)
-                70 MAKE_FUNCTION            4 (annotations)
-                72 STORE_NAME              12 (create_export_base_query)
-   
-    88          74 NOP
-   
-    89          76 NOP
-   
-    86          78 LOAD_CONST              17 ((True, True))
-                80 LOAD_CONST               9 ('column_list')
-                82 LOAD_NAME               13 (list)
-                84 LOAD_NAME               14 (str)
-                86 BINARY_SUBSCR
-                96 LOAD_CONST              10 ('export_data')
-   
-    87          98 LOAD_NAME               11 (dict)
-   
-    86         100 LOAD_CONST              11 ('return')
-   
-    89         102 LOAD_NAME                4 (sqlalchemy)
-               104 LOAD_ATTR               15 (orm)
-               114 LOAD_ATTR               16 (Query)
-   
-    86         124 BUILD_TUPLE              6
-               126 LOAD_CONST              12 (<code object add_participants_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 86>)
-               128 MAKE_FUNCTION            5 (defaults, annotations)
-               130 STORE_NAME              17 (add_participants_to_export)
-   
-   128         132 NOP
-   
-   125         134 LOAD_CONST              18 ((True,))
-               136 LOAD_CONST               9 ('column_list')
-               138 LOAD_NAME               13 (list)
-               140 LOAD_NAME               14 (str)
-               142 BINARY_SUBSCR
-               152 LOAD_CONST              10 ('export_data')
-   
-   126         154 LOAD_NAME               11 (dict)
-   
-   125         156 LOAD_CONST              13 ('query_participants')
-   
-   127         158 LOAD_NAME                4 (sqlalchemy)
-               160 LOAD_ATTR               15 (orm)
-               170 LOAD_ATTR               16 (Query)
-   
-   125         180 LOAD_CONST              11 ('return')
-   
-   128         182 LOAD_CONST               2 (None)
-   
-   125         184 BUILD_TUPLE              8
-               186 LOAD_CONST              14 (<code object add_questionnaires_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 125>)
-               188 MAKE_FUNCTION            5 (defaults, annotations)
-               190 STORE_NAME              18 (add_questionnaires_to_export)
-   
-   195         192 NOP
-   
-   192         194 LOAD_CONST              18 ((True,))
-               196 LOAD_CONST               9 ('column_list')
-               198 LOAD_NAME               13 (list)
-               200 LOAD_NAME               14 (str)
-               202 BINARY_SUBSCR
-               212 LOAD_CONST              10 ('export_data')
-   
-   193         214 LOAD_NAME               11 (dict)
-   
-   192         216 LOAD_CONST              13 ('query_participants')
-   
-   194         218 LOAD_NAME                4 (sqlalchemy)
-               220 LOAD_ATTR               15 (orm)
-               230 LOAD_ATTR               16 (Query)
-   
-   192         240 LOAD_CONST              11 ('return')
-   
-   195         242 LOAD_CONST               2 (None)
-   
-   192         244 BUILD_TUPLE              8
-               246 LOAD_CONST              15 (<code object add_custom_exports_to_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 192>)
-               248 MAKE_FUNCTION            5 (defaults, annotations)
-               250 STORE_NAME              19 (add_custom_exports_to_export)
-   
-   239         252 LOAD_CONST               9 ('column_list')
-               254 LOAD_NAME               13 (list)
-               256 LOAD_NAME               14 (str)
-               258 BINARY_SUBSCR
-               268 LOAD_CONST              10 ('export_data')
-               270 LOAD_NAME               11 (dict)
-               272 LOAD_CONST              11 ('return')
-               274 LOAD_NAME               14 (str)
-               276 BUILD_TUPLE              6
-               278 LOAD_CONST              16 (<code object build_export_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\export_helpers.py", line 239>)
-               280 MAKE_FUNCTION            4 (annotations)
-               282 STORE_NAME              20 (build_export_csv)
-               284 LOAD_CONST               2 (None)
-               286 RETURN_VALUE
+     5          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               6 (('current_app',))
+                66 IMPORT_NAME             11 (flask)
+                68 IMPORT_FROM             12 (current_app)
+                70 STORE_NAME              12 (current_app)
+                72 POP_TOP
+   
+     6          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               3 (None)
+                78 IMPORT_NAME             13 (pandas)
+                80 STORE_NAME              14 (pd)
+   
+     7          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               3 (None)
+                86 IMPORT_NAME             15 (os)
+                88 STORE_NAME              15 (os)
+   
+     8          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               7 (('datetime',))
+                94 IMPORT_NAME             16 (datetime)
+                96 IMPORT_FROM             16 (datetime)
+                98 STORE_NAME              16 (datetime)
+               100 POP_TOP
+   
+    10         102 LOAD_CONST               8 (120)
+               104 STORE_NAME              17 (MAX_CACHE_SECONDS)
+   
+    13         106 PUSH_NULL
+               108 LOAD_BUILD_CLASS
+               110 LOAD_CONST               9 (<code object Results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 13>)
+               112 MAKE_FUNCTION            0
+               114 LOAD_CONST              10 ('Results')
+               116 LOAD_NAME               18 (object)
+               118 PRECALL                  3
+               122 CALL                     3
+               132 STORE_NAME              19 (Results)
+               134 LOAD_CONST               3 (None)
+               136 RETURN_VALUE
    consts
       0
+      ('Query',)
       ('db', 'questionnaires', 'page_list')
       None
       1
       ('escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label')
       ('current_app',)
-      'export_dict'
-      code
-         argcount  : 1
-         nlocals   : 12
-         stacksize : 7
-         flags     : 3
-         code
-            0x97007401000000000000000000007402000000000000000000007c0064
-            0119000000000000000000a6020000ab0200000000000000007d0164027d
-            0267007d0364027d0464027d0564027d0664027d0764037c00760072267c
-            0064031900000000000000000064046b0300000000721a74030000000000
-            00000000006a0200000000000000007c00640319000000000000000000a6
-            010000ab0100000000000000007d0464057c00760072227c006405190000
-            0000000000000064046b030000000072167401000000000000000000007c
-            017c00640519000000000000000000a6020000ab0200000000000000007d
-            0664067c0076009001727c7c0064061900000000000000000064046b0300
-            0000009001726f64077c00760072267c0064071900000000000000000064
-            046b0300000000721a7403000000000000000000006a0200000000000000
-            007c00640719000000000000000000a6010000ab0100000000000000007d
-            077402000000000000000000006a030000000000000000a0040000000000
-            000000000000000000000000000000a6000000ab0000000000000000007d
-            08740b000000000000000000007c00640619000000000000000000740c00
-            000000000000000000a6020000ab020000000000000000727767007d057c
-            0064061900000000000000000044005d6b7d097c05a00700000000000000
-            000000000000000000000000007401000000000000000000007c017c09a6
-            020000ab020000000000000000a6010000ab01000000000000000001007c
-            08a008000000000000000000000000000000000000000074010000000000
-            00000000007c017c09a6020000ab020000000000000000a6010000ab0100
-            000000000000007d087c08a0090000000000000000000000000000000000
-            0000007401000000000000000000007c017c09a6020000ab020000000000
-            000000a6010000ab0100000000000000007d088c6c6e4074010000000000
-            00000000007c017c00640619000000000000000000a6020000ab02000000
-            00000000007d057c08a00800000000000000000000000000000000000000
-            007c05a6010000ab0100000000000000007d087c08a00900000000000000
-            000000000000000000000000007c05a6010000ab0100000000000000007d
-            087c0672157c08a00a00000000000000000000000000000000000000007c
-            06a6010000ab0100000000000000007d087c0481287c08a00b0000000000
-            0000000000000000000000000000007c04a6010000ab0100000000000000
-            00a00c0000000000000000000000000000000000000000a6000000ab0000
-            000000000000007d026e147c08a00c000000000000000000000000000000
-            0000000000a6000000ab0000000000000000007d02740200000000000000
-            0000006a030000000000000000a004000000000000000000000000000000
-            00000000007c01a6010000ab0100000000000000007d0a7c05727b740b00
-            0000000000000000007c05740c00000000000000000000a6020000ab0200
-            00000000000000722a7c0544005d267d097c0aa009000000000000000000
-            00000000000000000000007401000000000000000000007c016408a60200
-            00ab0200000000000000007c09a6020000ab0200000000000000007d0a8c
-            276e247c0aa0090000000000000000000000000000000000000000740100
-            0000000000000000007c016408a6020000ab0200000000000000007c05a6
-            020000ab0200000000000000007d0a7c0781157c0aa00d00000000000000
-            000000000000000000000000007c07a6010000ab0100000000000000007d
-            0a6e237c0aa0090000000000000000000000000000000000000000740100
-            0000000000000000007c016408a6020000ab020000000000000000a60100
-            00ab0100000000000000007d0a7c0672157c0aa00a000000000000000000
-            00000000000000000000007c06a6010000ab0100000000000000007d0a7c
-            0481157c0aa00b00000000000000000000000000000000000000007c04a6
-            010000ab0100000000000000007d0a7c0064091900000000000000000044
-            005d8b7d0b741d000000000000000000007c017c0ba6020000ab02000000
-            0000000000721e741f000000000000000000007401000000000000000000
-            007c017c0ba6020000ab020000000000000000a6010000ab010000000000
-            00000072018c307c03a00700000000000000000000000000000000000000
-            007c0ba6010000ab01000000000000000001007c0aa00800000000000000
-            000000000000000000000000007403000000000000000000006a10000000
-            00000000007c006409190000000000000000007c0b190000000000000000
-            00a6010000ab010000000000000000a01100000000000000000000000000
-            000000000000007c0ba6010000ab010000000000000000a6010000ab0100
-            000000000000007d0a8c8c7c027c037c0a66035300
-           7           0 RESUME                   0
-         
-          14           2 LOAD_GLOBAL              1 (NULL + getattr)
-                      14 LOAD_GLOBAL              2 (db)
-                      26 LOAD_FAST                0 (export_dict)
-                      28 LOAD_CONST               1 ('table')
-                      30 BINARY_SUBSCR
-                      40 PRECALL                  2
-                      44 CALL                     2
-                      54 STORE_FAST               1 (table)
-         
-          16          56 LOAD_CONST               2 (None)
-                      58 STORE_FAST               2 (levels)
-         
-          17          60 BUILD_LIST               0
-                      62 STORE_FAST               3 (fields)
-         
-          18          64 LOAD_CONST               2 (None)
-                      66 STORE_FAST               4 (filter)
-         
-          19          68 LOAD_CONST               2 (None)
-                      70 STORE_FAST               5 (groupBy)
-         
-          20          72 LOAD_CONST               2 (None)
-                      74 STORE_FAST               6 (orderBy)
-         
-          21          76 LOAD_CONST               2 (None)
-                      78 STORE_FAST               7 (having)
-         
-          23          80 LOAD_CONST               3 ('filter')
-                      82 LOAD_FAST                0 (export_dict)
-                      84 CONTAINS_OP              0
-                      86 POP_JUMP_FORWARD_IF_FALSE    38 (to 164)
-                      88 LOAD_FAST                0 (export_dict)
-                      90 LOAD_CONST               3 ('filter')
-                      92 BINARY_SUBSCR
-                     102 LOAD_CONST               4 ('')
-                     104 COMPARE_OP               3 (!=)
-                     110 POP_JUMP_FORWARD_IF_FALSE    26 (to 164)
-         
-          24         112 LOAD_GLOBAL              3 (NULL + db)
-                     124 LOAD_ATTR                2 (text)
-                     134 LOAD_FAST                0 (export_dict)
-                     136 LOAD_CONST               3 ('filter')
-                     138 BINARY_SUBSCR
-                     148 PRECALL                  1
-                     152 CALL                     1
-                     162 STORE_FAST               4 (filter)
-         
-          26     >>  164 LOAD_CONST               5 ('order_by')
-                     166 LOAD_FAST                0 (export_dict)
-                     168 CONTAINS_OP              0
-                     170 POP_JUMP_FORWARD_IF_FALSE    34 (to 240)
-                     172 LOAD_FAST                0 (export_dict)
-                     174 LOAD_CONST               5 ('order_by')
-                     176 BINARY_SUBSCR
-                     186 LOAD_CONST               4 ('')
-                     188 COMPARE_OP               3 (!=)
-                     194 POP_JUMP_FORWARD_IF_FALSE    22 (to 240)
-         
-          27         196 LOAD_GLOBAL              1 (NULL + getattr)
-                     208 LOAD_FAST                1 (table)
-                     210 LOAD_FAST                0 (export_dict)
-                     212 LOAD_CONST               5 ('order_by')
-                     214 BINARY_SUBSCR
-                     224 PRECALL                  2
-                     228 CALL                     2
-                     238 STORE_FAST               6 (orderBy)
-         
-          30     >>  240 LOAD_CONST               6 ('group_by')
-                     242 LOAD_FAST                0 (export_dict)
-                     244 CONTAINS_OP              0
-                     246 EXTENDED_ARG             1
-                     248 POP_JUMP_FORWARD_IF_FALSE   380 (to 1010)
-                     250 LOAD_FAST                0 (export_dict)
-                     252 LOAD_CONST               6 ('group_by')
-                     254 BINARY_SUBSCR
-                     264 LOAD_CONST               4 ('')
-                     266 COMPARE_OP               3 (!=)
-                     272 EXTENDED_ARG             1
-                     274 POP_JUMP_FORWARD_IF_FALSE   367 (to 1010)
-         
-          31         276 LOAD_CONST               7 ('having')
-                     278 LOAD_FAST                0 (export_dict)
-                     280 CONTAINS_OP              0
-                     282 POP_JUMP_FORWARD_IF_FALSE    38 (to 360)
-                     284 LOAD_FAST                0 (export_dict)
-                     286 LOAD_CONST               7 ('having')
-                     288 BINARY_SUBSCR
-                     298 LOAD_CONST               4 ('')
-                     300 COMPARE_OP               3 (!=)
-                     306 POP_JUMP_FORWARD_IF_FALSE    26 (to 360)
-         
-          32         308 LOAD_GLOBAL              3 (NULL + db)
-                     320 LOAD_ATTR                2 (text)
-                     330 LOAD_FAST                0 (export_dict)
-                     332 LOAD_CONST               7 ('having')
-                     334 BINARY_SUBSCR
-                     344 PRECALL                  1
-                     348 CALL                     1
-                     358 STORE_FAST               7 (having)
-         
-          34     >>  360 LOAD_GLOBAL              2 (db)
-                     372 LOAD_ATTR                3 (session)
-                     382 LOAD_METHOD              4 (query)
-                     404 PRECALL                  0
-                     408 CALL                     0
-                     418 STORE_FAST               8 (levelsQ)
-         
-          36         420 LOAD_GLOBAL             11 (NULL + isinstance)
-                     432 LOAD_FAST                0 (export_dict)
-                     434 LOAD_CONST               6 ('group_by')
-                     436 BINARY_SUBSCR
-                     446 LOAD_GLOBAL             12 (list)
-                     458 PRECALL                  2
-                     462 CALL                     2
-                     472 POP_JUMP_FORWARD_IF_FALSE   119 (to 712)
-         
-          37         474 BUILD_LIST               0
-                     476 STORE_FAST               5 (groupBy)
-         
-          38         478 LOAD_FAST                0 (export_dict)
-                     480 LOAD_CONST               6 ('group_by')
-                     482 BINARY_SUBSCR
-                     492 GET_ITER
-                 >>  494 FOR_ITER               107 (to 710)
-                     496 STORE_FAST               9 (gb)
-         
-          39         498 LOAD_FAST                5 (groupBy)
-                     500 LOAD_METHOD              7 (append)
-                     522 LOAD_GLOBAL              1 (NULL + getattr)
-                     534 LOAD_FAST                1 (table)
-                     536 LOAD_FAST                9 (gb)
-                     538 PRECALL                  2
-                     542 CALL                     2
-                     552 PRECALL                  1
-                     556 CALL                     1
-                     566 POP_TOP
-         
-          40         568 LOAD_FAST                8 (levelsQ)
-                     570 LOAD_METHOD              8 (add_columns)
-                     592 LOAD_GLOBAL              1 (NULL + getattr)
-                     604 LOAD_FAST                1 (table)
-                     606 LOAD_FAST                9 (gb)
-                     608 PRECALL                  2
-                     612 CALL                     2
-                     622 PRECALL                  1
-                     626 CALL                     1
-                     636 STORE_FAST               8 (levelsQ)
-         
-          41         638 LOAD_FAST                8 (levelsQ)
-                     640 LOAD_METHOD              9 (group_by)
-                     662 LOAD_GLOBAL              1 (NULL + getattr)
-                     674 LOAD_FAST                1 (table)
-                     676 LOAD_FAST                9 (gb)
-                     678 PRECALL                  2
-                     682 CALL                     2
-                     692 PRECALL                  1
-                     696 CALL                     1
-                     706 STORE_FAST               8 (levelsQ)
-                     708 JUMP_BACKWARD          108 (to 494)
-         
-          38     >>  710 JUMP_FORWARD            64 (to 840)
-         
-          43     >>  712 LOAD_GLOBAL              1 (NULL + getattr)
-                     724 LOAD_FAST                1 (table)
-                     726 LOAD_FAST                0 (export_dict)
-                     728 LOAD_CONST               6 ('group_by')
-                     730 BINARY_SUBSCR
-                     740 PRECALL                  2
-                     744 CALL                     2
-                     754 STORE_FAST               5 (groupBy)
-         
-          44         756 LOAD_FAST                8 (levelsQ)
-                     758 LOAD_METHOD              8 (add_columns)
-                     780 LOAD_FAST                5 (groupBy)
-                     782 PRECALL                  1
-                     786 CALL                     1
-                     796 STORE_FAST               8 (levelsQ)
-         
-          45         798 LOAD_FAST                8 (levelsQ)
-                     800 LOAD_METHOD              9 (group_by)
-                     822 LOAD_FAST                5 (groupBy)
-                     824 PRECALL                  1
-                     828 CALL                     1
-                     838 STORE_FAST               8 (levelsQ)
-         
-          47     >>  840 LOAD_FAST                6 (orderBy)
-                     842 POP_JUMP_FORWARD_IF_FALSE    21 (to 886)
-         
-          48         844 LOAD_FAST                8 (levelsQ)
-                     846 LOAD_METHOD             10 (order_by)
-                     868 LOAD_FAST                6 (orderBy)
-                     870 PRECALL                  1
-                     874 CALL                     1
-                     884 STORE_FAST               8 (levelsQ)
-         
-          50     >>  886 LOAD_FAST                4 (filter)
-                     888 POP_JUMP_FORWARD_IF_NONE    40 (to 970)
-         
-          51         890 LOAD_FAST                8 (levelsQ)
-                     892 LOAD_METHOD             11 (filter)
-                     914 LOAD_FAST                4 (filter)
-                     916 PRECALL                  1
-                     920 CALL                     1
-                     930 LOAD_METHOD             12 (all)
-                     952 PRECALL                  0
-                     956 CALL                     0
-                     966 STORE_FAST               2 (levels)
-                     968 JUMP_FORWARD            20 (to 1010)
-         
-          53     >>  970 LOAD_FAST                8 (levelsQ)
-                     972 LOAD_METHOD             12 (all)
-                     994 PRECALL                  0
-                     998 CALL                     0
-                    1008 STORE_FAST               2 (levels)
-         
-          56     >> 1010 LOAD_GLOBAL              2 (db)
-                    1022 LOAD_ATTR                3 (session)
-                    1032 LOAD_METHOD              4 (query)
-                    1054 LOAD_FAST                1 (table)
-                    1056 PRECALL                  1
-                    1060 CALL                     1
-                    1070 STORE_FAST              10 (baseQuery)
-         
-          58        1072 LOAD_FAST                5 (groupBy)
-                    1074 POP_JUMP_FORWARD_IF_FALSE   123 (to 1322)
-         
-          59        1076 LOAD_GLOBAL             11 (NULL + isinstance)
-                    1088 LOAD_FAST                5 (groupBy)
-                    1090 LOAD_GLOBAL             12 (list)
-                    1102 PRECALL                  2
-                    1106 CALL                     2
-                    1116 POP_JUMP_FORWARD_IF_FALSE    42 (to 1202)
-         
-          60        1118 LOAD_FAST                5 (groupBy)
-                    1120 GET_ITER
-                 >> 1122 FOR_ITER                38 (to 1200)
-                    1124 STORE_FAST               9 (gb)
-         
-          61        1126 LOAD_FAST               10 (baseQuery)
-                    1128 LOAD_METHOD              9 (group_by)
-                    1150 LOAD_GLOBAL              1 (NULL + getattr)
-                    1162 LOAD_FAST                1 (table)
-                    1164 LOAD_CONST               8 ('participantID')
-                    1166 PRECALL                  2
-                    1170 CALL                     2
-                    1180 LOAD_FAST                9 (gb)
-                    1182 PRECALL                  2
-                    1186 CALL                     2
-                    1196 STORE_FAST              10 (baseQuery)
-                    1198 JUMP_BACKWARD           39 (to 1122)
-         
-          60     >> 1200 JUMP_FORWARD            36 (to 1274)
-         
-          63     >> 1202 LOAD_FAST               10 (baseQuery)
-                    1204 LOAD_METHOD              9 (group_by)
-                    1226 LOAD_GLOBAL              1 (NULL + getattr)
-                    1238 LOAD_FAST                1 (table)
-                    1240 LOAD_CONST               8 ('participantID')
-                    1242 PRECALL                  2
-                    1246 CALL                     2
-                    1256 LOAD_FAST                5 (groupBy)
-                    1258 PRECALL                  2
-                    1262 CALL                     2
-                    1272 STORE_FAST              10 (baseQuery)
-         
-          65     >> 1274 LOAD_FAST                7 (having)
-                    1276 POP_JUMP_FORWARD_IF_NONE    21 (to 1320)
-         
-          66        1278 LOAD_FAST               10 (baseQuery)
-                    1280 LOAD_METHOD             13 (having)
-                    1302 LOAD_FAST                7 (having)
-                    1304 PRECALL                  1
-                    1308 CALL                     1
-                    1318 STORE_FAST              10 (baseQuery)
-                 >> 1320 JUMP_FORWARD            35 (to 1392)
-         
-          68     >> 1322 LOAD_FAST               10 (baseQuery)
-                    1324 LOAD_METHOD              9 (group_by)
-                    1346 LOAD_GLOBAL              1 (NULL + getattr)
-                    1358 LOAD_FAST                1 (table)
-                    1360 LOAD_CONST               8 ('participantID')
-                    1362 PRECALL                  2
-                    1366 CALL                     2
-                    1376 PRECALL                  1
-                    1380 CALL                     1
-                    1390 STORE_FAST              10 (baseQuery)
-         
-          70     >> 1392 LOAD_FAST                6 (orderBy)
-                    1394 POP_JUMP_FORWARD_IF_FALSE    21 (to 1438)
-         
-          71        1396 LOAD_FAST               10 (baseQuery)
-                    1398 LOAD_METHOD             10 (order_by)
-                    1420 LOAD_FAST                6 (orderBy)
-                    1422 PRECALL                  1
-                    1426 CALL                     1
-                    1436 STORE_FAST              10 (baseQuery)
-         
-          73     >> 1438 LOAD_FAST                4 (filter)
-                    1440 POP_JUMP_FORWARD_IF_NONE    21 (to 1484)
-         
-          74        1442 LOAD_FAST               10 (baseQuery)
-                    1444 LOAD_METHOD             11 (filter)
-                    1466 LOAD_FAST                4 (filter)
-                    1468 PRECALL                  1
-                    1472 CALL                     1
-                    1482 STORE_FAST              10 (baseQuery)
-         
-          77     >> 1484 LOAD_FAST                0 (export_dict)
-                    1486 LOAD_CONST               9 ('fields')
-                    1488 BINARY_SUBSCR
-                    1498 GET_ITER
-                 >> 1500 FOR_ITER               139 (to 1780)
-                    1502 STORE_FAST              11 (field)
-         
-          78        1504 LOAD_GLOBAL             29 (NULL + hasattr)
-                    1516 LOAD_FAST                1 (table)
-                    1518 LOAD_FAST               11 (field)
-                    1520 PRECALL                  2
-                    1524 CALL                     2
-                    1534 POP_JUMP_FORWARD_IF_FALSE    30 (to 1596)
-                    1536 LOAD_GLOBAL             31 (NULL + callable)
-                    1548 LOAD_GLOBAL              1 (NULL + getattr)
-                    1560 LOAD_FAST                1 (table)
-                    1562 LOAD_FAST               11 (field)
-                    1564 PRECALL                  2
-                    1568 CALL                     2
-                    1578 PRECALL                  1
-                    1582 CALL                     1
-                    1592 POP_JUMP_FORWARD_IF_FALSE     1 (to 1596)
-         
-          79        1594 JUMP_BACKWARD           48 (to 1500)
-         
-          80     >> 1596 LOAD_FAST                3 (fields)
-                    1598 LOAD_METHOD              7 (append)
-                    1620 LOAD_FAST               11 (field)
-                    1622 PRECALL                  1
-                    1626 CALL                     1
-                    1636 POP_TOP
-         
-          81        1638 LOAD_FAST               10 (baseQuery)
-                    1640 LOAD_METHOD              8 (add_columns)
-                    1662 LOAD_GLOBAL              3 (NULL + db)
-                    1674 LOAD_ATTR               16 (literal_column)
-                    1684 LOAD_FAST                0 (export_dict)
-                    1686 LOAD_CONST               9 ('fields')
-                    1688 BINARY_SUBSCR
-                    1698 LOAD_FAST               11 (field)
-                    1700 BINARY_SUBSCR
-                    1710 PRECALL                  1
-                    1714 CALL                     1
-                    1724 LOAD_METHOD             17 (label)
-                    1746 LOAD_FAST               11 (field)
-                    1748 PRECALL                  1
-                    1752 CALL                     1
-                    1762 PRECALL                  1
-                    1766 CALL                     1
-                    1776 STORE_FAST              10 (baseQuery)
-                    1778 JUMP_BACKWARD          140 (to 1500)
-         
-          83     >> 1780 LOAD_FAST                2 (levels)
-                    1782 LOAD_FAST                3 (fields)
-                    1784 LOAD_FAST               10 (baseQuery)
-                    1786 BUILD_TUPLE              3
-                    1788 RETURN_VALUE
-         consts
-            "\n    Builds the base query for exporting values in blueprint-defined tables.\n    To be used for each entry in the config's EXPORT\n    :param export_dict:\n    :return:\n    "
-            'table'
-            None
-            'filter'
-            ''
-            'order_by'
-            'group_by'
-            'having'
-            'participantID'
-            'fields'
-         names      ('getattr', 'db', 'text', 'session', 'query', 'isinstance', 'list', 'append', 'add_columns', 'group_by', 'order_by', 'filter', 'all', 'having', 'hasattr', 'callable', 'literal_column', 'label')
-         varnames   ('export_dict', 'table', 'levels', 'fields', 'filter', 'groupBy', 'orderBy', 'having', 'levelsQ', 'gb', 'baseQuery', 'field')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
-         name       'create_export_base_query'
-         firstlineno 7
-         lnotab
-            0x020736020401040104010401040104022001340220012c032401200134
-            023c023601040114014601460148fd02052c012a012a0204012a02040150
-            0228033e0204012a0108014aff0203480204012c02460204012a0204012a
-            0314015a0102012a018e02
-      True
-      'column_list'
-      'export_data'
-      'return'
-      code
-         argcount  : 4
-         nlocals   : 7
-         stacksize : 7
-         flags     : 3
-         code
-            0x97007400000000000000000000006a010000000000000000a002000000
-            00000000000000000000000000000000007400000000000000000000006a
-            030000000000000000a6010000ab0100000000000000007d047c0273287c
-            04a004000000000000000000000000000000000000000074000000000000
-            00000000006a0300000000000000006a05000000000000000064016b0200
-            000000a6010000ab0100000000000000007d047c03734e7c04a004000000
-            00000000000000000000000000000000007401000000000000000000006a
-            0600000000000000007400000000000000000000006a0300000000000000
-            006a07000000000000000064026b02000000007400000000000000000000
-            006a0300000000000000006a07000000000000000064036b0200000000a6
-            020000ab020000000000000000a6010000ab0100000000000000007d047c
-            00a008000000000000000000000000000000000000000067006404a201a6
-            010000ab01000000000000000001007c04a0090000000000000000000000
-            000000000000000000a6000000ab0000000000000000007d057c0544005d
-            387d067c066a0a00000000000000007c066a0b0000000000000000741900
-            0000000000000000007c066a0d0000000000000000a6010000ab01000000
-            00000000007c066a0e00000000000000007c066a05000000000000000064
-            049c057c017c066a0a00000000000000003c0000008c397c045300
-          86           0 RESUME                   0
-         
-          96           2 LOAD_GLOBAL              0 (db)
-                      14 LOAD_ATTR                1 (session)
-                      24 LOAD_METHOD              2 (query)
-                      46 LOAD_GLOBAL              0 (db)
-                      58 LOAD_ATTR                3 (Participant)
-                      68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               4 (query_participants)
-         
-          97          84 LOAD_FAST                2 (include_unfinished)
-                      86 POP_JUMP_FORWARD_IF_TRUE    40 (to 168)
-         
-          98          88 LOAD_FAST                4 (query_participants)
-                      90 LOAD_METHOD              4 (filter)
-                     112 LOAD_GLOBAL              0 (db)
-                     124 LOAD_ATTR                3 (Participant)
-                     134 LOAD_ATTR                5 (finished)
-                     144 LOAD_CONST               1 (True)
-                     146 COMPARE_OP               2 (==)
-                     152 PRECALL                  1
-                     156 CALL                     1
-                     166 STORE_FAST               4 (query_participants)
-         
-         100     >>  168 LOAD_FAST                3 (include_exluded)
-                     170 POP_JUMP_FORWARD_IF_TRUE    78 (to 328)
-         
-         101         172 LOAD_FAST                4 (query_participants)
-                     174 LOAD_METHOD              4 (filter)
-                     196 LOAD_GLOBAL              1 (NULL + db)
-                     208 LOAD_ATTR                6 (or_)
-                     218 LOAD_GLOBAL              0 (db)
-                     230 LOAD_ATTR                3 (Participant)
-                     240 LOAD_ATTR                7 (excludeFromCount)
-                     250 LOAD_CONST               2 (False)
-                     252 COMPARE_OP               2 (==)
-                     258 LOAD_GLOBAL              0 (db)
-                     270 LOAD_ATTR                3 (Participant)
-                     280 LOAD_ATTR                7 (excludeFromCount)
-                     290 LOAD_CONST               3 (None)
-                     292 COMPARE_OP               2 (==)
-                     298 PRECALL                  2
-                     302 CALL                     2
-                     312 PRECALL                  1
-                     316 CALL                     1
-                     326 STORE_FAST               4 (query_participants)
-         
-         103     >>  328 LOAD_FAST                0 (column_list)
-                     330 LOAD_METHOD              8 (extend)
-                     352 BUILD_LIST               0
-                     354 LOAD_CONST               4 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
-                     356 LIST_EXTEND              1
-                     358 PRECALL                  1
-                     362 CALL                     1
-                     372 POP_TOP
-         
-         111         374 LOAD_FAST                4 (query_participants)
-                     376 LOAD_METHOD              9 (all)
-                     398 PRECALL                  0
-                     402 CALL                     0
-                     412 STORE_FAST               5 (query_result)
-         
-         113         414 LOAD_FAST                5 (query_result)
-                     416 GET_ITER
-                 >>  418 FOR_ITER                56 (to 532)
-                     420 STORE_FAST               6 (row)
-         
-         115         422 LOAD_FAST                6 (row)
-                     424 LOAD_ATTR               10 (participantID)
-         
-         116         434 LOAD_FAST                6 (row)
-                     436 LOAD_ATTR               11 (mTurkID)
-         
-         117         446 LOAD_GLOBAL             25 (NULL + condition_num_to_label)
-                     458 LOAD_FAST                6 (row)
-                     460 LOAD_ATTR               13 (condition)
-                     470 PRECALL                  1
-                     474 CALL                     1
-         
-         118         484 LOAD_FAST                6 (row)
-                     486 LOAD_ATTR               14 (duration)
-         
-         119         496 LOAD_FAST                6 (row)
-                     498 LOAD_ATTR                5 (finished)
-         
-         114         508 LOAD_CONST               4 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
-                     510 BUILD_CONST_KEY_MAP      5
-                     512 LOAD_FAST                1 (export_data)
-                     514 LOAD_FAST                6 (row)
-                     516 LOAD_ATTR               10 (participantID)
-                     526 STORE_SUBSCR
-                     530 JUMP_BACKWARD           57 (to 418)
-         
-         122     >>  532 LOAD_FAST                4 (query_participants)
-                     534 RETURN_VALUE
-         consts
-            '\n    Add participant columns to column_list and their data to export_data.\n    :param column_list: A list of strings that will be the columns in the CSV export.\n    :param export_data: Gets updated with data for the participants\n    :return: A SQLAlchemy query.\n    '
-            True
-            False
-            None
-            ('participantID', 'externalID', 'condition', 'duration', 'finished')
-         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'or_', 'excludeFromCount', 'extend', 'all', 'participantID', 'mTurkID', 'condition_num_to_label', 'condition', 'duration')
-         varnames   ('column_list', 'export_data', 'include_unfinished', 'include_exluded', 'query_participants', 'query_result', 'row')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
-         name       'add_participants_to_export'
-         firstlineno 86
-         lnotab
-            0x020a52010401500204019c022e08280208020c010c0126010c010cfb18
-            08
-      'query_participants'
-      code
-         argcount  : 4
-         nlocals   : 19
-         stacksize : 8
-         flags     : 3
-         code
-            0x97007401000000000000000000006a0100000000000000006401ac02a6
-            010000ab0100000000000000007d047c027d0569007d0669007d077c0444
-            0090015d8e7d0867007c067c083c00000067007c077c083c000000740500
-            0000000000000000007c08a6010000ab0100000000000000005c0200007d
-            097d0a7406000000000000000000007c09190000000000000000007d0b74
-            09000000000000000000006a0500000000000000007c0b6a060000000000
-            0000007c08ac03a6020000ab0200000000000000007d0c74090000000000
-            00000000006a0700000000000000007c0c6a080000000000000000740800
-            0000000000000000006a0900000000000000006a0800000000000000006b
-            02000000007c0c6a0a00000000000000007c0a6b0200000000a6020000ab
-            0200000000000000007d0d7c03722a7c05a00b0000000000000000000000
-            0000000000000000007c0c7c0da6020000ab020000000000000000a00c00
-            000000000000000000000000000000000000007c0ca6010000ab01000000
-            00000000007d056e297c05a00d0000000000000000000000000000000000
-            0000007c0c7c0da6020000ab020000000000000000a00c00000000000000
-            000000000000000000000000007c0ca6010000ab0100000000000000007d
-            057c0ba00e0000000000000000000000000000000000000000a6000000ab
-            00000000000000000044005d427d0e7c00a00f0000000000000000000000
-            0000000000000000007c0864047a0000007c0e6a1000000000000000007a
-            000000a6010000ab01000000000000000001007c067c0819000000000000
-            000000a00f00000000000000000000000000000000000000007c0e6a1000
-            00000000000000a6010000ab01000000000000000001008c437c0ba01100
-            00000000000000000000000000000000000000a6000000ab000000000000
-            00000044005d387d0e7c00a00f0000000000000000000000000000000000
-            0000007c0864047a0000007c0e7a000000a6010000ab0100000000000000
-            0001007c077c0819000000000000000000a00f0000000000000000000000
-            0000000000000000007c0ea6010000ab01000000000000000001008c397c
-            00a00f00000000000000000000000000000000000000007c0864057a0000
-            00a6010000ab010000000000000000010090018c907c05a0120000000000
-            000000000000000000000000000000a6000000ab0000000000000000007d
-            0f7c0f44005db57d107c0444005db07d087427000000000000000000007c
-            107c08a6020000ab0200000000000000007d117c11729c7c067c08190000
-            0000000000000044005d2b7d127427000000000000000000007c117c12a6
-            020000ab0200000000000000007c017c106a0900000000000000006a0800
-            00000000000000190000000000000000007c0864047a0000007c127a0000
-            003c0000008c2c7c077c081900000000000000000044005d357d127c1172
-            3102007427000000000000000000007c117c12a6020000ab020000000000
-            000000a6000000ab0000000000000000007c017c106a0900000000000000
-            006a080000000000000000190000000000000000007c0864047a0000007c
-            127a0000003c0000008c367c11a014000000000000000000000000000000
-            0000000000a6000000ab0000000000000000007c017c106a090000000000
-            0000006a080000000000000000190000000000000000007c0864057a0000
-            003c0000008cb18cb664005300
-         125           0 RESUME                   0
-         
-         129           2 LOAD_GLOBAL              1 (NULL + page_list)
-                      14 LOAD_ATTR                1 (get_questionnaire_list)
-                      24 LOAD_CONST               1 (True)
-                      26 KW_NAMES                 2
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 STORE_FAST               4 (list_of_questionnaires)
-         
-         131          44 LOAD_FAST                2 (query_participants)
-                      46 STORE_FAST               5 (query_questionnaires)
-         
-         132          48 BUILD_MAP                0
-                      50 STORE_FAST               6 (columns)
-         
-         133          52 BUILD_MAP                0
-                      54 STORE_FAST               7 (calculated_columns)
-         
-         136          56 LOAD_FAST                4 (list_of_questionnaires)
-                      58 GET_ITER
-                 >>   60 EXTENDED_ARG             1
-                      62 FOR_ITER               398 (to 860)
-                      64 STORE_FAST               8 (entry)
-         
-         137          66 BUILD_LIST               0
-                      68 LOAD_FAST                6 (columns)
-                      70 LOAD_FAST                8 (entry)
-                      72 STORE_SUBSCR
-         
-         138          76 BUILD_LIST               0
-                      78 LOAD_FAST                7 (calculated_columns)
-                      80 LOAD_FAST                8 (entry)
-                      82 STORE_SUBSCR
-         
-         139          86 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
-                      98 LOAD_FAST                8 (entry)
-                     100 PRECALL                  1
-                     104 CALL                     1
-                     114 UNPACK_SEQUENCE          2
-                     118 STORE_FAST               9 (questionnaire_name)
-                     120 STORE_FAST              10 (questionnaire_tag)
-         
-         142         122 LOAD_GLOBAL              6 (questionnaires)
-                     134 LOAD_FAST                9 (questionnaire_name)
-                     136 BINARY_SUBSCR
-                     146 STORE_FAST              11 (questionnaire)
-         
-         145         148 LOAD_GLOBAL              9 (NULL + db)
-                     160 LOAD_ATTR                5 (aliased)
-                     170 LOAD_FAST               11 (questionnaire)
-                     172 LOAD_ATTR                6 (db_class)
-                     182 LOAD_FAST                8 (entry)
-                     184 KW_NAMES                 3
-                     186 PRECALL                  2
-                     190 CALL                     2
-                     200 STORE_FAST              12 (questionnaire_db_class)
-         
-         146         202 LOAD_GLOBAL              9 (NULL + db)
-                     214 LOAD_ATTR                7 (and_)
-                     224 LOAD_FAST               12 (questionnaire_db_class)
-                     226 LOAD_ATTR                8 (participantID)
-                     236 LOAD_GLOBAL              8 (db)
-                     248 LOAD_ATTR                9 (Participant)
-                     258 LOAD_ATTR                8 (participantID)
-                     268 COMPARE_OP               2 (==)
-         
-         147         274 LOAD_FAST               12 (questionnaire_db_class)
-                     276 LOAD_ATTR               10 (tag)
-                     286 LOAD_FAST               10 (questionnaire_tag)
-                     288 COMPARE_OP               2 (==)
-         
-         146         294 PRECALL                  2
-                     298 CALL                     2
-                     308 STORE_FAST              13 (join_condition)
-         
-         150         310 LOAD_FAST                3 (include_missing)
-                     312 POP_JUMP_FORWARD_IF_FALSE    42 (to 398)
-         
-         151         314 LOAD_FAST                5 (query_questionnaires)
-                     316 LOAD_METHOD             11 (outerjoin)
-                     338 LOAD_FAST               12 (questionnaire_db_class)
-                     340 LOAD_FAST               13 (join_condition)
-                     342 PRECALL                  2
-                     346 CALL                     2
-         
-         152         356 LOAD_METHOD             12 (add_entity)
-                     378 LOAD_FAST               12 (questionnaire_db_class)
-                     380 PRECALL                  1
-                     384 CALL                     1
-         
-         151         394 STORE_FAST               5 (query_questionnaires)
-                     396 JUMP_FORWARD            41 (to 480)
-         
-         154     >>  398 LOAD_FAST                5 (query_questionnaires)
-                     400 LOAD_METHOD             13 (join)
-                     422 LOAD_FAST               12 (questionnaire_db_class)
-                     424 LOAD_FAST               13 (join_condition)
-                     426 PRECALL                  2
-                     430 CALL                     2
-         
-         155         440 LOAD_METHOD             12 (add_entity)
-                     462 LOAD_FAST               12 (questionnaire_db_class)
-                     464 PRECALL                  1
-                     468 CALL                     1
-         
-         154         478 STORE_FAST               5 (query_questionnaires)
-         
-         159     >>  480 LOAD_FAST               11 (questionnaire)
-                     482 LOAD_METHOD             14 (fetch_fields)
-                     504 PRECALL                  0
-                     508 CALL                     0
-                     518 GET_ITER
-                 >>  520 FOR_ITER                66 (to 654)
-                     522 STORE_FAST              14 (column)
-         
-         160         524 LOAD_FAST                0 (column_list)
-                     526 LOAD_METHOD             15 (append)
-                     548 LOAD_FAST                8 (entry)
-                     550 LOAD_CONST               4 ('_')
-                     552 BINARY_OP                0 (+)
-                     556 LOAD_FAST               14 (column)
-                     558 LOAD_ATTR               16 (id)
-                     568 BINARY_OP                0 (+)
-                     572 PRECALL                  1
-                     576 CALL                     1
-                     586 POP_TOP
-         
-         161         588 LOAD_FAST                6 (columns)
-                     590 LOAD_FAST                8 (entry)
-                     592 BINARY_SUBSCR
-                     602 LOAD_METHOD             15 (append)
-                     624 LOAD_FAST               14 (column)
-                     626 LOAD_ATTR               16 (id)
-                     636 PRECALL                  1
-                     640 CALL                     1
-                     650 POP_TOP
-                     652 JUMP_BACKWARD           67 (to 520)
-         
-         164     >>  654 LOAD_FAST               11 (questionnaire)
-                     656 LOAD_METHOD             17 (get_calculated_fields)
-                     678 PRECALL                  0
-                     682 CALL                     0
-                     692 GET_ITER
-                 >>  694 FOR_ITER                56 (to 808)
-                     696 STORE_FAST              14 (column)
-         
-         165         698 LOAD_FAST                0 (column_list)
-                     700 LOAD_METHOD             15 (append)
-                     722 LOAD_FAST                8 (entry)
-                     724 LOAD_CONST               4 ('_')
-                     726 BINARY_OP                0 (+)
-                     730 LOAD_FAST               14 (column)
-                     732 BINARY_OP                0 (+)
-                     736 PRECALL                  1
-                     740 CALL                     1
-                     750 POP_TOP
-         
-         166         752 LOAD_FAST                7 (calculated_columns)
-                     754 LOAD_FAST                8 (entry)
-                     756 BINARY_SUBSCR
-                     766 LOAD_METHOD             15 (append)
-                     788 LOAD_FAST               14 (column)
-                     790 PRECALL                  1
-                     794 CALL                     1
-                     804 POP_TOP
-                     806 JUMP_BACKWARD           57 (to 694)
-         
-         169     >>  808 LOAD_FAST                0 (column_list)
-                     810 LOAD_METHOD             15 (append)
-                     832 LOAD_FAST                8 (entry)
-                     834 LOAD_CONST               5 ('_duration')
-                     836 BINARY_OP                0 (+)
-                     840 PRECALL                  1
-                     844 CALL                     1
-                     854 POP_TOP
-                     856 EXTENDED_ARG             1
-                     858 JUMP_BACKWARD          400 (to 60)
-         
-         171     >>  860 LOAD_FAST                5 (query_questionnaires)
-                     862 LOAD_METHOD             18 (all)
-                     884 PRECALL                  0
-                     888 CALL                     0
-                     898 STORE_FAST              15 (query_result)
-         
-         174         900 LOAD_FAST               15 (query_result)
-                     902 GET_ITER
-                 >>  904 FOR_ITER               181 (to 1268)
-                     906 STORE_FAST              16 (row)
-         
-         175         908 LOAD_FAST                4 (list_of_questionnaires)
-                     910 GET_ITER
-                 >>  912 FOR_ITER               176 (to 1266)
-                     914 STORE_FAST               8 (entry)
-         
-         176         916 LOAD_GLOBAL             39 (NULL + getattr)
-                     928 LOAD_FAST               16 (row)
-                     930 LOAD_FAST                8 (entry)
-                     932 PRECALL                  2
-                     936 CALL                     2
-                     946 STORE_FAST              17 (questionnaire_data)
-         
-         178         948 LOAD_FAST               17 (questionnaire_data)
-                     950 POP_JUMP_FORWARD_IF_FALSE   156 (to 1264)
-         
-         180         952 LOAD_FAST                6 (columns)
-                     954 LOAD_FAST                8 (entry)
-                     956 BINARY_SUBSCR
-                     966 GET_ITER
-                 >>  968 FOR_ITER                43 (to 1056)
-                     970 STORE_FAST              18 (col)
-         
-         181         972 LOAD_GLOBAL             39 (NULL + getattr)
-                     984 LOAD_FAST               17 (questionnaire_data)
-                     986 LOAD_FAST               18 (col)
-                     988 PRECALL                  2
-                     992 CALL                     2
-                    1002 LOAD_FAST                1 (export_data)
-                    1004 LOAD_FAST               16 (row)
-                    1006 LOAD_ATTR                9 (Participant)
-                    1016 LOAD_ATTR                8 (participantID)
-                    1026 BINARY_SUBSCR
-                    1036 LOAD_FAST                8 (entry)
-                    1038 LOAD_CONST               4 ('_')
-                    1040 BINARY_OP                0 (+)
-                    1044 LOAD_FAST               18 (col)
-                    1046 BINARY_OP                0 (+)
-                    1050 STORE_SUBSCR
-                    1054 JUMP_BACKWARD           44 (to 968)
-         
-         184     >> 1056 LOAD_FAST                7 (calculated_columns)
-                    1058 LOAD_FAST                8 (entry)
-                    1060 BINARY_SUBSCR
-                    1070 GET_ITER
-                 >> 1072 FOR_ITER                53 (to 1180)
-                    1074 STORE_FAST              18 (col)
-         
-         185        1076 LOAD_FAST               17 (questionnaire_data)
-                    1078 POP_JUMP_FORWARD_IF_FALSE    49 (to 1178)
-         
-         186        1080 PUSH_NULL
-                    1082 LOAD_GLOBAL             39 (NULL + getattr)
-                    1094 LOAD_FAST               17 (questionnaire_data)
-                    1096 LOAD_FAST               18 (col)
-                    1098 PRECALL                  2
-                    1102 CALL                     2
-                    1112 PRECALL                  0
-                    1116 CALL                     0
-                    1126 LOAD_FAST                1 (export_data)
-                    1128 LOAD_FAST               16 (row)
-                    1130 LOAD_ATTR                9 (Participant)
-                    1140 LOAD_ATTR                8 (participantID)
-                    1150 BINARY_SUBSCR
-                    1160 LOAD_FAST                8 (entry)
-                    1162 LOAD_CONST               4 ('_')
-                    1164 BINARY_OP                0 (+)
-                    1168 LOAD_FAST               18 (col)
-                    1170 BINARY_OP                0 (+)
-                    1174 STORE_SUBSCR
-                 >> 1178 JUMP_BACKWARD           54 (to 1072)
-         
-         189     >> 1180 LOAD_FAST               17 (questionnaire_data)
-                    1182 LOAD_METHOD             20 (duration)
-                    1204 PRECALL                  0
-                    1208 CALL                     0
-                    1218 LOAD_FAST                1 (export_data)
-                    1220 LOAD_FAST               16 (row)
-                    1222 LOAD_ATTR                9 (Participant)
-                    1232 LOAD_ATTR                8 (participantID)
-                    1242 BINARY_SUBSCR
-                    1252 LOAD_FAST                8 (entry)
-                    1254 LOAD_CONST               5 ('_duration')
-                    1256 BINARY_OP                0 (+)
-                    1260 STORE_SUBSCR
-                 >> 1264 JUMP_BACKWARD          177 (to 912)
-         
-         175     >> 1266 JUMP_BACKWARD          182 (to 904)
-         
-         174     >> 1268 LOAD_CONST               0 (None)
-                    1270 RETURN_VALUE
-         consts
-            None
-            True
-            ('include_tags',)
-            ('name',)
-            '_'
-            '_duration'
-         names      ('page_list', 'get_questionnaire_list', 'questionnaire_name_and_tag', 'questionnaires', 'db', 'aliased', 'db_class', 'and_', 'participantID', 'Participant', 'tag', 'outerjoin', 'add_entity', 'join', 'fetch_fields', 'append', 'id', 'get_calculated_fields', 'all', 'getattr', 'duration')
-         varnames   ('column_list', 'export_data', 'query_participants', 'include_missing', 'list_of_questionnaires', 'query_questionnaires', 'columns', 'calculated_columns', 'entry', 'questionnaire_name', 'questionnaire_tag', 'questionnaire', 'questionnaire_db_class', 'join_condition', 'column', 'query_result', 'row', 'questionnaire_data', 'col')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
-         name       'add_questionnaires_to_export'
-         firstlineno 125
-         lnotab
-            0x02042a020401040104030a010a010a0124031a033601480114ff100404
-            012a0126ff04032a0126ff02052c01400142032c01360138033402280308
-            010801200204021401540314010401640356f202ff
+      ('datetime',)
+      120
       code
-         argcount  : 4
-         nlocals   : 21
-         stacksize : 12
-         flags     : 3
-         code
-            0x970067007d047400000000000000000000006a01000000000000000064
-            011900000000000000000044005d2f7d057405000000000000000000007c
-            05a6010000ab0100000000000000005c0300007d067d077d087c04a00300
-            000000000000000000000000000000000000007c057c077c087c0664029c
-            04a6010000ab01000000000000000001008c307c0444005dda7d057c0564
-            031900000000000000000072917c0564031900000000000000000044005d
-            877d097c0564041900000000000000000064051900000000000000000044
-            005d767d0a740800000000000000000000a0050000000000000000000000
-            00000000000000000064067c0aa6020000ab0200000000000000007d0b7c
-            0944005d417d0c7c0b740800000000000000000000a00500000000000000
-            0000000000000000000000000064077409000000000000000000007c0ca6
-            010000ab010000000000000000a006000000000000000000000000000000
-            000000000064086409a6020000ab020000000000000000a6020000ab0200
-            000000000000007a0d00007d0b8c427c00a0030000000000000000000000
-            0000000000000000007c0ba6010000ab01000000000000000001008c778c
-            888c9b7c0564041900000000000000000064051900000000000000000044
-            005d307d0a7c00a003000000000000000000000000000000000000000074
-            0800000000000000000000a0050000000000000000000000000000000000
-            00000064067c0aa6020000ab020000000000000000a6010000ab01000000
-            000000000001008c318cdb7c02a007000000000000000000000000000000
-            0000000000a6000000ab0000000000000000007d0d7c0d44005dbb7d0e7c
-            0e6a0800000000000000007d0f7c0444005daf7d057c05640a1900000000
-            00000000007d107c10a00900000000000000000000000000000000000000
-            007415000000000000000000006a0b0000000000000000640ba6010000ab
-            0100000000000000007c0e6a0800000000000000006b0200000000a60100
-            00ab0100000000000000007d107c10a00700000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d11640c7d127c1144
-            005d5c7d137c0564051900000000000000000044005d4c7d0a7c0a7d147c
-            0564031900000000000000000072277c0a64097a00000074090000000000
-            00000000007c056403190000000000000000007c12190000000000000000
-            00640c19000000000000000000a6010000ab0100000000000000007a0000
-            007d147419000000000000000000007c137c0aa6020000ab020000000000
-            0000007c017c0f190000000000000000007c143c0000008c4d7c12640d7a
-            0d00007d128c5d8cb08cbc64005300
-         192           0 RESUME                   0
-         
-         197           2 BUILD_LIST               0
-                       4 STORE_FAST               4 (custom_exports)
-         
-         199           6 LOAD_GLOBAL              0 (current_app)
-                      18 LOAD_ATTR                1 (config)
-                      28 LOAD_CONST               1 ('EXPORT')
-                      30 BINARY_SUBSCR
-                      40 GET_ITER
-                 >>   42 FOR_ITER                47 (to 138)
-                      44 STORE_FAST               5 (export)
-         
-         200          46 LOAD_GLOBAL              5 (NULL + create_export_base_query)
-                      58 LOAD_FAST                5 (export)
-                      60 PRECALL                  1
-                      64 CALL                     1
-                      74 UNPACK_SEQUENCE          3
-                      78 STORE_FAST               6 (levels)
-                      80 STORE_FAST               7 (fields)
-                      82 STORE_FAST               8 (base_query)
-         
-         201          84 LOAD_FAST                4 (custom_exports)
-                      86 LOAD_METHOD              3 (append)
-                     108 LOAD_FAST                5 (export)
-                     110 LOAD_FAST                7 (fields)
-                     112 LOAD_FAST                8 (base_query)
-                     114 LOAD_FAST                6 (levels)
-                     116 LOAD_CONST               2 (('options', 'fields', 'base_query', 'levels'))
-                     118 BUILD_CONST_KEY_MAP      4
-                     120 PRECALL                  1
-                     124 CALL                     1
-                     134 POP_TOP
-                     136 JUMP_BACKWARD           48 (to 42)
-         
-         204     >>  138 LOAD_FAST                4 (custom_exports)
-                     140 GET_ITER
-                 >>  142 FOR_ITER               218 (to 580)
-                     144 STORE_FAST               5 (export)
-         
-         205         146 LOAD_FAST                5 (export)
-                     148 LOAD_CONST               3 ('levels')
-                     150 BINARY_SUBSCR
-                     160 POP_JUMP_FORWARD_IF_FALSE   145 (to 452)
-         
-         206         162 LOAD_FAST                5 (export)
-                     164 LOAD_CONST               3 ('levels')
-                     166 BINARY_SUBSCR
-                     176 GET_ITER
-                 >>  178 FOR_ITER               135 (to 450)
-                     180 STORE_FAST               9 (level)
-         
-         207         182 LOAD_FAST                5 (export)
-                     184 LOAD_CONST               4 ('options')
-                     186 BINARY_SUBSCR
-                     196 LOAD_CONST               5 ('fields')
-                     198 BINARY_SUBSCR
-                     208 GET_ITER
-                 >>  210 FOR_ITER               118 (to 448)
-                     212 STORE_FAST              10 (field)
-         
-         208         214 LOAD_GLOBAL              8 (str)
-                     226 LOAD_METHOD              5 (format)
-                     248 LOAD_CONST               6 ('{}')
-                     250 LOAD_FAST               10 (field)
-                     252 PRECALL                  2
-                     256 CALL                     2
-                     266 STORE_FAST              11 (column_header)
-         
-         209         268 LOAD_FAST                9 (level)
-                     270 GET_ITER
-                 >>  272 FOR_ITER                65 (to 404)
-                     274 STORE_FAST              12 (level_name)
-         
-         210         276 LOAD_FAST               11 (column_header)
-                     278 LOAD_GLOBAL              8 (str)
-                     290 LOAD_METHOD              5 (format)
-                     312 LOAD_CONST               7 ('_{}')
-                     314 LOAD_GLOBAL              9 (NULL + str)
-                     326 LOAD_FAST               12 (level_name)
-                     328 PRECALL                  1
-                     332 CALL                     1
-                     342 LOAD_METHOD              6 (replace)
-                     364 LOAD_CONST               8 (' ')
-                     366 LOAD_CONST               9 ('_')
-                     368 PRECALL                  2
-                     372 CALL                     2
-                     382 PRECALL                  2
-                     386 CALL                     2
-                     396 BINARY_OP               13 (+=)
-                     400 STORE_FAST              11 (column_header)
-                     402 JUMP_BACKWARD           66 (to 272)
-         
-         211     >>  404 LOAD_FAST                0 (column_list)
-                     406 LOAD_METHOD              3 (append)
-                     428 LOAD_FAST               11 (column_header)
-                     430 PRECALL                  1
-                     434 CALL                     1
-                     444 POP_TOP
-                     446 JUMP_BACKWARD          119 (to 210)
-         
-         207     >>  448 JUMP_BACKWARD          136 (to 178)
-         
-         206     >>  450 JUMP_BACKWARD          155 (to 142)
-         
-         213     >>  452 LOAD_FAST                5 (export)
-                     454 LOAD_CONST               4 ('options')
-                     456 BINARY_SUBSCR
-                     466 LOAD_CONST               5 ('fields')
-                     468 BINARY_SUBSCR
-                     478 GET_ITER
-                 >>  480 FOR_ITER                48 (to 578)
-                     482 STORE_FAST              10 (field)
-         
-         214         484 LOAD_FAST                0 (column_list)
-                     486 LOAD_METHOD              3 (append)
-                     508 LOAD_GLOBAL              8 (str)
-                     520 LOAD_METHOD              5 (format)
-                     542 LOAD_CONST               6 ('{}')
-                     544 LOAD_FAST               10 (field)
-                     546 PRECALL                  2
-                     550 CALL                     2
-                     560 PRECALL                  1
-                     564 CALL                     1
-                     574 POP_TOP
-                     576 JUMP_BACKWARD           49 (to 480)
-         
-         213     >>  578 JUMP_BACKWARD          219 (to 142)
-         
-         216     >>  580 LOAD_FAST                2 (query_participants)
-                     582 LOAD_METHOD              7 (all)
-                     604 PRECALL                  0
-                     608 CALL                     0
-                     618 STORE_FAST              13 (query_result)
-         
-         219         620 LOAD_FAST               13 (query_result)
-                     622 GET_ITER
-                 >>  624 FOR_ITER               187 (to 1000)
-                     626 STORE_FAST              14 (row)
-         
-         220         628 LOAD_FAST               14 (row)
-                     630 LOAD_ATTR                8 (participantID)
-                     640 STORE_FAST              15 (participant_id)
-         
-         222         642 LOAD_FAST                4 (custom_exports)
-                     644 GET_ITER
-                 >>  646 FOR_ITER               175 (to 998)
-                     648 STORE_FAST               5 (export)
-         
-         223         650 LOAD_FAST                5 (export)
-                     652 LOAD_CONST              10 ('base_query')
-                     654 BINARY_SUBSCR
-                     664 STORE_FAST              16 (query)
-         
-         224         666 LOAD_FAST               16 (query)
-                     668 LOAD_METHOD              9 (filter)
-                     690 LOAD_GLOBAL             21 (NULL + db)
-                     702 LOAD_ATTR               11 (literal_column)
-                     712 LOAD_CONST              11 ('participantID')
-                     714 PRECALL                  1
-                     718 CALL                     1
-                     728 LOAD_FAST               14 (row)
-                     730 LOAD_ATTR                8 (participantID)
-                     740 COMPARE_OP               2 (==)
-                     746 PRECALL                  1
-                     750 CALL                     1
-                     760 STORE_FAST              16 (query)
-         
-         225         762 LOAD_FAST               16 (query)
-                     764 LOAD_METHOD              7 (all)
-                     786 PRECALL                  0
-                     790 CALL                     0
-                     800 STORE_FAST              17 (custom_export_data)
-         
-         227         802 LOAD_CONST              12 (0)
-                     804 STORE_FAST              18 (export_row_index)
-         
-         228         806 LOAD_FAST               17 (custom_export_data)
-                     808 GET_ITER
-                 >>  810 FOR_ITER                92 (to 996)
-                     812 STORE_FAST              19 (custom_export_row)
-         
-         229         814 LOAD_FAST                5 (export)
-                     816 LOAD_CONST               5 ('fields')
-                     818 BINARY_SUBSCR
-                     828 GET_ITER
-                 >>  830 FOR_ITER                76 (to 984)
-                     832 STORE_FAST              10 (field)
-         
-         230         834 LOAD_FAST               10 (field)
-                     836 STORE_FAST              20 (export_column_name)
-         
-         231         838 LOAD_FAST                5 (export)
-                     840 LOAD_CONST               3 ('levels')
-                     842 BINARY_SUBSCR
-                     852 POP_JUMP_FORWARD_IF_FALSE    39 (to 932)
-         
-         232         854 LOAD_FAST               10 (field)
-                     856 LOAD_CONST               9 ('_')
-                     858 BINARY_OP                0 (+)
-                     862 LOAD_GLOBAL              9 (NULL + str)
-                     874 LOAD_FAST                5 (export)
-                     876 LOAD_CONST               3 ('levels')
-                     878 BINARY_SUBSCR
-                     888 LOAD_FAST               18 (export_row_index)
-                     890 BINARY_SUBSCR
-                     900 LOAD_CONST              12 (0)
-                     902 BINARY_SUBSCR
-                     912 PRECALL                  1
-                     916 CALL                     1
-                     926 BINARY_OP                0 (+)
-                     930 STORE_FAST              20 (export_column_name)
-         
-         234     >>  932 LOAD_GLOBAL             25 (NULL + getattr)
-                     944 LOAD_FAST               19 (custom_export_row)
-                     946 LOAD_FAST               10 (field)
-                     948 PRECALL                  2
-                     952 CALL                     2
-                     962 LOAD_FAST                1 (export_data)
-                     964 LOAD_FAST               15 (participant_id)
-                     966 BINARY_SUBSCR
-                     976 LOAD_FAST               20 (export_column_name)
-                     978 STORE_SUBSCR
-                     982 JUMP_BACKWARD           77 (to 830)
-         
-         236     >>  984 LOAD_FAST               18 (export_row_index)
-                     986 LOAD_CONST              13 (1)
-                     988 BINARY_OP               13 (+=)
-                     992 STORE_FAST              18 (export_row_index)
-                     994 JUMP_BACKWARD           93 (to 810)
-         
-         228     >>  996 JUMP_BACKWARD          176 (to 646)
-         
-         222     >>  998 JUMP_BACKWARD          188 (to 624)
-         
-         219     >> 1000 LOAD_CONST               0 (None)
-                    1002 RETURN_VALUE
-         consts
-            None
-            'EXPORT'
-            ('options', 'fields', 'base_query', 'levels')
-            'levels'
-            'options'
-            'fields'
-            '{}'
-            '_{}'
-            ' '
-            '_'
-            'base_query'
-            'participantID'
-            0
-            1
-         names      ('current_app', 'config', 'create_export_base_query', 'append', 'str', 'format', 'replace', 'all', 'participantID', 'filter', 'db', 'literal_column', 'getattr')
-         varnames   ('column_list', 'export_data', 'query_participants', 'include_missing', 'custom_exports', 'export', 'levels', 'fields', 'base_query', 'level', 'field', 'column_header', 'level_name', 'query_result', 'row', 'participant_id', 'query', 'custom_export_data', 'export_row_index', 'custom_export_row', 'export_column_name')
-         freevars   ()
-         cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
-         name       'add_custom_exports_to_export'
-         firstlineno 192
-         lnotab
-            0x0205040228012601360308011001140120013601080180012cfc02ff02
-            0720015eff0203280308010e020801100160012802040108011401040110
-            014e0234020cf802fa02fd
-      code
-         argcount  : 2
-         nlocals   : 6
+         argcount  : 0
+         nlocals   : 0
          stacksize : 7
-         flags     : 3
+         flags     : 0
          code
-            0x97006401a00000000000000000000000000000000000000000007c00a6
-            010000ab01000000000000000064027a0000007d027c01a0010000000000
-            000000000000000000000000000000a6000000ab00000000000000000044
-            005d3e7d0364037d047c0044005d277d057c057c037600721c7c04740500
-            0000000000000000007c037c0519000000000000000000a6010000ab0100
-            0000000000000064017a0000007a0d00007d048c227c0464017a0d00007d
-            048c287c027c046400640485021900000000000000000064027a0000007a
-            0d00007d028c3f7c02640064048502190000000000000000005300
-         239           0 RESUME                   0
-         
-         240           2 LOAD_CONST               1 (',')
-                       4 LOAD_METHOD              0 (join)
-                      26 LOAD_FAST                0 (column_list)
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 LOAD_CONST               2 ('\n')
-                      44 BINARY_OP                0 (+)
-                      48 STORE_FAST               2 (csv_string)
-         
-         242          50 LOAD_FAST                1 (export_data)
-                      52 LOAD_METHOD              1 (values)
-                      74 PRECALL                  0
-                      78 CALL                     0
-                      88 GET_ITER
-                 >>   90 FOR_ITER                62 (to 216)
-                      92 STORE_FAST               3 (row)
-         
-         243          94 LOAD_CONST               3 ('')
-                      96 STORE_FAST               4 (csv_line)
-         
-         244          98 LOAD_FAST                0 (column_list)
-                     100 GET_ITER
-                 >>  102 FOR_ITER                39 (to 182)
-                     104 STORE_FAST               5 (column)
-         
-         245         106 LOAD_FAST                5 (column)
-                     108 LOAD_FAST                3 (row)
-                     110 CONTAINS_OP              0
-                     112 POP_JUMP_FORWARD_IF_FALSE    28 (to 170)
-         
-         246         114 LOAD_FAST                4 (csv_line)
-                     116 LOAD_GLOBAL              5 (NULL + escape_csv)
-                     128 LOAD_FAST                3 (row)
-                     130 LOAD_FAST                5 (column)
-                     132 BINARY_SUBSCR
-                     142 PRECALL                  1
-                     146 CALL                     1
-                     156 LOAD_CONST               1 (',')
-                     158 BINARY_OP                0 (+)
-                     162 BINARY_OP               13 (+=)
-                     166 STORE_FAST               4 (csv_line)
-                     168 JUMP_BACKWARD           34 (to 102)
-         
-         248     >>  170 LOAD_FAST                4 (csv_line)
-                     172 LOAD_CONST               1 (',')
-                     174 BINARY_OP               13 (+=)
-                     178 STORE_FAST               4 (csv_line)
-                     180 JUMP_BACKWARD           40 (to 102)
-         
-         250     >>  182 LOAD_FAST                2 (csv_string)
-                     184 LOAD_FAST                4 (csv_line)
-                     186 LOAD_CONST               0 (None)
-                     188 LOAD_CONST               4 (-1)
-                     190 BUILD_SLICE              2
-                     192 BINARY_SUBSCR
-                     202 LOAD_CONST               2 ('\n')
-                     204 BINARY_OP                0 (+)
-                     208 BINARY_OP               13 (+=)
-                     212 STORE_FAST               2 (csv_string)
-                     214 JUMP_BACKWARD           63 (to 90)
-         
-         252     >>  216 LOAD_FAST                2 (csv_string)
-                     218 LOAD_CONST               0 (None)
-                     220 LOAD_CONST               4 (-1)
-                     222 BUILD_SLICE              2
-                     224 BINARY_SUBSCR
-                     234 RETURN_VALUE
+            0x970065005a0164005a02640f6402650364017a0700006602640384055a
+            046410640584045a056410640684045a066410640784045a076408650864
+            046509650a650a64096603190000000000000000006604640a84045a0b64
+            0b84005a0c6411640d84045a0d640465036602640e84045a0e64015300
+          13           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('Results')
+                       8 STORE_NAME               2 (__qualname__)
+         
+          14          10 LOAD_CONST              15 ((None, None))
+                      12 LOAD_CONST               2 ('cache_path')
+                      14 LOAD_NAME                3 (str)
+                      16 LOAD_CONST               1 (None)
+                      18 BINARY_OP                7 (|)
+                      22 BUILD_TUPLE              2
+                      24 LOAD_CONST               3 (<code object __init__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 14>)
+                      26 MAKE_FUNCTION            5 (defaults, annotations)
+                      28 STORE_NAME               4 (__init__)
+         
+          37          30 LOAD_CONST              16 (('return', None))
+                      32 LOAD_CONST               5 (<code object handle_participants_table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 37>)
+                      34 MAKE_FUNCTION            4 (annotations)
+                      36 STORE_NAME               5 (handle_participants_table)
+         
+          68          38 LOAD_CONST              16 (('return', None))
+                      40 LOAD_CONST               6 (<code object handle_questionnaires, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 68>)
+                      42 MAKE_FUNCTION            4 (annotations)
+                      44 STORE_NAME               6 (handle_questionnaires)
+         
+         129          46 LOAD_CONST              16 (('return', None))
+                      48 LOAD_CONST               7 (<code object handle_custom_exports, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 129>)
+                      50 MAKE_FUNCTION            4 (annotations)
+                      52 STORE_NAME               7 (handle_custom_exports)
+         
+         172          54 LOAD_CONST               8 ('export_definition')
+                      56 LOAD_NAME                8 (dict)
+                      58 LOAD_CONST               4 ('return')
+                      60 LOAD_NAME                9 (tuple)
+                      62 LOAD_NAME               10 (list)
+                      64 LOAD_NAME               10 (list)
+                      66 LOAD_CONST               9 ('Query')
+                      68 BUILD_TUPLE              3
+                      70 BINARY_SUBSCR
+                      80 BUILD_TUPLE              4
+                      82 LOAD_CONST              10 (<code object create_export_base_query, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 172>)
+                      84 MAKE_FUNCTION            4 (annotations)
+                      86 STORE_NAME              11 (create_export_base_query)
+         
+         250          88 LOAD_CONST              11 (<code object load_data_frame, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 250>)
+                      90 MAKE_FUNCTION            0
+                      92 STORE_NAME              12 (load_data_frame)
+         
+         257          94 LOAD_CONST              17 (('return', 'pd.DataFrame'))
+                      96 LOAD_CONST              13 (<code object build_data_frame, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 257>)
+                      98 MAKE_FUNCTION            4 (annotations)
+                     100 STORE_NAME              13 (build_data_frame)
+         
+         272         102 LOAD_CONST               4 ('return')
+                     104 LOAD_NAME                3 (str)
+                     106 BUILD_TUPLE              2
+                     108 LOAD_CONST              14 (<code object build_export_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\Results.py", line 272>)
+                     110 MAKE_FUNCTION            4 (annotations)
+                     112 STORE_NAME              14 (build_export_csv)
+                     114 LOAD_CONST               1 (None)
+                     116 RETURN_VALUE
          consts
+            'Results'
             None
-            ','
-            '\n'
-            ''
-            -1
-         names      ('join', 'values', 'escape_csv')
-         varnames   ('column_list', 'export_data', 'csv_string', 'row', 'csv_line', 'column')
+            'cache_path'
+            code
+               argcount  : 3
+               nlocals   : 5
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007c027c005f00000000000000000064017d037c0281837402000000
+                  000000000000006a020000000000000000a0030000000000000000000000
+                  0000000000000000007c02a6010000ab0100000000000000007264740900
+                  0000000000000000006a0500000000000000007402000000000000000000
+                  006a020000000000000000a0060000000000000000000000000000000000
+                  0000007c02a6010000ab010000000000000000a6010000ab010000000000
+                  0000007d047409000000000000000000006a070000000000000000a60000
+                  00ab0000000000000000007c047a0a0000a0080000000000000000000000
+                  000000000000000000a6000000ab00000000000000000074120000000000
+                  00000000006b0000000000720264027d0364007c005f0a00000000000000
+                  0067007c005f0b000000000000000069007c005f0c00000000000000007c
+                  0001007c017c005f0d00000000000000007c0372167c00a00e0000000000
+                  000000000000000000000000000000a6000000ab00000000000000000001
+                  00640053007c00a00f0000000000000000000000000000000000000000a6
+                  000000ab00000000000000000001007c00a0100000000000000000000000
+                  000000000000000000a6000000ab00000000000000000001007c00a01100
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  000000010064005300
+                14           0 RESUME                   0
+               
+                15           2 LOAD_FAST                2 (cache_path)
+                             4 LOAD_FAST                0 (self)
+                             6 STORE_ATTR               0 (cache_path)
+               
+                16          16 LOAD_CONST               1 (False)
+                            18 STORE_FAST               3 (use_cache)
+               
+                18          20 LOAD_FAST                2 (cache_path)
+                            22 POP_JUMP_FORWARD_IF_NONE   131 (to 286)
+               
+                19          24 LOAD_GLOBAL              2 (os)
+                            36 LOAD_ATTR                2 (path)
+                            46 LOAD_METHOD              3 (exists)
+                            68 LOAD_FAST                2 (cache_path)
+                            70 PRECALL                  1
+                            74 CALL                     1
+                            84 POP_JUMP_FORWARD_IF_FALSE   100 (to 286)
+               
+                20          86 LOAD_GLOBAL              9 (NULL + datetime)
+                            98 LOAD_ATTR                5 (utcfromtimestamp)
+                           108 LOAD_GLOBAL              2 (os)
+                           120 LOAD_ATTR                2 (path)
+                           130 LOAD_METHOD              6 (getmtime)
+                           152 LOAD_FAST                2 (cache_path)
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 PRECALL                  1
+                           172 CALL                     1
+                           182 STORE_FAST               4 (modified_time)
+               
+                21         184 LOAD_GLOBAL              9 (NULL + datetime)
+                           196 LOAD_ATTR                7 (utcnow)
+                           206 PRECALL                  0
+                           210 CALL                     0
+                           220 LOAD_FAST                4 (modified_time)
+                           222 BINARY_OP               10 (-)
+                           226 LOAD_METHOD              8 (total_seconds)
+                           248 PRECALL                  0
+                           252 CALL                     0
+                           262 LOAD_GLOBAL             18 (MAX_CACHE_SECONDS)
+                           274 COMPARE_OP               0 (<)
+                           280 POP_JUMP_FORWARD_IF_FALSE     2 (to 286)
+               
+                22         282 LOAD_CONST               2 (True)
+                           284 STORE_FAST               3 (use_cache)
+               
+                24     >>  286 LOAD_CONST               0 (None)
+                           288 LOAD_FAST                0 (self)
+                           290 STORE_ATTR              10 (df)
+               
+                25         300 BUILD_LIST               0
+                           302 LOAD_FAST                0 (self)
+                           304 STORE_ATTR              11 (column_list)
+               
+                26         314 BUILD_MAP                0
+                           316 LOAD_FAST                0 (self)
+                           318 STORE_ATTR              12 (export_data)
+               
+                27         328 LOAD_FAST                0 (self)
+                           330 POP_TOP
+               
+                28         332 LOAD_FAST                1 (filter_criterion)
+                           334 LOAD_FAST                0 (self)
+                           336 STORE_ATTR              13 (query_filter_criterion)
+               
+                30         346 LOAD_FAST                3 (use_cache)
+                           348 POP_JUMP_FORWARD_IF_FALSE    22 (to 394)
+               
+                31         350 LOAD_FAST                0 (self)
+                           352 LOAD_METHOD             14 (load_data_frame)
+                           374 PRECALL                  0
+                           378 CALL                     0
+                           388 POP_TOP
+                           390 LOAD_CONST               0 (None)
+                           392 RETURN_VALUE
+               
+                33     >>  394 LOAD_FAST                0 (self)
+                           396 LOAD_METHOD             15 (handle_participants_table)
+                           418 PRECALL                  0
+                           422 CALL                     0
+                           432 POP_TOP
+               
+                34         434 LOAD_FAST                0 (self)
+                           436 LOAD_METHOD             16 (handle_questionnaires)
+                           458 PRECALL                  0
+                           462 CALL                     0
+                           472 POP_TOP
+               
+                35         474 LOAD_FAST                0 (self)
+                           476 LOAD_METHOD             17 (handle_custom_exports)
+                           498 PRECALL                  0
+                           502 CALL                     0
+                           512 POP_TOP
+                           514 LOAD_CONST               0 (None)
+                           516 RETURN_VALUE
+               consts
+                  None
+                  False
+                  True
+               names      ('cache_path', 'os', 'path', 'exists', 'datetime', 'utcfromtimestamp', 'getmtime', 'utcnow', 'total_seconds', 'MAX_CACHE_SECONDS', 'df', 'column_list', 'export_data', 'query_filter_criterion', 'load_data_frame', 'handle_participants_table', 'handle_questionnaires', 'handle_custom_exports')
+               varnames   ('self', 'filter_criterion', 'cache_path', 'use_cache', 'modified_time')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       '__init__'
+               firstlineno 14
+               lnotab
+                  0x02010e01040204013e016201620104020e010e010e0104010e0204012c
+                  0228012801
+            'return'
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 7
+               flags     : 3
+               code
+                  0x97007400000000000000000000006a010000000000000000a002000000
+                  00000000000000000000000000000000007400000000000000000000006a
+                  030000000000000000a6010000ab0100000000000000007c005f04000000
+                  00000000007c006a05000000000000000081247c006a0400000000000000
+                  00a00600000000000000000000000000000000000000007c006a05000000
+                  0000000000a6010000ab0100000000000000007c005f0400000000000000
+                  007c006a070000000000000000a008000000000000000000000000000000
+                  000000000067006402a201a6010000ab01000000000000000001007c006a
+                  040000000000000000a00900000000000000000000000000000000000000
+                  00a6000000ab0000000000000000007d017c0144005d3d7d027c026a0a00
+                  000000000000007c026a0b00000000000000007419000000000000000000
+                  007c026a0d0000000000000000a6010000ab0100000000000000007c026a
+                  0e00000000000000007c026a0f000000000000000064029c057c006a1000
+                  000000000000007c026a0a00000000000000003c0000008c3e64015300
+                37           0 RESUME                   0
+               
+                44           2 LOAD_GLOBAL              0 (db)
+                            14 LOAD_ATTR                1 (session)
+                            24 LOAD_METHOD              2 (query)
+                            46 LOAD_GLOBAL              0 (db)
+                            58 LOAD_ATTR                3 (Participant)
+                            68 PRECALL                  1
+                            72 CALL                     1
+                            82 LOAD_FAST                0 (self)
+                            84 STORE_ATTR               4 (query_participants)
+               
+                46          94 LOAD_FAST                0 (self)
+                            96 LOAD_ATTR                5 (query_filter_criterion)
+                           106 POP_JUMP_FORWARD_IF_NONE    36 (to 180)
+               
+                47         108 LOAD_FAST                0 (self)
+                           110 LOAD_ATTR                4 (query_participants)
+                           120 LOAD_METHOD              6 (filter)
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                5 (query_filter_criterion)
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 LOAD_FAST                0 (self)
+                           170 STORE_ATTR               4 (query_participants)
+               
+                49     >>  180 LOAD_FAST                0 (self)
+                           182 LOAD_ATTR                7 (column_list)
+                           192 LOAD_METHOD              8 (extend)
+                           214 BUILD_LIST               0
+                           216 LOAD_CONST               2 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
+                           218 LIST_EXTEND              1
+                           220 PRECALL                  1
+                           224 CALL                     1
+                           234 POP_TOP
+               
+                57         236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                4 (query_participants)
+                           248 LOAD_METHOD              9 (all)
+                           270 PRECALL                  0
+                           274 CALL                     0
+                           284 STORE_FAST               1 (query_result)
+               
+                59         286 LOAD_FAST                1 (query_result)
+                           288 GET_ITER
+                       >>  290 FOR_ITER                61 (to 414)
+                           292 STORE_FAST               2 (row)
+               
+                61         294 LOAD_FAST                2 (row)
+                           296 LOAD_ATTR               10 (participantID)
+               
+                62         306 LOAD_FAST                2 (row)
+                           308 LOAD_ATTR               11 (mTurkID)
+               
+                63         318 LOAD_GLOBAL             25 (NULL + condition_num_to_label)
+                           330 LOAD_FAST                2 (row)
+                           332 LOAD_ATTR               13 (condition)
+                           342 PRECALL                  1
+                           346 CALL                     1
+               
+                64         356 LOAD_FAST                2 (row)
+                           358 LOAD_ATTR               14 (duration)
+               
+                65         368 LOAD_FAST                2 (row)
+                           370 LOAD_ATTR               15 (finished)
+               
+                60         380 LOAD_CONST               2 (('participantID', 'externalID', 'condition', 'duration', 'finished'))
+                           382 BUILD_CONST_KEY_MAP      5
+                           384 LOAD_FAST                0 (self)
+                           386 LOAD_ATTR               16 (export_data)
+                           396 LOAD_FAST                2 (row)
+                           398 LOAD_ATTR               10 (participantID)
+                           408 STORE_SUBSCR
+                           412 JUMP_BACKWARD           62 (to 290)
+               
+                59     >>  414 LOAD_CONST               1 (None)
+                           416 RETURN_VALUE
+               consts
+                  '\n        Add participant columns to column_list and their data to export_data.\n        :param column_list: A list of strings that will be the columns in the CSV export.\n        :param export_data: Gets updated with data for the participants\n        :return: A SQLAlchemy query.\n        '
+                  None
+                  ('participantID', 'externalID', 'condition', 'duration', 'finished')
+               names      ('db', 'session', 'query', 'Participant', 'query_participants', 'query_filter_criterion', 'filter', 'column_list', 'extend', 'all', 'participantID', 'mTurkID', 'condition_num_to_label', 'condition', 'duration', 'finished', 'export_data')
+               varnames   ('self', 'query_result', 'row')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'handle_participants_table'
+               firstlineno 37
+               lnotab 0x02075c020e0148023808320208020c010c0126010c010cfb22ff
+            code
+               argcount  : 1
+               nlocals   : 16
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007401000000000000000000006a0100000000000000006401ac02a6
+                  010000ab0100000000000000007d017c006a0200000000000000007d0269
+                  007d0369007d047c01440090015d717d0567007c037c053c00000067007c
+                  047c053c0000007407000000000000000000007c05a6010000ab01000000
+                  00000000005c0200007d067d077408000000000000000000007c06190000
+                  000000000000007d08740b000000000000000000006a0600000000000000
+                  007c086a0700000000000000007c05ac03a6020000ab0200000000000000
+                  007d09740b000000000000000000006a0800000000000000007c096a0900
+                  00000000000000740a000000000000000000006a0a00000000000000006a
+                  0900000000000000006b02000000007c096a0b00000000000000007c076b
+                  0200000000a6020000ab0200000000000000007d0a7c02a00c0000000000
+                  0000000000000000000000000000007c097c0aa6020000ab020000000000
+                  000000a00d00000000000000000000000000000000000000007c09a60100
+                  00ab0100000000000000007d027c08a00e00000000000000000000000000
+                  00000000000000a6000000ab00000000000000000044005d477d0b7c006a
+                  0f0000000000000000a01000000000000000000000000000000000000000
+                  007c0564047a0000007c0b6a1100000000000000007a000000a6010000ab
+                  01000000000000000001007c037c0519000000000000000000a010000000
+                  00000000000000000000000000000000007c0b6a110000000000000000a6
+                  010000ab01000000000000000001008c487c08a012000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000044005d3d7d
+                  0b7c006a0f0000000000000000a010000000000000000000000000000000
+                  00000000007c0564047a0000007c0b7a000000a6010000ab010000000000
+                  00000001007c047c0519000000000000000000a010000000000000000000
+                  00000000000000000000007c0ba6010000ab01000000000000000001008c
+                  3e7c006a0f0000000000000000a010000000000000000000000000000000
+                  00000000007c0564057a000000a6010000ab010000000000000000010090
+                  018c737c02a0130000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007d0c7c0c44005dc47d0d7c0144005dbf7d0574
+                  29000000000000000000007c0d7c05a6020000ab0200000000000000007d
+                  0e7c0e72ab7c037c051900000000000000000044005d307d0f7429000000
+                  000000000000007c0e7c0fa6020000ab0200000000000000007c006a1500
+                  000000000000007c0d6a0a00000000000000006a09000000000000000019
+                  0000000000000000007c0564047a0000007c0f7a0000003c0000008c317c
+                  047c051900000000000000000044005d3a7d0f7c0e723602007429000000
+                  000000000000007c0e7c0fa6020000ab020000000000000000a6000000ab
+                  0000000000000000007c006a1500000000000000007c0d6a0a0000000000
+                  0000006a090000000000000000190000000000000000007c0564047a0000
+                  007c0f7a0000003c0000008c3b7c0ea01600000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007c006a150000000000
+                  0000007c0d6a0a00000000000000006a0900000000000000001900000000
+                  00000000007c0564057a0000003c0000008cc08cc564005300
+                68           0 RESUME                   0
+               
+                69           2 LOAD_GLOBAL              1 (NULL + page_list)
+                            14 LOAD_ATTR                1 (get_questionnaire_list)
+                            24 LOAD_CONST               1 (True)
+                            26 KW_NAMES                 2
+                            28 PRECALL                  1
+                            32 CALL                     1
+                            42 STORE_FAST               1 (list_of_questionnaires)
+               
+                71          44 LOAD_FAST                0 (self)
+                            46 LOAD_ATTR                2 (query_participants)
+                            56 STORE_FAST               2 (query_questionnaires)
+               
+                72          58 BUILD_MAP                0
+                            60 STORE_FAST               3 (q_columns)
+               
+                73          62 BUILD_MAP                0
+                            64 STORE_FAST               4 (q_calculated_columns)
+               
+                76          66 LOAD_FAST                1 (list_of_questionnaires)
+                            68 GET_ITER
+                       >>   70 EXTENDED_ARG             1
+                            72 FOR_ITER               369 (to 812)
+                            74 STORE_FAST               5 (entry)
+               
+                77          76 BUILD_LIST               0
+                            78 LOAD_FAST                3 (q_columns)
+                            80 LOAD_FAST                5 (entry)
+                            82 STORE_SUBSCR
+               
+                78          86 BUILD_LIST               0
+                            88 LOAD_FAST                4 (q_calculated_columns)
+                            90 LOAD_FAST                5 (entry)
+                            92 STORE_SUBSCR
+               
+                79          96 LOAD_GLOBAL              7 (NULL + questionnaire_name_and_tag)
+                           108 LOAD_FAST                5 (entry)
+                           110 PRECALL                  1
+                           114 CALL                     1
+                           124 UNPACK_SEQUENCE          2
+                           128 STORE_FAST               6 (questionnaire_name)
+                           130 STORE_FAST               7 (questionnaire_tag)
+               
+                82         132 LOAD_GLOBAL              8 (questionnaires)
+                           144 LOAD_FAST                6 (questionnaire_name)
+                           146 BINARY_SUBSCR
+                           156 STORE_FAST               8 (questionnaire)
+               
+                85         158 LOAD_GLOBAL             11 (NULL + db)
+                           170 LOAD_ATTR                6 (aliased)
+                           180 LOAD_FAST                8 (questionnaire)
+                           182 LOAD_ATTR                7 (db_class)
+                           192 LOAD_FAST                5 (entry)
+                           194 KW_NAMES                 3
+                           196 PRECALL                  2
+                           200 CALL                     2
+                           210 STORE_FAST               9 (questionnaire_db_class)
+               
+                86         212 LOAD_GLOBAL             11 (NULL + db)
+                           224 LOAD_ATTR                8 (and_)
+                           234 LOAD_FAST                9 (questionnaire_db_class)
+                           236 LOAD_ATTR                9 (participantID)
+                           246 LOAD_GLOBAL             10 (db)
+                           258 LOAD_ATTR               10 (Participant)
+                           268 LOAD_ATTR                9 (participantID)
+                           278 COMPARE_OP               2 (==)
+               
+                87         284 LOAD_FAST                9 (questionnaire_db_class)
+                           286 LOAD_ATTR               11 (tag)
+                           296 LOAD_FAST                7 (questionnaire_tag)
+                           298 COMPARE_OP               2 (==)
+               
+                86         304 PRECALL                  2
+                           308 CALL                     2
+                           318 STORE_FAST              10 (join_condition)
+               
+                90         320 LOAD_FAST                2 (query_questionnaires)
+                           322 LOAD_METHOD             12 (outerjoin)
+                           344 LOAD_FAST                9 (questionnaire_db_class)
+                           346 LOAD_FAST               10 (join_condition)
+                           348 PRECALL                  2
+                           352 CALL                     2
+               
+                91         362 LOAD_METHOD             13 (add_entity)
+                           384 LOAD_FAST                9 (questionnaire_db_class)
+                           386 PRECALL                  1
+                           390 CALL                     1
+               
+                90         400 STORE_FAST               2 (query_questionnaires)
+               
+                95         402 LOAD_FAST                8 (questionnaire)
+                           404 LOAD_METHOD             14 (fetch_fields)
+                           426 PRECALL                  0
+                           430 CALL                     0
+                           440 GET_ITER
+                       >>  442 FOR_ITER                71 (to 586)
+                           444 STORE_FAST              11 (column)
+               
+                96         446 LOAD_FAST                0 (self)
+                           448 LOAD_ATTR               15 (column_list)
+                           458 LOAD_METHOD             16 (append)
+                           480 LOAD_FAST                5 (entry)
+                           482 LOAD_CONST               4 ('_')
+                           484 BINARY_OP                0 (+)
+                           488 LOAD_FAST               11 (column)
+                           490 LOAD_ATTR               17 (id)
+                           500 BINARY_OP                0 (+)
+                           504 PRECALL                  1
+                           508 CALL                     1
+                           518 POP_TOP
+               
+                97         520 LOAD_FAST                3 (q_columns)
+                           522 LOAD_FAST                5 (entry)
+                           524 BINARY_SUBSCR
+                           534 LOAD_METHOD             16 (append)
+                           556 LOAD_FAST               11 (column)
+                           558 LOAD_ATTR               17 (id)
+                           568 PRECALL                  1
+                           572 CALL                     1
+                           582 POP_TOP
+                           584 JUMP_BACKWARD           72 (to 442)
+               
+               100     >>  586 LOAD_FAST                8 (questionnaire)
+                           588 LOAD_METHOD             18 (get_calculated_fields)
+                           610 PRECALL                  0
+                           614 CALL                     0
+                           624 GET_ITER
+                       >>  626 FOR_ITER                61 (to 750)
+                           628 STORE_FAST              11 (column)
+               
+               101         630 LOAD_FAST                0 (self)
+                           632 LOAD_ATTR               15 (column_list)
+                           642 LOAD_METHOD             16 (append)
+                           664 LOAD_FAST                5 (entry)
+                           666 LOAD_CONST               4 ('_')
+                           668 BINARY_OP                0 (+)
+                           672 LOAD_FAST               11 (column)
+                           674 BINARY_OP                0 (+)
+                           678 PRECALL                  1
+                           682 CALL                     1
+                           692 POP_TOP
+               
+               102         694 LOAD_FAST                4 (q_calculated_columns)
+                           696 LOAD_FAST                5 (entry)
+                           698 BINARY_SUBSCR
+                           708 LOAD_METHOD             16 (append)
+                           730 LOAD_FAST               11 (column)
+                           732 PRECALL                  1
+                           736 CALL                     1
+                           746 POP_TOP
+                           748 JUMP_BACKWARD           62 (to 626)
+               
+               105     >>  750 LOAD_FAST                0 (self)
+                           752 LOAD_ATTR               15 (column_list)
+                           762 LOAD_METHOD             16 (append)
+                           784 LOAD_FAST                5 (entry)
+                           786 LOAD_CONST               5 ('_duration')
+                           788 BINARY_OP                0 (+)
+                           792 PRECALL                  1
+                           796 CALL                     1
+                           806 POP_TOP
+                           808 EXTENDED_ARG             1
+                           810 JUMP_BACKWARD          371 (to 70)
+               
+               107     >>  812 LOAD_FAST                2 (query_questionnaires)
+                           814 LOAD_METHOD             19 (all)
+                           836 PRECALL                  0
+                           840 CALL                     0
+                           850 STORE_FAST              12 (query_result)
+               
+               110         852 LOAD_FAST               12 (query_result)
+                           854 GET_ITER
+                       >>  856 FOR_ITER               196 (to 1250)
+                           858 STORE_FAST              13 (row)
+               
+               111         860 LOAD_FAST                1 (list_of_questionnaires)
+                           862 GET_ITER
+                       >>  864 FOR_ITER               191 (to 1248)
+                           866 STORE_FAST               5 (entry)
+               
+               112         868 LOAD_GLOBAL             41 (NULL + getattr)
+                           880 LOAD_FAST               13 (row)
+                           882 LOAD_FAST                5 (entry)
+                           884 PRECALL                  2
+                           888 CALL                     2
+                           898 STORE_FAST              14 (questionnaire_data)
+               
+               114         900 LOAD_FAST               14 (questionnaire_data)
+                           902 POP_JUMP_FORWARD_IF_FALSE   171 (to 1246)
+               
+               116         904 LOAD_FAST                3 (q_columns)
+                           906 LOAD_FAST                5 (entry)
+                           908 BINARY_SUBSCR
+                           918 GET_ITER
+                       >>  920 FOR_ITER                48 (to 1018)
+                           922 STORE_FAST              15 (col)
+               
+               118         924 LOAD_GLOBAL             41 (NULL + getattr)
+                           936 LOAD_FAST               14 (questionnaire_data)
+                           938 LOAD_FAST               15 (col)
+                           940 PRECALL                  2
+                           944 CALL                     2
+               
+               117         954 LOAD_FAST                0 (self)
+                           956 LOAD_ATTR               21 (export_data)
+                           966 LOAD_FAST               13 (row)
+                           968 LOAD_ATTR               10 (Participant)
+                           978 LOAD_ATTR                9 (participantID)
+                           988 BINARY_SUBSCR
+                           998 LOAD_FAST                5 (entry)
+                          1000 LOAD_CONST               4 ('_')
+                          1002 BINARY_OP                0 (+)
+                          1006 LOAD_FAST               15 (col)
+                          1008 BINARY_OP                0 (+)
+                          1012 STORE_SUBSCR
+                          1016 JUMP_BACKWARD           49 (to 920)
+               
+               121     >> 1018 LOAD_FAST                4 (q_calculated_columns)
+                          1020 LOAD_FAST                5 (entry)
+                          1022 BINARY_SUBSCR
+                          1032 GET_ITER
+                       >> 1034 FOR_ITER                58 (to 1152)
+                          1036 STORE_FAST              15 (col)
+               
+               122        1038 LOAD_FAST               14 (questionnaire_data)
+                          1040 POP_JUMP_FORWARD_IF_FALSE    54 (to 1150)
+               
+               124        1042 PUSH_NULL
+                          1044 LOAD_GLOBAL             41 (NULL + getattr)
+                          1056 LOAD_FAST               14 (questionnaire_data)
+                          1058 LOAD_FAST               15 (col)
+                          1060 PRECALL                  2
+                          1064 CALL                     2
+                          1074 PRECALL                  0
+                          1078 CALL                     0
+               
+               123        1088 LOAD_FAST                0 (self)
+                          1090 LOAD_ATTR               21 (export_data)
+                          1100 LOAD_FAST               13 (row)
+                          1102 LOAD_ATTR               10 (Participant)
+                          1112 LOAD_ATTR                9 (participantID)
+                          1122 BINARY_SUBSCR
+                          1132 LOAD_FAST                5 (entry)
+                          1134 LOAD_CONST               4 ('_')
+                          1136 BINARY_OP                0 (+)
+                          1140 LOAD_FAST               15 (col)
+                          1142 BINARY_OP                0 (+)
+                          1146 STORE_SUBSCR
+                       >> 1150 JUMP_BACKWARD           59 (to 1034)
+               
+               127     >> 1152 LOAD_FAST               14 (questionnaire_data)
+                          1154 LOAD_METHOD             22 (duration)
+                          1176 PRECALL                  0
+                          1180 CALL                     0
+                          1190 LOAD_FAST                0 (self)
+                          1192 LOAD_ATTR               21 (export_data)
+                          1202 LOAD_FAST               13 (row)
+                          1204 LOAD_ATTR               10 (Participant)
+                          1214 LOAD_ATTR                9 (participantID)
+                          1224 BINARY_SUBSCR
+                          1234 LOAD_FAST                5 (entry)
+                          1236 LOAD_CONST               5 ('_duration')
+                          1238 BINARY_OP                0 (+)
+                          1242 STORE_SUBSCR
+                       >> 1246 JUMP_BACKWARD          192 (to 864)
+               
+               111     >> 1248 JUMP_BACKWARD          197 (to 856)
+               
+               110     >> 1250 LOAD_CONST               0 (None)
+                          1252 RETURN_VALUE
+               consts
+                  None
+                  True
+                  ('include_tags',)
+                  ('name',)
+                  '_'
+                  '_duration'
+               names      ('page_list', 'get_questionnaire_list', 'query_participants', 'questionnaire_name_and_tag', 'questionnaires', 'db', 'aliased', 'db_class', 'and_', 'participantID', 'Participant', 'tag', 'outerjoin', 'add_entity', 'fetch_fields', 'column_list', 'append', 'id', 'get_calculated_fields', 'all', 'getattr', 'export_data', 'duration')
+               varnames   ('self', 'list_of_questionnaires', 'query_questionnaires', 'q_columns', 'q_calculated_columns', 'entry', 'questionnaire_name', 'questionnaire_tag', 'questionnaire', 'questionnaire_db_class', 'join_condition', 'column', 'query_result', 'row', 'questionnaire_data', 'col')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'handle_questionnaires'
+               firstlineno 68
+               lnotab
+                  0x02012a020e01040104030a010a010a0124031a033601480114ff10042a
+                  0126ff02052c014a0142032c01400138033e022803080108012002040214
+                  021eff4004140104022eff400460f002ff
+            code
+               argcount  : 1
+               nlocals   : 18
+               stacksize : 12
+               flags     : 3
+               code
+                  0x970067007d017400000000000000000000006a01000000000000000064
+                  011900000000000000000044005d357d027c00a002000000000000000000
+                  00000000000000000000007c02a6010000ab0100000000000000005c0300
+                  007d037d047d057c01a00300000000000000000000000000000000000000
+                  007c027c047c057c0364029c04a6010000ab01000000000000000001008c
+                  367c0144005de47d027c0264031900000000000000000072967c02640319
+                  00000000000000000044005d8c7d067c0264041900000000000000000064
+                  051900000000000000000044005d7b7d07740800000000000000000000a0
+                  05000000000000000000000000000000000000000064067c07a6020000ab
+                  0200000000000000007d087c0644005d417d097c08740800000000000000
+                  000000a00500000000000000000000000000000000000000006407740900
+                  0000000000000000007c09a6010000ab010000000000000000a006000000
+                  000000000000000000000000000000000064086409a6020000ab02000000
+                  0000000000a6020000ab0200000000000000007a0d00007d088c427c006a
+                  070000000000000000a00300000000000000000000000000000000000000
+                  007c08a6010000ab01000000000000000001008c7c8c8d8ca07c02640419
+                  00000000000000000064051900000000000000000044005d357d077c006a
+                  070000000000000000a00300000000000000000000000000000000000000
+                  00740800000000000000000000a005000000000000000000000000000000
+                  000000000064067c07a6020000ab020000000000000000a6010000ab0100
+                  0000000000000001008c368ce57c006a080000000000000000a009000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  007d0a7c0a44005dc07d0b7c0b6a0a00000000000000007d0c7c0144005d
+                  b47d027c02640a190000000000000000007d0d7c0da00b00000000000000
+                  000000000000000000000000007419000000000000000000006a0d000000
+                  0000000000640ba6010000ab0100000000000000007c0b6a0a0000000000
+                  0000006b0200000000a6010000ab0100000000000000007d0d7c0da00900
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  0000007d0e640c7d0f7c0e44005d617d107c026405190000000000000000
+                  0044005d517d077c077d117c0264031900000000000000000072277c0764
+                  097a0000007409000000000000000000007c026403190000000000000000
+                  007c0f19000000000000000000640c19000000000000000000a6010000ab
+                  0100000000000000007a0000007d11741d000000000000000000007c107c
+                  07a6020000ab0200000000000000007c006a0f00000000000000007c0c19
+                  0000000000000000007c113c0000008c527c0f640d7a0d00007d0f8c628c
+                  b58cc164005300
+               129           0 RESUME                   0
+               
+               131           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (custom_exports)
+               
+               133           6 LOAD_GLOBAL              0 (current_app)
+                            18 LOAD_ATTR                1 (config)
+                            28 LOAD_CONST               1 ('EXPORT')
+                            30 BINARY_SUBSCR
+                            40 GET_ITER
+                       >>   42 FOR_ITER                53 (to 150)
+                            44 STORE_FAST               2 (export)
+               
+               134          46 LOAD_FAST                0 (self)
+                            48 LOAD_METHOD              2 (create_export_base_query)
+                            70 LOAD_FAST                2 (export)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 UNPACK_SEQUENCE          3
+                            90 STORE_FAST               3 (levels)
+                            92 STORE_FAST               4 (fields)
+                            94 STORE_FAST               5 (base_query)
+               
+               135          96 LOAD_FAST                1 (custom_exports)
+                            98 LOAD_METHOD              3 (append)
+                           120 LOAD_FAST                2 (export)
+                           122 LOAD_FAST                4 (fields)
+                           124 LOAD_FAST                5 (base_query)
+                           126 LOAD_FAST                3 (levels)
+                           128 LOAD_CONST               2 (('options', 'fields', 'base_query', 'levels'))
+                           130 BUILD_CONST_KEY_MAP      4
+                           132 PRECALL                  1
+                           136 CALL                     1
+                           146 POP_TOP
+                           148 JUMP_BACKWARD           54 (to 42)
+               
+               138     >>  150 LOAD_FAST                1 (custom_exports)
+                           152 GET_ITER
+                       >>  154 FOR_ITER               228 (to 612)
+                           156 STORE_FAST               2 (export)
+               
+               139         158 LOAD_FAST                2 (export)
+                           160 LOAD_CONST               3 ('levels')
+                           162 BINARY_SUBSCR
+                           172 POP_JUMP_FORWARD_IF_FALSE   150 (to 474)
+               
+               140         174 LOAD_FAST                2 (export)
+                           176 LOAD_CONST               3 ('levels')
+                           178 BINARY_SUBSCR
+                           188 GET_ITER
+                       >>  190 FOR_ITER               140 (to 472)
+                           192 STORE_FAST               6 (level)
+               
+               141         194 LOAD_FAST                2 (export)
+                           196 LOAD_CONST               4 ('options')
+                           198 BINARY_SUBSCR
+                           208 LOAD_CONST               5 ('fields')
+                           210 BINARY_SUBSCR
+                           220 GET_ITER
+                       >>  222 FOR_ITER               123 (to 470)
+                           224 STORE_FAST               7 (field)
+               
+               142         226 LOAD_GLOBAL              8 (str)
+                           238 LOAD_METHOD              5 (format)
+                           260 LOAD_CONST               6 ('{}')
+                           262 LOAD_FAST                7 (field)
+                           264 PRECALL                  2
+                           268 CALL                     2
+                           278 STORE_FAST               8 (column_header)
+               
+               143         280 LOAD_FAST                6 (level)
+                           282 GET_ITER
+                       >>  284 FOR_ITER                65 (to 416)
+                           286 STORE_FAST               9 (level_name)
+               
+               144         288 LOAD_FAST                8 (column_header)
+                           290 LOAD_GLOBAL              8 (str)
+                           302 LOAD_METHOD              5 (format)
+                           324 LOAD_CONST               7 ('_{}')
+                           326 LOAD_GLOBAL              9 (NULL + str)
+                           338 LOAD_FAST                9 (level_name)
+                           340 PRECALL                  1
+                           344 CALL                     1
+                           354 LOAD_METHOD              6 (replace)
+                           376 LOAD_CONST               8 (' ')
+                           378 LOAD_CONST               9 ('_')
+                           380 PRECALL                  2
+                           384 CALL                     2
+                           394 PRECALL                  2
+                           398 CALL                     2
+                           408 BINARY_OP               13 (+=)
+                           412 STORE_FAST               8 (column_header)
+                           414 JUMP_BACKWARD           66 (to 284)
+               
+               145     >>  416 LOAD_FAST                0 (self)
+                           418 LOAD_ATTR                7 (column_list)
+                           428 LOAD_METHOD              3 (append)
+                           450 LOAD_FAST                8 (column_header)
+                           452 PRECALL                  1
+                           456 CALL                     1
+                           466 POP_TOP
+                           468 JUMP_BACKWARD          124 (to 222)
+               
+               141     >>  470 JUMP_BACKWARD          141 (to 190)
+               
+               140     >>  472 JUMP_BACKWARD          160 (to 154)
+               
+               147     >>  474 LOAD_FAST                2 (export)
+                           476 LOAD_CONST               4 ('options')
+                           478 BINARY_SUBSCR
+                           488 LOAD_CONST               5 ('fields')
+                           490 BINARY_SUBSCR
+                           500 GET_ITER
+                       >>  502 FOR_ITER                53 (to 610)
+                           504 STORE_FAST               7 (field)
+               
+               148         506 LOAD_FAST                0 (self)
+                           508 LOAD_ATTR                7 (column_list)
+                           518 LOAD_METHOD              3 (append)
+                           540 LOAD_GLOBAL              8 (str)
+                           552 LOAD_METHOD              5 (format)
+                           574 LOAD_CONST               6 ('{}')
+                           576 LOAD_FAST                7 (field)
+                           578 PRECALL                  2
+                           582 CALL                     2
+                           592 PRECALL                  1
+                           596 CALL                     1
+                           606 POP_TOP
+                           608 JUMP_BACKWARD           54 (to 502)
+               
+               147     >>  610 JUMP_BACKWARD          229 (to 154)
+               
+               150     >>  612 LOAD_FAST                0 (self)
+                           614 LOAD_ATTR                8 (query_participants)
+                           624 LOAD_METHOD              9 (all)
+                           646 PRECALL                  0
+                           650 CALL                     0
+                           660 STORE_FAST              10 (query_result)
+               
+               153         662 LOAD_FAST               10 (query_result)
+                           664 GET_ITER
+                       >>  666 FOR_ITER               192 (to 1052)
+                           668 STORE_FAST              11 (row)
+               
+               154         670 LOAD_FAST               11 (row)
+                           672 LOAD_ATTR               10 (participantID)
+                           682 STORE_FAST              12 (participant_id)
+               
+               156         684 LOAD_FAST                1 (custom_exports)
+                           686 GET_ITER
+                       >>  688 FOR_ITER               180 (to 1050)
+                           690 STORE_FAST               2 (export)
+               
+               157         692 LOAD_FAST                2 (export)
+                           694 LOAD_CONST              10 ('base_query')
+                           696 BINARY_SUBSCR
+                           706 STORE_FAST              13 (query)
+               
+               158         708 LOAD_FAST               13 (query)
+                           710 LOAD_METHOD             11 (filter)
+                           732 LOAD_GLOBAL             25 (NULL + db)
+                           744 LOAD_ATTR               13 (literal_column)
+                           754 LOAD_CONST              11 ('participantID')
+                           756 PRECALL                  1
+                           760 CALL                     1
+                           770 LOAD_FAST               11 (row)
+                           772 LOAD_ATTR               10 (participantID)
+                           782 COMPARE_OP               2 (==)
+                           788 PRECALL                  1
+                           792 CALL                     1
+                           802 STORE_FAST              13 (query)
+               
+               159         804 LOAD_FAST               13 (query)
+                           806 LOAD_METHOD              9 (all)
+                           828 PRECALL                  0
+                           832 CALL                     0
+                           842 STORE_FAST              14 (custom_export_data)
+               
+               161         844 LOAD_CONST              12 (0)
+                           846 STORE_FAST              15 (export_row_index)
+               
+               162         848 LOAD_FAST               14 (custom_export_data)
+                           850 GET_ITER
+                       >>  852 FOR_ITER                97 (to 1048)
+                           854 STORE_FAST              16 (custom_export_row)
+               
+               163         856 LOAD_FAST                2 (export)
+                           858 LOAD_CONST               5 ('fields')
+                           860 BINARY_SUBSCR
+                           870 GET_ITER
+                       >>  872 FOR_ITER                81 (to 1036)
+                           874 STORE_FAST               7 (field)
+               
+               164         876 LOAD_FAST                7 (field)
+                           878 STORE_FAST              17 (export_column_name)
+               
+               165         880 LOAD_FAST                2 (export)
+                           882 LOAD_CONST               3 ('levels')
+                           884 BINARY_SUBSCR
+                           894 POP_JUMP_FORWARD_IF_FALSE    39 (to 974)
+               
+               166         896 LOAD_FAST                7 (field)
+                           898 LOAD_CONST               9 ('_')
+                           900 BINARY_OP                0 (+)
+                           904 LOAD_GLOBAL              9 (NULL + str)
+                           916 LOAD_FAST                2 (export)
+                           918 LOAD_CONST               3 ('levels')
+                           920 BINARY_SUBSCR
+                           930 LOAD_FAST               15 (export_row_index)
+                           932 BINARY_SUBSCR
+                           942 LOAD_CONST              12 (0)
+                           944 BINARY_SUBSCR
+                           954 PRECALL                  1
+                           958 CALL                     1
+                           968 BINARY_OP                0 (+)
+                           972 STORE_FAST              17 (export_column_name)
+               
+               168     >>  974 LOAD_GLOBAL             29 (NULL + getattr)
+                           986 LOAD_FAST               16 (custom_export_row)
+                           988 LOAD_FAST                7 (field)
+                           990 PRECALL                  2
+                           994 CALL                     2
+                          1004 LOAD_FAST                0 (self)
+                          1006 LOAD_ATTR               15 (export_data)
+                          1016 LOAD_FAST               12 (participant_id)
+                          1018 BINARY_SUBSCR
+                          1028 LOAD_FAST               17 (export_column_name)
+                          1030 STORE_SUBSCR
+                          1034 JUMP_BACKWARD           82 (to 872)
+               
+               170     >> 1036 LOAD_FAST               15 (export_row_index)
+                          1038 LOAD_CONST              13 (1)
+                          1040 BINARY_OP               13 (+=)
+                          1044 STORE_FAST              15 (export_row_index)
+                          1046 JUMP_BACKWARD           98 (to 852)
+               
+               162     >> 1048 JUMP_BACKWARD          181 (to 688)
+               
+               156     >> 1050 JUMP_BACKWARD          193 (to 666)
+               
+               153     >> 1052 LOAD_CONST               0 (None)
+                          1054 RETURN_VALUE
+               consts
+                  None
+                  'EXPORT'
+                  ('options', 'fields', 'base_query', 'levels')
+                  'levels'
+                  'options'
+                  'fields'
+                  '{}'
+                  '_{}'
+                  ' '
+                  '_'
+                  'base_query'
+                  'participantID'
+                  0
+                  1
+               names      ('current_app', 'config', 'create_export_base_query', 'append', 'str', 'format', 'replace', 'column_list', 'query_participants', 'all', 'participantID', 'filter', 'db', 'literal_column', 'getattr', 'export_data')
+               varnames   ('self', 'custom_exports', 'export', 'levels', 'fields', 'base_query', 'level', 'field', 'column_header', 'level_name', 'query_result', 'row', 'participant_id', 'query', 'custom_export_data', 'export_row_index', 'custom_export_row', 'export_column_name')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'handle_custom_exports'
+               firstlineno 129
+               lnotab
+                  0x02020402280132013603080110011401200136010801800136fc02ff02
+                  07200168ff0203320308010e020801100160012802040108011401040110
+                  014e023e020cf802fa02fd
+            'export_definition'
+            'Query'
+            code
+               argcount  : 2
+               nlocals   : 13
+               stacksize : 7
+               flags     : 3
+               code
+                  0x97007401000000000000000000007402000000000000000000007c0164
+                  0119000000000000000000a6020000ab0200000000000000007d0264027d
+                  0367007d0464027d0564027d0664027d0764027d0864037c01760072267c
+                  0164031900000000000000000064046b0300000000721a74030000000000
+                  00000000006a0200000000000000007c01640319000000000000000000a6
+                  010000ab0100000000000000007d0564057c01760072227c016405190000
+                  0000000000000064046b030000000072167401000000000000000000007c
+                  027c01640519000000000000000000a6020000ab0200000000000000007d
+                  0764067c0176009001727c7c0164061900000000000000000064046b0300
+                  0000009001726f64077c01760072267c0164071900000000000000000064
+                  046b0300000000721a7403000000000000000000006a0200000000000000
+                  007c01640719000000000000000000a6010000ab0100000000000000007d
+                  087402000000000000000000006a030000000000000000a0040000000000
+                  000000000000000000000000000000a6000000ab0000000000000000007d
+                  09740b000000000000000000007c01640619000000000000000000740c00
+                  000000000000000000a6020000ab020000000000000000727767007d067c
+                  0164061900000000000000000044005d6b7d0a7c06a00700000000000000
+                  000000000000000000000000007401000000000000000000007c027c0aa6
+                  020000ab020000000000000000a6010000ab01000000000000000001007c
+                  09a008000000000000000000000000000000000000000074010000000000
+                  00000000007c027c0aa6020000ab020000000000000000a6010000ab0100
+                  000000000000007d097c09a0090000000000000000000000000000000000
+                  0000007401000000000000000000007c027c0aa6020000ab020000000000
+                  000000a6010000ab0100000000000000007d098c6c6e4074010000000000
+                  00000000007c027c01640619000000000000000000a6020000ab02000000
+                  00000000007d067c09a00800000000000000000000000000000000000000
+                  007c06a6010000ab0100000000000000007d097c09a00900000000000000
+                  000000000000000000000000007c06a6010000ab0100000000000000007d
+                  097c0772157c09a00a00000000000000000000000000000000000000007c
+                  07a6010000ab0100000000000000007d097c0581287c09a00b0000000000
+                  0000000000000000000000000000007c05a6010000ab0100000000000000
+                  00a00c0000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d036e147c09a00c000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000007d03740200000000000000
+                  0000006a030000000000000000a004000000000000000000000000000000
+                  00000000007c02a6010000ab0100000000000000007d0b7c06727b740b00
+                  0000000000000000007c06740c00000000000000000000a6020000ab0200
+                  00000000000000722a7c0644005d267d0a7c0ba009000000000000000000
+                  00000000000000000000007401000000000000000000007c026408a60200
+                  00ab0200000000000000007c0aa6020000ab0200000000000000007d0b8c
+                  276e247c0ba0090000000000000000000000000000000000000000740100
+                  0000000000000000007c026408a6020000ab0200000000000000007c06a6
+                  020000ab0200000000000000007d0b7c0881157c0ba00d00000000000000
+                  000000000000000000000000007c08a6010000ab0100000000000000007d
+                  0b6e237c0ba0090000000000000000000000000000000000000000740100
+                  0000000000000000007c026408a6020000ab020000000000000000a60100
+                  00ab0100000000000000007d0b7c0772157c0ba00a000000000000000000
+                  00000000000000000000007c07a6010000ab0100000000000000007d0b7c
+                  0581157c0ba00b00000000000000000000000000000000000000007c05a6
+                  010000ab0100000000000000007d0b7c0164091900000000000000000044
+                  005d8b7d0c741d000000000000000000007c027c0ca6020000ab02000000
+                  0000000000721e741f000000000000000000007401000000000000000000
+                  007c027c0ca6020000ab020000000000000000a6010000ab010000000000
+                  00000072018c307c04a00700000000000000000000000000000000000000
+                  007c0ca6010000ab01000000000000000001007c0ba00800000000000000
+                  000000000000000000000000007403000000000000000000006a10000000
+                  00000000007c016409190000000000000000007c0c190000000000000000
+                  00a6010000ab010000000000000000a01100000000000000000000000000
+                  000000000000007c0ca6010000ab010000000000000000a6010000ab0100
+                  000000000000007d0b8c8c7c037c047c0b66035300
+               172           0 RESUME                   0
+               
+               179           2 LOAD_GLOBAL              1 (NULL + getattr)
+                            14 LOAD_GLOBAL              2 (db)
+                            26 LOAD_FAST                1 (export_definition)
+                            28 LOAD_CONST               1 ('table')
+                            30 BINARY_SUBSCR
+                            40 PRECALL                  2
+                            44 CALL                     2
+                            54 STORE_FAST               2 (table)
+               
+               181          56 LOAD_CONST               2 (None)
+                            58 STORE_FAST               3 (levels)
+               
+               182          60 BUILD_LIST               0
+                            62 STORE_FAST               4 (fields)
+               
+               183          64 LOAD_CONST               2 (None)
+                            66 STORE_FAST               5 (filter)
+               
+               184          68 LOAD_CONST               2 (None)
+                            70 STORE_FAST               6 (groupBy)
+               
+               185          72 LOAD_CONST               2 (None)
+                            74 STORE_FAST               7 (orderBy)
+               
+               186          76 LOAD_CONST               2 (None)
+                            78 STORE_FAST               8 (having)
+               
+               188          80 LOAD_CONST               3 ('filter')
+                            82 LOAD_FAST                1 (export_definition)
+                            84 CONTAINS_OP              0
+                            86 POP_JUMP_FORWARD_IF_FALSE    38 (to 164)
+                            88 LOAD_FAST                1 (export_definition)
+                            90 LOAD_CONST               3 ('filter')
+                            92 BINARY_SUBSCR
+                           102 LOAD_CONST               4 ('')
+                           104 COMPARE_OP               3 (!=)
+                           110 POP_JUMP_FORWARD_IF_FALSE    26 (to 164)
+               
+               189         112 LOAD_GLOBAL              3 (NULL + db)
+                           124 LOAD_ATTR                2 (text)
+                           134 LOAD_FAST                1 (export_definition)
+                           136 LOAD_CONST               3 ('filter')
+                           138 BINARY_SUBSCR
+                           148 PRECALL                  1
+                           152 CALL                     1
+                           162 STORE_FAST               5 (filter)
+               
+               191     >>  164 LOAD_CONST               5 ('order_by')
+                           166 LOAD_FAST                1 (export_definition)
+                           168 CONTAINS_OP              0
+                           170 POP_JUMP_FORWARD_IF_FALSE    34 (to 240)
+                           172 LOAD_FAST                1 (export_definition)
+                           174 LOAD_CONST               5 ('order_by')
+                           176 BINARY_SUBSCR
+                           186 LOAD_CONST               4 ('')
+                           188 COMPARE_OP               3 (!=)
+                           194 POP_JUMP_FORWARD_IF_FALSE    22 (to 240)
+               
+               192         196 LOAD_GLOBAL              1 (NULL + getattr)
+                           208 LOAD_FAST                2 (table)
+                           210 LOAD_FAST                1 (export_definition)
+                           212 LOAD_CONST               5 ('order_by')
+                           214 BINARY_SUBSCR
+                           224 PRECALL                  2
+                           228 CALL                     2
+                           238 STORE_FAST               7 (orderBy)
+               
+               195     >>  240 LOAD_CONST               6 ('group_by')
+                           242 LOAD_FAST                1 (export_definition)
+                           244 CONTAINS_OP              0
+                           246 EXTENDED_ARG             1
+                           248 POP_JUMP_FORWARD_IF_FALSE   380 (to 1010)
+                           250 LOAD_FAST                1 (export_definition)
+                           252 LOAD_CONST               6 ('group_by')
+                           254 BINARY_SUBSCR
+                           264 LOAD_CONST               4 ('')
+                           266 COMPARE_OP               3 (!=)
+                           272 EXTENDED_ARG             1
+                           274 POP_JUMP_FORWARD_IF_FALSE   367 (to 1010)
+               
+               196         276 LOAD_CONST               7 ('having')
+                           278 LOAD_FAST                1 (export_definition)
+                           280 CONTAINS_OP              0
+                           282 POP_JUMP_FORWARD_IF_FALSE    38 (to 360)
+                           284 LOAD_FAST                1 (export_definition)
+                           286 LOAD_CONST               7 ('having')
+                           288 BINARY_SUBSCR
+                           298 LOAD_CONST               4 ('')
+                           300 COMPARE_OP               3 (!=)
+                           306 POP_JUMP_FORWARD_IF_FALSE    26 (to 360)
+               
+               197         308 LOAD_GLOBAL              3 (NULL + db)
+                           320 LOAD_ATTR                2 (text)
+                           330 LOAD_FAST                1 (export_definition)
+                           332 LOAD_CONST               7 ('having')
+                           334 BINARY_SUBSCR
+                           344 PRECALL                  1
+                           348 CALL                     1
+                           358 STORE_FAST               8 (having)
+               
+               199     >>  360 LOAD_GLOBAL              2 (db)
+                           372 LOAD_ATTR                3 (session)
+                           382 LOAD_METHOD              4 (query)
+                           404 PRECALL                  0
+                           408 CALL                     0
+                           418 STORE_FAST               9 (levelsQ)
+               
+               201         420 LOAD_GLOBAL             11 (NULL + isinstance)
+                           432 LOAD_FAST                1 (export_definition)
+                           434 LOAD_CONST               6 ('group_by')
+                           436 BINARY_SUBSCR
+                           446 LOAD_GLOBAL             12 (list)
+                           458 PRECALL                  2
+                           462 CALL                     2
+                           472 POP_JUMP_FORWARD_IF_FALSE   119 (to 712)
+               
+               202         474 BUILD_LIST               0
+                           476 STORE_FAST               6 (groupBy)
+               
+               203         478 LOAD_FAST                1 (export_definition)
+                           480 LOAD_CONST               6 ('group_by')
+                           482 BINARY_SUBSCR
+                           492 GET_ITER
+                       >>  494 FOR_ITER               107 (to 710)
+                           496 STORE_FAST              10 (gb)
+               
+               204         498 LOAD_FAST                6 (groupBy)
+                           500 LOAD_METHOD              7 (append)
+                           522 LOAD_GLOBAL              1 (NULL + getattr)
+                           534 LOAD_FAST                2 (table)
+                           536 LOAD_FAST               10 (gb)
+                           538 PRECALL                  2
+                           542 CALL                     2
+                           552 PRECALL                  1
+                           556 CALL                     1
+                           566 POP_TOP
+               
+               205         568 LOAD_FAST                9 (levelsQ)
+                           570 LOAD_METHOD              8 (add_columns)
+                           592 LOAD_GLOBAL              1 (NULL + getattr)
+                           604 LOAD_FAST                2 (table)
+                           606 LOAD_FAST               10 (gb)
+                           608 PRECALL                  2
+                           612 CALL                     2
+                           622 PRECALL                  1
+                           626 CALL                     1
+                           636 STORE_FAST               9 (levelsQ)
+               
+               206         638 LOAD_FAST                9 (levelsQ)
+                           640 LOAD_METHOD              9 (group_by)
+                           662 LOAD_GLOBAL              1 (NULL + getattr)
+                           674 LOAD_FAST                2 (table)
+                           676 LOAD_FAST               10 (gb)
+                           678 PRECALL                  2
+                           682 CALL                     2
+                           692 PRECALL                  1
+                           696 CALL                     1
+                           706 STORE_FAST               9 (levelsQ)
+                           708 JUMP_BACKWARD          108 (to 494)
+               
+               203     >>  710 JUMP_FORWARD            64 (to 840)
+               
+               208     >>  712 LOAD_GLOBAL              1 (NULL + getattr)
+                           724 LOAD_FAST                2 (table)
+                           726 LOAD_FAST                1 (export_definition)
+                           728 LOAD_CONST               6 ('group_by')
+                           730 BINARY_SUBSCR
+                           740 PRECALL                  2
+                           744 CALL                     2
+                           754 STORE_FAST               6 (groupBy)
+               
+               209         756 LOAD_FAST                9 (levelsQ)
+                           758 LOAD_METHOD              8 (add_columns)
+                           780 LOAD_FAST                6 (groupBy)
+                           782 PRECALL                  1
+                           786 CALL                     1
+                           796 STORE_FAST               9 (levelsQ)
+               
+               210         798 LOAD_FAST                9 (levelsQ)
+                           800 LOAD_METHOD              9 (group_by)
+                           822 LOAD_FAST                6 (groupBy)
+                           824 PRECALL                  1
+                           828 CALL                     1
+                           838 STORE_FAST               9 (levelsQ)
+               
+               212     >>  840 LOAD_FAST                7 (orderBy)
+                           842 POP_JUMP_FORWARD_IF_FALSE    21 (to 886)
+               
+               213         844 LOAD_FAST                9 (levelsQ)
+                           846 LOAD_METHOD             10 (order_by)
+                           868 LOAD_FAST                7 (orderBy)
+                           870 PRECALL                  1
+                           874 CALL                     1
+                           884 STORE_FAST               9 (levelsQ)
+               
+               215     >>  886 LOAD_FAST                5 (filter)
+                           888 POP_JUMP_FORWARD_IF_NONE    40 (to 970)
+               
+               216         890 LOAD_FAST                9 (levelsQ)
+                           892 LOAD_METHOD             11 (filter)
+                           914 LOAD_FAST                5 (filter)
+                           916 PRECALL                  1
+                           920 CALL                     1
+                           930 LOAD_METHOD             12 (all)
+                           952 PRECALL                  0
+                           956 CALL                     0
+                           966 STORE_FAST               3 (levels)
+                           968 JUMP_FORWARD            20 (to 1010)
+               
+               218     >>  970 LOAD_FAST                9 (levelsQ)
+                           972 LOAD_METHOD             12 (all)
+                           994 PRECALL                  0
+                           998 CALL                     0
+                          1008 STORE_FAST               3 (levels)
+               
+               221     >> 1010 LOAD_GLOBAL              2 (db)
+                          1022 LOAD_ATTR                3 (session)
+                          1032 LOAD_METHOD              4 (query)
+                          1054 LOAD_FAST                2 (table)
+                          1056 PRECALL                  1
+                          1060 CALL                     1
+                          1070 STORE_FAST              11 (baseQuery)
+               
+               223        1072 LOAD_FAST                6 (groupBy)
+                          1074 POP_JUMP_FORWARD_IF_FALSE   123 (to 1322)
+               
+               224        1076 LOAD_GLOBAL             11 (NULL + isinstance)
+                          1088 LOAD_FAST                6 (groupBy)
+                          1090 LOAD_GLOBAL             12 (list)
+                          1102 PRECALL                  2
+                          1106 CALL                     2
+                          1116 POP_JUMP_FORWARD_IF_FALSE    42 (to 1202)
+               
+               225        1118 LOAD_FAST                6 (groupBy)
+                          1120 GET_ITER
+                       >> 1122 FOR_ITER                38 (to 1200)
+                          1124 STORE_FAST              10 (gb)
+               
+               226        1126 LOAD_FAST               11 (baseQuery)
+                          1128 LOAD_METHOD              9 (group_by)
+                          1150 LOAD_GLOBAL              1 (NULL + getattr)
+                          1162 LOAD_FAST                2 (table)
+                          1164 LOAD_CONST               8 ('participantID')
+                          1166 PRECALL                  2
+                          1170 CALL                     2
+                          1180 LOAD_FAST               10 (gb)
+                          1182 PRECALL                  2
+                          1186 CALL                     2
+                          1196 STORE_FAST              11 (baseQuery)
+                          1198 JUMP_BACKWARD           39 (to 1122)
+               
+               225     >> 1200 JUMP_FORWARD            36 (to 1274)
+               
+               228     >> 1202 LOAD_FAST               11 (baseQuery)
+                          1204 LOAD_METHOD              9 (group_by)
+                          1226 LOAD_GLOBAL              1 (NULL + getattr)
+                          1238 LOAD_FAST                2 (table)
+                          1240 LOAD_CONST               8 ('participantID')
+                          1242 PRECALL                  2
+                          1246 CALL                     2
+                          1256 LOAD_FAST                6 (groupBy)
+                          1258 PRECALL                  2
+                          1262 CALL                     2
+                          1272 STORE_FAST              11 (baseQuery)
+               
+               230     >> 1274 LOAD_FAST                8 (having)
+                          1276 POP_JUMP_FORWARD_IF_NONE    21 (to 1320)
+               
+               231        1278 LOAD_FAST               11 (baseQuery)
+                          1280 LOAD_METHOD             13 (having)
+                          1302 LOAD_FAST                8 (having)
+                          1304 PRECALL                  1
+                          1308 CALL                     1
+                          1318 STORE_FAST              11 (baseQuery)
+                       >> 1320 JUMP_FORWARD            35 (to 1392)
+               
+               233     >> 1322 LOAD_FAST               11 (baseQuery)
+                          1324 LOAD_METHOD              9 (group_by)
+                          1346 LOAD_GLOBAL              1 (NULL + getattr)
+                          1358 LOAD_FAST                2 (table)
+                          1360 LOAD_CONST               8 ('participantID')
+                          1362 PRECALL                  2
+                          1366 CALL                     2
+                          1376 PRECALL                  1
+                          1380 CALL                     1
+                          1390 STORE_FAST              11 (baseQuery)
+               
+               235     >> 1392 LOAD_FAST                7 (orderBy)
+                          1394 POP_JUMP_FORWARD_IF_FALSE    21 (to 1438)
+               
+               236        1396 LOAD_FAST               11 (baseQuery)
+                          1398 LOAD_METHOD             10 (order_by)
+                          1420 LOAD_FAST                7 (orderBy)
+                          1422 PRECALL                  1
+                          1426 CALL                     1
+                          1436 STORE_FAST              11 (baseQuery)
+               
+               238     >> 1438 LOAD_FAST                5 (filter)
+                          1440 POP_JUMP_FORWARD_IF_NONE    21 (to 1484)
+               
+               239        1442 LOAD_FAST               11 (baseQuery)
+                          1444 LOAD_METHOD             11 (filter)
+                          1466 LOAD_FAST                5 (filter)
+                          1468 PRECALL                  1
+                          1472 CALL                     1
+                          1482 STORE_FAST              11 (baseQuery)
+               
+               242     >> 1484 LOAD_FAST                1 (export_definition)
+                          1486 LOAD_CONST               9 ('fields')
+                          1488 BINARY_SUBSCR
+                          1498 GET_ITER
+                       >> 1500 FOR_ITER               139 (to 1780)
+                          1502 STORE_FAST              12 (field)
+               
+               243        1504 LOAD_GLOBAL             29 (NULL + hasattr)
+                          1516 LOAD_FAST                2 (table)
+                          1518 LOAD_FAST               12 (field)
+                          1520 PRECALL                  2
+                          1524 CALL                     2
+                          1534 POP_JUMP_FORWARD_IF_FALSE    30 (to 1596)
+                          1536 LOAD_GLOBAL             31 (NULL + callable)
+                          1548 LOAD_GLOBAL              1 (NULL + getattr)
+                          1560 LOAD_FAST                2 (table)
+                          1562 LOAD_FAST               12 (field)
+                          1564 PRECALL                  2
+                          1568 CALL                     2
+                          1578 PRECALL                  1
+                          1582 CALL                     1
+                          1592 POP_JUMP_FORWARD_IF_FALSE     1 (to 1596)
+               
+               244        1594 JUMP_BACKWARD           48 (to 1500)
+               
+               245     >> 1596 LOAD_FAST                4 (fields)
+                          1598 LOAD_METHOD              7 (append)
+                          1620 LOAD_FAST               12 (field)
+                          1622 PRECALL                  1
+                          1626 CALL                     1
+                          1636 POP_TOP
+               
+               246        1638 LOAD_FAST               11 (baseQuery)
+                          1640 LOAD_METHOD              8 (add_columns)
+                          1662 LOAD_GLOBAL              3 (NULL + db)
+                          1674 LOAD_ATTR               16 (literal_column)
+                          1684 LOAD_FAST                1 (export_definition)
+                          1686 LOAD_CONST               9 ('fields')
+                          1688 BINARY_SUBSCR
+                          1698 LOAD_FAST               12 (field)
+                          1700 BINARY_SUBSCR
+                          1710 PRECALL                  1
+                          1714 CALL                     1
+                          1724 LOAD_METHOD             17 (label)
+                          1746 LOAD_FAST               12 (field)
+                          1748 PRECALL                  1
+                          1752 CALL                     1
+                          1762 PRECALL                  1
+                          1766 CALL                     1
+                          1776 STORE_FAST              11 (baseQuery)
+                          1778 JUMP_BACKWARD          140 (to 1500)
+               
+               248     >> 1780 LOAD_FAST                3 (levels)
+                          1782 LOAD_FAST                4 (fields)
+                          1784 LOAD_FAST               11 (baseQuery)
+                          1786 BUILD_TUPLE              3
+                          1788 RETURN_VALUE
+               consts
+                  "\n        Builds the base query for exporting values in blueprint-defined tables.\n        To be used for each entry in the config's EXPORT\n        :param export_definition:\n        :return: levels, fields, baseQuery\n        "
+                  'table'
+                  None
+                  'filter'
+                  ''
+                  'order_by'
+                  'group_by'
+                  'having'
+                  'participantID'
+                  'fields'
+               names      ('getattr', 'db', 'text', 'session', 'query', 'isinstance', 'list', 'append', 'add_columns', 'group_by', 'order_by', 'filter', 'all', 'having', 'hasattr', 'callable', 'literal_column', 'label')
+               varnames   ('self', 'export_definition', 'table', 'levels', 'fields', 'filter', 'groupBy', 'orderBy', 'having', 'levelsQ', 'gb', 'baseQuery', 'field')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'create_export_base_query'
+               firstlineno 172
+               lnotab
+                  0x020736020401040104010401040104022001340220012c032401200134
+                  023c023601040114014601460148fd02052c012a012a0204012a02040150
+                  0228033e0204012a0108014aff0203480204012c02460204012a0204012a
+                  0314015a0102012a018e02
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007401000000000000000000006a0100000000000000007c006a0200
+                  00000000000000a6010000ab0100000000000000007c005f030000000000
+                  0000007409000000000000000000007c006a0300000000000000006a0500
+                  000000000000006a060000000000000000a6010000ab0100000000000000
+                  007c005f0700000000000000007c006a07000000000000000044005d247d
+                  017409000000000000000000007c006a0300000000000000007c01190000
+                  00000000000000a6010000ab0100000000000000007c006a080000000000
+                  0000007c013c0000008c2564005300
+               250           0 RESUME                   0
+               
+               251           2 LOAD_GLOBAL              1 (NULL + pd)
+                            14 LOAD_ATTR                1 (read_json)
+                            24 LOAD_FAST                0 (self)
+                            26 LOAD_ATTR                2 (cache_path)
+                            36 PRECALL                  1
+                            40 CALL                     1
+                            50 LOAD_FAST                0 (self)
+                            52 STORE_ATTR               3 (df)
+               
+               252          62 LOAD_GLOBAL              9 (NULL + list)
+                            74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                3 (df)
+                            86 LOAD_ATTR                5 (columns)
+                            96 LOAD_ATTR                6 (values)
+                           106 PRECALL                  1
+                           110 CALL                     1
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               7 (column_list)
+               
+               254         132 LOAD_FAST                0 (self)
+                           134 LOAD_ATTR                7 (column_list)
+                           144 GET_ITER
+                       >>  146 FOR_ITER                36 (to 220)
+                           148 STORE_FAST               1 (column)
+               
+               255         150 LOAD_GLOBAL              9 (NULL + list)
+                           162 LOAD_FAST                0 (self)
+                           164 LOAD_ATTR                3 (df)
+                           174 LOAD_FAST                1 (column)
+                           176 BINARY_SUBSCR
+                           186 PRECALL                  1
+                           190 CALL                     1
+                           200 LOAD_FAST                0 (self)
+                           202 LOAD_ATTR                8 (export_data)
+                           212 LOAD_FAST                1 (column)
+                           214 STORE_SUBSCR
+                           218 JUMP_BACKWARD           37 (to 146)
+               
+               254     >>  220 LOAD_CONST               0 (None)
+                           222 RETURN_VALUE
+               consts
+                  None
+               names      ('pd', 'read_json', 'cache_path', 'df', 'list', 'columns', 'values', 'column_list', 'export_data')
+               varnames   ('self', 'column')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'load_data_frame'
+               firstlineno 250
+               lnotab 0x02013c014602120146ff
+            'pd.DataFrame'
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007c006a00000000000000000081077c006a00000000000000000053
+                  0067007d017c006a01000000000000000044005d227d027c01a002000000
+                  00000000000000000000000000000000007c006a0100000000000000007c
+                  0219000000000000000000a6010000ab01000000000000000001008c2374
+                  07000000000000000000006a0400000000000000007c01a6010000ab0100
+                  000000000000007c005f0000000000000000007c006a0500000000000000
+                  00811f7c006a000000000000000000a00600000000000000000000000000
+                  000000000000007c006a050000000000000000a6010000ab010000000000
+                  00000001007c006a0000000000000000005300
+               257           0 RESUME                   0
+               
+               258           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (df)
+                            14 POP_JUMP_FORWARD_IF_NONE     7 (to 30)
+               
+               259          16 LOAD_FAST                0 (self)
+                            18 LOAD_ATTR                0 (df)
+                            28 RETURN_VALUE
+               
+               261     >>   30 BUILD_LIST               0
+                            32 STORE_FAST               1 (data)
+               
+               262          34 LOAD_FAST                0 (self)
+                            36 LOAD_ATTR                1 (export_data)
+                            46 GET_ITER
+                       >>   48 FOR_ITER                34 (to 118)
+                            50 STORE_FAST               2 (key)
+               
+               263          52 LOAD_FAST                1 (data)
+                            54 LOAD_METHOD              2 (append)
+                            76 LOAD_FAST                0 (self)
+                            78 LOAD_ATTR                1 (export_data)
+                            88 LOAD_FAST                2 (key)
+                            90 BINARY_SUBSCR
+                           100 PRECALL                  1
+                           104 CALL                     1
+                           114 POP_TOP
+                           116 JUMP_BACKWARD           35 (to 48)
+               
+               265     >>  118 LOAD_GLOBAL              7 (NULL + pd)
+                           130 LOAD_ATTR                4 (DataFrame)
+                           140 LOAD_FAST                1 (data)
+                           142 PRECALL                  1
+                           146 CALL                     1
+                           156 LOAD_FAST                0 (self)
+                           158 STORE_ATTR               0 (df)
+               
+               267         168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                5 (cache_path)
+                           180 POP_JUMP_FORWARD_IF_NONE    31 (to 244)
+               
+               268         182 LOAD_FAST                0 (self)
+                           184 LOAD_ATTR                0 (df)
+                           194 LOAD_METHOD              6 (to_json)
+                           216 LOAD_FAST                0 (self)
+                           218 LOAD_ATTR                5 (cache_path)
+                           228 PRECALL                  1
+                           232 CALL                     1
+                           242 POP_TOP
+               
+               270     >>  244 LOAD_FAST                0 (self)
+                           246 LOAD_ATTR                0 (df)
+                           256 RETURN_VALUE
+               consts
+                  None
+               names      ('df', 'export_data', 'append', 'pd', 'DataFrame', 'cache_path', 'to_json')
+               varnames   ('self', 'data', 'key')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'build_data_frame'
+               firstlineno 257
+               lnotab 0x02010e010e0204011201420232020e013e02
+            code
+               argcount  : 1
+               nlocals   : 5
+               stacksize : 7
+               flags     : 3
+               code
+                  0x97006401a00000000000000000000000000000000000000000007c006a
+                  010000000000000000a6010000ab01000000000000000064027a0000007d
+                  017c006a020000000000000000a003000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000044005d437d0264037d037c
+                  006a01000000000000000044005d277d047c047c027600721c7c03740900
+                  0000000000000000007c027c0419000000000000000000a6010000ab0100
+                  0000000000000064017a0000007a0d00007d038c227c0364017a0d00007d
+                  038c287c017c036400640485021900000000000000000064027a0000007a
+                  0d00007d018c447c01640064048502190000000000000000005300
+               272           0 RESUME                   0
+               
+               273           2 LOAD_CONST               1 (',')
+                             4 LOAD_METHOD              0 (join)
+                            26 LOAD_FAST                0 (self)
+                            28 LOAD_ATTR                1 (column_list)
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 LOAD_CONST               2 ('\n')
+                            54 BINARY_OP                0 (+)
+                            58 STORE_FAST               1 (csv_string)
+               
+               275          60 LOAD_FAST                0 (self)
+                            62 LOAD_ATTR                2 (export_data)
+                            72 LOAD_METHOD              3 (values)
+                            94 PRECALL                  0
+                            98 CALL                     0
+                           108 GET_ITER
+                       >>  110 FOR_ITER                67 (to 246)
+                           112 STORE_FAST               2 (row)
+               
+               276         114 LOAD_CONST               3 ('')
+                           116 STORE_FAST               3 (csv_line)
+               
+               277         118 LOAD_FAST                0 (self)
+                           120 LOAD_ATTR                1 (column_list)
+                           130 GET_ITER
+                       >>  132 FOR_ITER                39 (to 212)
+                           134 STORE_FAST               4 (column)
+               
+               278         136 LOAD_FAST                4 (column)
+                           138 LOAD_FAST                2 (row)
+                           140 CONTAINS_OP              0
+                           142 POP_JUMP_FORWARD_IF_FALSE    28 (to 200)
+               
+               279         144 LOAD_FAST                3 (csv_line)
+                           146 LOAD_GLOBAL              9 (NULL + escape_csv)
+                           158 LOAD_FAST                2 (row)
+                           160 LOAD_FAST                4 (column)
+                           162 BINARY_SUBSCR
+                           172 PRECALL                  1
+                           176 CALL                     1
+                           186 LOAD_CONST               1 (',')
+                           188 BINARY_OP                0 (+)
+                           192 BINARY_OP               13 (+=)
+                           196 STORE_FAST               3 (csv_line)
+                           198 JUMP_BACKWARD           34 (to 132)
+               
+               281     >>  200 LOAD_FAST                3 (csv_line)
+                           202 LOAD_CONST               1 (',')
+                           204 BINARY_OP               13 (+=)
+                           208 STORE_FAST               3 (csv_line)
+                           210 JUMP_BACKWARD           40 (to 132)
+               
+               283     >>  212 LOAD_FAST                1 (csv_string)
+                           214 LOAD_FAST                3 (csv_line)
+                           216 LOAD_CONST               0 (None)
+                           218 LOAD_CONST               4 (-1)
+                           220 BUILD_SLICE              2
+                           222 BINARY_SUBSCR
+                           232 LOAD_CONST               2 ('\n')
+                           234 BINARY_OP                0 (+)
+                           238 BINARY_OP               13 (+=)
+                           242 STORE_FAST               1 (csv_string)
+                           244 JUMP_BACKWARD           68 (to 110)
+               
+               285     >>  246 LOAD_FAST                1 (csv_string)
+                           248 LOAD_CONST               0 (None)
+                           250 LOAD_CONST               4 (-1)
+                           252 BUILD_SLICE              2
+                           254 BINARY_SUBSCR
+                           264 RETURN_VALUE
+               consts
+                  None
+                  ','
+                  '\n'
+                  ''
+                  -1
+               names      ('join', 'column_list', 'export_data', 'values', 'escape_csv')
+               varnames   ('self', 'csv_string', 'row', 'csv_line', 'column')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+               name       'build_export_csv'
+               firstlineno 272
+               lnotab 0x02013a02360104011201080138020c022202
+            (None, None)
+            ('return', None)
+            ('return', 'pd.DataFrame')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'handle_participants_table', 'handle_questionnaires', 'handle_custom_exports', 'dict', 'tuple', 'list', 'create_export_base_query', 'load_data_frame', 'build_data_frame', 'build_export_csv')
+         varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
-         name       'build_export_csv'
-         firstlineno 239
-         lnotab 0x020130022c0104010801080138020c022202
-      (True, True)
-      (True,)
-   names      ('BOFS.globals', 'db', 'questionnaires', 'page_list', 'sqlalchemy', 'util', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'flask', 'current_app', 'dict', 'create_export_base_query', 'list', 'str', 'orm', 'Query', 'add_participants_to_export', 'add_questionnaires_to_export', 'add_custom_exports_to_export', 'build_export_csv')
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
+         name       'Results'
+         firstlineno 13
+         lnotab 0x0a011417081f083d082b224e0607080f
+      'Results'
+   names      ('sqlalchemy.orm', 'Query', 'BOFS.globals', 'db', 'questionnaires', 'page_list', 'sqlalchemy', 'util', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'flask', 'current_app', 'pandas', 'pd', 'os', 'datetime', 'MAX_CACHE_SECONDS', 'object', 'Results')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\export_helpers.py'
+   filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\Results.py'
    name       '<module>'
    firstlineno 1
-   lnotab
-      0x00ff02011401080114010c030c51020102fd140102ff020316fd082a02
-      fd140102ff020216fe020302fd084602fd140102ff020216fe020302fd08
-      2f
+   lnotab 0x00ff02010c011401080114010c01080108010c020403
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/util.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/util.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/__pycache__/views.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,534 +1,588 @@
 magic:    0xa70d0d0a
-moddate:  0x06051e66 (Tue Apr 16 04:56:38 2024 UTC)
-files sz: 16351
+moddate:  0xaf5c2066 (Wed Apr 17 23:35:11 2024 UTC)
+files sz: 17920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
-      055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b010064
-      0064036c0c6d0d5a0d6d0e5a0e6d0f5a0f0100640064046c106d115a116d
-      125a126d135a136d145a140100640564066c156d165a166d175a176d185a
-      186d195a196d1a5a1a0100640564076c1b5400640064016c1c5a1c640564
-      076c1d5400640064086c1e6d1e5a1e0100640064096c1f6d205a206d215a
-      2101006400640a6c226d235a23010002006502640b6524640c640d640eac
-      0fa6050000ab0500000000000000005a2565256a26000000000000000064
-      108400a6000000ab0000000000000000005a276525a02800000000000000
-      000000000000000000000000006411a6010000ab01000000000000000064
-      128400a6000000ab0000000000000000005a296525a02800000000000000
-      000000000000000000000000006413641464156702ac16a6020000ab0200
-      0000000000000064178400a6000000ab0000000000000000005a2a641884
-      005a2b641984005a2c6525a0280000000000000000000000000000000000
-      000000641aa6010000ab0100000000000000006517641b8400a6000000ab
-      000000000000000000a6000000ab0000000000000000005a2d6525a02800
-      00000000000000000000000000000000000000641ca6010000ab01000000
-      00000000006517641d8400a6000000ab000000000000000000a6000000ab
-      0000000000000000005a2e6525a028000000000000000000000000000000
-      0000000000641ea6010000ab0100000000000000006517641f8400a60000
-      00ab000000000000000000a6000000ab0000000000000000005a2f6525a0
-      3000000000000000000000000000000000000000006420a6010000ab0100
-      0000000000000064218400a6000000ab0000000000000000005a316525a0
-      2800000000000000000000000000000000000000006422a6010000ab0100
-      00000000000000651764238400a6000000ab000000000000000000a60000
-      00ab0000000000000000005a326525a02800000000000000000000000000
-      000000000000006424a6010000ab0100000000000000006525a028000000
-      000000000000000000000000000000000064256426ac27a6020000ab0200
-      00000000000000651764288400a6000000ab000000000000000000a60000
-      00ab000000000000000000a6000000ab0000000000000000005a336525a0
-      2800000000000000000000000000000000000000006429a6010000ab0100
-      000000000000006517642a8400a6000000ab000000000000000000a60000
-      00ab0000000000000000005a346525a02800000000000000000000000000
-      00000000000000642b641464156702ac16a6020000ab0200000000000000
-      006517642c8400a6000000ab000000000000000000a6000000ab00000000
-      00000000005a356525a02800000000000000000000000000000000000000
-      00642da6010000ab0100000000000000006517642e8400a6000000ab0000
-      00000000000000a6000000ab0000000000000000005a36642f84005a3765
-      25a02800000000000000000000000000000000000000006430a6010000ab
-      010000000000000000651764318400a6000000ab000000000000000000a6
-      000000ab0000000000000000005a386525a0280000000000000000000000
-      0000000000000000006432a6010000ab0100000000000000006517643384
+      0x9700640064016c005a00640064016c015a02640064026c036d045a046d
+      055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b6d0c5a
+      0c6d0d5a0d0100640064036c0e6d0f5a0f6d105a106d115a110100640064
+      046c126d135a136d145a146d155a156d165a160100640564066c176d185a
+      186d195a196d1a5a1a6d1b5a1b6d1c5a1c0100640564076c1d6d1d5a1d01
+      00640064016c1e5a1e640564086c1f6d1f5a1f0100640064096c206d205a
+      2001006400640a6c006d215a216d225a2201006400640b6c236d245a2401
+      0002006504640c6525640d640e640fac10a6050000ab0500000000000000
+      005a2665266a27000000000000000064118400a6000000ab000000000000
+      0000005a286526a029000000000000000000000000000000000000000064
+      12a6010000ab01000000000000000064138400a6000000ab000000000000
+      0000005a2a6526a029000000000000000000000000000000000000000064
+      14641564166702ac17a6020000ab02000000000000000064188400a60000
+      00ab0000000000000000005a2b641984005a2c641a84005a2d6526a02900
+      00000000000000000000000000000000000000641ba6010000ab01000000
+      00000000006519641c8400a6000000ab000000000000000000a6000000ab
+      0000000000000000005a2e6526a029000000000000000000000000000000
+      0000000000641da6010000ab0100000000000000006519641e8400a60000
+      00ab000000000000000000a6000000ab0000000000000000005a2f6526a0
+      290000000000000000000000000000000000000000641fa6010000ab0100
+      00000000000000651964208400a6000000ab000000000000000000a60000
+      00ab0000000000000000005a306526a03100000000000000000000000000
+      000000000000006421a6010000ab01000000000000000064228400a60000
+      00ab0000000000000000005a326526a02900000000000000000000000000
+      000000000000006423a6010000ab010000000000000000651964248400a6
+      000000ab000000000000000000a6000000ab0000000000000000005a3365
+      26a02900000000000000000000000000000000000000006425a6010000ab
+      0100000000000000006526a0290000000000000000000000000000000000
+      00000064266427ac28a6020000ab020000000000000000651964298400a6
+      000000ab000000000000000000a6000000ab000000000000000000a60000
+      00ab0000000000000000005a34642a6535651d65026a3600000000000000
+      0065376538651f6602190000000000000000006603190000000000000000
+      006602642b84045a396526a0290000000000000000000000000000000000
+      000000642ca6010000ab0100000000000000006519642d8400a6000000ab
+      000000000000000000a6000000ab0000000000000000005a3a6526a02900
+      00000000000000000000000000000000000000642ea6010000ab01000000
+      00000000006519642f6538660264308404a6000000ab0000000000000000
+      00a6000000ab0000000000000000005a3b6526a029000000000000000000
+      00000000000000000000006431641564166702ac17a6020000ab02000000
+      0000000000651964328400a6000000ab000000000000000000a6000000ab
+      0000000000000000005a3c6526a029000000000000000000000000000000
+      00000000006433a6010000ab010000000000000000651964348400a60000
+      00ab000000000000000000a6000000ab0000000000000000005a3d643584
+      005a3e6526a02900000000000000000000000000000000000000006436a6
+      010000ab010000000000000000651964378400a6000000ab000000000000
+      000000a6000000ab0000000000000000005a3f6526a02900000000000000
+      000000000000000000000000006438a6010000ab01000000000000000065
+      1964398400a6000000ab000000000000000000a6000000ab000000000000
+      0000005a406526a029000000000000000000000000000000000000000064
+      3aa6010000ab0100000000000000006519643b8400a6000000ab00000000
+      0000000000a6000000ab0000000000000000005a416526a0290000000000
+      000000000000000000000000000000643ca6010000ab0100000000000000
+      006519643d8400a6000000ab000000000000000000a6000000ab00000000
+      00000000005a426526a02900000000000000000000000000000000000000
+      00643e641564166702ac17a6020000ab0200000000000000006519643f84
       00a6000000ab000000000000000000a6000000ab0000000000000000005a
-      396525a02800000000000000000000000000000000000000006434a60100
-      00ab010000000000000000651764358400a6000000ab0000000000000000
-      00a6000000ab0000000000000000005a3a6525a028000000000000000000
-      00000000000000000000006436a6010000ab010000000000000000651764
-      378400a6000000ab000000000000000000a6000000ab0000000000000000
-      005a3b6525a0280000000000000000000000000000000000000000643864
-      1464156702ac16a6020000ab020000000000000000651764398400a60000
-      00ab000000000000000000a6000000ab0000000000000000005a3c640153
-      00
+      4364015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (sqlalchemy)
-                 8 STORE_NAME               0 (sqlalchemy)
+                 6 IMPORT_NAME              0 (os)
+                 8 STORE_NAME               0 (os)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file'))
-                14 IMPORT_NAME              1 (flask)
-                16 IMPORT_FROM              2 (Blueprint)
-                18 STORE_NAME               2 (Blueprint)
-                20 IMPORT_FROM              3 (render_template)
-                22 STORE_NAME               3 (render_template)
-                24 IMPORT_FROM              4 (current_app)
-                26 STORE_NAME               4 (current_app)
-                28 IMPORT_FROM              5 (redirect)
-                30 STORE_NAME               5 (redirect)
-                32 IMPORT_FROM              6 (g)
-                34 STORE_NAME               6 (g)
-                36 IMPORT_FROM              7 (request)
-                38 STORE_NAME               7 (request)
-                40 IMPORT_FROM              8 (session)
-                42 STORE_NAME               8 (session)
-                44 IMPORT_FROM              9 (url_for)
-                46 STORE_NAME               9 (url_for)
-                48 IMPORT_FROM             10 (Response)
-                50 STORE_NAME              10 (Response)
-                52 IMPORT_FROM             11 (send_file)
-                54 STORE_NAME              11 (send_file)
-                56 POP_TOP
-   
-     3          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               3 (('db', 'questionnaires', 'page_list'))
-                62 IMPORT_NAME             12 (BOFS.globals)
-                64 IMPORT_FROM             13 (db)
-                66 STORE_NAME              13 (db)
-                68 IMPORT_FROM             14 (questionnaires)
-                70 STORE_NAME              14 (questionnaires)
-                72 IMPORT_FROM             15 (page_list)
-                74 STORE_NAME              15 (page_list)
-                76 POP_TOP
-   
-     4          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               4 (('fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0'))
-                82 IMPORT_NAME             16 (BOFS.util)
-                84 IMPORT_FROM             17 (fetch_condition_count)
-                86 STORE_NAME              17 (fetch_condition_count)
-                88 IMPORT_FROM             18 (display_time)
-                90 STORE_NAME              18 (display_time)
-                92 IMPORT_FROM             19 (provide_consent)
-                94 STORE_NAME              19 (provide_consent)
-                96 IMPORT_FROM             20 (int_or_0)
-                98 STORE_NAME              20 (int_or_0)
-               100 POP_TOP
-   
-     5         102 LOAD_CONST               5 (1)
-               104 LOAD_CONST               6 (('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
-               106 IMPORT_NAME             21 (util)
-               108 IMPORT_FROM             22 (sqlalchemy_to_json)
-               110 STORE_NAME              22 (sqlalchemy_to_json)
-               112 IMPORT_FROM             23 (verify_admin)
-               114 STORE_NAME              23 (verify_admin)
-               116 IMPORT_FROM             24 (escape_csv)
-               118 STORE_NAME              24 (escape_csv)
-               120 IMPORT_FROM             25 (questionnaire_name_and_tag)
-               122 STORE_NAME              25 (questionnaire_name_and_tag)
-               124 IMPORT_FROM             26 (condition_num_to_label)
-               126 STORE_NAME              26 (condition_num_to_label)
-               128 POP_TOP
-   
-     6         130 LOAD_CONST               5 (1)
-               132 LOAD_CONST               7 (('*',))
-               134 IMPORT_NAME             27 (export_helpers)
-               136 IMPORT_STAR
-   
-     7         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST               1 (None)
-               142 IMPORT_NAME             28 (json)
-               144 STORE_NAME              28 (json)
-   
-     8         146 LOAD_CONST               5 (1)
-               148 LOAD_CONST               7 (('*',))
-               150 IMPORT_NAME             29 (QuestionnaireResults)
-               152 IMPORT_STAR
-   
-     9         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST               8 (('datetime',))
-               158 IMPORT_NAME             30 (datetime)
-               160 IMPORT_FROM             30 (datetime)
-               162 STORE_NAME              30 (datetime)
-               164 POP_TOP
-   
-    10         166 LOAD_CONST               0 (0)
-               168 LOAD_CONST               9 (('path', 'listdir'))
-               170 IMPORT_NAME             31 (os)
-               172 IMPORT_FROM             32 (path)
-               174 STORE_NAME              32 (path)
-               176 IMPORT_FROM             33 (listdir)
-               178 STORE_NAME              33 (listdir)
+                12 LOAD_CONST               1 (None)
+                14 IMPORT_NAME              1 (pandas)
+                16 STORE_NAME               2 (pd)
+   
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file'))
+                22 IMPORT_NAME              3 (flask)
+                24 IMPORT_FROM              4 (Blueprint)
+                26 STORE_NAME               4 (Blueprint)
+                28 IMPORT_FROM              5 (render_template)
+                30 STORE_NAME               5 (render_template)
+                32 IMPORT_FROM              6 (current_app)
+                34 STORE_NAME               6 (current_app)
+                36 IMPORT_FROM              7 (redirect)
+                38 STORE_NAME               7 (redirect)
+                40 IMPORT_FROM              8 (g)
+                42 STORE_NAME               8 (g)
+                44 IMPORT_FROM              9 (request)
+                46 STORE_NAME               9 (request)
+                48 IMPORT_FROM             10 (session)
+                50 STORE_NAME              10 (session)
+                52 IMPORT_FROM             11 (url_for)
+                54 STORE_NAME              11 (url_for)
+                56 IMPORT_FROM             12 (Response)
+                58 STORE_NAME              12 (Response)
+                60 IMPORT_FROM             13 (send_file)
+                62 STORE_NAME              13 (send_file)
+                64 POP_TOP
+   
+     4          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               3 (('db', 'questionnaires', 'page_list'))
+                70 IMPORT_NAME             14 (BOFS.globals)
+                72 IMPORT_FROM             15 (db)
+                74 STORE_NAME              15 (db)
+                76 IMPORT_FROM             16 (questionnaires)
+                78 STORE_NAME              16 (questionnaires)
+                80 IMPORT_FROM             17 (page_list)
+                82 STORE_NAME              17 (page_list)
+                84 POP_TOP
+   
+     5          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               4 (('fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0'))
+                90 IMPORT_NAME             18 (BOFS.util)
+                92 IMPORT_FROM             19 (fetch_condition_count)
+                94 STORE_NAME              19 (fetch_condition_count)
+                96 IMPORT_FROM             20 (display_time)
+                98 STORE_NAME              20 (display_time)
+               100 IMPORT_FROM             21 (provide_consent)
+               102 STORE_NAME              21 (provide_consent)
+               104 IMPORT_FROM             22 (int_or_0)
+               106 STORE_NAME              22 (int_or_0)
+               108 POP_TOP
+   
+     6         110 LOAD_CONST               5 (1)
+               112 LOAD_CONST               6 (('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label'))
+               114 IMPORT_NAME             23 (util)
+               116 IMPORT_FROM             24 (sqlalchemy_to_json)
+               118 STORE_NAME              24 (sqlalchemy_to_json)
+               120 IMPORT_FROM             25 (verify_admin)
+               122 STORE_NAME              25 (verify_admin)
+               124 IMPORT_FROM             26 (escape_csv)
+               126 STORE_NAME              26 (escape_csv)
+               128 IMPORT_FROM             27 (questionnaire_name_and_tag)
+               130 STORE_NAME              27 (questionnaire_name_and_tag)
+               132 IMPORT_FROM             28 (condition_num_to_label)
+               134 STORE_NAME              28 (condition_num_to_label)
+               136 POP_TOP
+   
+     7         138 LOAD_CONST               5 (1)
+               140 LOAD_CONST               7 (('Results',))
+               142 IMPORT_NAME             29 (Results)
+               144 IMPORT_FROM             29 (Results)
+               146 STORE_NAME              29 (Results)
+               148 POP_TOP
+   
+     8         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST               1 (None)
+               154 IMPORT_NAME             30 (json)
+               156 STORE_NAME              30 (json)
+   
+     9         158 LOAD_CONST               5 (1)
+               160 LOAD_CONST               8 (('SummaryStats',))
+               162 IMPORT_NAME             31 (SummaryStats)
+               164 IMPORT_FROM             31 (SummaryStats)
+               166 STORE_NAME              31 (SummaryStats)
+               168 POP_TOP
+   
+    10         170 LOAD_CONST               0 (0)
+               172 LOAD_CONST               9 (('datetime',))
+               174 IMPORT_NAME             32 (datetime)
+               176 IMPORT_FROM             32 (datetime)
+               178 STORE_NAME              32 (datetime)
                180 POP_TOP
    
     11         182 LOAD_CONST               0 (0)
-               184 LOAD_CONST              10 (('copyfile',))
-               186 IMPORT_NAME             34 (shutil)
-               188 IMPORT_FROM             35 (copyfile)
-               190 STORE_NAME              35 (copyfile)
-               192 POP_TOP
+               184 LOAD_CONST              10 (('path', 'listdir'))
+               186 IMPORT_NAME              0 (os)
+               188 IMPORT_FROM             33 (path)
+               190 STORE_NAME              33 (path)
+               192 IMPORT_FROM             34 (listdir)
+               194 STORE_NAME              34 (listdir)
+               196 POP_TOP
    
-    13         194 PUSH_NULL
-               196 LOAD_NAME                2 (Blueprint)
-               198 LOAD_CONST              11 ('admin')
-               200 LOAD_NAME               36 (__name__)
-               202 LOAD_CONST              12 ('templates')
-               204 LOAD_CONST              13 ('static')
-               206 LOAD_CONST              14 ('/admin')
-               208 KW_NAMES                15
-               210 PRECALL                  5
-               214 CALL                     5
-               224 STORE_NAME              37 (admin)
+    12         198 LOAD_CONST               0 (0)
+               200 LOAD_CONST              11 (('copyfile',))
+               202 IMPORT_NAME             35 (shutil)
+               204 IMPORT_FROM             36 (copyfile)
+               206 STORE_NAME              36 (copyfile)
+               208 POP_TOP
    
-    16         226 LOAD_NAME               37 (admin)
-               228 LOAD_ATTR               38 (context_processor)
+    14         210 PUSH_NULL
+               212 LOAD_NAME                4 (Blueprint)
+               214 LOAD_CONST              12 ('admin')
+               216 LOAD_NAME               37 (__name__)
+               218 LOAD_CONST              13 ('templates')
+               220 LOAD_CONST              14 ('static')
+               222 LOAD_CONST              15 ('/admin')
+               224 KW_NAMES                16
+               226 PRECALL                  5
+               230 CALL                     5
+               240 STORE_NAME              38 (admin)
    
-    17         238 LOAD_CONST              16 (<code object inject_template_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 16>)
-               240 MAKE_FUNCTION            0
+    17         242 LOAD_NAME               38 (admin)
+               244 LOAD_ATTR               39 (context_processor)
    
-    16         242 PRECALL                  0
-               246 CALL                     0
+    18         254 LOAD_CONST              17 (<code object inject_template_vars, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 17>)
+               256 MAKE_FUNCTION            0
    
-    17         256 STORE_NAME              39 (inject_template_vars)
+    17         258 PRECALL                  0
+               262 CALL                     0
    
-    59         258 LOAD_NAME               37 (admin)
-               260 LOAD_METHOD             40 (route)
-               282 LOAD_CONST              17 ('/')
-               284 PRECALL                  1
-               288 CALL                     1
+    18         272 STORE_NAME              40 (inject_template_vars)
    
-    60         298 LOAD_CONST              18 (<code object admin_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 59>)
-               300 MAKE_FUNCTION            0
+    60         274 LOAD_NAME               38 (admin)
+               276 LOAD_METHOD             41 (route)
+               298 LOAD_CONST              18 ('/')
+               300 PRECALL                  1
+               304 CALL                     1
    
-    59         302 PRECALL                  0
-               306 CALL                     0
+    61         314 LOAD_CONST              19 (<code object admin_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 60>)
+               316 MAKE_FUNCTION            0
    
-    60         316 STORE_NAME              41 (admin_index)
+    60         318 PRECALL                  0
+               322 CALL                     0
    
-    64         318 LOAD_NAME               37 (admin)
-               320 LOAD_METHOD             40 (route)
-               342 LOAD_CONST              19 ('/login')
-               344 LOAD_CONST              20 ('GET')
-               346 LOAD_CONST              21 ('POST')
-               348 BUILD_LIST               2
-               350 KW_NAMES                22
-               352 PRECALL                  2
-               356 CALL                     2
+    61         332 STORE_NAME              42 (admin_index)
    
-    65         366 LOAD_CONST              23 (<code object admin_login, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 64>)
-               368 MAKE_FUNCTION            0
+    65         334 LOAD_NAME               38 (admin)
+               336 LOAD_METHOD             41 (route)
+               358 LOAD_CONST              20 ('/login')
+               360 LOAD_CONST              21 ('GET')
+               362 LOAD_CONST              22 ('POST')
+               364 BUILD_LIST               2
+               366 KW_NAMES                23
+               368 PRECALL                  2
+               372 CALL                     2
    
-    64         370 PRECALL                  0
-               374 CALL                     0
+    66         382 LOAD_CONST              24 (<code object admin_login, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 65>)
+               384 MAKE_FUNCTION            0
    
-    65         384 STORE_NAME              42 (admin_login)
+    65         386 PRECALL                  0
+               390 CALL                     0
    
-    94         386 LOAD_CONST              24 (<code object fetch_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 94>)
-               388 MAKE_FUNCTION            0
-               390 STORE_NAME              43 (fetch_progress)
+    66         400 STORE_NAME              43 (admin_login)
    
-   116         392 LOAD_CONST              25 (<code object fetch_progress_summary, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 116>)
-               394 MAKE_FUNCTION            0
-               396 STORE_NAME              44 (fetch_progress_summary)
+    95         402 LOAD_CONST              25 (<code object fetch_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 95>)
+               404 MAKE_FUNCTION            0
+               406 STORE_NAME              44 (fetch_progress)
    
-   141         398 LOAD_NAME               37 (admin)
-               400 LOAD_METHOD             40 (route)
-               422 LOAD_CONST              26 ('/progress')
-               424 PRECALL                  1
-               428 CALL                     1
+   117         408 LOAD_CONST              26 (<code object fetch_progress_summary, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 117>)
+               410 MAKE_FUNCTION            0
+               412 STORE_NAME              45 (fetch_progress_summary)
    
-   142         438 LOAD_NAME               23 (verify_admin)
+   142         414 LOAD_NAME               38 (admin)
+               416 LOAD_METHOD             41 (route)
+               438 LOAD_CONST              27 ('/progress')
+               440 PRECALL                  1
+               444 CALL                     1
    
-   143         440 LOAD_CONST              27 (<code object route_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 141>)
-               442 MAKE_FUNCTION            0
+   143         454 LOAD_NAME               25 (verify_admin)
    
-   142         444 PRECALL                  0
-               448 CALL                     0
+   144         456 LOAD_CONST              28 (<code object route_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 142>)
+               458 MAKE_FUNCTION            0
    
-   141         458 PRECALL                  0
-               462 CALL                     0
+   143         460 PRECALL                  0
+               464 CALL                     0
    
-   143         472 STORE_NAME              45 (route_progress)
+   142         474 PRECALL                  0
+               478 CALL                     0
    
-   152         474 LOAD_NAME               37 (admin)
-               476 LOAD_METHOD             40 (route)
-               498 LOAD_CONST              28 ('/progress_ajax')
-               500 PRECALL                  1
-               504 CALL                     1
+   144         488 STORE_NAME              46 (route_progress)
    
-   153         514 LOAD_NAME               23 (verify_admin)
+   153         490 LOAD_NAME               38 (admin)
+               492 LOAD_METHOD             41 (route)
+               514 LOAD_CONST              29 ('/progress_ajax')
+               516 PRECALL                  1
+               520 CALL                     1
    
-   154         516 LOAD_CONST              29 (<code object route_progress_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 152>)
-               518 MAKE_FUNCTION            0
+   154         530 LOAD_NAME               25 (verify_admin)
    
-   153         520 PRECALL                  0
-               524 CALL                     0
+   155         532 LOAD_CONST              30 (<code object route_progress_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 153>)
+               534 MAKE_FUNCTION            0
    
-   152         534 PRECALL                  0
-               538 CALL                     0
+   154         536 PRECALL                  0
+               540 CALL                     0
    
-   154         548 STORE_NAME              46 (route_progress_ajax)
+   153         550 PRECALL                  0
+               554 CALL                     0
    
-   159         550 LOAD_NAME               37 (admin)
-               552 LOAD_METHOD             40 (route)
-               574 LOAD_CONST              30 ('/progress_summary_ajax')
-               576 PRECALL                  1
-               580 CALL                     1
+   155         564 STORE_NAME              47 (route_progress_ajax)
    
-   160         590 LOAD_NAME               23 (verify_admin)
+   160         566 LOAD_NAME               38 (admin)
+               568 LOAD_METHOD             41 (route)
+               590 LOAD_CONST              31 ('/progress_summary_ajax')
+               592 PRECALL                  1
+               596 CALL                     1
    
-   161         592 LOAD_CONST              31 (<code object route_progress_summary_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 159>)
-               594 MAKE_FUNCTION            0
+   161         606 LOAD_NAME               25 (verify_admin)
    
-   160         596 PRECALL                  0
-               600 CALL                     0
+   162         608 LOAD_CONST              32 (<code object route_progress_summary_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 160>)
+               610 MAKE_FUNCTION            0
    
-   159         610 PRECALL                  0
-               614 CALL                     0
+   161         612 PRECALL                  0
+               616 CALL                     0
    
-   161         624 STORE_NAME              47 (route_progress_summary_ajax)
+   160         626 PRECALL                  0
+               630 CALL                     0
    
-   166         626 LOAD_NAME               37 (admin)
-               628 LOAD_METHOD             48 (post)
-               650 LOAD_CONST              32 ('/update_exclude_from_count')
-               652 PRECALL                  1
-               656 CALL                     1
+   162         640 STORE_NAME              48 (route_progress_summary_ajax)
    
-   167         666 LOAD_CONST              33 (<code object route_update_exclude_from_count, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 166>)
-               668 MAKE_FUNCTION            0
+   167         642 LOAD_NAME               38 (admin)
+               644 LOAD_METHOD             49 (post)
+               666 LOAD_CONST              33 ('/update_exclude_from_count')
+               668 PRECALL                  1
+               672 CALL                     1
    
-   166         670 PRECALL                  0
-               674 CALL                     0
+   168         682 LOAD_CONST              34 (<code object route_update_exclude_from_count, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 167>)
+               684 MAKE_FUNCTION            0
    
-   167         684 STORE_NAME              49 (route_update_exclude_from_count)
+   167         686 PRECALL                  0
+               690 CALL                     0
    
-   177         686 LOAD_NAME               37 (admin)
-               688 LOAD_METHOD             40 (route)
-               710 LOAD_CONST              34 ('/export_item_timing')
-               712 PRECALL                  1
-               716 CALL                     1
+   168         700 STORE_NAME              50 (route_update_exclude_from_count)
    
-   178         726 LOAD_NAME               23 (verify_admin)
+   178         702 LOAD_NAME               38 (admin)
+               704 LOAD_METHOD             41 (route)
+               726 LOAD_CONST              35 ('/export_item_timing')
+               728 PRECALL                  1
+               732 CALL                     1
    
-   179         728 LOAD_CONST              35 (<code object route_export_item_timing, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 177>)
-               730 MAKE_FUNCTION            0
+   179         742 LOAD_NAME               25 (verify_admin)
    
-   178         732 PRECALL                  0
-               736 CALL                     0
+   180         744 LOAD_CONST              36 (<code object route_export_item_timing, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 178>)
+               746 MAKE_FUNCTION            0
    
-   177         746 PRECALL                  0
-               750 CALL                     0
+   179         748 PRECALL                  0
+               752 CALL                     0
    
-   179         760 STORE_NAME              50 (route_export_item_timing)
+   178         762 PRECALL                  0
+               766 CALL                     0
    
-   218         762 LOAD_NAME               37 (admin)
-               764 LOAD_METHOD             40 (route)
-               786 LOAD_CONST              36 ('/export')
-               788 PRECALL                  1
-               792 CALL                     1
+   180         776 STORE_NAME              51 (route_export_item_timing)
    
-   219         802 LOAD_NAME               37 (admin)
-               804 LOAD_METHOD             40 (route)
-               826 LOAD_CONST              37 ('/export/download')
-               828 LOAD_CONST              38 ('route_export_download')
-               830 KW_NAMES                39
-               832 PRECALL                  2
-               836 CALL                     2
+   219         778 LOAD_NAME               38 (admin)
+               780 LOAD_METHOD             41 (route)
+               802 LOAD_CONST              37 ('/export')
+               804 PRECALL                  1
+               808 CALL                     1
    
-   220         846 LOAD_NAME               23 (verify_admin)
+   220         818 LOAD_NAME               38 (admin)
+               820 LOAD_METHOD             41 (route)
+               842 LOAD_CONST              38 ('/export/download')
+               844 LOAD_CONST              39 ('route_export_download')
+               846 KW_NAMES                40
+               848 PRECALL                  2
+               852 CALL                     2
    
-   221         848 LOAD_CONST              40 (<code object route_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 218>)
-               850 MAKE_FUNCTION            0
+   221         862 LOAD_NAME               25 (verify_admin)
    
-   220         852 PRECALL                  0
-               856 CALL                     0
+   222         864 LOAD_CONST              41 (<code object route_export, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 219>)
+               866 MAKE_FUNCTION            0
    
-   219         866 PRECALL                  0
-               870 CALL                     0
+   221         868 PRECALL                  0
+               872 CALL                     0
    
-   218         880 PRECALL                  0
-               884 CALL                     0
+   220         882 PRECALL                  0
+               886 CALL                     0
    
-   221         894 STORE_NAME              51 (route_export)
+   219         896 PRECALL                  0
+               900 CALL                     0
    
-   255         896 LOAD_NAME               37 (admin)
-               898 LOAD_METHOD             40 (route)
-               920 LOAD_CONST              41 ('/results')
-               922 PRECALL                  1
-               926 CALL                     1
+   222         910 STORE_NAME              52 (route_export)
    
-   256         936 LOAD_NAME               23 (verify_admin)
+   261         912 LOAD_CONST              42 ('return')
+               914 LOAD_NAME               53 (tuple)
+               916 LOAD_NAME               29 (Results)
+               918 LOAD_NAME                2 (pd)
+               920 LOAD_ATTR               54 (DataFrame)
+               930 LOAD_NAME               55 (dict)
+               932 LOAD_NAME               56 (str)
+               934 LOAD_NAME               31 (SummaryStats)
+               936 BUILD_TUPLE              2
+               938 BINARY_SUBSCR
+               948 BUILD_TUPLE              3
+               950 BINARY_SUBSCR
+               960 BUILD_TUPLE              2
+               962 LOAD_CONST              43 (<code object calculate_results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 261>)
+               964 MAKE_FUNCTION            4 (annotations)
+               966 STORE_NAME              57 (calculate_results)
    
-   257         938 LOAD_CONST              42 (<code object route_results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 255>)
-               940 MAKE_FUNCTION            0
+   278         968 LOAD_NAME               38 (admin)
+               970 LOAD_METHOD             41 (route)
+               992 LOAD_CONST              44 ('/results')
+               994 PRECALL                  1
+               998 CALL                     1
    
-   256         942 PRECALL                  0
-               946 CALL                     0
+   279        1008 LOAD_NAME               25 (verify_admin)
    
-   255         956 PRECALL                  0
-               960 CALL                     0
+   280        1010 LOAD_CONST              45 (<code object route_results, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 278>)
+              1012 MAKE_FUNCTION            0
    
-   257         970 STORE_NAME              52 (route_results)
+   279        1014 PRECALL                  0
+              1018 CALL                     0
    
-   273         972 LOAD_NAME               37 (admin)
-               974 LOAD_METHOD             40 (route)
-               996 LOAD_CONST              43 ('/preview_questionnaire/<questionnaireName>')
-               998 LOAD_CONST              20 ('GET')
-              1000 LOAD_CONST              21 ('POST')
-              1002 BUILD_LIST               2
-              1004 KW_NAMES                22
-              1006 PRECALL                  2
-              1010 CALL                     2
+   278        1028 PRECALL                  0
+              1032 CALL                     0
    
-   274        1020 LOAD_NAME               23 (verify_admin)
+   280        1042 STORE_NAME              58 (route_results)
    
-   275        1022 LOAD_CONST              44 (<code object route_preview_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 273>)
-              1024 MAKE_FUNCTION            0
+   285        1044 LOAD_NAME               38 (admin)
+              1046 LOAD_METHOD             41 (route)
+              1068 LOAD_CONST              46 ('/results_boxplot/<path:field_name>')
+              1070 PRECALL                  1
+              1074 CALL                     1
    
-   274        1026 PRECALL                  0
-              1030 CALL                     0
+   286        1084 LOAD_NAME               25 (verify_admin)
    
-   273        1040 PRECALL                  0
-              1044 CALL                     0
+   287        1086 LOAD_CONST              47 ('field_name')
+              1088 LOAD_NAME               56 (str)
+              1090 BUILD_TUPLE              2
+              1092 LOAD_CONST              48 (<code object route_results_boxplot, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 285>)
+              1094 MAKE_FUNCTION            4 (annotations)
    
-   275        1054 STORE_NAME              53 (route_preview_questionnaire)
+   286        1096 PRECALL                  0
+              1100 CALL                     0
    
-   301        1056 LOAD_NAME               37 (admin)
-              1058 LOAD_METHOD             40 (route)
-              1080 LOAD_CONST              45 ('/questionnaire_html/<questionnaireName>')
-              1082 PRECALL                  1
-              1086 CALL                     1
+   285        1110 PRECALL                  0
+              1114 CALL                     0
    
-   302        1096 LOAD_NAME               23 (verify_admin)
+   287        1124 STORE_NAME              59 (route_results_boxplot)
    
-   303        1098 LOAD_CONST              46 (<code object route_questionnaire_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 301>)
-              1100 MAKE_FUNCTION            0
+   309        1126 LOAD_NAME               38 (admin)
+              1128 LOAD_METHOD             41 (route)
+              1150 LOAD_CONST              49 ('/preview_questionnaire/<questionnaireName>')
+              1152 LOAD_CONST              21 ('GET')
+              1154 LOAD_CONST              22 ('POST')
+              1156 BUILD_LIST               2
+              1158 KW_NAMES                23
+              1160 PRECALL                  2
+              1164 CALL                     2
    
-   302        1102 PRECALL                  0
-              1106 CALL                     0
+   310        1174 LOAD_NAME               25 (verify_admin)
    
-   301        1116 PRECALL                  0
-              1120 CALL                     0
+   311        1176 LOAD_CONST              50 (<code object route_preview_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 309>)
+              1178 MAKE_FUNCTION            0
    
-   303        1130 STORE_NAME              54 (route_questionnaire_html)
+   310        1180 PRECALL                  0
+              1184 CALL                     0
    
-   352        1132 LOAD_CONST              47 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 352>)
-              1134 MAKE_FUNCTION            0
-              1136 STORE_NAME              55 (table_data)
+   309        1194 PRECALL                  0
+              1198 CALL                     0
    
-   369        1138 LOAD_NAME               37 (admin)
-              1140 LOAD_METHOD             40 (route)
-              1162 LOAD_CONST              48 ('/table_view/<tableName>')
-              1164 PRECALL                  1
-              1168 CALL                     1
+   311        1208 STORE_NAME              60 (route_preview_questionnaire)
    
-   370        1178 LOAD_NAME               23 (verify_admin)
+   337        1210 LOAD_NAME               38 (admin)
+              1212 LOAD_METHOD             41 (route)
+              1234 LOAD_CONST              51 ('/questionnaire_html/<questionnaireName>')
+              1236 PRECALL                  1
+              1240 CALL                     1
    
-   371        1180 LOAD_CONST              49 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 369>)
-              1182 MAKE_FUNCTION            0
+   338        1250 LOAD_NAME               25 (verify_admin)
    
-   370        1184 PRECALL                  0
-              1188 CALL                     0
+   339        1252 LOAD_CONST              52 (<code object route_questionnaire_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 337>)
+              1254 MAKE_FUNCTION            0
    
-   369        1198 PRECALL                  0
-              1202 CALL                     0
+   338        1256 PRECALL                  0
+              1260 CALL                     0
    
-   371        1212 STORE_NAME              56 (route_table_view)
+   337        1270 PRECALL                  0
+              1274 CALL                     0
    
-   376        1214 LOAD_NAME               37 (admin)
-              1216 LOAD_METHOD             40 (route)
-              1238 LOAD_CONST              50 ('/table_ajax/<tableName>')
-              1240 PRECALL                  1
-              1244 CALL                     1
+   339        1284 STORE_NAME              61 (route_questionnaire_html)
    
-   377        1254 LOAD_NAME               23 (verify_admin)
+   388        1286 LOAD_CONST              53 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 388>)
+              1288 MAKE_FUNCTION            0
+              1290 STORE_NAME              62 (table_data)
    
-   378        1256 LOAD_CONST              51 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 376>)
-              1258 MAKE_FUNCTION            0
+   405        1292 LOAD_NAME               38 (admin)
+              1294 LOAD_METHOD             41 (route)
+              1316 LOAD_CONST              54 ('/table_view/<tableName>')
+              1318 PRECALL                  1
+              1322 CALL                     1
    
-   377        1260 PRECALL                  0
-              1264 CALL                     0
+   406        1332 LOAD_NAME               25 (verify_admin)
    
-   376        1274 PRECALL                  0
-              1278 CALL                     0
+   407        1334 LOAD_CONST              55 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 405>)
+              1336 MAKE_FUNCTION            0
    
-   378        1288 STORE_NAME              57 (route_table_ajax)
+   406        1338 PRECALL                  0
+              1342 CALL                     0
    
-   383        1290 LOAD_NAME               37 (admin)
-              1292 LOAD_METHOD             40 (route)
-              1314 LOAD_CONST              52 ('/table_csv/<tableName>')
-              1316 PRECALL                  1
-              1320 CALL                     1
+   405        1352 PRECALL                  0
+              1356 CALL                     0
    
-   384        1330 LOAD_NAME               23 (verify_admin)
+   407        1366 STORE_NAME              63 (route_table_view)
    
-   385        1332 LOAD_CONST              53 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 383>)
-              1334 MAKE_FUNCTION            0
+   412        1368 LOAD_NAME               38 (admin)
+              1370 LOAD_METHOD             41 (route)
+              1392 LOAD_CONST              56 ('/table_ajax/<tableName>')
+              1394 PRECALL                  1
+              1398 CALL                     1
    
-   384        1336 PRECALL                  0
-              1340 CALL                     0
+   413        1408 LOAD_NAME               25 (verify_admin)
    
-   383        1350 PRECALL                  0
-              1354 CALL                     0
+   414        1410 LOAD_CONST              57 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 412>)
+              1412 MAKE_FUNCTION            0
    
-   385        1364 STORE_NAME              58 (route_table_csv)
+   413        1414 PRECALL                  0
+              1418 CALL                     0
    
-   403        1366 LOAD_NAME               37 (admin)
-              1368 LOAD_METHOD             40 (route)
-              1390 LOAD_CONST              54 ('/database_download')
-              1392 PRECALL                  1
-              1396 CALL                     1
+   412        1428 PRECALL                  0
+              1432 CALL                     0
    
-   404        1406 LOAD_NAME               23 (verify_admin)
+   414        1442 STORE_NAME              64 (route_table_ajax)
    
-   405        1408 LOAD_CONST              55 (<code object route_database_download, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 403>)
-              1410 MAKE_FUNCTION            0
+   419        1444 LOAD_NAME               38 (admin)
+              1446 LOAD_METHOD             41 (route)
+              1468 LOAD_CONST              58 ('/table_csv/<tableName>')
+              1470 PRECALL                  1
+              1474 CALL                     1
    
-   404        1412 PRECALL                  0
-              1416 CALL                     0
+   420        1484 LOAD_NAME               25 (verify_admin)
    
-   403        1426 PRECALL                  0
-              1430 CALL                     0
+   421        1486 LOAD_CONST              59 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 419>)
+              1488 MAKE_FUNCTION            0
    
-   405        1440 STORE_NAME              59 (route_database_download)
+   420        1490 PRECALL                  0
+              1494 CALL                     0
    
-   414        1442 LOAD_NAME               37 (admin)
-              1444 LOAD_METHOD             40 (route)
-              1466 LOAD_CONST              56 ('/database_delete')
-              1468 LOAD_CONST              20 ('GET')
-              1470 LOAD_CONST              21 ('POST')
-              1472 BUILD_LIST               2
-              1474 KW_NAMES                22
-              1476 PRECALL                  2
-              1480 CALL                     2
+   419        1504 PRECALL                  0
+              1508 CALL                     0
    
-   415        1490 LOAD_NAME               23 (verify_admin)
+   421        1518 STORE_NAME              65 (route_table_csv)
    
-   416        1492 LOAD_CONST              57 (<code object route_database_delete, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 414>)
-              1494 MAKE_FUNCTION            0
+   439        1520 LOAD_NAME               38 (admin)
+              1522 LOAD_METHOD             41 (route)
+              1544 LOAD_CONST              60 ('/database_download')
+              1546 PRECALL                  1
+              1550 CALL                     1
    
-   415        1496 PRECALL                  0
-              1500 CALL                     0
+   440        1560 LOAD_NAME               25 (verify_admin)
    
-   414        1510 PRECALL                  0
-              1514 CALL                     0
+   441        1562 LOAD_CONST              61 (<code object route_database_download, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 439>)
+              1564 MAKE_FUNCTION            0
    
-   416        1524 STORE_NAME              60 (route_database_delete)
-              1526 LOAD_CONST               1 (None)
-              1528 RETURN_VALUE
+   440        1566 PRECALL                  0
+              1570 CALL                     0
+   
+   439        1580 PRECALL                  0
+              1584 CALL                     0
+   
+   441        1594 STORE_NAME              66 (route_database_download)
+   
+   450        1596 LOAD_NAME               38 (admin)
+              1598 LOAD_METHOD             41 (route)
+              1620 LOAD_CONST              62 ('/database_delete')
+              1622 LOAD_CONST              21 ('GET')
+              1624 LOAD_CONST              22 ('POST')
+              1626 BUILD_LIST               2
+              1628 KW_NAMES                23
+              1630 PRECALL                  2
+              1634 CALL                     2
+   
+   451        1644 LOAD_NAME               25 (verify_admin)
+   
+   452        1646 LOAD_CONST              63 (<code object route_database_delete, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 450>)
+              1648 MAKE_FUNCTION            0
+   
+   451        1650 PRECALL                  0
+              1654 CALL                     0
+   
+   450        1664 PRECALL                  0
+              1668 CALL                     0
+   
+   452        1678 STORE_NAME              67 (route_database_delete)
+              1680 LOAD_CONST               1 (None)
+              1682 RETURN_VALUE
    consts
       0
       None
       ('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file')
       ('db', 'questionnaires', 'page_list')
       ('fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0')
       1
       ('sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label')
-      ('*',)
+      ('Results',)
+      ('SummaryStats',)
       ('datetime',)
       ('path', 'listdir')
       ('copyfile',)
       'admin'
       'templates'
       'static'
       '/admin'
@@ -562,156 +616,156 @@
             00000000007c03a6010000ab0100000000000000007d0374000000000000
             00000000006a010000000000000000640719000000000000000000a00f00
             000000000000000000000000000000000000006408a6010000ab01000000
             00000000007d077421000000000000000000007c007c017c057c067c0374
             00000000000000000000006a010000000000000000640919000000000000
             0000007c07742200000000000000000000ac0aa6080000ab080000000000
             0000005300
-          16           0 RESUME                   0
+          17           0 RESUME                   0
          
-          24           2 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
+          25           2 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
                        4 LOAD_GLOBAL              0 (current_app)
                       16 LOAD_ATTR                1 (config)
                       26 CONTAINS_OP              0
                       28 POP_JUMP_FORWARD_IF_FALSE    19 (to 68)
          
-          25          30 LOAD_GLOBAL              0 (current_app)
+          26          30 LOAD_GLOBAL              0 (current_app)
                       42 LOAD_ATTR                1 (config)
                       52 LOAD_CONST               1 ('ADDITIONAL_ADMIN_PAGES')
                       54 BINARY_SUBSCR
                       64 STORE_FAST               0 (additionalAdminPages)
                       66 JUMP_FORWARD             2 (to 72)
          
-          27     >>   68 LOAD_CONST               2 (None)
+          28     >>   68 LOAD_CONST               2 (None)
                       70 STORE_FAST               0 (additionalAdminPages)
          
-          29     >>   72 BUILD_LIST               0
+          30     >>   72 BUILD_LIST               0
                       74 STORE_FAST               1 (tableNames)
          
-          30          76 LOAD_GLOBAL              4 (db)
+          31          76 LOAD_GLOBAL              4 (db)
                       88 LOAD_ATTR                3 (metadata)
                       98 LOAD_ATTR                4 (tables)
                      108 GET_ITER
                  >>  110 FOR_ITER                23 (to 158)
                      112 STORE_FAST               2 (t)
          
-          31         114 LOAD_FAST                1 (tableNames)
+          32         114 LOAD_FAST                1 (tableNames)
                      116 LOAD_METHOD              5 (append)
                      138 LOAD_FAST                2 (t)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
                      156 JUMP_BACKWARD           24 (to 110)
          
-          33     >>  158 BUILD_LIST               0
+          34     >>  158 BUILD_LIST               0
                      160 STORE_FAST               3 (questionnairesSystem)
          
-          35         162 LOAD_GLOBAL             13 (NULL + path)
+          36         162 LOAD_GLOBAL             13 (NULL + path)
                      174 LOAD_ATTR                7 (exists)
                      184 LOAD_GLOBAL              0 (current_app)
                      196 LOAD_ATTR                8 (root_path)
                      206 LOAD_CONST               3 ('/questionnaires')
                      208 BINARY_OP                0 (+)
                      212 PRECALL                  1
                      216 CALL                     1
                      226 POP_JUMP_FORWARD_IF_FALSE    93 (to 414)
          
-          36         228 LOAD_GLOBAL             19 (NULL + listdir)
+          37         228 LOAD_GLOBAL             19 (NULL + listdir)
                      240 LOAD_GLOBAL              0 (current_app)
                      252 LOAD_ATTR                8 (root_path)
                      262 LOAD_CONST               3 ('/questionnaires')
                      264 BINARY_OP                0 (+)
                      268 PRECALL                  1
                      272 CALL                     1
                      282 GET_ITER
                  >>  284 FOR_ITER                64 (to 414)
                      286 STORE_FAST               4 (q)
          
-          37         288 LOAD_FAST                4 (q)
+          38         288 LOAD_FAST                4 (q)
                      290 LOAD_METHOD             10 (endswith)
                      312 LOAD_CONST               4 ('.json')
                      314 PRECALL                  1
                      318 CALL                     1
                      328 POP_JUMP_FORWARD_IF_FALSE    41 (to 412)
          
-          38         330 LOAD_FAST                3 (questionnairesSystem)
+          39         330 LOAD_FAST                3 (questionnairesSystem)
                      332 LOAD_METHOD              5 (append)
                      354 LOAD_FAST                4 (q)
                      356 LOAD_METHOD             11 (replace)
                      378 LOAD_CONST               4 ('.json')
                      380 LOAD_CONST               5 ('')
                      382 PRECALL                  2
                      386 CALL                     2
                      396 PRECALL                  1
                      400 CALL                     1
                      410 POP_TOP
                  >>  412 JUMP_BACKWARD           65 (to 284)
          
-          40     >>  414 LOAD_GLOBAL             25 (NULL + sorted)
+          41     >>  414 LOAD_GLOBAL             25 (NULL + sorted)
                      426 LOAD_FAST                1 (tableNames)
                      428 PRECALL                  1
                      432 CALL                     1
                      442 STORE_FAST               1 (tableNames)
          
-          41         444 LOAD_GLOBAL              0 (current_app)
+          42         444 LOAD_GLOBAL              0 (current_app)
                      456 LOAD_ATTR               13 (page_list)
                      466 LOAD_METHOD             14 (get_questionnaire_list)
                      488 LOAD_CONST               6 (True)
                      490 PRECALL                  1
                      494 CALL                     1
                      504 STORE_FAST               5 (questionnairesLive)
          
-          42         506 LOAD_GLOBAL             25 (NULL + sorted)
+          43         506 LOAD_GLOBAL             25 (NULL + sorted)
                      518 LOAD_GLOBAL              0 (current_app)
                      530 LOAD_ATTR               13 (page_list)
                      540 LOAD_METHOD             14 (get_questionnaire_list)
                      562 PRECALL                  0
                      566 CALL                     0
                      576 PRECALL                  1
                      580 CALL                     1
                      590 STORE_FAST               6 (questionnairesLiveUntagged)
          
-          43         592 LOAD_GLOBAL             25 (NULL + sorted)
+          44         592 LOAD_GLOBAL             25 (NULL + sorted)
                      604 LOAD_FAST                3 (questionnairesSystem)
                      606 PRECALL                  1
                      610 CALL                     1
                      620 STORE_FAST               3 (questionnairesSystem)
          
-          44         622 LOAD_GLOBAL              0 (current_app)
+          45         622 LOAD_GLOBAL              0 (current_app)
                      634 LOAD_ATTR                1 (config)
                      644 LOAD_CONST               7 ('SQLALCHEMY_DATABASE_URI')
                      646 BINARY_SUBSCR
                      656 LOAD_METHOD             15 (startswith)
                      678 LOAD_CONST               8 ('sqlite:///')
                      680 PRECALL                  1
                      684 CALL                     1
                      694 STORE_FAST               7 (isSqliteDb)
          
-          47         696 LOAD_GLOBAL             33 (NULL + dict)
+          48         696 LOAD_GLOBAL             33 (NULL + dict)
          
-          48         708 LOAD_FAST                0 (additionalAdminPages)
+          49         708 LOAD_FAST                0 (additionalAdminPages)
          
-          49         710 LOAD_FAST                1 (tableNames)
+          50         710 LOAD_FAST                1 (tableNames)
          
-          50         712 LOAD_FAST                5 (questionnairesLive)
+          51         712 LOAD_FAST                5 (questionnairesLive)
          
-          51         714 LOAD_FAST                6 (questionnairesLiveUntagged)
+          52         714 LOAD_FAST                6 (questionnairesLiveUntagged)
          
-          52         716 LOAD_FAST                3 (questionnairesSystem)
+          53         716 LOAD_FAST                3 (questionnairesSystem)
          
-          53         718 LOAD_GLOBAL              0 (current_app)
+          54         718 LOAD_GLOBAL              0 (current_app)
                      730 LOAD_ATTR                1 (config)
                      740 LOAD_CONST               9 ('LOG_GRID_CLICKS')
                      742 BINARY_SUBSCR
          
-          54         752 LOAD_FAST                7 (isSqliteDb)
+          55         752 LOAD_FAST                7 (isSqliteDb)
          
-          55         754 LOAD_GLOBAL             34 (condition_num_to_label)
+          56         754 LOAD_GLOBAL             34 (condition_num_to_label)
          
-          47         766 KW_NAMES                10
+          48         766 KW_NAMES                10
                      768 PRECALL                  8
                      772 CALL                     8
                      782 RETURN_VALUE
          consts
             '\n    Inject additional variables into the context of templates within this blueprint\n    See http://flask.pocoo.org/docs/1.0/templating/#context-processors\n    :return:\n    '
             'ADDITIONAL_ADMIN_PAGES'
             None
@@ -725,30 +779,30 @@
             ('additionalAdminPages', 'tableNames', 'questionnairesLive', 'questionnairesLiveUntagged', 'questionnairesSystem', 'logGridClicks', 'isSqliteDb', 'condition_num_to_label')
          names      ('current_app', 'config', 'db', 'metadata', 'tables', 'append', 'path', 'exists', 'root_path', 'listdir', 'endswith', 'replace', 'sorted', 'page_list', 'get_questionnaire_list', 'startswith', 'dict', 'condition_num_to_label')
          varnames   ('additionalAdminPages', 'tableNames', 't', 'questionnairesSystem', 'q', 'questionnairesLive', 'questionnairesLiveUntagged', 'isSqliteDb')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'inject_template_vars'
-         firstlineno 16
+         firstlineno 17
          lnotab
             0x02081c0126020402040126012c02040242013c012a0154021e013e0156
             011e014a030c0102010201020102010201220102010cf8
       '/'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007403000000000000000000006401a6
             010000ab010000000000000000a6010000ab0100000000000000005300
-          59           0 RESUME                   0
+          60           0 RESUME                   0
          
-          61           2 LOAD_GLOBAL              1 (NULL + redirect)
+          62           2 LOAD_GLOBAL              1 (NULL + redirect)
                       14 LOAD_GLOBAL              3 (NULL + url_for)
                       26 LOAD_CONST               1 ('admin.admin_login')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 PRECALL                  1
                       46 CALL                     1
                       56 RETURN_VALUE
@@ -757,15 +811,15 @@
             'admin.admin_login'
          names      ('redirect', 'url_for')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'admin_index'
-         firstlineno 59
+         firstlineno 60
          lnotab 0x0202
       '/login'
       'GET'
       'POST'
       ('methods',)
       code
          argcount  : 0
@@ -792,135 +846,135 @@
             0000000000640ca6010000ab010000000000000000812f740f0000000000
             0000000000640d7410000000000000000000006a0f0000000000000000a0
             050000000000000000000000000000000000000000640ca6010000ab0100
             000000000000007a000000a6010000ab0100000000000000007d016e0723
             00010059006e03780359007701740d000000000000000000007c01a60100
             00ab0100000000000000005300741b000000000000000000006409a60100
             00ab0100000000000000005300
-          64           0 RESUME                   0
+          65           0 RESUME                   0
          
-          66           2 LOAD_CONST               1 ('participantID')
+          67           2 LOAD_CONST               1 ('participantID')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              1
                       18 POP_JUMP_FORWARD_IF_FALSE    52 (to 124)
          
-          67          20 LOAD_GLOBAL              3 (NULL + provide_consent)
+          68          20 LOAD_GLOBAL              3 (NULL + provide_consent)
                       32 LOAD_CONST               2 (True)
                       34 PRECALL                  1
                       38 CALL                     1
                       48 STORE_FAST               0 (p)
          
-          68          50 LOAD_CONST               2 (True)
+          69          50 LOAD_CONST               2 (True)
                       52 LOAD_FAST                0 (p)
                       54 STORE_ATTR               2 (excludeFromCount)
          
-          69          64 LOAD_GLOBAL              6 (db)
+          70          64 LOAD_GLOBAL              6 (db)
                       76 LOAD_ATTR                0 (session)
                       86 LOAD_METHOD              4 (commit)
                      108 PRECALL                  0
                      112 CALL                     0
                      122 POP_TOP
          
-          71     >>  124 LOAD_GLOBAL              1 (NULL + session)
+          72     >>  124 LOAD_GLOBAL              1 (NULL + session)
                      136 LOAD_ATTR                5 (get)
                      146 LOAD_CONST               3 ('loggedIn')
                      148 LOAD_CONST               4 (False)
                      150 PRECALL                  2
                      154 CALL                     2
                      164 POP_JUMP_FORWARD_IF_FALSE    28 (to 222)
          
-          72         166 LOAD_GLOBAL             13 (NULL + redirect)
+          73         166 LOAD_GLOBAL             13 (NULL + redirect)
                      178 LOAD_GLOBAL             15 (NULL + url_for)
                      190 LOAD_CONST               5 ('admin.route_progress')
                      192 PRECALL                  1
                      196 CALL                     1
                      206 PRECALL                  1
                      210 CALL                     1
                      220 RETURN_VALUE
          
-          74     >>  222 LOAD_GLOBAL             16 (request)
+          75     >>  222 LOAD_GLOBAL             16 (request)
                      234 LOAD_ATTR                9 (method)
                      244 LOAD_CONST               6 ('POST')
                      246 COMPARE_OP               2 (==)
                      252 POP_JUMP_FORWARD_IF_FALSE   194 (to 642)
          
-          75         254 LOAD_GLOBAL             16 (request)
+          76         254 LOAD_GLOBAL             16 (request)
                      266 LOAD_ATTR               10 (form)
                      276 LOAD_CONST               7 ('password')
                      278 BINARY_SUBSCR
                      288 LOAD_GLOBAL             22 (current_app)
                      300 LOAD_ATTR               12 (config)
                      310 LOAD_CONST               8 ('ADMIN_PASSWORD')
                      312 BINARY_SUBSCR
                      322 COMPARE_OP               3 (!=)
                      328 POP_JUMP_FORWARD_IF_FALSE    17 (to 364)
          
-          76         330 LOAD_GLOBAL             27 (NULL + render_template)
+          77         330 LOAD_GLOBAL             27 (NULL + render_template)
                      342 LOAD_CONST               9 ('login_admin.html')
                      344 LOAD_CONST              10 ('The password you entered is incorrect.')
                      346 KW_NAMES                11
                      348 PRECALL                  2
                      352 CALL                     2
                      362 RETURN_VALUE
          
-          78     >>  364 LOAD_CONST               2 (True)
+          79     >>  364 LOAD_CONST               2 (True)
                      366 LOAD_GLOBAL              0 (session)
                      378 LOAD_CONST               3 ('loggedIn')
                      380 STORE_SUBSCR
          
-          79         384 LOAD_CONST               2 (True)
+          80         384 LOAD_CONST               2 (True)
                      386 LOAD_GLOBAL              0 (session)
                      398 STORE_ATTR              14 (modified)
          
-          81         408 LOAD_GLOBAL             15 (NULL + url_for)
+          82         408 LOAD_GLOBAL             15 (NULL + url_for)
                      420 LOAD_CONST               5 ('admin.route_progress')
                      422 PRECALL                  1
                      426 CALL                     1
                      436 STORE_FAST               1 (redirect_to)
          
-          83         438 NOP
+          84         438 NOP
          
-          84         440 LOAD_GLOBAL             16 (request)
+          85         440 LOAD_GLOBAL             16 (request)
                      452 LOAD_ATTR               15 (args)
                      462 LOAD_METHOD              5 (get)
                      484 LOAD_CONST              12 ('r')
                      486 PRECALL                  1
                      490 CALL                     1
                      500 POP_JUMP_FORWARD_IF_NONE    47 (to 596)
          
-          85         502 LOAD_GLOBAL             15 (NULL + url_for)
+          86         502 LOAD_GLOBAL             15 (NULL + url_for)
                      514 LOAD_CONST              13 ('admin.')
                      516 LOAD_GLOBAL             16 (request)
                      528 LOAD_ATTR               15 (args)
                      538 LOAD_METHOD              5 (get)
                      560 LOAD_CONST              12 ('r')
                      562 PRECALL                  1
                      566 CALL                     1
                      576 BINARY_OP                0 (+)
                      580 PRECALL                  1
                      584 CALL                     1
                      594 STORE_FAST               1 (redirect_to)
                  >>  596 JUMP_FORWARD             7 (to 612)
                  >>  598 PUSH_EXC_INFO
          
-          86         600 POP_TOP
+          87         600 POP_TOP
          
-          87         602 POP_EXCEPT
+          88         602 POP_EXCEPT
                      604 JUMP_FORWARD             3 (to 612)
                  >>  606 COPY                     3
                      608 POP_EXCEPT
                      610 RERAISE                  1
          
-          89     >>  612 LOAD_GLOBAL             13 (NULL + redirect)
+          90     >>  612 LOAD_GLOBAL             13 (NULL + redirect)
                      624 LOAD_FAST                1 (redirect_to)
                      626 PRECALL                  1
                      630 CALL                     1
                      640 RETURN_VALUE
          
-          91     >>  642 LOAD_GLOBAL             27 (NULL + render_template)
+          92     >>  642 LOAD_GLOBAL             27 (NULL + render_template)
                      654 LOAD_CONST               9 ('login_admin.html')
                      656 PRECALL                  1
                      660 CALL                     1
                      670 RETURN_VALUE
          ExceptionTable:
            440 to 594 -> 598 [0]
            598 to 600 -> 606 [1] lasti
@@ -941,15 +995,15 @@
             'admin.'
          names      ('session', 'provide_consent', 'excludeFromCount', 'db', 'commit', 'get', 'redirect', 'url_for', 'request', 'method', 'form', 'current_app', 'config', 'render_template', 'modified', 'args')
          varnames   ('p', 'redirect_to')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'admin_login'
-         firstlineno 64
+         firstlineno 65
          lnotab
             0x020212011e010e013c022a01380220014c012202140118021e0202013e
             01620102010a021e02
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 10
@@ -972,24 +1026,24 @@
             000000000000007c036a0e00000000000000007406000000000000000000
             006a0600000000000000006a0e00000000000000006b02000000007c036a
             0f00000000000000007c026402190000000000000000006b0200000000a6
             020000ab020000000000000000a6020000ab020000000000000000a01000
             000000000000000000000000000000000000007c03a6010000ab01000000
             00000000007d018c8c7c01a0110000000000000000000000000000000000
             000000a6000000ab0000000000000000007d017c007c0166025300
-          94           0 RESUME                   0
+          95           0 RESUME                   0
          
-          95           2 LOAD_GLOBAL              0 (current_app)
+          96           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (page_list)
                       24 LOAD_METHOD              2 (flat_page_list)
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_FAST               0 (pages)
          
-          96          62 LOAD_GLOBAL              6 (db)
+          97          62 LOAD_GLOBAL              6 (db)
                       74 LOAD_ATTR                4 (session)
                       84 LOAD_METHOD              5 (query)
                      106 LOAD_GLOBAL              6 (db)
                      118 LOAD_ATTR                6 (Participant)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 LOAD_METHOD              7 (filter)
@@ -998,96 +1052,96 @@
                      186 LOAD_ATTR                8 (isCrawler)
                      196 LOAD_CONST               1 (False)
                      198 COMPARE_OP               2 (==)
                      204 PRECALL                  1
                      208 CALL                     1
                      218 STORE_FAST               1 (progress)
          
-          98         220 LOAD_FAST                0 (pages)
+          99         220 LOAD_FAST                0 (pages)
                      222 GET_ITER
                  >>  224 FOR_ITER                34 (to 294)
                      226 STORE_FAST               2 (page)
          
-          99         228 LOAD_FAST                2 (page)
+         100         228 LOAD_FAST                2 (page)
                      230 LOAD_CONST               2 ('path')
                      232 BINARY_SUBSCR
                      242 LOAD_CONST               3 (('end', 'consent'))
                      244 CONTAINS_OP              0
                      246 POP_JUMP_FORWARD_IF_FALSE    22 (to 292)
          
-         100         248 LOAD_FAST                0 (pages)
+         101         248 LOAD_FAST                0 (pages)
                      250 LOAD_METHOD              9 (remove)
                      272 LOAD_FAST                2 (page)
                      274 PRECALL                  1
                      278 CALL                     1
                      288 POP_TOP
          
-         101         290 JUMP_BACKWARD           34 (to 224)
+         102         290 JUMP_BACKWARD           34 (to 224)
          
-          99     >>  292 JUMP_BACKWARD           35 (to 224)
+         100     >>  292 JUMP_BACKWARD           35 (to 224)
          
-         103     >>  294 LOAD_FAST                0 (pages)
+         104     >>  294 LOAD_FAST                0 (pages)
                      296 GET_ITER
                  >>  298 FOR_ITER               139 (to 578)
                      300 STORE_FAST               2 (page)
          
-         104         302 LOAD_GLOBAL              7 (NULL + db)
+         105         302 LOAD_GLOBAL              7 (NULL + db)
                      314 LOAD_ATTR               10 (aliased)
                      324 LOAD_GLOBAL              6 (db)
                      336 LOAD_ATTR               11 (Progress)
                      346 LOAD_FAST                2 (page)
                      348 LOAD_CONST               2 ('path')
                      350 BINARY_SUBSCR
                      360 KW_NAMES                 4
                      362 PRECALL                  2
                      366 CALL                     2
                      376 STORE_FAST               3 (pp)
          
-         105         378 LOAD_FAST                1 (progress)
+         106         378 LOAD_FAST                1 (progress)
                      380 LOAD_METHOD             12 (outerjoin)
                      402 LOAD_FAST                3 (pp)
                      404 LOAD_GLOBAL              7 (NULL + db)
                      416 LOAD_ATTR               13 (and_)
          
-         106         426 LOAD_FAST                3 (pp)
+         107         426 LOAD_FAST                3 (pp)
                      428 LOAD_ATTR               14 (participantID)
                      438 LOAD_GLOBAL              6 (db)
                      450 LOAD_ATTR                6 (Participant)
                      460 LOAD_ATTR               14 (participantID)
                      470 COMPARE_OP               2 (==)
          
-         107         476 LOAD_FAST                3 (pp)
+         108         476 LOAD_FAST                3 (pp)
                      478 LOAD_ATTR               15 (path)
                      488 LOAD_FAST                2 (page)
                      490 LOAD_CONST               2 ('path')
                      492 BINARY_SUBSCR
                      502 COMPARE_OP               2 (==)
          
-         105         508 PRECALL                  2
+         106         508 PRECALL                  2
                      512 CALL                     2
                      522 PRECALL                  2
                      526 CALL                     2
          
-         108         536 LOAD_METHOD             16 (add_entity)
+         109         536 LOAD_METHOD             16 (add_entity)
          
-         109         558 LOAD_FAST                3 (pp)
+         110         558 LOAD_FAST                3 (pp)
          
-         108         560 PRECALL                  1
+         109         560 PRECALL                  1
                      564 CALL                     1
          
-         105         574 STORE_FAST               1 (progress)
+         106         574 STORE_FAST               1 (progress)
                      576 JUMP_BACKWARD          140 (to 298)
          
-         112     >>  578 LOAD_FAST                1 (progress)
+         113     >>  578 LOAD_FAST                1 (progress)
                      580 LOAD_METHOD             17 (all)
                      602 PRECALL                  0
                      606 CALL                     0
                      616 STORE_FAST               1 (progress)
          
-         113         618 LOAD_FAST                0 (pages)
+         114         618 LOAD_FAST                0 (pages)
                      620 LOAD_FAST                1 (progress)
                      622 BUILD_TUPLE              2
                      624 RETURN_VALUE
          consts
             None
             False
             'path'
@@ -1095,15 +1149,15 @@
             ('name',)
          names      ('current_app', 'page_list', 'flat_page_list', 'db', 'session', 'query', 'Participant', 'filter', 'isCrawler', 'remove', 'aliased', 'Progress', 'outerjoin', 'and_', 'participantID', 'path', 'add_entity', 'all')
          varnames   ('pages', 'progress', 'page', 'pp')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'fetch_progress'
-         firstlineno 94
+         firstlineno 95
          lnotab
             0x02013c019e02080114012a0102fe020408014c013001320120fe1c0316
             0102ff0efd04072801
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 12
@@ -1188,38 +1242,38 @@
             00000000000000a011000000000000000000000000000000000000000074
             01000000000000000000006a120000000000000000740000000000000000
             0000006a0300000000000000006a1300000000000000000f007400000000
             000000000000006a0300000000000000006a13000000000000000064006b
             0200000000a6020000ab020000000000000000a6010000ab010000000000
             000000a0180000000000000000000000000000000000000000a6000000ab
             0000000000000000007d017c007c0166025300
-         116           0 RESUME                   0
+         117           0 RESUME                   0
          
-         117           2 LOAD_GLOBAL              0 (db)
+         118           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
          
-         118          46 LOAD_GLOBAL              0 (db)
+         119          46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (Participant)
                       68 LOAD_ATTR                4 (condition)
          
-         119          78 LOAD_GLOBAL              0 (db)
+         120          78 LOAD_GLOBAL              0 (db)
                       90 LOAD_ATTR                5 (func)
                      100 LOAD_METHOD              6 (count)
                      122 LOAD_GLOBAL              0 (db)
                      134 LOAD_ATTR                3 (Participant)
                      144 LOAD_ATTR                7 (participantID)
                      154 PRECALL                  1
                      158 CALL                     1
                      168 LOAD_METHOD              8 (label)
                      190 LOAD_CONST               1 ('count')
                      192 PRECALL                  1
                      196 CALL                     1
          
-         120         206 LOAD_GLOBAL              0 (db)
+         121         206 LOAD_GLOBAL              0 (db)
                      218 LOAD_ATTR                5 (func)
                      228 LOAD_METHOD              9 (sum)
                      250 LOAD_GLOBAL              1 (NULL + db)
                      262 LOAD_ATTR               10 (cast)
                      272 LOAD_GLOBAL              0 (db)
                      284 LOAD_ATTR                3 (Participant)
                      294 LOAD_ATTR               11 (is_abandoned)
@@ -1230,15 +1284,15 @@
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_METHOD              8 (label)
                      376 LOAD_CONST               2 ('countAbandoned')
                      378 PRECALL                  1
                      382 CALL                     1
          
-         121         392 LOAD_GLOBAL              0 (db)
+         122         392 LOAD_GLOBAL              0 (db)
                      404 LOAD_ATTR                5 (func)
                      414 LOAD_METHOD              9 (sum)
                      436 LOAD_GLOBAL              1 (NULL + db)
                      448 LOAD_ATTR               10 (cast)
                      458 LOAD_GLOBAL              0 (db)
                      470 LOAD_ATTR                3 (Participant)
                      480 LOAD_ATTR               13 (is_in_progress)
@@ -1249,15 +1303,15 @@
                      526 PRECALL                  1
                      530 CALL                     1
                      540 LOAD_METHOD              8 (label)
                      562 LOAD_CONST               3 ('countInProgress')
                      564 PRECALL                  1
                      568 CALL                     1
          
-         122         578 LOAD_GLOBAL              0 (db)
+         123         578 LOAD_GLOBAL              0 (db)
                      590 LOAD_ATTR                5 (func)
                      600 LOAD_METHOD              9 (sum)
                      622 LOAD_GLOBAL              1 (NULL + db)
                      634 LOAD_ATTR               10 (cast)
                      644 LOAD_GLOBAL              0 (db)
                      656 LOAD_ATTR                3 (Participant)
                      666 LOAD_ATTR               14 (finished)
@@ -1268,31 +1322,31 @@
                      712 PRECALL                  1
                      716 CALL                     1
                      726 LOAD_METHOD              8 (label)
                      748 LOAD_CONST               4 ('countFinished')
                      750 PRECALL                  1
                      754 CALL                     1
          
-         123         764 LOAD_GLOBAL              0 (db)
+         124         764 LOAD_GLOBAL              0 (db)
                      776 LOAD_ATTR                5 (func)
                      786 LOAD_METHOD             15 (avg)
                      808 LOAD_GLOBAL              0 (db)
                      820 LOAD_ATTR                3 (Participant)
                      830 LOAD_ATTR               16 (duration)
                      840 PRECALL                  1
                      844 CALL                     1
                      854 LOAD_METHOD              8 (label)
                      876 LOAD_CONST               5 ('minutes')
                      878 PRECALL                  1
                      882 CALL                     1
          
-         117         892 PRECALL                  6
+         118         892 PRECALL                  6
                      896 CALL                     6
          
-         124         906 LOAD_METHOD             17 (filter)
+         125         906 LOAD_METHOD             17 (filter)
                      928 LOAD_GLOBAL              1 (NULL + db)
                      940 LOAD_ATTR               18 (or_)
                      950 LOAD_GLOBAL              0 (db)
                      962 LOAD_ATTR                3 (Participant)
                      972 LOAD_ATTR               19 (excludeFromCount)
                      982 UNARY_INVERT
                      984 LOAD_GLOBAL              0 (db)
@@ -1301,44 +1355,44 @@
                     1016 LOAD_CONST               0 (None)
                     1018 COMPARE_OP               2 (==)
                     1024 PRECALL                  2
                     1028 CALL                     2
                     1038 PRECALL                  1
                     1042 CALL                     1
          
-         125        1052 LOAD_METHOD             20 (group_by)
+         126        1052 LOAD_METHOD             20 (group_by)
                     1074 LOAD_GLOBAL              0 (db)
                     1086 LOAD_ATTR                3 (Participant)
                     1096 LOAD_ATTR                4 (condition)
                     1106 PRECALL                  1
                     1110 CALL                     1
                     1120 LOAD_METHOD             21 (all)
                     1142 PRECALL                  0
                     1146 CALL                     0
          
-         117        1156 STORE_FAST               0 (summary_groups)
+         118        1156 STORE_FAST               0 (summary_groups)
          
-         127        1158 LOAD_GLOBAL              0 (db)
+         128        1158 LOAD_GLOBAL              0 (db)
                     1170 LOAD_ATTR                1 (session)
                     1180 LOAD_METHOD              2 (query)
          
-         128        1202 LOAD_GLOBAL              0 (db)
+         129        1202 LOAD_GLOBAL              0 (db)
                     1214 LOAD_ATTR                5 (func)
                     1224 LOAD_METHOD              6 (count)
                     1246 LOAD_GLOBAL              0 (db)
                     1258 LOAD_ATTR                3 (Participant)
                     1268 LOAD_ATTR                7 (participantID)
                     1278 PRECALL                  1
                     1282 CALL                     1
                     1292 LOAD_METHOD              8 (label)
                     1314 LOAD_CONST               1 ('count')
                     1316 PRECALL                  1
                     1320 CALL                     1
          
-         129        1330 LOAD_GLOBAL              0 (db)
+         130        1330 LOAD_GLOBAL              0 (db)
                     1342 LOAD_ATTR                5 (func)
                     1352 LOAD_METHOD              9 (sum)
                     1374 LOAD_GLOBAL              1 (NULL + db)
                     1386 LOAD_ATTR               10 (cast)
                     1396 LOAD_GLOBAL              0 (db)
                     1408 LOAD_ATTR                3 (Participant)
                     1418 LOAD_ATTR               11 (is_abandoned)
@@ -1349,15 +1403,15 @@
                     1464 PRECALL                  1
                     1468 CALL                     1
                     1478 LOAD_METHOD              8 (label)
                     1500 LOAD_CONST               2 ('countAbandoned')
                     1502 PRECALL                  1
                     1506 CALL                     1
          
-         130        1516 LOAD_GLOBAL              0 (db)
+         131        1516 LOAD_GLOBAL              0 (db)
                     1528 LOAD_ATTR                5 (func)
                     1538 LOAD_METHOD              9 (sum)
                     1560 LOAD_GLOBAL              1 (NULL + db)
                     1572 LOAD_ATTR               10 (cast)
                     1582 LOAD_GLOBAL              0 (db)
                     1594 LOAD_ATTR                3 (Participant)
                     1604 LOAD_ATTR               13 (is_in_progress)
@@ -1368,15 +1422,15 @@
                     1650 PRECALL                  1
                     1654 CALL                     1
                     1664 LOAD_METHOD              8 (label)
                     1686 LOAD_CONST               3 ('countInProgress')
                     1688 PRECALL                  1
                     1692 CALL                     1
          
-         131        1702 LOAD_GLOBAL              0 (db)
+         132        1702 LOAD_GLOBAL              0 (db)
                     1714 LOAD_ATTR                5 (func)
                     1724 LOAD_METHOD              9 (sum)
                     1746 LOAD_GLOBAL              1 (NULL + db)
                     1758 LOAD_ATTR               10 (cast)
                     1768 LOAD_GLOBAL              0 (db)
                     1780 LOAD_ATTR                3 (Participant)
                     1790 LOAD_ATTR               14 (finished)
@@ -1387,57 +1441,57 @@
                     1836 PRECALL                  1
                     1840 CALL                     1
                     1850 LOAD_METHOD              8 (label)
                     1872 LOAD_CONST               4 ('countFinished')
                     1874 PRECALL                  1
                     1878 CALL                     1
          
-         132        1888 LOAD_GLOBAL              0 (db)
+         133        1888 LOAD_GLOBAL              0 (db)
                     1900 LOAD_ATTR                5 (func)
                     1910 LOAD_METHOD             22 (min)
                     1932 LOAD_GLOBAL              0 (db)
                     1944 LOAD_ATTR                3 (Participant)
                     1954 LOAD_ATTR               16 (duration)
                     1964 PRECALL                  1
                     1968 CALL                     1
                     1978 LOAD_METHOD              8 (label)
                     2000 LOAD_CONST               6 ('minSeconds')
                     2002 PRECALL                  1
                     2006 CALL                     1
          
-         133        2016 LOAD_GLOBAL              0 (db)
+         134        2016 LOAD_GLOBAL              0 (db)
                     2028 LOAD_ATTR                5 (func)
                     2038 LOAD_METHOD             23 (max)
                     2060 LOAD_GLOBAL              0 (db)
                     2072 LOAD_ATTR                3 (Participant)
                     2082 LOAD_ATTR               16 (duration)
                     2092 PRECALL                  1
                     2096 CALL                     1
                     2106 LOAD_METHOD              8 (label)
                     2128 LOAD_CONST               7 ('maxSeconds')
                     2130 PRECALL                  1
                     2134 CALL                     1
          
-         134        2144 LOAD_GLOBAL              0 (db)
+         135        2144 LOAD_GLOBAL              0 (db)
                     2156 LOAD_ATTR                5 (func)
                     2166 LOAD_METHOD             15 (avg)
                     2188 LOAD_GLOBAL              0 (db)
                     2200 LOAD_ATTR                3 (Participant)
                     2210 LOAD_ATTR               16 (duration)
                     2220 PRECALL                  1
                     2224 CALL                     1
                     2234 LOAD_METHOD              8 (label)
                     2256 LOAD_CONST               8 ('seconds')
                     2258 PRECALL                  1
                     2262 CALL                     1
          
-         127        2272 PRECALL                  7
+         128        2272 PRECALL                  7
                     2276 CALL                     7
          
-         135        2286 LOAD_METHOD             17 (filter)
+         136        2286 LOAD_METHOD             17 (filter)
                     2308 LOAD_GLOBAL              1 (NULL + db)
                     2320 LOAD_ATTR               18 (or_)
                     2330 LOAD_GLOBAL              0 (db)
                     2342 LOAD_ATTR                3 (Participant)
                     2352 LOAD_ATTR               19 (excludeFromCount)
                     2362 UNARY_INVERT
                     2364 LOAD_GLOBAL              0 (db)
@@ -1446,21 +1500,21 @@
                     2396 LOAD_CONST               0 (None)
                     2398 COMPARE_OP               2 (==)
                     2404 PRECALL                  2
                     2408 CALL                     2
                     2418 PRECALL                  1
                     2422 CALL                     1
          
-         136        2432 LOAD_METHOD             24 (one)
+         137        2432 LOAD_METHOD             24 (one)
                     2454 PRECALL                  0
                     2458 CALL                     0
          
-         127        2468 STORE_FAST               1 (summary)
+         128        2468 STORE_FAST               1 (summary)
          
-         138        2470 LOAD_FAST                0 (summary_groups)
+         139        2470 LOAD_FAST                0 (summary_groups)
                     2472 LOAD_FAST                1 (summary)
                     2474 BUILD_TUPLE              2
                     2476 RETURN_VALUE
          consts
             None
             'count'
             'countAbandoned'
@@ -1472,15 +1526,15 @@
             'seconds'
          names      ('db', 'session', 'query', 'Participant', 'condition', 'func', 'count', 'participantID', 'label', 'sum', 'cast', 'is_abandoned', 'Integer', 'is_in_progress', 'finished', 'avg', 'duration', 'filter', 'or_', 'excludeFromCount', 'group_by', 'all', 'min', 'max', 'one')
          varnames   ('summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'fetch_progress_summary'
-         firstlineno 116
+         firstlineno 117
          lnotab
             0x02012c0120018001ba01ba01ba0180fa0e07920168f8020a2c018001ba
             01ba01ba018001800180f90e08920124f7020b
       '/progress'
       code
          argcount  : 0
          nlocals   : 4
@@ -1488,76 +1542,76 @@
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d01740300000000000000000000a6000000ab000000000000
             0000005c0200007d027d0374050000000000000000000064017c007c017c
             027c03740600000000000000000000ac02a6060000ab0600000000000000
             005300
-         141           0 RESUME                   0
+         142           0 RESUME                   0
          
-         144           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
+         145           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (pages)
                       34 STORE_FAST               1 (progress)
          
-         145          36 LOAD_GLOBAL              3 (NULL + fetch_progress_summary)
+         146          36 LOAD_GLOBAL              3 (NULL + fetch_progress_summary)
                       48 PRECALL                  0
                       52 CALL                     0
                       62 UNPACK_SEQUENCE          2
                       66 STORE_FAST               2 (summary_groups)
                       68 STORE_FAST               3 (summary)
          
-         147          70 LOAD_GLOBAL              5 (NULL + render_template)
+         148          70 LOAD_GLOBAL              5 (NULL + render_template)
                       82 LOAD_CONST               1 ('progress.html')
          
-         148          84 LOAD_FAST                0 (pages)
+         149          84 LOAD_FAST                0 (pages)
                       86 LOAD_FAST                1 (progress)
          
-         149          88 LOAD_FAST                2 (summary_groups)
+         150          88 LOAD_FAST                2 (summary_groups)
                       90 LOAD_FAST                3 (summary)
                       92 LOAD_GLOBAL              6 (display_time)
          
-         147         104 KW_NAMES                 2
+         148         104 KW_NAMES                 2
                      106 PRECALL                  6
                      110 CALL                     6
                      120 RETURN_VALUE
          consts
             None
             'progress.html'
             ('pages', 'progress', 'summary_groups', 'summary', 'display_time')
          names      ('fetch_progress', 'fetch_progress_summary', 'render_template', 'display_time')
          varnames   ('pages', 'progress', 'summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress'
-         firstlineno 141
+         firstlineno 142
          lnotab 0x0203220122020e01040110fe
       '/progress_ajax'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d0174030000000000000000000064017c007c01ac02a60300
             00ab0300000000000000005300
-         152           0 RESUME                   0
+         153           0 RESUME                   0
          
-         155           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
+         156           2 LOAD_GLOBAL              1 (NULL + fetch_progress)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (pages)
                       34 STORE_FAST               1 (progress)
          
-         156          36 LOAD_GLOBAL              3 (NULL + render_template)
+         157          36 LOAD_GLOBAL              3 (NULL + render_template)
                       48 LOAD_CONST               1 ('progress_ajax.html')
                       50 LOAD_FAST                0 (pages)
                       52 LOAD_FAST                1 (progress)
                       54 KW_NAMES                 2
                       56 PRECALL                  3
                       60 CALL                     3
                       70 RETURN_VALUE
@@ -1567,57 +1621,57 @@
             ('pages', 'progress')
          names      ('fetch_progress', 'render_template')
          varnames   ('pages', 'progress')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress_ajax'
-         firstlineno 152
+         firstlineno 153
          lnotab 0x02032201
       '/progress_summary_ajax'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0200007d007d0174030000000000000000000064017c007c017404000000
             00000000000000ac02a6040000ab0400000000000000005300
-         159           0 RESUME                   0
+         160           0 RESUME                   0
          
-         162           2 LOAD_GLOBAL              1 (NULL + fetch_progress_summary)
+         163           2 LOAD_GLOBAL              1 (NULL + fetch_progress_summary)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          2
                       32 STORE_FAST               0 (summary_groups)
                       34 STORE_FAST               1 (summary)
          
-         163          36 LOAD_GLOBAL              3 (NULL + render_template)
+         164          36 LOAD_GLOBAL              3 (NULL + render_template)
                       48 LOAD_CONST               1 ('progress_summary_ajax.html')
          
-         164          50 LOAD_FAST                0 (summary_groups)
+         165          50 LOAD_FAST                0 (summary_groups)
                       52 LOAD_FAST                1 (summary)
                       54 LOAD_GLOBAL              4 (display_time)
          
-         163          66 KW_NAMES                 2
+         164          66 KW_NAMES                 2
                       68 PRECALL                  4
                       72 CALL                     4
                       82 RETURN_VALUE
          consts
             None
             'progress_summary_ajax.html'
             ('summary_groups', 'summary', 'display_time')
          names      ('fetch_progress_summary', 'render_template', 'display_time')
          varnames   ('summary_groups', 'summary')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_progress_summary_ajax'
-         firstlineno 159
+         firstlineno 160
          lnotab 0x020322010e0110ff
       '/update_exclude_from_count'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 5
          flags     : 3
@@ -1631,31 +1685,31 @@
             00000000000000640119000000000000000000a6010000ab010000000000
             0000007d007400000000000000000000006a010000000000000000640219
             00000000000000000064046b02000000000c007c005f0700000000000000
             007404000000000000000000006a030000000000000000a0080000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             007413000000000000000000006405640664076901ac08a6020000ab0200
             000000000000005300
-         166           0 RESUME                   0
+         167           0 RESUME                   0
          
-         168           2 LOAD_CONST               1 ('participantID')
+         169           2 LOAD_CONST               1 ('participantID')
                        4 LOAD_GLOBAL              0 (request)
                       16 LOAD_ATTR                1 (form)
                       26 CONTAINS_OP              1
                       28 POP_JUMP_FORWARD_IF_TRUE    14 (to 58)
                       30 LOAD_CONST               2 ('excludeFromCount')
                       32 LOAD_GLOBAL              0 (request)
                       44 LOAD_ATTR                1 (form)
                       54 CONTAINS_OP              1
                       56 POP_JUMP_FORWARD_IF_FALSE     2 (to 62)
          
-         169     >>   58 LOAD_CONST               3 ('')
+         170     >>   58 LOAD_CONST               3 ('')
                       60 RETURN_VALUE
          
-         171     >>   62 LOAD_GLOBAL              4 (db)
+         172     >>   62 LOAD_GLOBAL              4 (db)
                       74 LOAD_ATTR                3 (session)
                       84 LOAD_METHOD              4 (query)
                      106 LOAD_GLOBAL              4 (db)
                      118 LOAD_ATTR                5 (Participant)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 LOAD_METHOD              6 (get)
@@ -1663,32 +1717,32 @@
                      176 LOAD_ATTR                1 (form)
                      186 LOAD_CONST               1 ('participantID')
                      188 BINARY_SUBSCR
                      198 PRECALL                  1
                      202 CALL                     1
                      212 STORE_FAST               0 (p)
          
-         172         214 LOAD_GLOBAL              0 (request)
+         173         214 LOAD_GLOBAL              0 (request)
                      226 LOAD_ATTR                1 (form)
                      236 LOAD_CONST               2 ('excludeFromCount')
                      238 BINARY_SUBSCR
                      248 LOAD_CONST               4 ('True')
                      250 COMPARE_OP               2 (==)
                      256 UNARY_NOT
                      258 LOAD_FAST                0 (p)
                      260 STORE_ATTR               7 (excludeFromCount)
          
-         173         270 LOAD_GLOBAL              4 (db)
+         174         270 LOAD_GLOBAL              4 (db)
                      282 LOAD_ATTR                3 (session)
                      292 LOAD_METHOD              8 (commit)
                      314 PRECALL                  0
                      318 CALL                     0
                      328 POP_TOP
          
-         175         330 LOAD_GLOBAL             19 (NULL + Response)
+         176         330 LOAD_GLOBAL             19 (NULL + Response)
                      342 LOAD_CONST               5 (200)
                      344 LOAD_CONST               6 ('HX-Trigger')
                      346 LOAD_CONST               7 ('excludeChanged')
                      348 BUILD_MAP                1
                      350 KW_NAMES                 8
                      352 PRECALL                  2
                      356 CALL                     2
@@ -1705,15 +1759,15 @@
             ('status', 'headers')
          names      ('request', 'form', 'db', 'session', 'query', 'Participant', 'get', 'excludeFromCount', 'commit', 'Response')
          varnames   ('p',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_update_exclude_from_count'
-         firstlineno 166
+         firstlineno 167
          lnotab 0x020238010402980138013c02
       '/export_item_timing'
       code
          argcount  : 0
          nlocals   : 13
          stacksize : 8
          flags     : 3
@@ -1746,34 +1800,34 @@
             00000000000000000000000000000000007c0b7c0ca6020000ab02000000
             00000000007a0d00007d017c02640ba00b00000000000000000000000000
             000000000000007c0a7c0c19000000000000000000a6010000ab01000000
             00000000007a0d00007d028c3c8ce27c02640c7a0d00007d0264017d0390
             018c2b742b00000000000000000000640d741400000000000000000000a0
             0b0000000000000000000000000000000000000000640e7c017c02a60300
             00ab030000000000000000ac0fa6020000ab0200000000000000005300
-         177           0 RESUME                   0
+         178           0 RESUME                   0
          
-         180           2 LOAD_GLOBAL              0 (current_app)
+         181           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (page_list)
                       24 LOAD_METHOD              2 (get_questionnaire_list)
                       46 LOAD_CONST               1 (True)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 STORE_FAST               0 (questionnaires)
          
-         181          64 LOAD_CONST               2 ('participantID,mTurkID')
+         182          64 LOAD_CONST               2 ('participantID,mTurkID')
                       66 STORE_FAST               1 (header)
          
-         182          68 LOAD_CONST               3 ('')
+         183          68 LOAD_CONST               3 ('')
                       70 STORE_FAST               2 (output)
          
-         184          72 LOAD_CONST               4 (False)
+         185          72 LOAD_CONST               4 (False)
                       74 STORE_FAST               3 (headerComplete)
          
-         186          76 LOAD_GLOBAL              6 (db)
+         187          76 LOAD_GLOBAL              6 (db)
                       88 LOAD_ATTR                4 (session)
                       98 LOAD_METHOD              5 (query)
                      120 LOAD_GLOBAL              6 (db)
                      132 LOAD_ATTR                6 (Participant)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 LOAD_METHOD              7 (filter)
@@ -1785,21 +1839,21 @@
                      218 PRECALL                  1
                      222 CALL                     1
                      232 LOAD_METHOD              9 (all)
                      254 PRECALL                  0
                      258 CALL                     0
                      268 STORE_FAST               4 (results)
          
-         188         270 LOAD_FAST                4 (results)
+         189         270 LOAD_FAST                4 (results)
                      272 GET_ITER
                  >>  274 EXTENDED_ARG             1
                      276 FOR_ITER               297 (to 872)
                      278 STORE_FAST               5 (p)
          
-         189         280 LOAD_FAST                2 (output)
+         190         280 LOAD_FAST                2 (output)
                      282 LOAD_GLOBAL             20 (str)
                      294 LOAD_METHOD             11 (format)
                      316 LOAD_CONST               5 ('{},"{}"')
                      318 LOAD_FAST                5 (p)
                      320 LOAD_ATTR               12 (participantID)
                      330 LOAD_FAST                5 (p)
                      332 LOAD_ATTR               13 (mTurkID)
@@ -1807,128 +1861,128 @@
                      364 PRECALL                  0
                      368 CALL                     0
                      378 PRECALL                  3
                      382 CALL                     3
                      392 BINARY_OP               13 (+=)
                      396 STORE_FAST               2 (output)
          
-         191         398 LOAD_FAST                0 (questionnaires)
+         192         398 LOAD_FAST                0 (questionnaires)
                      400 GET_ITER
                  >>  402 FOR_ITER               225 (to 854)
                      404 STORE_FAST               6 (qName)
          
-         192         406 LOAD_CONST               3 ('')
+         193         406 LOAD_CONST               3 ('')
                      408 STORE_FAST               7 (tag)
          
-         194         410 LOAD_CONST               6 ('/')
+         195         410 LOAD_CONST               6 ('/')
                      412 LOAD_FAST                6 (qName)
                      414 CONTAINS_OP              0
                      416 POP_JUMP_FORWARD_IF_FALSE    37 (to 492)
          
-         195         418 LOAD_FAST                6 (qName)
+         196         418 LOAD_FAST                6 (qName)
                      420 LOAD_METHOD             15 (split)
                      442 LOAD_CONST               6 ('/')
                      444 PRECALL                  1
                      448 CALL                     1
                      458 STORE_FAST               8 (qNameParts)
          
-         196         460 LOAD_FAST                8 (qNameParts)
+         197         460 LOAD_FAST                8 (qNameParts)
                      462 LOAD_CONST               7 (0)
                      464 BINARY_SUBSCR
                      474 STORE_FAST               6 (qName)
          
-         197         476 LOAD_FAST                8 (qNameParts)
+         198         476 LOAD_FAST                8 (qNameParts)
                      478 LOAD_CONST               8 (1)
                      480 BINARY_SUBSCR
                      490 STORE_FAST               7 (tag)
          
-         199     >>  492 LOAD_FAST                5 (p)
+         200     >>  492 LOAD_FAST                5 (p)
                      494 LOAD_METHOD             16 (questionnaire)
                      516 LOAD_FAST                6 (qName)
                      518 LOAD_FAST                7 (tag)
                      520 PRECALL                  2
                      524 CALL                     2
                      534 STORE_FAST               9 (q)
          
-         200         536 LOAD_FAST                5 (p)
+         201         536 LOAD_FAST                5 (p)
                      538 LOAD_METHOD             17 (questionnaire_log)
                      560 LOAD_FAST                6 (qName)
                      562 LOAD_FAST                7 (tag)
                      564 PRECALL                  2
                      568 CALL                     2
                      578 STORE_FAST              10 (logs)
          
-         202         580 LOAD_FAST                6 (qName)
+         203         580 LOAD_FAST                6 (qName)
                      582 STORE_FAST              11 (qNameFull)
          
-         203         584 LOAD_GLOBAL             37 (NULL + len)
+         204         584 LOAD_GLOBAL             37 (NULL + len)
                      596 LOAD_FAST                7 (tag)
                      598 PRECALL                  1
                      602 CALL                     1
                      612 LOAD_CONST               7 (0)
                      614 COMPARE_OP               4 (>)
                      620 POP_JUMP_FORWARD_IF_FALSE    22 (to 666)
          
-         204         622 LOAD_CONST               9 ('{}_{}')
+         205         622 LOAD_CONST               9 ('{}_{}')
                      624 LOAD_METHOD             11 (format)
                      646 LOAD_FAST                6 (qName)
                      648 LOAD_FAST                7 (tag)
                      650 PRECALL                  2
                      654 CALL                     2
                      664 STORE_FAST              11 (qNameFull)
          
-         206     >>  666 LOAD_GLOBAL             39 (NULL + sorted)
+         207     >>  666 LOAD_GLOBAL             39 (NULL + sorted)
                      678 LOAD_FAST               10 (logs)
                      680 LOAD_METHOD             20 (keys)
                      702 PRECALL                  0
                      706 CALL                     0
                      716 PRECALL                  1
                      720 CALL                     1
                      730 GET_ITER
                  >>  732 FOR_ITER                59 (to 852)
                      734 STORE_FAST              12 (key)
          
-         207         736 LOAD_FAST                3 (headerComplete)
+         208         736 LOAD_FAST                3 (headerComplete)
                      738 POP_JUMP_FORWARD_IF_TRUE    25 (to 790)
          
-         208         740 LOAD_FAST                1 (header)
+         209         740 LOAD_FAST                1 (header)
                      742 LOAD_CONST              10 (',{}_{}')
                      744 LOAD_METHOD             11 (format)
                      766 LOAD_FAST               11 (qNameFull)
                      768 LOAD_FAST               12 (key)
                      770 PRECALL                  2
                      774 CALL                     2
                      784 BINARY_OP               13 (+=)
                      788 STORE_FAST               1 (header)
          
-         210     >>  790 LOAD_FAST                2 (output)
+         211     >>  790 LOAD_FAST                2 (output)
                      792 LOAD_CONST              11 (',{}')
                      794 LOAD_METHOD             11 (format)
                      816 LOAD_FAST               10 (logs)
                      818 LOAD_FAST               12 (key)
                      820 BINARY_SUBSCR
                      830 PRECALL                  1
                      834 CALL                     1
                      844 BINARY_OP               13 (+=)
                      848 STORE_FAST               2 (output)
                      850 JUMP_BACKWARD           60 (to 732)
          
-         206     >>  852 JUMP_BACKWARD          226 (to 402)
+         207     >>  852 JUMP_BACKWARD          226 (to 402)
          
-         212     >>  854 LOAD_FAST                2 (output)
+         213     >>  854 LOAD_FAST                2 (output)
                      856 LOAD_CONST              12 ('\n')
                      858 BINARY_OP               13 (+=)
                      862 STORE_FAST               2 (output)
          
-         213         864 LOAD_CONST               1 (True)
+         214         864 LOAD_CONST               1 (True)
                      866 STORE_FAST               3 (headerComplete)
                      868 EXTENDED_ARG             1
                      870 JUMP_BACKWARD          299 (to 274)
          
-         215     >>  872 LOAD_GLOBAL             43 (NULL + render_template)
+         216     >>  872 LOAD_GLOBAL             43 (NULL + render_template)
                      884 LOAD_CONST              13 ('export_csv.html')
                      886 LOAD_GLOBAL             20 (str)
                      898 LOAD_METHOD             11 (format)
                      920 LOAD_CONST              14 ('{}\n{}')
                      922 LOAD_FAST                1 (header)
                      924 LOAD_FAST                2 (output)
                      926 PRECALL                  3
@@ -1956,25 +2010,25 @@
             ('data',)
          names      ('current_app', 'page_list', 'get_questionnaire_list', 'db', 'session', 'query', 'Participant', 'filter', 'finished', 'all', 'str', 'format', 'participantID', 'mTurkID', 'strip', 'split', 'questionnaire', 'questionnaire_log', 'len', 'sorted', 'keys', 'render_template')
          varnames   ('questionnaires', 'header', 'output', 'headerComplete', 'results', 'p', 'qName', 'tag', 'qNameParts', 'q', 'logs', 'qNameFull', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_export_item_timing'
-         firstlineno 177
+         firstlineno 178
          lnotab
             0x02033e01040104020402c2020a0176020801040208012a01100110022c
             012c02040126012c024601040132023efc02060a010802
       '/export'
       '/export/download'
       'route_export_download'
       ('endpoint',)
       code
          argcount  : 0
-         nlocals   : 9
+         nlocals   : 8
          stacksize : 10
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007400000000000000000000006a
             030000000000000000a6010000ab010000000000000000a0040000000000
             0000000000000000000000000000007400000000000000000000006a0300
@@ -1989,195 +2043,264 @@
             000000000000000000000000000000a6000000ab0000000000000000007d
             017410000000000000000000006a090000000000000000a00a0000000000
             00000000000000000000000000000064036401a6020000ab020000000000
             0000007d027410000000000000000000006a090000000000000000a00a00
             0000000000000000000000000000000000000064046402a6020000ab0200
             000000000000007d037410000000000000000000006a0900000000000000
             00a00a000000000000000000000000000000000000000064056401a60200
-            00ab0200000000000000007d0467007d0569007d06741700000000000000
-            0000007c057c067c027c04a6040000ab0400000000000000007d07741900
-            0000000000000000007c057c067c077c03a6040000ab0400000000000000
-            000100741b000000000000000000007c057c067c077c03a6040000ab0400
-            000000000000000100741d000000000000000000007c057c06a6020000ab
-            0200000000000000007d087410000000000000000000006a0f0000000000
-            000000a01000000000000000000000000000000000000000006406a60100
-            00ab010000000000000000723e7423000000000000000000007c08640764
-            086409640a7425000000000000000000006a130000000000000000a60000
-            00ab000000000000000000a0140000000000000000000000000000000000
-            000000640ba6010000ab0100000000000000007a0000007a0600006901ac
-            0ca6030000ab0300000000000000005300742b0000000000000000000064
-            0d7c08742d000000000000000000007c06a6010000ab0100000000000000
-            007c007c01ac0ea6050000ab0500000000000000005300
-         218           0 RESUME                   0
+            00ab0200000000000000007d047c04733e7c02723c740100000000000000
+            0000006a0b00000000000000007400000000000000000000006a03000000
+            00000000006a07000000000000000064016b020000000074000000000000
+            00000000006a0300000000000000006a07000000000000000064006b0200
+            000000a6020000ab0200000000000000007d056e907c0473627401000000
+            000000000000006a0c00000000000000007400000000000000000000006a
+            0300000000000000006a05000000000000000064026b0200000000740100
+            0000000000000000006a0b00000000000000007400000000000000000000
+            006a0300000000000000006a07000000000000000064016b020000000074
+            00000000000000000000006a0300000000000000006a0700000000000000
+            0064006b0200000000a6020000ab020000000000000000a6020000ab0200
+            000000000000007d056e2c7c02730364007d056e27740100000000000000
+            0000006a0c00000000000000007400000000000000000000006a03000000
+            00000000006a05000000000000000064026b0200000000a6010000ab0100
+            000000000000007d05741b000000000000000000007c05a6010000ab0100
+            000000000000007d067c06a00e0000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d077410000000000000000000
+            006a0f0000000000000000a0100000000000000000000000000000000000
+            0000006406a6010000ab0100000000000000007250742300000000000000
+            0000007c07a0120000000000000000000000000000000000000000a60000
+            00ab000000000000000000640764086409640a7427000000000000000000
+            006a140000000000000000a6000000ab000000000000000000a015000000
+            0000000000000000000000000000000000640ba6010000ab010000000000
+            0000007a0000007a0600006901ac0ca6030000ab03000000000000000053
+            00742d00000000000000000000640d7c07a0170000000000000000000000
+            0000000000000000006401640e640fac10a6030000ab0300000000000000
+            007431000000000000000000007c066a190000000000000000a6010000ab
+            0100000000000000007c007c01ac11a6050000ab05000000000000000053
+            00
+         219           0 RESUME                   0
          
-         222           2 LOAD_GLOBAL              0 (db)
+         223           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
                       46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (Participant)
                       68 PRECALL                  1
                       72 CALL                     1
          
-         223          82 LOAD_METHOD              4 (filter)
+         224          82 LOAD_METHOD              4 (filter)
                      104 LOAD_GLOBAL              0 (db)
                      116 LOAD_ATTR                3 (Participant)
                      126 LOAD_ATTR                5 (finished)
                      136 LOAD_CONST               1 (False)
                      138 COMPARE_OP               2 (==)
                      144 PRECALL                  1
                      148 CALL                     1
                      158 LOAD_METHOD              6 (count)
                      180 PRECALL                  0
                      184 CALL                     0
          
-         222         194 STORE_FAST               0 (unfinished_count)
+         223         194 STORE_FAST               0 (unfinished_count)
          
-         224         196 LOAD_GLOBAL              0 (db)
+         225         196 LOAD_GLOBAL              0 (db)
                      208 LOAD_ATTR                1 (session)
                      218 LOAD_METHOD              2 (query)
                      240 LOAD_GLOBAL              0 (db)
                      252 LOAD_ATTR                3 (Participant)
                      262 PRECALL                  1
                      266 CALL                     1
          
-         225         276 LOAD_METHOD              4 (filter)
+         226         276 LOAD_METHOD              4 (filter)
                      298 LOAD_GLOBAL              0 (db)
                      310 LOAD_ATTR                3 (Participant)
                      320 LOAD_ATTR                7 (excludeFromCount)
                      330 LOAD_CONST               2 (True)
                      332 COMPARE_OP               2 (==)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_METHOD              6 (count)
                      374 PRECALL                  0
                      378 CALL                     0
          
-         224         388 STORE_FAST               1 (excluded_count)
+         225         388 STORE_FAST               1 (excluded_count)
          
-         227         390 LOAD_GLOBAL             16 (request)
+         228         390 LOAD_GLOBAL             16 (request)
                      402 LOAD_ATTR                9 (args)
                      412 LOAD_METHOD             10 (get)
                      434 LOAD_CONST               3 ('includeUnfinished')
                      436 LOAD_CONST               1 (False)
                      438 PRECALL                  2
                      442 CALL                     2
                      452 STORE_FAST               2 (include_unfinished)
          
-         228         454 LOAD_GLOBAL             16 (request)
+         229         454 LOAD_GLOBAL             16 (request)
                      466 LOAD_ATTR                9 (args)
                      476 LOAD_METHOD             10 (get)
                      498 LOAD_CONST               4 ('includeMissing')
                      500 LOAD_CONST               2 (True)
                      502 PRECALL                  2
                      506 CALL                     2
                      516 STORE_FAST               3 (include_missing)
          
-         229         518 LOAD_GLOBAL             16 (request)
+         230         518 LOAD_GLOBAL             16 (request)
                      530 LOAD_ATTR                9 (args)
                      540 LOAD_METHOD             10 (get)
                      562 LOAD_CONST               5 ('includeExcluded')
                      564 LOAD_CONST               1 (False)
                      566 PRECALL                  2
                      570 CALL                     2
                      580 STORE_FAST               4 (include_excluded)
          
-         231         582 BUILD_LIST               0
-                     584 STORE_FAST               5 (column_list)
-         
-         232         586 BUILD_MAP                0
-                     588 STORE_FAST               6 (export_data)
-         
-         234         590 LOAD_GLOBAL             23 (NULL + add_participants_to_export)
-                     602 LOAD_FAST                5 (column_list)
-                     604 LOAD_FAST                6 (export_data)
-                     606 LOAD_FAST                2 (include_unfinished)
-                     608 LOAD_FAST                4 (include_excluded)
-                     610 PRECALL                  4
-                     614 CALL                     4
-                     624 STORE_FAST               7 (query)
-         
-         235         626 LOAD_GLOBAL             25 (NULL + add_questionnaires_to_export)
-                     638 LOAD_FAST                5 (column_list)
-                     640 LOAD_FAST                6 (export_data)
-                     642 LOAD_FAST                7 (query)
-                     644 LOAD_FAST                3 (include_missing)
-                     646 PRECALL                  4
-                     650 CALL                     4
-                     660 POP_TOP
-         
-         236         662 LOAD_GLOBAL             27 (NULL + add_custom_exports_to_export)
-                     674 LOAD_FAST                5 (column_list)
-                     676 LOAD_FAST                6 (export_data)
-                     678 LOAD_FAST                7 (query)
-                     680 LOAD_FAST                3 (include_missing)
-                     682 PRECALL                  4
-                     686 CALL                     4
-                     696 POP_TOP
-         
-         238         698 LOAD_GLOBAL             29 (NULL + build_export_csv)
-                     710 LOAD_FAST                5 (column_list)
-                     712 LOAD_FAST                6 (export_data)
-                     714 PRECALL                  2
-                     718 CALL                     2
-                     728 STORE_FAST               8 (csv_string)
-         
-         240         730 LOAD_GLOBAL             16 (request)
-                     742 LOAD_ATTR               15 (base_url)
-                     752 LOAD_METHOD             16 (endswith)
-                     774 LOAD_CONST               6 ('/download')
-                     776 PRECALL                  1
-                     780 CALL                     1
-                     790 POP_JUMP_FORWARD_IF_FALSE    62 (to 916)
-         
-         241         792 LOAD_GLOBAL             35 (NULL + Response)
-                     804 LOAD_FAST                8 (csv_string)
-         
-         242         806 LOAD_CONST               7 ('text/csv')
-         
-         244         808 LOAD_CONST               8 ('Content-disposition')
-                     810 LOAD_CONST               9 ('attachment; filename=%s.csv')
-         
-         245         812 LOAD_CONST              10 ('export_')
-                     814 LOAD_GLOBAL             37 (NULL + datetime)
-                     826 LOAD_ATTR               19 (utcnow)
-                     836 PRECALL                  0
-                     840 CALL                     0
-                     850 LOAD_METHOD             20 (strftime)
-                     872 LOAD_CONST              11 ('%Y-%m-%d_%H-%M')
-                     874 PRECALL                  1
-                     878 CALL                     1
-                     888 BINARY_OP                0 (+)
-         
-         244         892 BINARY_OP                6 (%)
-         
-         243         896 BUILD_MAP                1
-         
-         241         898 KW_NAMES                12
-                     900 PRECALL                  3
-                     904 CALL                     3
-                     914 RETURN_VALUE
-         
-         248     >>  916 LOAD_GLOBAL             43 (NULL + render_template)
-                     928 LOAD_CONST              13 ('export.html')
-         
-         249         930 LOAD_FAST                8 (csv_string)
-         
-         250         932 LOAD_GLOBAL             45 (NULL + len)
-                     944 LOAD_FAST                6 (export_data)
-                     946 PRECALL                  1
-                     950 CALL                     1
-         
-         251         960 LOAD_FAST                0 (unfinished_count)
-         
-         252         962 LOAD_FAST                1 (excluded_count)
-         
-         248         964 KW_NAMES                14
-                     966 PRECALL                  5
-                     970 CALL                     5
-                     980 RETURN_VALUE
+         232         582 LOAD_FAST                4 (include_excluded)
+                     584 POP_JUMP_FORWARD_IF_TRUE    62 (to 710)
+                     586 LOAD_FAST                2 (include_unfinished)
+                     588 POP_JUMP_FORWARD_IF_FALSE    60 (to 710)
+         
+         233         590 LOAD_GLOBAL              1 (NULL + db)
+                     602 LOAD_ATTR               11 (or_)
+                     612 LOAD_GLOBAL              0 (db)
+                     624 LOAD_ATTR                3 (Participant)
+                     634 LOAD_ATTR                7 (excludeFromCount)
+                     644 LOAD_CONST               1 (False)
+                     646 COMPARE_OP               2 (==)
+                     652 LOAD_GLOBAL              0 (db)
+                     664 LOAD_ATTR                3 (Participant)
+                     674 LOAD_ATTR                7 (excludeFromCount)
+                     684 LOAD_CONST               0 (None)
+                     686 COMPARE_OP               2 (==)
+                     692 PRECALL                  2
+                     696 CALL                     2
+                     706 STORE_FAST               5 (query_filter)
+                     708 JUMP_FORWARD           144 (to 998)
+         
+         234     >>  710 LOAD_FAST                4 (include_excluded)
+                     712 POP_JUMP_FORWARD_IF_TRUE    98 (to 910)
+         
+         235         714 LOAD_GLOBAL              1 (NULL + db)
+                     726 LOAD_ATTR               12 (and_)
+                     736 LOAD_GLOBAL              0 (db)
+                     748 LOAD_ATTR                3 (Participant)
+                     758 LOAD_ATTR                5 (finished)
+                     768 LOAD_CONST               2 (True)
+                     770 COMPARE_OP               2 (==)
+         
+         236         776 LOAD_GLOBAL              1 (NULL + db)
+                     788 LOAD_ATTR               11 (or_)
+                     798 LOAD_GLOBAL              0 (db)
+                     810 LOAD_ATTR                3 (Participant)
+                     820 LOAD_ATTR                7 (excludeFromCount)
+                     830 LOAD_CONST               1 (False)
+                     832 COMPARE_OP               2 (==)
+                     838 LOAD_GLOBAL              0 (db)
+                     850 LOAD_ATTR                3 (Participant)
+                     860 LOAD_ATTR                7 (excludeFromCount)
+                     870 LOAD_CONST               0 (None)
+                     872 COMPARE_OP               2 (==)
+                     878 PRECALL                  2
+                     882 CALL                     2
+         
+         235         892 PRECALL                  2
+                     896 CALL                     2
+                     906 STORE_FAST               5 (query_filter)
+                     908 JUMP_FORWARD            44 (to 998)
+         
+         237     >>  910 LOAD_FAST                2 (include_unfinished)
+                     912 POP_JUMP_FORWARD_IF_TRUE     3 (to 920)
+         
+         238         914 LOAD_CONST               0 (None)
+                     916 STORE_FAST               5 (query_filter)
+                     918 JUMP_FORWARD            39 (to 998)
+         
+         240     >>  920 LOAD_GLOBAL              1 (NULL + db)
+                     932 LOAD_ATTR               12 (and_)
+                     942 LOAD_GLOBAL              0 (db)
+                     954 LOAD_ATTR                3 (Participant)
+                     964 LOAD_ATTR                5 (finished)
+                     974 LOAD_CONST               2 (True)
+                     976 COMPARE_OP               2 (==)
+                     982 PRECALL                  1
+                     986 CALL                     1
+                     996 STORE_FAST               5 (query_filter)
+         
+         242     >>  998 LOAD_GLOBAL             27 (NULL + Results)
+                    1010 LOAD_FAST                5 (query_filter)
+                    1012 PRECALL                  1
+                    1016 CALL                     1
+                    1026 STORE_FAST               6 (results)
+         
+         243        1028 LOAD_FAST                6 (results)
+                    1030 LOAD_METHOD             14 (build_data_frame)
+                    1052 PRECALL                  0
+                    1056 CALL                     0
+                    1066 STORE_FAST               7 (df)
+         
+         246        1068 LOAD_GLOBAL             16 (request)
+                    1080 LOAD_ATTR               15 (base_url)
+                    1090 LOAD_METHOD             16 (endswith)
+                    1112 LOAD_CONST               6 ('/download')
+                    1114 PRECALL                  1
+                    1118 CALL                     1
+                    1128 POP_JUMP_FORWARD_IF_FALSE    80 (to 1290)
+         
+         247        1130 LOAD_GLOBAL             35 (NULL + Response)
+                    1142 LOAD_FAST                7 (df)
+                    1144 LOAD_METHOD             18 (to_csv)
+                    1166 PRECALL                  0
+                    1170 CALL                     0
+         
+         248        1180 LOAD_CONST               7 ('text/csv')
+         
+         250        1182 LOAD_CONST               8 ('Content-disposition')
+                    1184 LOAD_CONST               9 ('attachment; filename=%s.csv')
+         
+         251        1186 LOAD_CONST              10 ('export_')
+                    1188 LOAD_GLOBAL             39 (NULL + datetime)
+                    1200 LOAD_ATTR               20 (utcnow)
+                    1210 PRECALL                  0
+                    1214 CALL                     0
+                    1224 LOAD_METHOD             21 (strftime)
+                    1246 LOAD_CONST              11 ('%Y-%m-%d_%H-%M')
+                    1248 PRECALL                  1
+                    1252 CALL                     1
+                    1262 BINARY_OP                0 (+)
+         
+         250        1266 BINARY_OP                6 (%)
+         
+         249        1270 BUILD_MAP                1
+         
+         247        1272 KW_NAMES                12
+                    1274 PRECALL                  3
+                    1278 CALL                     3
+                    1288 RETURN_VALUE
+         
+         254     >> 1290 LOAD_GLOBAL             45 (NULL + render_template)
+                    1302 LOAD_CONST              13 ('export.html')
+         
+         255        1304 LOAD_FAST                7 (df)
+                    1306 LOAD_METHOD             23 (to_html)
+                    1328 LOAD_CONST               1 (False)
+                    1330 LOAD_CONST              14 ('table table-striped border')
+                    1332 LOAD_CONST              15 ('left')
+                    1334 KW_NAMES                16
+                    1336 PRECALL                  3
+                    1340 CALL                     3
+         
+         256        1350 LOAD_GLOBAL             49 (NULL + len)
+                    1362 LOAD_FAST                6 (results)
+                    1364 LOAD_ATTR               25 (export_data)
+                    1374 PRECALL                  1
+                    1378 CALL                     1
+         
+         257        1388 LOAD_FAST                0 (unfinished_count)
+         
+         258        1390 LOAD_FAST                1 (excluded_count)
+         
+         254        1392 KW_NAMES                17
+                    1394 PRECALL                  5
+                    1398 CALL                     5
+                    1408 RETURN_VALUE
          consts
             None
             False
             True
             'includeUnfinished'
             'includeMissing'
             'includeExcluded'
@@ -2185,116 +2308,329 @@
             'text/csv'
             'Content-disposition'
             'attachment; filename=%s.csv'
             'export_'
             '%Y-%m-%d_%H-%M'
             ('mimetype', 'headers')
             'export.html'
-            ('data', 'rowCount', 'unfinishedCount', 'excludedCount')
-         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'count', 'excludeFromCount', 'request', 'args', 'get', 'add_participants_to_export', 'add_questionnaires_to_export', 'add_custom_exports_to_export', 'build_export_csv', 'base_url', 'endswith', 'Response', 'datetime', 'utcnow', 'strftime', 'render_template', 'len')
-         varnames   ('unfinished_count', 'excluded_count', 'include_unfinished', 'include_missing', 'include_excluded', 'column_list', 'export_data', 'query', 'csv_string')
+            'table table-striped border'
+            'left'
+            ('index', 'classes', 'justify')
+            ('data_table', 'rowCount', 'unfinishedCount', 'excludedCount')
+         names      ('db', 'session', 'query', 'Participant', 'filter', 'finished', 'count', 'excludeFromCount', 'request', 'args', 'get', 'or_', 'and_', 'Results', 'build_data_frame', 'base_url', 'endswith', 'Response', 'to_csv', 'datetime', 'utcnow', 'strftime', 'render_template', 'to_html', 'len', 'export_data')
+         varnames   ('unfinished_count', 'excluded_count', 'include_unfinished', 'include_missing', 'include_excluded', 'query_filter', 'results', 'df')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_export'
-         firstlineno 218
+         firstlineno 219
          lnotab
-            0x0204500170ff0202500170ff0203400140014002040104022401240124
-            0220023e010e010202040150ff04ff02fe12070e0102011c01020102fc
-      '/results'
+            0x0204500170ff0202500170ff02034001400140020801780104013e0174
+            ff1202040106024e021e0128033e0132010202040150ff04ff02fe12070e
+            012e012601020102fc
+      'return'
       code
          argcount  : 0
-         nlocals   : 6
-         stacksize : 5
+         nlocals   : 7
+         stacksize : 7
          flags     : 3
          code
-            0x97007401000000000000000000006a0100000000000000006401ac02a6
-            010000ab0100000000000000007d0069007d017c0044005d5c7d02740500
-            0000000000000000007c02a6010000ab0100000000000000005c0200007d
-            037d047407000000000000000000007408000000000000000000007c0319
-            0000000000000000007c04a6020000ab0200000000000000007d057c05a0
-            050000000000000000000000000000000000000000a6000000ab00000000
-            000000000001007c05a00600000000000000000000000000000000000000
-            00a6000000ab00000000000000000001007c057c017c023c0000008c5d74
-            0f0000000000000000000064037c01ac04a6020000ab0200000000000000
-            005300
-         255           0 RESUME                   0
-         
-         258           2 LOAD_GLOBAL              1 (NULL + page_list)
-                      14 LOAD_ATTR                1 (get_questionnaire_list)
-                      24 LOAD_CONST               1 (True)
-                      26 KW_NAMES                 2
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 STORE_FAST               0 (qList)
-         
-         259          44 BUILD_MAP                0
-                      46 STORE_FAST               1 (results)
-         
-         261          48 LOAD_FAST                0 (qList)
-                      50 GET_ITER
-                 >>   52 FOR_ITER                92 (to 238)
-                      54 STORE_FAST               2 (qNameAndTag)
+            0x97007400000000000000000000006a010000000000000000a002000000
+            00000000000000000000000000000000007406000000000000000000006a
+            0400000000000000006401a6020000ab0200000000000000007d00740b00
+            000000000000000000740d000000000000000000006a0700000000000000
+            00740c000000000000000000006a0800000000000000006a090000000000
+            00000064026b0200000000740c000000000000000000006a080000000000
+            0000006a0a000000000000000064036b0200000000a6020000ab02000000
+            00000000007c00a6020000ab0200000000000000007d017c01a00b000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            007d027c02a00c00000000000000000000000000000000000000006404ac
+            05a6010000ab0100000000000000007d0369007d04741b00000000000000
+            0000007c03a00e0000000000000000000000000000000000000000a60000
+            00ab000000000000000000a6010000ab01000000000000000044005d417d
+            057c027c0519000000000000000000a00e00000000000000000000000000
+            00000000000000a6000000ab0000000000000000006a0f00000000000000
+            006a1000000000000000007d067c066406760072177c0564077601721374
+            23000000000000000000007c037c05a6020000ab0200000000000000007c
+            047c053c0000008c427c017c027c0466035300
+         261           0 RESUME                   0
+         
+         262           2 LOAD_GLOBAL              0 (os)
+                      14 LOAD_ATTR                1 (path)
+                      24 LOAD_METHOD              2 (join)
+                      46 LOAD_GLOBAL              6 (current_app)
+                      58 LOAD_ATTR                4 (root_path)
+                      68 LOAD_CONST               1 ('cached_results.json')
+                      70 PRECALL                  2
+                      74 CALL                     2
+                      84 STORE_FAST               0 (cache_path)
+         
+         263          86 LOAD_GLOBAL             11 (NULL + Results)
+                      98 LOAD_GLOBAL             13 (NULL + db)
+                     110 LOAD_ATTR                7 (and_)
+                     120 LOAD_GLOBAL             12 (db)
+                     132 LOAD_ATTR                8 (Participant)
+                     142 LOAD_ATTR                9 (finished)
+                     152 LOAD_CONST               2 (True)
+                     154 COMPARE_OP               2 (==)
+                     160 LOAD_GLOBAL             12 (db)
+                     172 LOAD_ATTR                8 (Participant)
+                     182 LOAD_ATTR               10 (excludeFromCount)
+                     192 LOAD_CONST               3 (False)
+                     194 COMPARE_OP               2 (==)
+                     200 PRECALL                  2
+                     204 CALL                     2
+                     214 LOAD_FAST                0 (cache_path)
+                     216 PRECALL                  2
+                     220 CALL                     2
+                     230 STORE_FAST               1 (results)
+         
+         264         232 LOAD_FAST                1 (results)
+                     234 LOAD_METHOD             11 (build_data_frame)
+                     256 PRECALL                  0
+                     260 CALL                     0
+                     270 STORE_FAST               2 (df)
+         
+         266         272 LOAD_FAST                2 (df)
+                     274 LOAD_METHOD             12 (groupby)
+                     296 LOAD_CONST               4 ('condition')
+                     298 KW_NAMES                 5
+                     300 PRECALL                  1
+                     304 CALL                     1
+                     314 STORE_FAST               3 (df_grouped)
+         
+         267         316 BUILD_MAP                0
+                     318 STORE_FAST               4 (summary_stats)
+         
+         269         320 LOAD_GLOBAL             27 (NULL + list)
+                     332 LOAD_FAST                3 (df_grouped)
+                     334 LOAD_METHOD             14 (head)
+                     356 PRECALL                  0
+                     360 CALL                     0
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 GET_ITER
+                 >>  386 FOR_ITER                65 (to 518)
+                     388 STORE_FAST               5 (column)
          
-         262          56 LOAD_GLOBAL              5 (NULL + questionnaire_name_and_tag)
-                      68 LOAD_FAST                2 (qNameAndTag)
-                      70 PRECALL                  1
-                      74 CALL                     1
-                      84 UNPACK_SEQUENCE          2
-                      88 STORE_FAST               3 (qName)
-                      90 STORE_FAST               4 (qTag)
-         
-         264          92 LOAD_GLOBAL              7 (NULL + QuestionnaireResults)
-                     104 LOAD_GLOBAL              8 (questionnaires)
-                     116 LOAD_FAST                3 (qName)
-                     118 BINARY_SUBSCR
-                     128 LOAD_FAST                4 (qTag)
-                     130 PRECALL                  2
-                     134 CALL                     2
-                     144 STORE_FAST               5 (qResults)
-         
-         265         146 LOAD_FAST                5 (qResults)
-                     148 LOAD_METHOD              5 (run_query)
-                     170 PRECALL                  0
-                     174 CALL                     0
-                     184 POP_TOP
-         
-         266         186 LOAD_FAST                5 (qResults)
-                     188 LOAD_METHOD              6 (calc_descriptives)
-                     210 PRECALL                  0
-                     214 CALL                     0
-                     224 POP_TOP
-         
-         268         226 LOAD_FAST                5 (qResults)
-                     228 LOAD_FAST                1 (results)
-                     230 LOAD_FAST                2 (qNameAndTag)
-                     232 STORE_SUBSCR
-                     236 JUMP_BACKWARD           93 (to 52)
-         
-         270     >>  238 LOAD_GLOBAL             15 (NULL + render_template)
-                     250 LOAD_CONST               3 ('results.html')
-                     252 LOAD_FAST                1 (results)
-                     254 KW_NAMES                 4
-                     256 PRECALL                  2
-                     260 CALL                     2
-                     270 RETURN_VALUE
+         270         390 LOAD_FAST                2 (df)
+                     392 LOAD_FAST                5 (column)
+                     394 BINARY_SUBSCR
+                     404 LOAD_METHOD             14 (head)
+                     426 PRECALL                  0
+                     430 CALL                     0
+                     440 LOAD_ATTR               15 (dtype)
+                     450 LOAD_ATTR               16 (name)
+                     460 STORE_FAST               6 (dtype)
+         
+         271         462 LOAD_FAST                6 (dtype)
+                     464 LOAD_CONST               6 (('int64', 'float64', 'bool'))
+                     466 CONTAINS_OP              0
+                     468 POP_JUMP_FORWARD_IF_FALSE    23 (to 516)
+                     470 LOAD_FAST                5 (column)
+                     472 LOAD_CONST               7 (('participantID', 'condition', 'duration', 'finished'))
+                     474 CONTAINS_OP              1
+                     476 POP_JUMP_FORWARD_IF_FALSE    19 (to 516)
+         
+         273         478 LOAD_GLOBAL             35 (NULL + SummaryStats)
+                     490 LOAD_FAST                3 (df_grouped)
+                     492 LOAD_FAST                5 (column)
+                     494 PRECALL                  2
+                     498 CALL                     2
+                     508 LOAD_FAST                4 (summary_stats)
+                     510 LOAD_FAST                5 (column)
+                     512 STORE_SUBSCR
+                 >>  516 JUMP_BACKWARD           66 (to 386)
+         
+         275     >>  518 LOAD_FAST                1 (results)
+                     520 LOAD_FAST                2 (df)
+                     522 LOAD_FAST                4 (summary_stats)
+                     524 BUILD_TUPLE              3
+                     526 RETURN_VALUE
          consts
             None
+            'cached_results.json'
             True
-            ('include_tags',)
+            False
+            'condition'
+            ('by',)
+            ('int64', 'float64', 'bool')
+            ('participantID', 'condition', 'duration', 'finished')
+         names      ('os', 'path', 'join', 'current_app', 'root_path', 'Results', 'db', 'and_', 'Participant', 'finished', 'excludeFromCount', 'build_data_frame', 'groupby', 'list', 'head', 'dtype', 'name', 'SummaryStats')
+         varnames   ('cache_path', 'results', 'df', 'df_grouped', 'summary_stats', 'column', 'dtype')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
+         name       'calculate_results'
+         firstlineno 261
+         lnotab 0x02015401920128022c0104024601480110022802
+      '/results'
+      code
+         argcount  : 0
+         nlocals   : 3
+         stacksize : 4
+         flags     : 3
+         code
+            0x9700740100000000000000000000a6000000ab0000000000000000005c
+            0300007d007d017d0274030000000000000000000064017c02ac02a60200
+            00ab0200000000000000005300
+         278           0 RESUME                   0
+         
+         281           2 LOAD_GLOBAL              1 (NULL + calculate_results)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 UNPACK_SEQUENCE          3
+                      32 STORE_FAST               0 (results)
+                      34 STORE_FAST               1 (df)
+                      36 STORE_FAST               2 (summary_stats)
+         
+         283          38 LOAD_GLOBAL              3 (NULL + render_template)
+                      50 LOAD_CONST               1 ('results.html')
+                      52 LOAD_FAST                2 (summary_stats)
+                      54 KW_NAMES                 2
+                      56 PRECALL                  2
+                      60 CALL                     2
+                      70 RETURN_VALUE
+         consts
+            None
             'results.html'
-            ('results',)
-         names      ('page_list', 'get_questionnaire_list', 'questionnaire_name_and_tag', 'QuestionnaireResults', 'questionnaires', 'run_query', 'calc_descriptives', 'render_template')
-         varnames   ('qList', 'results', 'qNameAndTag', 'qName', 'qTag', 'qResults')
+            ('summary_stats',)
+         names      ('calculate_results', 'render_template')
+         varnames   ('results', 'df', 'summary_stats')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_results'
-         firstlineno 255
-         lnotab 0x02032a010402080124023601280128020c02
+         firstlineno 278
+         lnotab 0x02032402
+      '/results_boxplot/<path:field_name>'
+      'field_name'
+      code
+         argcount  : 1
+         nlocals   : 10
+         stacksize : 6
+         flags     : 3
+         code
+            0x9700740100000000000000000000a6000000ab0000000000000000005c
+            0300007d017d027d037c02640119000000000000000000a0010000000000
+            000000000000000000000000000000a6000000ab000000000000000000a0
+            020000000000000000000000000000000000000000a6000000ab00000000
+            00000000007d047c04a00300000000000000000000000000000000000000
+            00a6000000ab000000000000000000010067007d057c0444005d6d7d067c
+            026a0400000000000000007c026a0500000000000000007c066b02000000
+            00190000000000000000007d077c07a00600000000000000000000000000
+            00000000000000a6000000ab0000000000000000007d087c077c00190000
+            00000000000000a0070000000000000000000000000000000000000000a6
+            000000ab0000000000000000007411000000000000000000007c06a60100
+            00ab0100000000000000006402640364049c047d097c05a0090000000000
+            0000000000000000000000000000007c09a6010000ab0100000000000000
+            0001008c6e74150000000000000000000064057c007c05ac06a6030000ab
+            0300000000000000005300
+         285           0 RESUME                   0
+         
+         288           2 LOAD_GLOBAL              1 (NULL + calculate_results)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 UNPACK_SEQUENCE          3
+                      32 STORE_FAST               1 (results)
+                      34 STORE_FAST               2 (df)
+                      36 STORE_FAST               3 (summary_stats)
+         
+         290          38 LOAD_FAST                2 (df)
+                      40 LOAD_CONST               1 ('condition')
+                      42 BINARY_SUBSCR
+                      52 LOAD_METHOD              1 (unique)
+                      74 PRECALL                  0
+                      78 CALL                     0
+                      88 LOAD_METHOD              2 (tolist)
+                     110 PRECALL                  0
+                     114 CALL                     0
+                     124 STORE_FAST               4 (unique_conditions)
+         
+         291         126 LOAD_FAST                4 (unique_conditions)
+                     128 LOAD_METHOD              3 (sort)
+                     150 PRECALL                  0
+                     154 CALL                     0
+                     164 POP_TOP
+         
+         292         166 BUILD_LIST               0
+                     168 STORE_FAST               5 (plot_data)
+         
+         294         170 LOAD_FAST                4 (unique_conditions)
+                     172 GET_ITER
+                 >>  174 FOR_ITER               109 (to 394)
+                     176 STORE_FAST               6 (condition)
+         
+         295         178 LOAD_FAST                2 (df)
+                     180 LOAD_ATTR                4 (loc)
+                     190 LOAD_FAST                2 (df)
+                     192 LOAD_ATTR                5 (condition)
+                     202 LOAD_FAST                6 (condition)
+                     204 COMPARE_OP               2 (==)
+                     210 BINARY_SUBSCR
+                     220 STORE_FAST               7 (df_part)
+         
+         296         222 LOAD_FAST                7 (df_part)
+                     224 LOAD_METHOD              6 (count)
+                     246 PRECALL                  0
+                     250 CALL                     0
+                     260 STORE_FAST               8 (count)
+         
+         299         262 LOAD_FAST                7 (df_part)
+                     264 LOAD_FAST                0 (field_name)
+                     266 BINARY_SUBSCR
+                     276 LOAD_METHOD              7 (to_list)
+                     298 PRECALL                  0
+                     302 CALL                     0
+         
+         301         312 LOAD_GLOBAL             17 (NULL + str)
+                     324 LOAD_FAST                6 (condition)
+                     326 PRECALL                  1
+                     330 CALL                     1
+         
+         302         340 LOAD_CONST               2 ('box')
+         
+         303         342 LOAD_CONST               3 ('Outliers')
+         
+         298         344 LOAD_CONST               4 (('y', 'name', 'type', 'boxpoints'))
+                     346 BUILD_CONST_KEY_MAP      4
+                     348 STORE_FAST               9 (data)
+         
+         305         350 LOAD_FAST                5 (plot_data)
+                     352 LOAD_METHOD              9 (append)
+                     374 LOAD_FAST                9 (data)
+                     376 PRECALL                  1
+                     380 CALL                     1
+                     390 POP_TOP
+                     392 JUMP_BACKWARD          110 (to 174)
+         
+         307     >>  394 LOAD_GLOBAL             21 (NULL + render_template)
+                     406 LOAD_CONST               5 ('results_boxplot.html')
+                     408 LOAD_FAST                0 (field_name)
+                     410 LOAD_FAST                5 (plot_data)
+                     412 KW_NAMES                 6
+                     414 PRECALL                  3
+                     418 CALL                     3
+                     428 RETURN_VALUE
+         consts
+            None
+            'condition'
+            'box'
+            'Outliers'
+            ('y', 'name', 'type', 'boxpoints')
+            'results_boxplot.html'
+            ('field_name', 'plot_data')
+         names      ('calculate_results', 'unique', 'tolist', 'sort', 'loc', 'condition', 'count', 'to_list', 'str', 'append', 'render_template')
+         varnames   ('field_name', 'results', 'df', 'summary_stats', 'unique_conditions', 'plot_data', 'condition', 'df_part', 'count', 'data')
+         freevars   ()
+         cellvars   ()
+         filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
+         name       'route_results_boxplot'
+         firstlineno 285
+         lnotab 0x0203240258012801040208012c01280332021c01020102fb06072c02
       '/preview_questionnaire/<questionnaireName>'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 5
          flags     : 3
          code
@@ -2318,109 +2654,109 @@
             00000000007c04a6010000ab0100000000000000007d047c03a011000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0001006e2b23007424000000000000000000002400721e7d057427000000
             000000000000007c056a140000000000000000a6010000ab010000000000
             0000007d02590064007d057e056e0864007d057e05770177007803590077
             0164057c007a0000007d06742b0000000000000000000064067c047c02ac
             07a6030000ab0300000000000000005300
-         273           0 RESUME                   0
+         309           0 RESUME                   0
          
-         276           2 LOAD_GLOBAL              0 (request)
+         312           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 POP_JUMP_FORWARD_IF_FALSE   172 (to 378)
                       34 LOAD_CONST               2 ('condition')
                       36 LOAD_GLOBAL              0 (request)
                       48 LOAD_ATTR                2 (form)
                       58 CONTAINS_OP              0
                       60 POP_JUMP_FORWARD_IF_FALSE   158 (to 378)
          
-         277          62 LOAD_GLOBAL              7 (NULL + int_or_0)
+         313          62 LOAD_GLOBAL              7 (NULL + int_or_0)
                       74 LOAD_GLOBAL              0 (request)
                       86 LOAD_ATTR                2 (form)
                       96 LOAD_CONST               2 ('condition')
                       98 BINARY_SUBSCR
                      108 PRECALL                  1
                      112 CALL                     1
                      122 LOAD_GLOBAL              8 (session)
                      134 LOAD_CONST               2 ('condition')
                      136 STORE_SUBSCR
          
-         279         140 LOAD_GLOBAL             10 (db)
+         315         140 LOAD_GLOBAL             10 (db)
                      152 LOAD_ATTR                4 (session)
                      162 LOAD_METHOD              6 (query)
                      184 LOAD_GLOBAL             10 (db)
                      196 LOAD_ATTR                7 (Participant)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 LOAD_METHOD              8 (get)
                      242 LOAD_GLOBAL              8 (session)
                      254 LOAD_CONST               3 ('participantID')
                      256 BINARY_SUBSCR
                      266 PRECALL                  1
                      270 CALL                     1
                      280 STORE_FAST               1 (p)
          
-         280         282 LOAD_GLOBAL              8 (session)
+         316         282 LOAD_GLOBAL              8 (session)
                      294 LOAD_CONST               2 ('condition')
                      296 BINARY_SUBSCR
                      306 LOAD_FAST                1 (p)
                      308 STORE_ATTR               9 (condition)
          
-         282         318 LOAD_GLOBAL             10 (db)
+         318         318 LOAD_GLOBAL             10 (db)
                      330 LOAD_ATTR                4 (session)
                      340 LOAD_METHOD             10 (commit)
                      362 PRECALL                  0
                      366 CALL                     0
                      376 POP_TOP
          
-         284     >>  378 BUILD_LIST               0
+         320     >>  378 BUILD_LIST               0
                      380 STORE_FAST               2 (errors)
          
-         286         382 NOP
+         322         382 NOP
          
-         287         384 LOAD_GLOBAL             23 (NULL + open)
+         323         384 LOAD_GLOBAL             23 (NULL + open)
                      396 LOAD_GLOBAL             25 (NULL + current_app)
                      408 LOAD_ATTR               13 (get_questionnaire_path)
                      418 LOAD_FAST                0 (questionnaireName)
                      420 PRECALL                  1
                      424 CALL                     1
                      434 LOAD_CONST               4 ('r')
                      436 PRECALL                  2
                      440 CALL                     2
                      450 STORE_FAST               3 (f)
          
-         288         452 LOAD_FAST                3 (f)
+         324         452 LOAD_FAST                3 (f)
                      454 LOAD_METHOD             14 (read)
                      476 PRECALL                  0
                      480 CALL                     0
                      490 STORE_FAST               4 (json_data)
          
-         289         492 LOAD_GLOBAL             31 (NULL + json)
+         325         492 LOAD_GLOBAL             31 (NULL + json)
                      504 LOAD_ATTR               16 (loads)
                      514 LOAD_FAST                4 (json_data)
                      516 PRECALL                  1
                      520 CALL                     1
                      530 STORE_FAST               4 (json_data)
          
-         290         532 LOAD_FAST                3 (f)
+         326         532 LOAD_FAST                3 (f)
                      534 LOAD_METHOD             17 (close)
                      556 PRECALL                  0
                      560 CALL                     0
                      570 POP_TOP
                      572 JUMP_FORWARD            43 (to 660)
                  >>  574 PUSH_EXC_INFO
          
-         291         576 LOAD_GLOBAL             36 (Exception)
+         327         576 LOAD_GLOBAL             36 (Exception)
                      588 CHECK_EXC_MATCH
                      590 POP_JUMP_FORWARD_IF_FALSE    30 (to 652)
                      592 STORE_FAST               5 (e)
          
-         292         594 LOAD_GLOBAL             39 (NULL + list)
+         328         594 LOAD_GLOBAL             39 (NULL + list)
                      606 LOAD_FAST                5 (e)
                      608 LOAD_ATTR               20 (args)
                      618 PRECALL                  1
                      622 CALL                     1
                      632 STORE_FAST               2 (errors)
                      634 POP_EXCEPT
                      636 LOAD_CONST               0 (None)
@@ -2428,32 +2764,32 @@
                      640 DELETE_FAST              5 (e)
                      642 JUMP_FORWARD             8 (to 660)
                  >>  644 LOAD_CONST               0 (None)
                      646 STORE_FAST               5 (e)
                      648 DELETE_FAST              5 (e)
                      650 RERAISE                  1
          
-         291     >>  652 RERAISE                  0
+         327     >>  652 RERAISE                  0
                  >>  654 COPY                     3
                      656 POP_EXCEPT
                      658 RERAISE                  1
          
-         294     >>  660 LOAD_CONST               5 ('questionnaire_')
+         330     >>  660 LOAD_CONST               5 ('questionnaire_')
                      662 LOAD_FAST                0 (questionnaireName)
                      664 BINARY_OP                0 (+)
                      668 STORE_FAST               6 (table_name)
          
-         296         670 LOAD_GLOBAL             43 (NULL + render_template)
+         332         670 LOAD_GLOBAL             43 (NULL + render_template)
                      682 LOAD_CONST               6 ('preview_questionnaire.html')
          
-         297         684 LOAD_FAST                4 (json_data)
+         333         684 LOAD_FAST                4 (json_data)
          
-         298         686 LOAD_FAST                2 (errors)
+         334         686 LOAD_FAST                2 (errors)
          
-         296         688 KW_NAMES                 7
+         332         688 KW_NAMES                 7
                      690 PRECALL                  3
                      694 CALL                     3
                      704 RETURN_VALUE
          ExceptionTable:
            384 to 570 -> 574 [0]
            574 to 592 -> 654 [1] lasti
            594 to 632 -> 644 [1] lasti
@@ -2469,15 +2805,15 @@
             ('q', 'errors')
          names      ('request', 'method', 'form', 'int_or_0', 'session', 'db', 'query', 'Participant', 'get', 'condition', 'commit', 'open', 'current_app', 'get_questionnaire_path', 'read', 'json', 'loads', 'close', 'Exception', 'list', 'args', 'render_template')
          varnames   ('questionnaireName', 'p', 'errors', 'f', 'json_data', 'e', 'table_name')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_preview_questionnaire'
-         firstlineno 273
+         firstlineno 309
          lnotab
             0x02033c014e028e0124023c02040202014401280128012c0112013aff08
             030a020e01020102fe
       '/questionnaire_html/<questionnaireName>'
       code
          argcount  : 1
          nlocals   : 5
@@ -2491,59 +2827,59 @@
             0000000000000000006a0500000000000000007c03a6010000ab01000000
             00000000007d037c02a00600000000000000000000000000000000000000
             00a6000000ab00000000000000000001006e2b2300740e00000000000000
             0000002400721e7d047411000000000000000000007c046a090000000000
             000000a6010000ab0100000000000000007d01590064007d047e046e0864
             007d047e047701770078035900770174150000000000000000000064027c
             03ac03a6020000ab0200000000000000005300
-         301           0 RESUME                   0
+         337           0 RESUME                   0
          
-         304           2 BUILD_LIST               0
+         340           2 BUILD_LIST               0
                        4 STORE_FAST               1 (errors)
          
-         306           6 NOP
+         342           6 NOP
          
-         307           8 LOAD_GLOBAL              1 (NULL + open)
+         343           8 LOAD_GLOBAL              1 (NULL + open)
                       20 LOAD_GLOBAL              3 (NULL + current_app)
                       32 LOAD_ATTR                2 (get_questionnaire_path)
                       42 LOAD_FAST                0 (questionnaireName)
                       44 PRECALL                  1
                       48 CALL                     1
                       58 LOAD_CONST               1 ('r')
                       60 PRECALL                  2
                       64 CALL                     2
                       74 STORE_FAST               2 (f)
          
-         308          76 LOAD_FAST                2 (f)
+         344          76 LOAD_FAST                2 (f)
                       78 LOAD_METHOD              3 (read)
                      100 PRECALL                  0
                      104 CALL                     0
                      114 STORE_FAST               3 (json_data)
          
-         309         116 LOAD_GLOBAL              9 (NULL + json)
+         345         116 LOAD_GLOBAL              9 (NULL + json)
                      128 LOAD_ATTR                5 (loads)
                      138 LOAD_FAST                3 (json_data)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               3 (json_data)
          
-         310         156 LOAD_FAST                2 (f)
+         346         156 LOAD_FAST                2 (f)
                      158 LOAD_METHOD              6 (close)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_TOP
                      196 JUMP_FORWARD            43 (to 284)
                  >>  198 PUSH_EXC_INFO
          
-         311         200 LOAD_GLOBAL             14 (Exception)
+         347         200 LOAD_GLOBAL             14 (Exception)
                      212 CHECK_EXC_MATCH
                      214 POP_JUMP_FORWARD_IF_FALSE    30 (to 276)
                      216 STORE_FAST               4 (e)
          
-         312         218 LOAD_GLOBAL             17 (NULL + list)
+         348         218 LOAD_GLOBAL             17 (NULL + list)
                      230 LOAD_FAST                4 (e)
                      232 LOAD_ATTR                9 (args)
                      242 PRECALL                  1
                      246 CALL                     1
                      256 STORE_FAST               1 (errors)
                      258 POP_EXCEPT
                      260 LOAD_CONST               0 (None)
@@ -2551,20 +2887,20 @@
                      264 DELETE_FAST              4 (e)
                      266 JUMP_FORWARD             8 (to 284)
                  >>  268 LOAD_CONST               0 (None)
                      270 STORE_FAST               4 (e)
                      272 DELETE_FAST              4 (e)
                      274 RERAISE                  1
          
-         311     >>  276 RERAISE                  0
+         347     >>  276 RERAISE                  0
                  >>  278 COPY                     3
                      280 POP_EXCEPT
                      282 RERAISE                  1
          
-         314     >>  284 LOAD_GLOBAL             21 (NULL + render_template)
+         350     >>  284 LOAD_GLOBAL             21 (NULL + render_template)
                      296 LOAD_CONST               2 ('preview_questionnaire_simple.html')
                      298 LOAD_FAST                3 (json_data)
                      300 KW_NAMES                 3
                      302 PRECALL                  2
                      306 CALL                     2
                      316 RETURN_VALUE
          ExceptionTable:
@@ -2579,15 +2915,15 @@
             ('q',)
          names      ('open', 'current_app', 'get_questionnaire_path', 'read', 'json', 'loads', 'close', 'Exception', 'list', 'args', 'render_template')
          varnames   ('questionnaireName', 'errors', 'f', 'json_data', 'e')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_questionnaire_html'
-         firstlineno 301
+         firstlineno 337
          lnotab 0x0203040202014401280128012c0112013aff0803
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 4
          flags     : 3
          code
@@ -2602,86 +2938,86 @@
             00000000007d047c04a00900000000000000000000000000000000000000
             006401a6010000ab01000000000000000073157c04a00900000000000000
             000000000000000000000000006402a6010000ab01000000000000000072
             0264037d047c036a0a00000000000000007c04a00b000000000000000000
             0000000000000000000000a6000000ab00000000000000000064049c027d
             057c02a00c00000000000000000000000000000000000000007c05a60100
             00ab01000000000000000001008c747c027c0166025300
-         352           0 RESUME                   0
+         388           0 RESUME                   0
          
-         353           2 LOAD_GLOBAL              0 (db)
+         389           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
                       46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (metadata)
                       68 LOAD_ATTR                4 (tables)
                       78 LOAD_FAST                0 (tableName)
                       80 BINARY_SUBSCR
                       90 PRECALL                  1
                       94 CALL                     1
                      104 LOAD_METHOD              5 (all)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 STORE_FAST               1 (rows)
          
-         355         142 BUILD_LIST               0
+         391         142 BUILD_LIST               0
                      144 STORE_FAST               2 (columns)
          
-         357         146 LOAD_GLOBAL              0 (db)
+         393         146 LOAD_GLOBAL              0 (db)
                      158 LOAD_ATTR                3 (metadata)
                      168 LOAD_ATTR                4 (tables)
                      178 LOAD_FAST                0 (tableName)
                      180 BINARY_SUBSCR
                      190 LOAD_ATTR                6 (columns)
                      200 GET_ITER
                  >>  202 FOR_ITER               115 (to 434)
                      204 STORE_FAST               3 (c)
          
-         358         206 LOAD_GLOBAL             15 (NULL + str)
+         394         206 LOAD_GLOBAL             15 (NULL + str)
                      218 LOAD_FAST                3 (c)
                      220 LOAD_ATTR                8 (type)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 STORE_FAST               4 (type)
          
-         359         246 LOAD_FAST                4 (type)
+         395         246 LOAD_FAST                4 (type)
                      248 LOAD_METHOD              9 (startswith)
                      270 LOAD_CONST               1 ('VARCHAR')
                      272 PRECALL                  1
                      276 CALL                     1
                      286 POP_JUMP_FORWARD_IF_TRUE    21 (to 330)
                      288 LOAD_FAST                4 (type)
                      290 LOAD_METHOD              9 (startswith)
                      312 LOAD_CONST               2 ('TEXT')
                      314 PRECALL                  1
                      318 CALL                     1
                      328 POP_JUMP_FORWARD_IF_FALSE     2 (to 334)
          
-         360     >>  330 LOAD_CONST               3 ('string')
+         396     >>  330 LOAD_CONST               3 ('string')
                      332 STORE_FAST               4 (type)
          
-         362     >>  334 LOAD_FAST                3 (c)
+         398     >>  334 LOAD_FAST                3 (c)
                      336 LOAD_ATTR               10 (description)
                      346 LOAD_FAST                4 (type)
                      348 LOAD_METHOD             11 (lower)
                      370 PRECALL                  0
                      374 CALL                     0
                      384 LOAD_CONST               4 (('name', 'type'))
                      386 BUILD_CONST_KEY_MAP      2
                      388 STORE_FAST               5 (column)
          
-         364         390 LOAD_FAST                2 (columns)
+         400         390 LOAD_FAST                2 (columns)
                      392 LOAD_METHOD             12 (append)
                      414 LOAD_FAST                5 (column)
                      416 PRECALL                  1
                      420 CALL                     1
                      430 POP_TOP
                      432 JUMP_BACKWARD          116 (to 202)
          
-         366     >>  434 LOAD_FAST                2 (columns)
+         402     >>  434 LOAD_FAST                2 (columns)
                      436 LOAD_FAST                1 (rows)
                      438 BUILD_TUPLE              2
                      440 RETURN_VALUE
          consts
             None
             'VARCHAR'
             'TEXT'
@@ -2689,37 +3025,37 @@
             ('name', 'type')
          names      ('db', 'session', 'query', 'metadata', 'tables', 'all', 'columns', 'str', 'type', 'startswith', 'description', 'lower', 'append')
          varnames   ('tableName', 'rows', 'columns', 'c', 'type', 'column')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'table_data'
-         firstlineno 352
+         firstlineno 388
          lnotab 0x02018c0204023c0128015401040238022c02
       '/table_view/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c007c027c01ac
             02a6040000ab0400000000000000005300
-         369           0 RESUME                   0
+         405           0 RESUME                   0
          
-         372           2 LOAD_GLOBAL              1 (NULL + table_data)
+         408           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         373          38 LOAD_GLOBAL              3 (NULL + render_template)
+         409          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_view.html')
                       52 LOAD_FAST                0 (tableName)
                       54 LOAD_FAST                2 (rows)
                       56 LOAD_FAST                1 (columns)
                       58 KW_NAMES                 2
                       60 PRECALL                  4
                       64 CALL                     4
@@ -2730,37 +3066,37 @@
             ('tableName', 'rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_view'
-         firstlineno 369
+         firstlineno 405
          lnotab 0x02032401
       '/table_ajax/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c027c01ac02a6
             030000ab0300000000000000005300
-         376           0 RESUME                   0
+         412           0 RESUME                   0
          
-         379           2 LOAD_GLOBAL              1 (NULL + table_data)
+         415           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         380          38 LOAD_GLOBAL              3 (NULL + render_template)
+         416          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_ajax.html')
                       52 LOAD_FAST                2 (rows)
                       54 LOAD_FAST                1 (columns)
                       56 KW_NAMES                 2
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -2770,15 +3106,15 @@
             ('rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_ajax'
-         firstlineno 376
+         firstlineno 412
          lnotab 0x02032401
       '/table_csv/<tableName>'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
@@ -2794,57 +3130,57 @@
             0000000000000000007c036406640764087c0064097a0000007409000000
             000000000000006a050000000000000000a6000000ab0000000000000000
             00a0060000000000000000000000000000000000000000640aa6010000ab
             0100000000000000007a0000007a0600006901ac0ba6030000ab03000000
             00000000005300
                        0 MAKE_CELL                5 (row)
          
-         383           2 RESUME                   0
+         419           2 RESUME                   0
          
-         386           4 LOAD_GLOBAL              1 (NULL + table_data)
+         422           4 LOAD_GLOBAL              1 (NULL + table_data)
                       16 LOAD_FAST                0 (tableName)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 UNPACK_SEQUENCE          2
                       36 STORE_FAST               1 (columns)
                       38 STORE_FAST               2 (rows)
          
-         388          40 LOAD_CONST               1 ('')
+         424          40 LOAD_CONST               1 ('')
                       42 STORE_FAST               3 (csv)
          
-         389          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 389>)
+         425          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 425>)
                       46 MAKE_FUNCTION            0
                       48 LOAD_FAST                1 (columns)
                       50 GET_ITER
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               4 (headers)
          
-         390          68 LOAD_FAST                3 (csv)
+         426          68 LOAD_FAST                3 (csv)
                       70 LOAD_CONST               3 (',')
                       72 LOAD_METHOD              1 (join)
                       94 LOAD_FAST                4 (headers)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               4 ('\n')
                      112 BINARY_OP                0 (+)
                      116 BINARY_OP               13 (+=)
                      120 STORE_FAST               3 (csv)
          
-         392         122 LOAD_FAST                2 (rows)
+         428         122 LOAD_FAST                2 (rows)
                      124 GET_ITER
                  >>  126 FOR_ITER                54 (to 236)
                      128 STORE_DEREF              5 (row)
          
-         393         130 LOAD_FAST                3 (csv)
+         429         130 LOAD_FAST                3 (csv)
                      132 LOAD_CONST               3 (',')
                      134 LOAD_METHOD              1 (join)
                      156 LOAD_CLOSURE             5 (row)
                      158 BUILD_TUPLE              1
-                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 393>)
+                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 429>)
                      162 MAKE_FUNCTION            8 (closure)
                      164 LOAD_GLOBAL              5 (NULL + enumerate)
                      176 LOAD_FAST                1 (columns)
                      178 PRECALL                  1
                      182 CALL                     1
                      192 GET_ITER
                      194 PRECALL                  0
@@ -2853,55 +3189,55 @@
                      212 CALL                     1
                      222 LOAD_CONST               4 ('\n')
                      224 BINARY_OP                0 (+)
                      228 BINARY_OP               13 (+=)
                      232 STORE_FAST               3 (csv)
                      234 JUMP_BACKWARD           55 (to 126)
          
-         395     >>  236 LOAD_GLOBAL              7 (NULL + Response)
+         431     >>  236 LOAD_GLOBAL              7 (NULL + Response)
                      248 LOAD_FAST                3 (csv)
          
-         396         250 LOAD_CONST               6 ('text/csv')
+         432         250 LOAD_CONST               6 ('text/csv')
          
-         398         252 LOAD_CONST               7 ('Content-disposition')
+         434         252 LOAD_CONST               7 ('Content-disposition')
                      254 LOAD_CONST               8 ('attachment; filename=%s.csv')
          
-         399         256 LOAD_FAST                0 (tableName)
+         435         256 LOAD_FAST                0 (tableName)
                      258 LOAD_CONST               9 ('_')
                      260 BINARY_OP                0 (+)
                      264 LOAD_GLOBAL              9 (NULL + datetime)
                      276 LOAD_ATTR                5 (utcnow)
                      286 PRECALL                  0
                      290 CALL                     0
                      300 LOAD_METHOD              6 (strftime)
                      322 LOAD_CONST              10 ('%Y-%m-%d')
                      324 PRECALL                  1
                      328 CALL                     1
                      338 BINARY_OP                0 (+)
          
-         398         342 BINARY_OP                6 (%)
+         434         342 BINARY_OP                6 (%)
          
-         397         346 BUILD_MAP                1
+         433         346 BUILD_MAP                1
          
-         395         348 KW_NAMES                11
+         431         348 KW_NAMES                11
                      350 PRECALL                  3
                      354 CALL                     3
                      364 RETURN_VALUE
          consts
             None
             ''
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                   00
-               389           0 RESUME                   0
+               425           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                10 (to 28)
                              8 STORE_FAST               1 (c)
                             10 LOAD_FAST                1 (c)
                             12 LOAD_CONST               0 ('name')
                             14 BINARY_SUBSCR
@@ -2912,30 +3248,30 @@
                   'name'
                names      ()
                varnames   ('.0', 'c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 389
+               firstlineno 425
                lnotab 0x
             ','
             '\n'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d1a5c0200007d017d027401000000000000000000
                   0089037c0119000000000000000000a6010000ab01000000000000000091
                   028c1b5300
                              0 COPY_FREE_VARS           1
                
-               393           2 RESUME                   0
+               429           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                26 (to 62)
                             10 UNPACK_SEQUENCE          2
                             14 STORE_FAST               1 (i)
                             16 STORE_FAST               2 (c)
                             18 LOAD_GLOBAL              1 (NULL + escape_csv)
@@ -2950,29 +3286,29 @@
                consts
                names      ('escape_csv',)
                varnames   ('.0', 'i', 'c')
                freevars   ('row',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 393
+               firstlineno 429
                lnotab 0x
             'text/csv'
             'Content-disposition'
             'attachment; filename=%s.csv'
             '_'
             '%Y-%m-%d'
             ('mimetype', 'headers')
          names      ('table_data', 'join', 'enumerate', 'Response', 'datetime', 'utcnow', 'strftime')
          varnames   ('tableName', 'columns', 'rows', 'csv', 'headers')
          freevars   ()
          cellvars   ('row',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_csv'
-         firstlineno 383
+         firstlineno 419
          lnotab 0x0403240204011801360208016a020e010202040156ff04ff02fe
       '/database_download'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
@@ -2980,41 +3316,41 @@
             0x97007400000000000000000000006a0100000000000000006401190000
             00000000000000a002000000000000000000000000000000000000000064
             02a6010000ab010000000000000000730264035300740000000000000000
             0000006a010000000000000000640119000000000000000000a003000000
             000000000000000000000000000000000064026404a6020000ab02000000
             00000000007d007409000000000000000000007c006405ac06a6020000ab
             0200000000000000005300
-         403           0 RESUME                   0
+         439           0 RESUME                   0
          
-         406           2 LOAD_GLOBAL              0 (current_app)
+         442           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (config)
                       24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                       26 BINARY_SUBSCR
                       36 LOAD_METHOD              2 (startswith)
                       58 LOAD_CONST               2 ('sqlite:///')
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
          
-         407          76 LOAD_CONST               3 ('Not using a SQLite database.')
+         443          76 LOAD_CONST               3 ('Not using a SQLite database.')
                       78 RETURN_VALUE
          
-         409     >>   80 LOAD_GLOBAL              0 (current_app)
+         445     >>   80 LOAD_GLOBAL              0 (current_app)
                       92 LOAD_ATTR                1 (config)
                      102 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                      104 BINARY_SUBSCR
                      114 LOAD_METHOD              3 (replace)
                      136 LOAD_CONST               2 ('sqlite:///')
                      138 LOAD_CONST               4 ('')
                      140 PRECALL                  2
                      144 CALL                     2
                      154 STORE_FAST               0 (db_uri)
          
-         411         156 LOAD_GLOBAL              9 (NULL + send_file)
+         447         156 LOAD_GLOBAL              9 (NULL + send_file)
                      168 LOAD_FAST                0 (db_uri)
                      170 LOAD_CONST               5 (True)
                      172 KW_NAMES                 6
                      174 PRECALL                  2
                      178 CALL                     2
                      188 RETURN_VALUE
          consts
@@ -3027,15 +3363,15 @@
             ('as_attachment',)
          names      ('current_app', 'config', 'startswith', 'replace', 'send_file')
          varnames   ('db_uri',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_database_download'
-         firstlineno 403
+         firstlineno 439
          lnotab 0x02034a0104024c02
       '/database_delete'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 7
          flags     : 3
@@ -3062,67 +3398,67 @@
             007c01a6010000ab010000000000000000a0120000000000000000000000
             000000000000000000a6000000ab00000000000000000001008c34741a00
             0000000000000000006a100000000000000000a013000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100742900
             000000000000000000742b00000000000000000000640ea6010000ab0100
             00000000000000a6010000ab0100000000000000005300740d0000000000
             00000000006407a6010000ab0100000000000000005300
-         414           0 RESUME                   0
+         450           0 RESUME                   0
          
-         417           2 LOAD_GLOBAL              0 (current_app)
+         453           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (config)
                       24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                       26 BINARY_SUBSCR
                       36 LOAD_METHOD              2 (startswith)
                       58 LOAD_CONST               2 ('sqlite:///')
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
          
-         418          76 LOAD_CONST               3 ('Not using a SQLite database.')
+         454          76 LOAD_CONST               3 ('Not using a SQLite database.')
                       78 RETURN_VALUE
          
-         420     >>   80 LOAD_GLOBAL              6 (request)
+         456     >>   80 LOAD_GLOBAL              6 (request)
                       92 LOAD_ATTR                4 (method)
                      102 LOAD_CONST               4 ('POST')
                      104 COMPARE_OP               2 (==)
                      110 EXTENDED_ARG             1
                      112 POP_JUMP_FORWARD_IF_FALSE   314 (to 742)
          
-         421         114 LOAD_GLOBAL              6 (request)
+         457         114 LOAD_GLOBAL              6 (request)
                      126 LOAD_ATTR                5 (form)
                      136 LOAD_CONST               5 ('password')
                      138 BINARY_SUBSCR
                      148 LOAD_GLOBAL              0 (current_app)
                      160 LOAD_ATTR                1 (config)
                      170 LOAD_CONST               6 ('ADMIN_PASSWORD')
                      172 BINARY_SUBSCR
                      182 COMPARE_OP               3 (!=)
                      188 POP_JUMP_FORWARD_IF_FALSE    17 (to 224)
          
-         422         190 LOAD_GLOBAL             13 (NULL + render_template)
+         458         190 LOAD_GLOBAL             13 (NULL + render_template)
                      202 LOAD_CONST               7 ('database_delete.html')
                      204 LOAD_CONST               8 ('The password you entered is incorrect.')
                      206 KW_NAMES                 9
                      208 PRECALL                  2
                      212 CALL                     2
                      222 RETURN_VALUE
          
-         424     >>  224 LOAD_GLOBAL              0 (current_app)
+         460     >>  224 LOAD_GLOBAL              0 (current_app)
                      236 LOAD_ATTR                1 (config)
                      246 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                      248 BINARY_SUBSCR
                      258 LOAD_METHOD              7 (replace)
                      280 LOAD_CONST               2 ('sqlite:///')
                      282 LOAD_CONST              10 ('')
                      284 PRECALL                  2
                      288 CALL                     2
                      298 STORE_FAST               0 (db_uri)
          
-         425         300 LOAD_GLOBAL             17 (NULL + copyfile)
+         461         300 LOAD_GLOBAL             17 (NULL + copyfile)
                      312 LOAD_FAST                0 (db_uri)
                      314 LOAD_FAST                0 (db_uri)
                      316 LOAD_METHOD              7 (replace)
                      338 LOAD_CONST              11 ('.db')
                      340 LOAD_CONST              10 ('')
                      342 PRECALL                  2
                      346 CALL                     2
@@ -3139,53 +3475,53 @@
                      436 BINARY_OP                0 (+)
                      440 LOAD_CONST              11 ('.db')
                      442 BINARY_OP                0 (+)
                      446 PRECALL                  2
                      450 CALL                     2
                      460 POP_TOP
          
-         428         462 LOAD_GLOBAL             25 (NULL + reversed)
+         464         462 LOAD_GLOBAL             25 (NULL + reversed)
                      474 LOAD_GLOBAL             26 (db)
                      486 LOAD_ATTR               14 (metadata)
                      496 LOAD_ATTR               15 (sorted_tables)
                      506 PRECALL                  1
                      510 CALL                     1
                      520 GET_ITER
                  >>  522 FOR_ITER                51 (to 626)
                      524 STORE_FAST               1 (tbl)
          
-         429         526 LOAD_GLOBAL             26 (db)
+         465         526 LOAD_GLOBAL             26 (db)
                      538 LOAD_ATTR               16 (session)
                      548 LOAD_METHOD             17 (query)
                      570 LOAD_FAST                1 (tbl)
                      572 PRECALL                  1
                      576 CALL                     1
                      586 LOAD_METHOD             18 (delete)
                      608 PRECALL                  0
                      612 CALL                     0
                      622 POP_TOP
                      624 JUMP_BACKWARD           52 (to 522)
          
-         430     >>  626 LOAD_GLOBAL             26 (db)
+         466     >>  626 LOAD_GLOBAL             26 (db)
                      638 LOAD_ATTR               16 (session)
                      648 LOAD_METHOD             19 (commit)
                      670 PRECALL                  0
                      674 CALL                     0
                      684 POP_TOP
          
-         432         686 LOAD_GLOBAL             41 (NULL + redirect)
+         468         686 LOAD_GLOBAL             41 (NULL + redirect)
                      698 LOAD_GLOBAL             43 (NULL + url_for)
                      710 LOAD_CONST              14 ('admin.route_progress')
                      712 PRECALL                  1
                      716 CALL                     1
                      726 PRECALL                  1
                      730 CALL                     1
                      740 RETURN_VALUE
          
-         434     >>  742 LOAD_GLOBAL             13 (NULL + render_template)
+         470     >>  742 LOAD_GLOBAL             13 (NULL + render_template)
                      754 LOAD_CONST               7 ('database_delete.html')
                      756 PRECALL                  1
                      760 CALL                     1
                      770 RETURN_VALUE
          consts
             None
             'SQLALCHEMY_DATABASE_URI'
@@ -3204,25 +3540,26 @@
             'admin.route_progress'
          names      ('current_app', 'config', 'startswith', 'request', 'method', 'form', 'render_template', 'replace', 'copyfile', 'datetime', 'utcnow', 'strftime', 'reversed', 'db', 'metadata', 'sorted_tables', 'session', 'query', 'delete', 'commit', 'redirect', 'url_for')
          varnames   ('db_uri', 'tbl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_database_delete'
-         firstlineno 414
+         firstlineno 450
          lnotab 0x02034a01040222014c0122024c01a203400164013c023802
-   names      ('sqlalchemy', 'flask', 'Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file', 'BOFS.globals', 'db', 'questionnaires', 'page_list', 'BOFS.util', 'fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0', 'util', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'export_helpers', 'json', 'QuestionnaireResults', 'datetime', 'os', 'path', 'listdir', 'shutil', 'copyfile', '__name__', 'admin', 'context_processor', 'inject_template_vars', 'route', 'admin_index', 'admin_login', 'fetch_progress', 'fetch_progress_summary', 'route_progress', 'route_progress_ajax', 'route_progress_summary_ajax', 'post', 'route_update_exclude_from_count', 'route_export_item_timing', 'route_export', 'route_results', 'route_preview_questionnaire', 'route_questionnaire_html', 'table_data', 'route_table_view', 'route_table_ajax', 'route_table_csv', 'route_database_download', 'route_database_delete')
+   names      ('os', 'pandas', 'pd', 'flask', 'Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file', 'BOFS.globals', 'db', 'questionnaires', 'page_list', 'BOFS.util', 'fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0', 'util', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'Results', 'json', 'SummaryStats', 'datetime', 'path', 'listdir', 'shutil', 'copyfile', '__name__', 'admin', 'context_processor', 'inject_template_vars', 'route', 'admin_index', 'admin_login', 'fetch_progress', 'fetch_progress_summary', 'route_progress', 'route_progress_ajax', 'route_progress_summary_ajax', 'post', 'route_update_exclude_from_count', 'route_export_item_timing', 'route_export', 'tuple', 'DataFrame', 'dict', 'str', 'calculate_results', 'route_results', 'route_results_boxplot', 'route_preview_questionnaire', 'route_questionnaire_html', 'table_data', 'route_table_view', 'route_table_ajax', 'route_table_csv', 'route_database_download', 'route_database_delete')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108013001140118011c010801080108010c0110010c0220030c
-      0104ff0e01022a280104ff0e010204300104ff0e01021d06160619280102
-      0104ff0eff0e0202092801020104ff0eff0e0202052801020104ff0eff0e
-      020205280104ff0e01020a2801020104ff0eff0e02022728012c01020104
-      ff0eff0eff0e0302222801020104ff0eff0e0202103001020104ff0eff0e
-      02021a2801020104ff0eff0e02023106112801020104ff0eff0e02020528
-      01020104ff0eff0e0202052801020104ff0eff0e0202122801020104ff0e
-      ff0e0202093001020104ff0eff0e02
+      0x00ff0201080108013001140118011c010c0108010c010c0110010c0220
+      030c0104ff0e01022a280104ff0e010204300104ff0e01021d0616061928
+      01020104ff0eff0e0202092801020104ff0eff0e0202052801020104ff0e
+      ff0e020205280104ff0e01020a2801020104ff0eff0e02022728012c0102
+      0104ff0eff0eff0e03022738112801020104ff0eff0e020205280102010a
+      ff0eff0e0202163001020104ff0eff0e02021a2801020104ff0eff0e0202
+      3106112801020104ff0eff0e0202052801020104ff0eff0e020205280102
+      0104ff0eff0e0202122801020104ff0eff0e0202093001020104ff0eff0e
+      02
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/export_helpers.py` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/Results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,253 +1,286 @@
+from sqlalchemy.orm import Query
 from BOFS.globals import db, questionnaires, page_list
 import sqlalchemy
 from .util import escape_csv, questionnaire_name_and_tag, condition_num_to_label
 from flask  import current_app
+import pandas as pd
+import os
+from datetime import datetime
+
+MAX_CACHE_SECONDS = 60 * 2
+
+
+class Results(object):
+    def __init__(self, filter_criterion=None, cache_path: str | None =None):
+        self.cache_path = cache_path
+        use_cache = False
+
+        if cache_path is not None:
+            if os.path.exists(cache_path):
+                modified_time = datetime.utcfromtimestamp(os.path.getmtime(cache_path))
+                if (datetime.utcnow() - modified_time).total_seconds() < MAX_CACHE_SECONDS:
+                    use_cache = True
+
+        self.df = None
+        self.column_list = []
+        self.export_data: dict[dict] | dict = {}
+        self.query_participants: Query
+        self.query_filter_criterion = filter_criterion
 
+        if use_cache:
+            self.load_data_frame()
+        else:
+            self.handle_participants_table()
+            self.handle_questionnaires()
+            self.handle_custom_exports()
+
+    def handle_participants_table(self) -> None:
+        """
+        Add participant columns to column_list and their data to export_data.
+        :param column_list: A list of strings that will be the columns in the CSV export.
+        :param export_data: Gets updated with data for the participants
+        :return: A SQLAlchemy query.
+        """
+        self.query_participants = db.session.query(db.Participant)
+
+        if self.query_filter_criterion is not None:
+            self.query_participants = self.query_participants.filter(self.query_filter_criterion)
+
+        self.column_list.extend([
+            "participantID",
+            "externalID",
+            "condition",
+            "duration",
+            "finished"
+        ])
+
+        query_result = self.query_participants.all()
+
+        for row in query_result:
+            self.export_data[row.participantID] = {
+                'participantID': row.participantID,
+                'externalID': row.mTurkID,
+                'condition': condition_num_to_label(row.condition),
+                'duration': row.duration,
+                'finished': row.finished
+            }
+
+    def handle_questionnaires(self) -> None:
+        list_of_questionnaires = page_list.get_questionnaire_list(include_tags=True)
+
+        query_questionnaires = self.query_participants
+        q_columns = {}
+        q_calculated_columns = {}
+
+        # First loop constructs the query and fetches the column names
+        for entry in list_of_questionnaires:
+            q_columns[entry] = []
+            q_calculated_columns[entry] = []
+            questionnaire_name, questionnaire_tag = questionnaire_name_and_tag(entry)
+
+            # The python class that describes the questionnaire
+            questionnaire = questionnaires[questionnaire_name]
+
+            # Add the questionnaire's table/class to the query...
+            questionnaire_db_class = db.aliased(questionnaire.db_class, name=entry)
+            join_condition = db.and_(questionnaire_db_class.participantID == db.Participant.participantID,
+                                     questionnaire_db_class.tag == questionnaire_tag
+                                     )
+
+            query_questionnaires = query_questionnaires.outerjoin(questionnaire_db_class, join_condition). \
+                add_entity(questionnaire_db_class)
+
+            # Make a list of the columns to later construct the CSV header row
+            # This could also be done with questionnaire.fields
+            for column in questionnaire.fetch_fields():
+                self.column_list.append(entry + "_" + column.id)
+                q_columns[entry].append(column.id)
+
+            # Similarly, make a list of calculated columns to later be part of the CSV header row.
+            for column in questionnaire.get_calculated_fields():
+                self.column_list.append(entry + "_" + column)
+                q_calculated_columns[entry].append(column)
+
+            # Duration always gets added
+            self.column_list.append(entry + "_duration")
+
+        query_result = query_questionnaires.all()
+
+        # Now we get the actual data
+        for row in query_result:
+            for entry in list_of_questionnaires:  # Need to look through the questionnaires again
+                questionnaire_data = getattr(row, entry)
+
+                if questionnaire_data:
+                    # Regular columns first
+                    for col in q_columns[entry]:
+                        self.export_data[row.Participant.participantID][entry + "_" + col] = (
+                            getattr(questionnaire_data, col))
+
+                    # Now calculated columns
+                    for col in q_calculated_columns[entry]:
+                        if questionnaire_data:
+                            self.export_data[row.Participant.participantID][entry + "_" + col] = (
+                                getattr(questionnaire_data, col)())
+
+                    # Duration always gets added
+                    self.export_data[row.Participant.participantID][entry + "_duration"] = questionnaire_data.duration()
+
+    def handle_custom_exports(self) -> None:
+        # Repeated measures in other tables...
+        custom_exports = []
+
+        for export in current_app.config['EXPORT']:
+            levels, fields, base_query = self.create_export_base_query(export)
+            custom_exports.append({'options': export, 'fields': fields, 'base_query': base_query, 'levels': levels})
+
+        # For custom exports, add columns based on levels determined by prior query
+        for export in custom_exports:
+            if export['levels']:
+                for level in export['levels']:
+                    for field in export['options']['fields']:
+                        column_header = str.format("{}", field)
+                        for level_name in level:
+                            column_header += str.format("_{}", str(level_name).replace(" ", "_"))
+                        self.column_list.append(column_header)
+            else:
+                for field in export['options']['fields']:
+                    self.column_list.append(str.format(u"{}", field))
+
+        query_result = self.query_participants.all()
+
+        # Now we get the actual data
+        for row in query_result:
+            participant_id = row.participantID
+
+            for export in custom_exports:
+                query = export['base_query']
+                query = query.filter(db.literal_column('participantID') == row.participantID)
+                custom_export_data = query.all()  # Running separate queries will get the job done, but be kind of slow with many participants...
+
+                export_row_index = 0
+                for custom_export_row in custom_export_data:
+                    for field in export['fields']:
+                        export_column_name = field
+                        if export['levels']:
+                            export_column_name = field + "_" + str(export['levels'][export_row_index][0])
+
+                        self.export_data[participant_id][export_column_name] = getattr(custom_export_row, field)
+
+                    export_row_index += 1
+
+    def create_export_base_query(self, export_definition: dict) -> tuple[list, list, "Query"]:
+        """
+        Builds the base query for exporting values in blueprint-defined tables.
+        To be used for each entry in the config's EXPORT
+        :param export_definition:
+        :return: levels, fields, baseQuery
+        """
+        table = getattr(db, export_definition['table'])
+
+        levels = None
+        fields = []
+        filter = None
+        groupBy = None
+        orderBy = None
+        having = None
+
+        if 'filter' in export_definition and export_definition['filter'] != '':
+            filter = db.text(export_definition['filter'])
+
+        if 'order_by' in export_definition and export_definition['order_by'] != '':
+            orderBy = getattr(table, export_definition['order_by'])
+
+        # determine how many columns to add to the export. If group_by is not used, then it's just one column
+        if 'group_by' in export_definition and export_definition['group_by'] != '':
+            if 'having' in export_definition and export_definition['having'] != '':  # Having can only work if group_by is used.
+                having = db.text(export_definition['having'])
+
+            levelsQ = db.session.query()
+
+            if isinstance(export_definition['group_by'], list):
+                groupBy = []
+                for gb in export_definition['group_by']:
+                    groupBy.append(getattr(table, gb))
+                    levelsQ = levelsQ.add_columns(getattr(table, gb))
+                    levelsQ = levelsQ.group_by(getattr(table, gb))
+            else:
+                groupBy = getattr(table, export_definition['group_by'])
+                levelsQ = levelsQ.add_columns(groupBy)
+                levelsQ = levelsQ.group_by(groupBy)
+
+            if orderBy:
+                levelsQ = levelsQ.order_by(orderBy)
+
+            if filter is not None:
+                levels = levelsQ.filter(filter).all()
+            else:
+                levels = levelsQ.all()
+
+        # pk = db.inspect(table).primary_key[0]
+        baseQuery = db.session.query(table)
 
-def create_export_base_query(export_dict: dict):
-    """
-    Builds the base query for exporting values in blueprint-defined tables.
-    To be used for each entry in the config's EXPORT
-    :param export_dict:
-    :return:
-    """
-    table = getattr(db, export_dict['table'])
-
-    levels = None
-    fields = []
-    filter = None
-    groupBy = None
-    orderBy = None
-    having = None
-
-    if 'filter' in export_dict and export_dict['filter'] != '':
-        filter = db.text(export_dict['filter'])
-
-    if 'order_by' in export_dict and export_dict['order_by'] != '':
-        orderBy = getattr(table, export_dict['order_by'])
-
-    # determine how many columns to add to the export. If group_by is not used, then it's just one column
-    if 'group_by' in export_dict and export_dict['group_by'] != '':
-        if 'having' in export_dict and export_dict['having'] != '':  # Having can only work if group_by is used.
-            having = db.text(export_dict['having'])
-
-        levelsQ = db.session.query()
-
-        if isinstance(export_dict['group_by'], list):
-            groupBy = []
-            for gb in export_dict['group_by']:
-                groupBy.append(getattr(table, gb))
-                levelsQ = levelsQ.add_columns(getattr(table, gb))
-                levelsQ = levelsQ.group_by(getattr(table, gb))
+        if groupBy:
+            if isinstance(groupBy, list):
+                for gb in groupBy:
+                    baseQuery = baseQuery.group_by(getattr(table, 'participantID'), gb)
+            else:
+                baseQuery = baseQuery.group_by(getattr(table, 'participantID'), groupBy)
+
+            if having is not None:
+                baseQuery = baseQuery.having(having)
         else:
-            groupBy = getattr(table, export_dict['group_by'])
-            levelsQ = levelsQ.add_columns(groupBy)
-            levelsQ = levelsQ.group_by(groupBy)
+            baseQuery = baseQuery.group_by(getattr(table, 'participantID'))
 
         if orderBy:
-            levelsQ = levelsQ.order_by(orderBy)
+            baseQuery = baseQuery.order_by(orderBy)
 
         if filter is not None:
-            levels = levelsQ.filter(filter).all()
-        else:
-            levels = levelsQ.all()
+            baseQuery = baseQuery.filter(filter)
 
-    # pk = db.inspect(table).primary_key[0]
-    baseQuery = db.session.query(table)
+        # Add the fields to the basequery
+        for field in export_definition['fields']:
+            if hasattr(table, field) and callable(getattr(table, field)):
+                continue  # We can't include this python property as part of the query
+            fields.append(field)
+            baseQuery = baseQuery.add_columns(db.literal_column(export_definition['fields'][field]).label(field))
 
-    if groupBy:
-        if isinstance(groupBy, list):
-            for gb in groupBy:
-                baseQuery = baseQuery.group_by(getattr(table, 'participantID'), gb)
-        else:
-            baseQuery = baseQuery.group_by(getattr(table, 'participantID'), groupBy)
+        return levels, fields, baseQuery
 
-        if having is not None:
-            baseQuery = baseQuery.having(having)
-    else:
-        baseQuery = baseQuery.group_by(getattr(table, 'participantID'))
-
-    if orderBy:
-        baseQuery = baseQuery.order_by(orderBy)
-
-    if filter is not None:
-        baseQuery = baseQuery.filter(filter)
-
-    # Add the fields to the basequery
-    for field in export_dict['fields']:
-        if hasattr(table, field) and callable(getattr(table, field)):
-            continue  # We can't include this python property as part of the query
-        fields.append(field)
-        baseQuery = baseQuery.add_columns(db.literal_column(export_dict['fields'][field]).label(field))
-
-    return levels, fields, baseQuery
-
-
-def add_participants_to_export(column_list: list[str],
-                               export_data: dict,
-                               include_unfinished=True,
-                               include_exluded=True) -> sqlalchemy.orm.Query:
-    """
-    Add participant columns to column_list and their data to export_data.
-    :param column_list: A list of strings that will be the columns in the CSV export.
-    :param export_data: Gets updated with data for the participants
-    :return: A SQLAlchemy query.
-    """
-    query_participants = db.session.query(db.Participant)
-    if not include_unfinished:
-        query_participants = query_participants.filter(db.Participant.finished == True)
-
-    if not include_exluded:
-        query_participants = query_participants.filter(db.or_(db.Participant.excludeFromCount == False, db.Participant.excludeFromCount == None))
-
-    column_list.extend([
-        "participantID",
-        "externalID",
-        "condition",
-        "duration",
-        "finished"
-    ])
-
-    query_result = query_participants.all()
-
-    for row in query_result:
-        export_data[row.participantID] = {
-            'participantID': row.participantID,
-            'externalID': row.mTurkID,
-            'condition': condition_num_to_label(row.condition),
-            'duration': row.duration,
-            'finished': row.finished
-        }
-
-    return query_participants
-
-
-def add_questionnaires_to_export(column_list: list[str],
-                                 export_data: dict,
-                                 query_participants: sqlalchemy.orm.Query,
-                                 include_missing=True) -> None:
-    list_of_questionnaires = page_list.get_questionnaire_list(include_tags=True)
-
-    query_questionnaires = query_participants
-    columns = {}
-    calculated_columns = {}
-
-    # First loop constructs the query and fetches the column names
-    for entry in list_of_questionnaires:
-        columns[entry] = []
-        calculated_columns[entry] = []
-        questionnaire_name, questionnaire_tag = questionnaire_name_and_tag(entry)
-
-        # The python class that describes the questionnaire
-        questionnaire = questionnaires[questionnaire_name]
-
-        # Add the questionnaire's table/class to the query...
-        questionnaire_db_class = db.aliased(questionnaire.db_class, name=entry)
-        join_condition = db.and_(questionnaire_db_class.participantID == db.Participant.participantID,
-                                 questionnaire_db_class.tag == questionnaire_tag
-                                 )
+    def load_data_frame(self):
+        self.df = pd.read_json(self.cache_path)
+        self.column_list = list(self.df.columns.values)
 
-        if include_missing:  # Need a left outer join
-            query_questionnaires = query_questionnaires.outerjoin(questionnaire_db_class, join_condition). \
-                add_entity(questionnaire_db_class)
-        else:
-            query_questionnaires = query_questionnaires.join(questionnaire_db_class, join_condition). \
-                add_entity(questionnaire_db_class)
+        for column in self.column_list:
+            self.export_data[column] = list(self.df[column])
 
-        # Make a list of the columns to later construct the CSV header row
-        # This could also be done with questionnaire.fields
-        for column in questionnaire.fetch_fields():
-            column_list.append(entry + "_" + column.id)
-            columns[entry].append(column.id)
-
-        # Similarly, make a list of calculated columns to later be part of the CSV header row.
-        for column in questionnaire.get_calculated_fields():
-            column_list.append(entry + "_" + column)
-            calculated_columns[entry].append(column)
-
-        # Duration always gets added
-        column_list.append(entry + "_duration")
-
-    query_result = query_questionnaires.all()
-
-    # Now we get the actual data
-    for row in query_result:
-        for entry in list_of_questionnaires:  # Need to look through the questionnaires again
-            questionnaire_data = getattr(row, entry)
-
-            if questionnaire_data:
-                # Regular columns first
-                for col in columns[entry]:
-                    export_data[row.Participant.participantID][entry + "_" + col] = getattr(questionnaire_data, col)
-
-                # Now calculated columns
-                for col in calculated_columns[entry]:
-                    if questionnaire_data:
-                        export_data[row.Participant.participantID][entry + "_" + col] = getattr(questionnaire_data, col)()
-
-                # Duration always gets added
-                export_data[row.Participant.participantID][entry + "_duration"] = questionnaire_data.duration()
-
-
-def add_custom_exports_to_export(column_list: list[str],
-                                 export_data: dict,
-                                 query_participants: sqlalchemy.orm.Query,
-                                 include_missing=True) -> None:
-    # Repeated measures in other tables...
-    custom_exports = []
-
-    for export in current_app.config['EXPORT']:
-        levels, fields, base_query = create_export_base_query(export)
-        custom_exports.append({'options': export, 'fields': fields, 'base_query': base_query, 'levels': levels})
-
-    # For custom exports, add columns based on levels determined by prior query
-    for export in custom_exports:
-        if export['levels']:
-            for level in export['levels']:
-                for field in export['options']['fields']:
-                    column_header = str.format("{}", field)
-                    for level_name in level:
-                        column_header += str.format("_{}", str(level_name).replace(" ", "_"))
-                    column_list.append(column_header)
-        else:
-            for field in export['options']['fields']:
-                column_list.append(str.format(u"{}", field))
+    def build_data_frame(self) -> "pd.DataFrame":
+        if self.df is not None:
+            return self.df
 
-    query_result = query_participants.all()
+        data = []
+        for key in self.export_data:
+            data.append(self.export_data[key])
 
-    # Now we get the actual data
-    for row in query_result:
-        participant_id = row.participantID
+        self.df = pd.DataFrame(data)
 
-        for export in custom_exports:
-            query = export['base_query']
-            query = query.filter(db.literal_column('participantID') == row.participantID)
-            custom_export_data = query.all()  # Running separate queries will get the job done, but be kind of slow with many participants...
-
-            export_row_index = 0
-            for custom_export_row in custom_export_data:
-                for field in export['fields']:
-                    export_column_name = field
-                    if export['levels']:
-                        export_column_name = field + "_" + str(export['levels'][export_row_index][0])
-
-                    export_data[participant_id][export_column_name] = getattr(custom_export_row, field)
-
-                export_row_index += 1
-
-
-def build_export_csv(column_list: list[str], export_data: dict) -> str:
-    csv_string = ",".join(column_list) + "\n"  # CSV Header
-
-    for row in export_data.values():
-        csv_line = ""
-        for column in column_list:
-            if column in row:
-                csv_line += escape_csv(row[column]) + ","
-            else:
-                csv_line += ","
+        if self.cache_path is not None:
+            self.df.to_json(self.cache_path)
+
+        return self.df
+
+    def build_export_csv(self) -> str:
+        csv_string = ",".join(self.column_list) + "\n"  # CSV Header
+
+        for row in self.export_data.values():
+            csv_line = ""
+            for column in self.column_list:
+                if column in row:
+                    csv_line += escape_csv(row[column]) + ","
+                else:
+                    csv_line += ","
 
-        csv_string += csv_line[:-1] + "\n"
+            csv_string += csv_line[:-1] + "\n"
 
-    return csv_string[:-1]  # return everything except last line break
+        return csv_string[:-1]  # return everything except last line break
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/database_delete.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/database_delete.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/export.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/export.html`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 <button type="submit" class="btn btn-dark" formaction="{{ url_for('admin.route_export_download') }}">Download CSV <i class="fa-solid fa-file-csv"></i></button>
             </div>
         </div>
 
         <div class="pt-3">
             <h4>Results for {{rowCount}} Participants</h4>
             <div>
-                <textarea style="width: 99%; height: 500px; white-space: pre;">{{ data | safe }}</textarea>
+                {{ data_table | safe }}
             </div>
         </div>
 
     </form>
 
 
 {% endblock %}
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/login_admin.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/login_admin.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/preview_questionnaire.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/preview_questionnaire.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress_ajax.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/progress_summary_ajax.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/progress_summary_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/questionnaire_results.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/questionnaire_results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/table_ajax.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/table_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/table_view.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/table_view.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/template_admin.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/template_admin.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
                     </li>
                     {% else %}
                     <li class="nav-item">
                         <a class="nav-link" href="{{ url_for('admin.route_export') }}">Export</a>
                     </li>
                     {% endif %}
 
+                    <li class="nav-item">
+                        <a class="nav-link" href="{{ url_for('admin.route_results') }}">Preview Results</a>
+                    </li>
+
                     <li class="nav-item dropdown">
                         <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">Preview Questionnaires</a>
                         <div class="dropdown-menu">
                             <h6 class="dropdown-header">In Use</h6>
                             {% for q in questionnairesLiveUntagged %}
                             <a class="dropdown-item" href="{{ url_for('admin.route_preview_questionnaire', questionnaireName=q) }}">{{ q }}</a>
                             {% endfor %}
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
     * _P_r_o_g_r_e_s_s
     * {% if logGridClicks %}
     * _E_x_p_o_r_t
       _Q_u_e_s_t_i_o_n_n_a_i_r_e_ _D_a_t_a _G_r_i_d_ _T_i_m_i_n_g_ _D_a_t_a<
     * {% else %}
     * _E_x_p_o_r_t
     * {% endif %}
+    * _P_r_e_v_i_e_w_ _R_e_s_u_l_t_s
     * _P_r_e_v_i_e_w_ _Q_u_e_s_t_i_o_n_n_a_i_r_e_s
       ** IInn UUssee **
       {% for q in questionnairesLiveUntagged %} _{_{_ _q_ _}_} {% endfor %}
       ** IInn tthhee SSyysstteemm **
       {% for q in questionnairesSystem %} _{_{_ _q_ _}_} {% endfor %}
     * _D_a_t_a_b_a_s_e
       {% if isSqliteDb %} _D_e_l_e_t_e_ _D_a_t_a_b_a_s_e _D_o_w_n_l_o_a_d_ _D_a_t_a_b_a_s_e {% endif %}
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/templates/template_admin_head.html` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/templates/template_admin_head.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/util.py` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/admin/views.py` & `bride-of-frankensystem-1.9.3.6/BOFS/admin/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import sqlalchemy
+import os
+import pandas as pd
 from flask import Blueprint, render_template, current_app, redirect, g, request, session, url_for, Response, send_file
 from BOFS.globals import db, questionnaires, page_list
 from BOFS.util import fetch_condition_count, display_time, provide_consent, int_or_0
 from .util import sqlalchemy_to_json, verify_admin, escape_csv, questionnaire_name_and_tag, condition_num_to_label
-from .export_helpers import *
+from .Results import Results
 import json
-from .QuestionnaireResults import *
+from .SummaryStats import SummaryStats
 from datetime import datetime
 from os import path, listdir
 from shutil import copyfile
 
 admin = Blueprint('admin', __name__, template_folder='templates', static_folder='static', url_prefix="/admin")
 
 
@@ -224,55 +225,90 @@
     excluded_count = db.session.query(db.Participant). \
         filter(db.Participant.excludeFromCount == True).count()  # For display only
 
     include_unfinished = request.args.get('includeUnfinished', False)
     include_missing = request.args.get('includeMissing', True)
     include_excluded = request.args.get('includeExcluded', False)
 
-    column_list = []
-    export_data = {}
+    if not include_excluded and include_unfinished:
+        query_filter = db.or_(db.Participant.excludeFromCount == False, db.Participant.excludeFromCount == None)
+    elif not include_excluded:
+        query_filter = db.and_(db.Participant.finished == True,
+                               db.or_(db.Participant.excludeFromCount == False, db.Participant.excludeFromCount == None))
+    elif not include_unfinished:
+        query_filter = None
+    else:
+        query_filter = db.and_(db.Participant.finished == True)
 
-    query = add_participants_to_export(column_list, export_data, include_unfinished, include_excluded)
-    add_questionnaires_to_export(column_list, export_data, query, include_missing)
-    add_custom_exports_to_export(column_list, export_data, query, include_missing)
+    results = Results(query_filter)
+    df = results.build_data_frame()
 
-    csv_string = build_export_csv(column_list, export_data)
 
     if request.base_url.endswith("/download"):
-        return Response(csv_string,
+        return Response(df.to_csv(),
                         mimetype="text/csv",
                         headers={
                             "Content-disposition": "attachment; filename=%s.csv" %
                                                    ("export_" + datetime.utcnow().strftime("%Y-%m-%d_%H-%M"))
                         })
     else:
         return render_template("export.html",
-                               data=csv_string,
-                               rowCount=len(export_data),
+                               data_table=df.to_html(index=False, classes="table table-striped border", justify="left"),
+                               rowCount=len(results.export_data),
                                unfinishedCount=unfinished_count,
                                excludedCount=excluded_count)
 
 
+def calculate_results() -> tuple[Results, pd.DataFrame, dict[str, SummaryStats]]:
+    cache_path = os.path.join(current_app.root_path, 'cached_results.json')
+    results = Results(db.and_(db.Participant.finished == True, db.Participant.excludeFromCount == False), cache_path)
+    df = results.build_data_frame()
+
+    df_grouped = df.groupby(by="condition")
+    summary_stats = {}
+
+    for column in list(df_grouped.head()):
+        dtype = df[column].head().dtype.name
+        if dtype in ['int64', 'float64', 'bool'] and column not in ['participantID', 'condition', 'duration',
+                                                                    'finished']:
+            summary_stats[column] = SummaryStats(df_grouped, column)
+
+    return results, df, summary_stats
+
+
 @admin.route("/results")
 @verify_admin
 def route_results():
-    qList = page_list.get_questionnaire_list(include_tags=True)
-    results = {}
-
-    for qNameAndTag in qList:
-        qName, qTag = questionnaire_name_and_tag(qNameAndTag)
+    results, df, summary_stats = calculate_results()
 
-        qResults = QuestionnaireResults(questionnaires[qName], qTag)
-        qResults.run_query()
-        qResults.calc_descriptives()
+    return render_template("results.html", summary_stats=summary_stats)
 
-        results[qNameAndTag] = qResults
+@admin.route("/results_boxplot/<path:field_name>")
+@verify_admin
+def route_results_boxplot(field_name: str):
+    results, df, summary_stats = calculate_results()
 
-    return render_template("results.html", results=results)
+    unique_conditions = df['condition'].unique().tolist()
+    unique_conditions.sort()
+    plot_data = []
+
+    for condition in unique_conditions:
+        df_part = df.loc[df.condition == condition]
+        count = df_part.count()
+
+        data = {
+            "y": df_part[field_name].to_list(),
+            #"x": [condition] * count,
+            "name": str(condition),
+            "type": "box",
+            "boxpoints": "Outliers"
+        }
+        plot_data.append(data)
 
+    return render_template("results_boxplot.html", field_name=field_name, plot_data=plot_data)
 
 @admin.route("/preview_questionnaire/<questionnaireName>", methods=["GET", "POST"])
 @verify_admin
 def route_preview_questionnaire(questionnaireName):
     if request.method == 'POST' and 'condition' in request.form:
         session['condition'] = int_or_0(request.form['condition'])
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-1.9.3.6/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/cli.py` & `bride-of-frankensystem-1.9.3.6/BOFS/cli.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/create_app.py` & `bride-of-frankensystem-1.9.3.6/BOFS/create_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         app.load_questionnaires()
         app.load_tables()
         app.db.create_all()
 
         # Check to see if all the columns are there
         # These are columns added to newer versions of BOFS
         check_and_add_column('participant', 'excludeFromCount', 'BOOLEAN', 0)
+        check_and_add_column('participant', 'notes', 'TEXT', '')
 
         if check_and_add_column('participant', 'isCrawler', 'BOOLEAN', 0):
             # If this column wasn't in there, then also check all prior participants' useragent.
             participants = app.db.session.query(app.db.Participant).all()
             for participant in participants:
                 participant.check_useragent_for_crawler()
             app.db.session.commit()
@@ -119,13 +120,14 @@
             for field in q_fields:
                 if check_and_add_column(table_name, field.id, field.get_type_ddl(), field.default):
                     print(f"Added new column to {table_name}: {field.id}")
 
         for t_key in app.tables:
             t = app.tables[t_key]
             columns = t.get_columns()
+            table_name = t.db_class.__tablename__
 
             for column in columns:
-                if check_and_add_column(t_key, column.name, column.get_type_ddl(), column.default):
+                if check_and_add_column(table_name, column.name, column.get_type_ddl(), column.default):
                     print(f"Added new column to {t_key}: {column.name}")
 
     return app
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/models.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/models.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/models.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x83fb1d66 (Tue Apr 16 04:16:03 2024 UTC)
-files sz: 9695
+moddate:  0x3e3a1f66 (Wed Apr 17 02:55:58 2024 UTC)
+files sz: 9703
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d005a006d015a010100640064026c026d035a0301
@@ -96,67 +96,67 @@
                       16 LOAD_CONST               2 ('Participant')
                       18 LOAD_DEREF               0 (db)
                       20 LOAD_ATTR                0 (Model)
                       30 PRECALL                  3
                       34 CALL                     3
                       44 STORE_FAST               1 (Participant)
          
-         176          46 PUSH_NULL
+         177          46 PUSH_NULL
                       48 LOAD_BUILD_CLASS
                       50 LOAD_CLOSURE             0 (db)
                       52 BUILD_TUPLE              1
-                      54 LOAD_CONST               3 (<code object Progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 176>)
+                      54 LOAD_CONST               3 (<code object Progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 177>)
                       56 MAKE_FUNCTION            8 (closure)
                       58 LOAD_CONST               4 ('Progress')
                       60 LOAD_DEREF               0 (db)
                       62 LOAD_ATTR                0 (Model)
                       72 PRECALL                  3
                       76 CALL                     3
                       86 STORE_FAST               2 (Progress)
          
-         194          88 PUSH_NULL
+         195          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
                       92 LOAD_CLOSURE             0 (db)
                       94 BUILD_TUPLE              1
-                      96 LOAD_CONST               5 (<code object RadioGridLog, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 194>)
+                      96 LOAD_CONST               5 (<code object RadioGridLog, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 195>)
                       98 MAKE_FUNCTION            8 (closure)
                      100 LOAD_CONST               6 ('RadioGridLog')
                      102 LOAD_DEREF               0 (db)
                      104 LOAD_ATTR                0 (Model)
                      114 PRECALL                  3
                      118 CALL                     3
                      128 STORE_FAST               3 (RadioGridLog)
          
-         206         130 PUSH_NULL
+         207         130 PUSH_NULL
                      132 LOAD_BUILD_CLASS
                      134 LOAD_CLOSURE             0 (db)
                      136 BUILD_TUPLE              1
-                     138 LOAD_CONST               7 (<code object Display, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 206>)
+                     138 LOAD_CONST               7 (<code object Display, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 207>)
                      140 MAKE_FUNCTION            8 (closure)
                      142 LOAD_CONST               8 ('Display')
                      144 LOAD_DEREF               0 (db)
                      146 LOAD_ATTR                0 (Model)
                      156 PRECALL                  3
                      160 CALL                     3
                      170 STORE_FAST               4 (Display)
          
-         218         172 PUSH_NULL
+         219         172 PUSH_NULL
                      174 LOAD_BUILD_CLASS
                      176 LOAD_CLOSURE             0 (db)
                      178 BUILD_TUPLE              1
-                     180 LOAD_CONST               9 (<code object SessionStore, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 218>)
+                     180 LOAD_CONST               9 (<code object SessionStore, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 219>)
                      182 MAKE_FUNCTION            8 (closure)
                      184 LOAD_CONST              10 ('SessionStore')
                      186 LOAD_DEREF               0 (db)
                      188 LOAD_ATTR                0 (Model)
                      198 PRECALL                  3
                      202 CALL                     3
                      212 STORE_FAST               5 (SessionStore)
          
-         235         214 LOAD_FAST                1 (Participant)
+         236         214 LOAD_FAST                1 (Participant)
                      216 LOAD_FAST                2 (Progress)
                      218 LOAD_FAST                3 (RadioGridLog)
                      220 LOAD_FAST                4 (Display)
                      222 LOAD_FAST                5 (SessionStore)
                      224 BUILD_TUPLE              5
                      226 RETURN_VALUE
          consts
@@ -187,21 +187,21 @@
                   00000094006a11000000000000000064046404ac06a6030000ab03000000
                   00000000005a139400a00400000000000000000000000000000000000000
                   0094006a11000000000000000064046404ac06a6030000ab030000000000
                   0000005a149400a004000000000000000000000000000000000000000094
                   006a07000000000000000064046407ac06a6030000ab0300000000000000
                   005a159400a004000000000000000000000000000000000000000094006a
                   0c00000000000000006404650d6a0e0000000000000000ac06a6030000ab
-                  0300000000000000005a166414640984015a176414640a65186602880066
-                  01640b840d5a19641588006601640d840c5a1a651b640a651c6602640e84
-                  04a6000000ab0000000000000000005a1d651d6a1e000000000000000088
-                  006601640f8408a6000000ab0000000000000000005a1d651f8800660164
-                  108408a6000000ab0000000000000000005a20651f8800660164118408a6
-                  000000ab0000000000000000005a21640a65226602641284045a23641384
-                  005a24640c5300
+                  0300000000000000005a16640984005a176415640a84015a186415640b65
+                  19660288006601640c840d5a1a641688006601640e840c5a1b651c640b65
+                  1d6602640f8404a6000000ab0000000000000000005a1e651e6a1f000000
+                  00000000008800660164108408a6000000ab0000000000000000005a1e65
+                  208800660164118408a6000000ab0000000000000000005a216520880066
+                  0164128408a6000000ab0000000000000000005a22640b65236602641384
+                  045a24641484005a25640d5300
                              0 COPY_FREE_VARS           1
                
                 10           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Participant')
                             10 STORE_NAME               2 (__qualname__)
@@ -338,109 +338,142 @@
                            700 LOAD_NAME               13 (datetime)
                            702 LOAD_ATTR               14 (utcnow)
                            712 KW_NAMES                 6
                            714 PRECALL                  3
                            718 CALL                     3
                            728 STORE_NAME              22 (lastActiveOn)
                
-                29         730 LOAD_CONST              20 (('',))
-                           732 LOAD_CONST               9 (<code object questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 29>)
-                           734 MAKE_FUNCTION            1 (defaults)
-                           736 STORE_NAME              23 (questionnaire)
-               
-                53         738 LOAD_CONST              20 (('',))
-                           740 LOAD_CONST              10 ('return')
-                           742 LOAD_NAME               24 (dict)
-                           744 BUILD_TUPLE              2
-                           746 LOAD_CLOSURE             0 (db)
-                           748 BUILD_TUPLE              1
-                           750 LOAD_CONST              11 (<code object questionnaire_log, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 53>)
-                           752 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                           754 STORE_NAME              25 (questionnaire_log)
-               
-                77         756 LOAD_CONST              21 (('return', None))
-                           758 LOAD_CLOSURE             0 (db)
-                           760 BUILD_TUPLE              1
-                           762 LOAD_CONST              13 (<code object assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 77>)
-                           764 MAKE_FUNCTION           12 (annotations, closure)
-                           766 STORE_NAME              26 (assign_condition)
-               
-               118         768 LOAD_NAME               27 (hybrid_property)
-               
-               119         770 LOAD_CONST              10 ('return')
-                           772 LOAD_NAME               28 (int)
-                           774 BUILD_TUPLE              2
-                           776 LOAD_CONST              14 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 118>)
-                           778 MAKE_FUNCTION            4 (annotations)
-               
-               118         780 PRECALL                  0
-                           784 CALL                     0
-               
-               119         794 STORE_NAME              29 (duration)
-               
-               124         796 LOAD_NAME               29 (duration)
-                           798 LOAD_ATTR               30 (expression)
-               
-               125         808 LOAD_CLOSURE             0 (db)
-                           810 BUILD_TUPLE              1
-                           812 LOAD_CONST              15 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 124>)
-                           814 MAKE_FUNCTION            8 (closure)
-               
-               124         816 PRECALL                  0
-                           820 CALL                     0
-               
-               125         830 STORE_NAME              29 (duration)
-               
-               131         832 LOAD_NAME               31 (declared_attr)
-               
-               132         834 LOAD_CLOSURE             0 (db)
-                           836 BUILD_TUPLE              1
-                           838 LOAD_CONST              16 (<code object is_in_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 131>)
-                           840 MAKE_FUNCTION            8 (closure)
-               
-               131         842 PRECALL                  0
-                           846 CALL                     0
-               
-               132         856 STORE_NAME              32 (is_in_progress)
-               
-               141         858 LOAD_NAME               31 (declared_attr)
-               
-               142         860 LOAD_CLOSURE             0 (db)
-                           862 BUILD_TUPLE              1
-                           864 LOAD_CONST              17 (<code object is_abandoned, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 141>)
-                           866 MAKE_FUNCTION            8 (closure)
-               
-               141         868 PRECALL                  0
-                           872 CALL                     0
-               
-               142         882 STORE_NAME              33 (is_abandoned)
-               
-               151         884 LOAD_CONST              10 ('return')
-                           886 LOAD_NAME               34 (str)
-                           888 BUILD_TUPLE              2
-                           890 LOAD_CONST              18 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 151>)
-                           892 MAKE_FUNCTION            4 (annotations)
-                           894 STORE_NAME              35 (display_duration)
-               
-               167         896 LOAD_CONST              19 (<code object check_useragent_for_crawler, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 167>)
-                           898 MAKE_FUNCTION            0
-                           900 STORE_NAME              36 (check_useragent_for_crawler)
-                           902 LOAD_CONST              12 (None)
-                           904 RETURN_VALUE
+                26         730 LOAD_CONST               9 (<code object table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 26>)
+                           732 MAKE_FUNCTION            0
+                           734 STORE_NAME              23 (table)
+               
+                30         736 LOAD_CONST              21 (('',))
+                           738 LOAD_CONST              10 (<code object questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 30>)
+                           740 MAKE_FUNCTION            1 (defaults)
+                           742 STORE_NAME              24 (questionnaire)
+               
+                54         744 LOAD_CONST              21 (('',))
+                           746 LOAD_CONST              11 ('return')
+                           748 LOAD_NAME               25 (dict)
+                           750 BUILD_TUPLE              2
+                           752 LOAD_CLOSURE             0 (db)
+                           754 BUILD_TUPLE              1
+                           756 LOAD_CONST              12 (<code object questionnaire_log, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 54>)
+                           758 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                           760 STORE_NAME              26 (questionnaire_log)
+               
+                78         762 LOAD_CONST              22 (('return', None))
+                           764 LOAD_CLOSURE             0 (db)
+                           766 BUILD_TUPLE              1
+                           768 LOAD_CONST              14 (<code object assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 78>)
+                           770 MAKE_FUNCTION           12 (annotations, closure)
+                           772 STORE_NAME              27 (assign_condition)
+               
+               119         774 LOAD_NAME               28 (hybrid_property)
+               
+               120         776 LOAD_CONST              11 ('return')
+                           778 LOAD_NAME               29 (int)
+                           780 BUILD_TUPLE              2
+                           782 LOAD_CONST              15 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 119>)
+                           784 MAKE_FUNCTION            4 (annotations)
+               
+               119         786 PRECALL                  0
+                           790 CALL                     0
+               
+               120         800 STORE_NAME              30 (duration)
+               
+               125         802 LOAD_NAME               30 (duration)
+                           804 LOAD_ATTR               31 (expression)
+               
+               126         814 LOAD_CLOSURE             0 (db)
+                           816 BUILD_TUPLE              1
+                           818 LOAD_CONST              16 (<code object duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 125>)
+                           820 MAKE_FUNCTION            8 (closure)
+               
+               125         822 PRECALL                  0
+                           826 CALL                     0
+               
+               126         836 STORE_NAME              30 (duration)
+               
+               132         838 LOAD_NAME               32 (declared_attr)
+               
+               133         840 LOAD_CLOSURE             0 (db)
+                           842 BUILD_TUPLE              1
+                           844 LOAD_CONST              17 (<code object is_in_progress, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 132>)
+                           846 MAKE_FUNCTION            8 (closure)
+               
+               132         848 PRECALL                  0
+                           852 CALL                     0
+               
+               133         862 STORE_NAME              33 (is_in_progress)
+               
+               142         864 LOAD_NAME               32 (declared_attr)
+               
+               143         866 LOAD_CLOSURE             0 (db)
+                           868 BUILD_TUPLE              1
+                           870 LOAD_CONST              18 (<code object is_abandoned, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 142>)
+                           872 MAKE_FUNCTION            8 (closure)
+               
+               142         874 PRECALL                  0
+                           878 CALL                     0
+               
+               143         888 STORE_NAME              34 (is_abandoned)
+               
+               152         890 LOAD_CONST              11 ('return')
+                           892 LOAD_NAME               35 (str)
+                           894 BUILD_TUPLE              2
+                           896 LOAD_CONST              19 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 152>)
+                           898 MAKE_FUNCTION            4 (annotations)
+                           900 STORE_NAME              36 (display_duration)
+               
+               168         902 LOAD_CONST              20 (<code object check_useragent_for_crawler, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 168>)
+                           904 MAKE_FUNCTION            0
+                           906 STORE_NAME              37 (check_useragent_for_crawler)
+                           908 LOAD_CONST              13 (None)
+                           910 RETURN_VALUE
                consts
                   'create.<locals>.Participant'
                   'participant'
                   True
                   ('primary_key', 'autoincrement')
                   False
                   ''
                   ('nullable', 'default')
                   0
                   ('nullable',)
                   code
+                     argcount  : 2
+                     nlocals   : 2
+                     stacksize : 5
+                     flags     : 19
+                     code
+                        0x97007401000000000000000000007c0064017c017a000000a6020000ab
+                        0200000000000000005300
+                      26           0 RESUME                   0
+                     
+                      27           2 LOAD_GLOBAL              1 (NULL + getattr)
+                                  14 LOAD_FAST                0 (self)
+                                  16 LOAD_CONST               1 ('table_')
+                                  18 LOAD_FAST                1 (name)
+                                  20 BINARY_OP                0 (+)
+                                  24 PRECALL                  2
+                                  28 CALL                     2
+                                  38 RETURN_VALUE
+                     consts
+                        None
+                        'table_'
+                     names      ('getattr',)
+                     varnames   ('self', 'name')
+                     freevars   ()
+                     cellvars   ()
+                     filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
+                     name       'table'
+                     firstlineno 26
+                     lnotab 0x0201
+                  code
                      argcount  : 3
                      nlocals   : 8
                      stacksize : 5
                      flags     : 19
                      code
                         0x9700640164026c006d017d0301007405000000000000000000007c0064
                         037c017a000000a6020000ab0200000000000000007d0467007d057c0444
@@ -451,109 +484,109 @@
                         010000ab01000000000000000064066b020000000072087c056401190000
                         000000000000005300740b000000000000000000007c05a6010000ab0100
                         0000000000000064066b0400000000721d64007d077c0544005d167d067c
                         0781107c076a0600000000000000007c066a0600000000000000006b0400
                         00000072027c067d078c177c0753007c037c0119000000000000000000a0
                         070000000000000000000000000000000000000000a6000000ab00000000
                         00000000005300
-                      29           0 RESUME                   0
+                      30           0 RESUME                   0
                      
-                      30           2 LOAD_CONST               1 (0)
+                      31           2 LOAD_CONST               1 (0)
                                    4 LOAD_CONST               2 (('questionnaires',))
                                    6 IMPORT_NAME              0 (BOFS.globals)
                                    8 IMPORT_FROM              1 (questionnaires)
                                   10 STORE_FAST               3 (questionnaires)
                                   12 POP_TOP
                      
-                      31          14 LOAD_GLOBAL              5 (NULL + getattr)
+                      32          14 LOAD_GLOBAL              5 (NULL + getattr)
                                   26 LOAD_FAST                0 (self)
                                   28 LOAD_CONST               3 ('questionnaire_')
                                   30 LOAD_FAST                1 (name)
                                   32 BINARY_OP                0 (+)
                                   36 PRECALL                  2
                                   40 CALL                     2
-                                  50 STORE_FAST               4 (qResults)
+                                  50 STORE_FAST               4 (q_results)
                      
-                      33          52 BUILD_LIST               0
+                      34          52 BUILD_LIST               0
                                   54 STORE_FAST               5 (toConsider)
                      
-                      35          56 LOAD_FAST                4 (qResults)
+                      36          56 LOAD_FAST                4 (q_results)
                                   58 GET_ITER
                              >>   60 FOR_ITER                51 (to 164)
                                   62 STORE_FAST               6 (result)
                      
-                      36          64 LOAD_FAST                6 (result)
+                      37          64 LOAD_FAST                6 (result)
                                   66 LOAD_ATTR                3 (tag)
                                   76 LOAD_FAST                2 (tag)
                                   78 COMPARE_OP               2 (==)
                                   84 POP_JUMP_FORWARD_IF_TRUE    17 (to 120)
                                   86 LOAD_FAST                6 (result)
                                   88 LOAD_ATTR                3 (tag)
                                   98 LOAD_CONST               4 ('0')
                                  100 COMPARE_OP               2 (==)
                                  106 POP_JUMP_FORWARD_IF_FALSE    27 (to 162)
                                  108 LOAD_FAST                2 (tag)
                                  110 LOAD_CONST               5 ('')
                                  112 COMPARE_OP               2 (==)
                                  118 POP_JUMP_FORWARD_IF_FALSE    21 (to 162)
                      
-                      37     >>  120 LOAD_FAST                5 (toConsider)
+                      38     >>  120 LOAD_FAST                5 (toConsider)
                                  122 LOAD_METHOD              4 (append)
                                  144 LOAD_FAST                6 (result)
                                  146 PRECALL                  1
                                  150 CALL                     1
                                  160 POP_TOP
                              >>  162 JUMP_BACKWARD           52 (to 60)
                      
-                      39     >>  164 LOAD_GLOBAL             11 (NULL + len)
+                      40     >>  164 LOAD_GLOBAL             11 (NULL + len)
                                  176 LOAD_FAST                5 (toConsider)
                                  178 PRECALL                  1
                                  182 CALL                     1
                                  192 LOAD_CONST               6 (1)
                                  194 COMPARE_OP               2 (==)
                                  200 POP_JUMP_FORWARD_IF_FALSE     8 (to 218)
                      
-                      40         202 LOAD_FAST                5 (toConsider)
+                      41         202 LOAD_FAST                5 (toConsider)
                                  204 LOAD_CONST               1 (0)
                                  206 BINARY_SUBSCR
                                  216 RETURN_VALUE
                      
-                      42     >>  218 LOAD_GLOBAL             11 (NULL + len)
+                      43     >>  218 LOAD_GLOBAL             11 (NULL + len)
                                  230 LOAD_FAST                5 (toConsider)
                                  232 PRECALL                  1
                                  236 CALL                     1
                                  246 LOAD_CONST               6 (1)
                                  248 COMPARE_OP               4 (>)
                                  254 POP_JUMP_FORWARD_IF_FALSE    29 (to 314)
                      
-                      43         256 LOAD_CONST               0 (None)
+                      44         256 LOAD_CONST               0 (None)
                                  258 STORE_FAST               7 (mostRecent)
                      
-                      44         260 LOAD_FAST                5 (toConsider)
+                      45         260 LOAD_FAST                5 (toConsider)
                                  262 GET_ITER
                              >>  264 FOR_ITER                22 (to 310)
                                  266 STORE_FAST               6 (result)
                      
-                      45         268 LOAD_FAST                7 (mostRecent)
+                      46         268 LOAD_FAST                7 (mostRecent)
                                  270 POP_JUMP_FORWARD_IF_NONE    16 (to 304)
                                  272 LOAD_FAST                7 (mostRecent)
                                  274 LOAD_ATTR                6 (timeEnded)
                                  284 LOAD_FAST                6 (result)
                                  286 LOAD_ATTR                6 (timeEnded)
                                  296 COMPARE_OP               4 (>)
                                  302 POP_JUMP_FORWARD_IF_FALSE     2 (to 308)
                      
-                      46     >>  304 LOAD_FAST                6 (result)
+                      47     >>  304 LOAD_FAST                6 (result)
                                  306 STORE_FAST               7 (mostRecent)
                              >>  308 JUMP_BACKWARD           23 (to 264)
                      
-                      48     >>  310 LOAD_FAST                7 (mostRecent)
+                      49     >>  310 LOAD_FAST                7 (mostRecent)
                                  312 RETURN_VALUE
                      
-                      50     >>  314 LOAD_FAST                3 (questionnaires)
+                      51     >>  314 LOAD_FAST                3 (questionnaires)
                                  316 LOAD_FAST                1 (name)
                                  318 BINARY_SUBSCR
                                  328 LOAD_METHOD              7 (create_blank)
                                  350 PRECALL                  0
                                  354 CALL                     0
                                  364 RETURN_VALUE
                      consts
@@ -561,20 +594,20 @@
                         0
                         ('questionnaires',)
                         'questionnaire_'
                         '0'
                         ''
                         1
                      names      ('BOFS.globals', 'questionnaires', 'getattr', 'tag', 'append', 'len', 'timeEnded', 'create_blank')
-                     varnames   ('self', 'name', 'tag', 'questionnaires', 'qResults', 'toConsider', 'result', 'mostRecent')
+                     varnames   ('self', 'name', 'tag', 'questionnaires', 'q_results', 'toConsider', 'result', 'mostRecent')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'questionnaire'
-                     firstlineno 29
+                     firstlineno 30
                      lnotab
                         0x02010c0126020402080138012c02260110022601040108012401060204
                         02
                   'return'
                   code
                      argcount  : 3
                      nlocals   : 9
@@ -595,120 +628,120 @@
                         0000000000000000000000a6000000ab0000000000000000007d0469007d
                         057c036a0a00000000000000007d067c0444005d2f7d077c076a08000000
                         00000000007c067a0a0000a00b0000000000000000000000000000000000
                         000000a6000000ab0000000000000000007d087c076a0800000000000000
                         007d067c087c057c076a0c00000000000000003c0000008c307c055300
                                    0 COPY_FREE_VARS           1
                      
-                      53           2 RESUME                   0
+                      54           2 RESUME                   0
                      
-                      54           4 LOAD_FAST                0 (self)
+                      55           4 LOAD_FAST                0 (self)
                                    6 LOAD_METHOD              0 (questionnaire)
                                   28 LOAD_FAST                1 (name)
                                   30 LOAD_FAST                2 (tag)
                                   32 PRECALL                  2
                                   36 CALL                     2
                                   46 STORE_FAST               3 (q)
                      
-                      56          48 LOAD_FAST                2 (tag)
+                      57          48 LOAD_FAST                2 (tag)
                                   50 LOAD_CONST               1 ('')
                                   52 COMPARE_OP               2 (==)
                                   58 POP_JUMP_FORWARD_IF_FALSE     2 (to 64)
                      
-                      57          60 LOAD_CONST               2 (0)
+                      58          60 LOAD_CONST               2 (0)
                                   62 STORE_FAST               2 (tag)
                      
-                      59     >>   64 LOAD_DEREF               9 (db)
+                      60     >>   64 LOAD_DEREF               9 (db)
                                   66 LOAD_ATTR                1 (session)
                                   76 LOAD_METHOD              2 (query)
                                   98 LOAD_DEREF               9 (db)
                                  100 LOAD_ATTR                3 (RadioGridLog)
                                  110 PRECALL                  1
                                  114 CALL                     1
                                  124 LOAD_METHOD              4 (filter)
                      
-                      60         146 LOAD_DEREF               9 (db)
+                      61         146 LOAD_DEREF               9 (db)
                                  148 LOAD_ATTR                3 (RadioGridLog)
                                  158 LOAD_ATTR                5 (participantID)
                                  168 LOAD_FAST                0 (self)
                                  170 LOAD_ATTR                5 (participantID)
                                  180 COMPARE_OP               2 (==)
                      
-                      61         186 LOAD_DEREF               9 (db)
+                      62         186 LOAD_DEREF               9 (db)
                                  188 LOAD_ATTR                3 (RadioGridLog)
                                  198 LOAD_ATTR                0 (questionnaire)
                                  208 LOAD_FAST                1 (name)
                                  210 COMPARE_OP               2 (==)
                      
-                      62         216 LOAD_DEREF               9 (db)
+                      63         216 LOAD_DEREF               9 (db)
                                  218 LOAD_ATTR                3 (RadioGridLog)
                                  228 LOAD_ATTR                6 (tag)
                                  238 LOAD_FAST                2 (tag)
                                  240 COMPARE_OP               2 (==)
                      
-                      59         246 PRECALL                  3
+                      60         246 PRECALL                  3
                                  250 CALL                     3
                      
-                      63         260 LOAD_METHOD              7 (order_by)
+                      64         260 LOAD_METHOD              7 (order_by)
                                  282 LOAD_DEREF               9 (db)
                                  284 LOAD_ATTR                3 (RadioGridLog)
                                  294 LOAD_ATTR                8 (timeClicked)
                                  304 PRECALL                  1
                                  308 CALL                     1
                                  318 LOAD_METHOD              9 (all)
                                  340 PRECALL                  0
                                  344 CALL                     0
                      
-                      59         354 STORE_FAST               4 (logs)
+                      60         354 STORE_FAST               4 (logs)
                      
-                      65         356 BUILD_MAP                0
+                      66         356 BUILD_MAP                0
                                  358 STORE_FAST               5 (result)
                      
-                      67         360 LOAD_FAST                3 (q)
+                      68         360 LOAD_FAST                3 (q)
                                  362 LOAD_ATTR               10 (timeStarted)
                                  372 STORE_FAST               6 (prevTime)
                      
-                      69         374 LOAD_FAST                4 (logs)
+                      70         374 LOAD_FAST                4 (logs)
                                  376 GET_ITER
                              >>  378 FOR_ITER                47 (to 474)
                                  380 STORE_FAST               7 (log)
                      
-                      70         382 LOAD_FAST                7 (log)
+                      71         382 LOAD_FAST                7 (log)
                                  384 LOAD_ATTR                8 (timeClicked)
                                  394 LOAD_FAST                6 (prevTime)
                                  396 BINARY_OP               10 (-)
                                  400 LOAD_METHOD             11 (total_seconds)
                                  422 PRECALL                  0
                                  426 CALL                     0
                                  436 STORE_FAST               8 (deltaTime)
                      
-                      71         438 LOAD_FAST                7 (log)
+                      72         438 LOAD_FAST                7 (log)
                                  440 LOAD_ATTR                8 (timeClicked)
                                  450 STORE_FAST               6 (prevTime)
                      
-                      73         452 LOAD_FAST                8 (deltaTime)
+                      74         452 LOAD_FAST                8 (deltaTime)
                                  454 LOAD_FAST                5 (result)
                                  456 LOAD_FAST                7 (log)
                                  458 LOAD_ATTR               12 (questionID)
                                  468 STORE_SUBSCR
                                  472 JUMP_BACKWARD           48 (to 378)
                      
-                      75     >>  474 LOAD_FAST                5 (result)
+                      76     >>  474 LOAD_FAST                5 (result)
                                  476 RETURN_VALUE
                      consts
                         None
                         ''
                         0
                      names      ('questionnaire', 'session', 'query', 'RadioGridLog', 'filter', 'participantID', 'tag', 'order_by', 'timeClicked', 'all', 'timeStarted', 'total_seconds', 'questionID')
                      varnames   ('self', 'name', 'tag', 'q', 'logs', 'result', 'prevTime', 'log', 'deltaTime')
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'questionnaire_log'
-                     firstlineno 53
+                     firstlineno 54
                      lnotab
                         0x04012c020c010402520128011e011efd0e045efc020604020e02080138
                         010e021602
                   None
                   code
                      argcount  : 1
                      nlocals   : 9
@@ -750,231 +783,231 @@
                         007c005f0a000000000000000001006e018c4c7c036409a0040000000000
                         0000000000000000000000000000007c006a0a0000000000000000a60100
                         00ab0100000000000000007a0d00007d037423000000000000000000007c
                         03a6010000ab01000000000000000001006400530064007c005f0a000000
                         000000000064005300
                                    0 COPY_FREE_VARS           1
                      
-                      77           2 RESUME                   0
+                      78           2 RESUME                   0
                      
-                      78           4 LOAD_FAST                0 (self)
+                      79           4 LOAD_FAST                0 (self)
                                    6 LOAD_METHOD              0 (check_useragent_for_crawler)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 POP_JUMP_FORWARD_IF_FALSE     2 (to 48)
                      
-                      79          44 LOAD_CONST               0 (None)
+                      80          44 LOAD_CONST               0 (None)
                                   46 RETURN_VALUE
                      
-                      81     >>   48 LOAD_GLOBAL              3 (NULL + len)
+                      82     >>   48 LOAD_GLOBAL              3 (NULL + len)
                                   60 LOAD_GLOBAL              4 (current_app)
                                   72 LOAD_ATTR                3 (config)
                                   82 LOAD_CONST               1 ('CONDITIONS')
                                   84 BINARY_SUBSCR
                                   94 PRECALL                  1
                                   98 CALL                     1
                                  108 STORE_FAST               1 (numConditions)
                      
-                      82         110 LOAD_FAST                1 (numConditions)
+                      83         110 LOAD_FAST                1 (numConditions)
                                  112 LOAD_CONST               2 (0)
                                  114 COMPARE_OP               4 (>)
                                  120 EXTENDED_ARG             1
                                  122 POP_JUMP_FORWARD_IF_FALSE   473 (to 1070)
                      
-                      83         124 LOAD_CONST               2 (0)
+                      84         124 LOAD_CONST               2 (0)
                                  126 BUILD_LIST               1
                                  128 LOAD_FAST                1 (numConditions)
                                  130 BINARY_OP                5 (*)
                                  134 STORE_FAST               2 (pCount)
                      
-                      85         136 LOAD_CONST               3 ('Total conditions: {}, Counts: ')
+                      86         136 LOAD_CONST               3 ('Total conditions: {}, Counts: ')
                                  138 LOAD_METHOD              4 (format)
                                  160 LOAD_FAST                1 (numConditions)
                                  162 PRECALL                  1
                                  166 CALL                     1
                                  176 STORE_FAST               3 (printText)
                      
-                      87         178 LOAD_GLOBAL             11 (NULL + range)
+                      88         178 LOAD_GLOBAL             11 (NULL + range)
                                  190 LOAD_CONST               4 (1)
                                  192 LOAD_FAST                1 (numConditions)
                                  194 LOAD_CONST               4 (1)
                                  196 BINARY_OP                0 (+)
                                  200 PRECALL                  2
                                  204 CALL                     2
                                  214 GET_ITER
                              >>  216 EXTENDED_ARG             1
                                  218 FOR_ITER               286 (to 792)
                                  220 STORE_FAST               4 (condition)
                      
-                      89         222 LOAD_GLOBAL              4 (current_app)
+                      90         222 LOAD_GLOBAL              4 (current_app)
                                  234 LOAD_ATTR                3 (config)
                                  244 LOAD_CONST               5 ('COUNTS_INCLUDE_ABANDONED')
                                  246 BINARY_SUBSCR
                                  256 POP_JUMP_FORWARD_IF_FALSE   101 (to 460)
                      
-                      90         258 LOAD_DEREF               9 (db)
+                      91         258 LOAD_DEREF               9 (db)
                                  260 LOAD_ATTR                6 (session)
                                  270 LOAD_METHOD              7 (query)
                                  292 LOAD_DEREF               9 (db)
                                  294 LOAD_ATTR                8 (Participant)
                                  304 PRECALL                  1
                                  308 CALL                     1
                      
-                      91         318 LOAD_METHOD              9 (filter)
+                      92         318 LOAD_METHOD              9 (filter)
                                  340 LOAD_DEREF               9 (db)
                                  342 LOAD_ATTR                8 (Participant)
                                  352 LOAD_ATTR               10 (condition)
                                  362 LOAD_FAST                4 (condition)
                                  364 COMPARE_OP               2 (==)
                      
-                      92         370 LOAD_DEREF               9 (db)
+                      93         370 LOAD_DEREF               9 (db)
                                  372 LOAD_ATTR                8 (Participant)
                                  382 LOAD_ATTR               11 (excludeFromCount)
                                  392 UNARY_INVERT
                      
-                      91         394 PRECALL                  2
+                      92         394 PRECALL                  2
                                  398 CALL                     2
                      
-                      93         408 LOAD_METHOD             12 (count)
+                      94         408 LOAD_METHOD             12 (count)
                                  430 PRECALL                  0
                                  434 CALL                     0
                      
-                      90         444 LOAD_FAST                2 (pCount)
+                      91         444 LOAD_FAST                2 (pCount)
                                  446 LOAD_FAST                4 (condition)
                                  448 LOAD_CONST               4 (1)
                                  450 BINARY_OP               10 (-)
                                  454 STORE_SUBSCR
                                  458 JUMP_FORWARD           131 (to 722)
                      
-                      95     >>  460 LOAD_DEREF               9 (db)
+                      96     >>  460 LOAD_DEREF               9 (db)
                                  462 LOAD_ATTR                6 (session)
                                  472 LOAD_METHOD              7 (query)
                                  494 LOAD_DEREF               9 (db)
                                  496 LOAD_ATTR                8 (Participant)
                                  506 PRECALL                  1
                                  510 CALL                     1
                      
-                      96         520 LOAD_METHOD              9 (filter)
+                      97         520 LOAD_METHOD              9 (filter)
                      
-                      97         542 LOAD_DEREF               9 (db)
+                      98         542 LOAD_DEREF               9 (db)
                                  544 LOAD_METHOD             13 (and_)
                                  566 LOAD_DEREF               9 (db)
                                  568 LOAD_ATTR                8 (Participant)
                                  578 LOAD_ATTR               10 (condition)
                                  588 LOAD_FAST                4 (condition)
                                  590 COMPARE_OP               2 (==)
                      
-                      98         596 LOAD_DEREF               9 (db)
+                      99         596 LOAD_DEREF               9 (db)
                                  598 LOAD_ATTR                8 (Participant)
                                  608 LOAD_ATTR               14 (is_abandoned)
                                  618 UNARY_INVERT
                      
-                      99         620 LOAD_DEREF               9 (db)
+                     100         620 LOAD_DEREF               9 (db)
                                  622 LOAD_ATTR                8 (Participant)
                                  632 LOAD_ATTR               11 (excludeFromCount)
                                  642 UNARY_INVERT
                      
-                      97         644 PRECALL                  3
+                      98         644 PRECALL                  3
                                  648 CALL                     3
                      
-                      96         658 PRECALL                  1
+                      97         658 PRECALL                  1
                                  662 CALL                     1
                      
-                     100         672 LOAD_METHOD             12 (count)
+                     101         672 LOAD_METHOD             12 (count)
                                  694 PRECALL                  0
                                  698 CALL                     0
                      
-                      95         708 LOAD_FAST                2 (pCount)
+                      96         708 LOAD_FAST                2 (pCount)
                                  710 LOAD_FAST                4 (condition)
                                  712 LOAD_CONST               4 (1)
                                  714 BINARY_OP               10 (-)
                                  718 STORE_SUBSCR
                      
-                     102     >>  722 LOAD_FAST                3 (printText)
+                     103     >>  722 LOAD_FAST                3 (printText)
                                  724 LOAD_CONST               6 ('{}, ')
                                  726 LOAD_METHOD              4 (format)
                                  748 LOAD_FAST                2 (pCount)
                                  750 LOAD_FAST                4 (condition)
                                  752 LOAD_CONST               4 (1)
                                  754 BINARY_OP               10 (-)
                                  758 BINARY_SUBSCR
                                  768 PRECALL                  1
                                  772 CALL                     1
                                  782 BINARY_OP               13 (+=)
                                  786 STORE_FAST               3 (printText)
                                  788 EXTENDED_ARG             1
                                  790 JUMP_BACKWARD          288 (to 216)
                      
-                     104     >>  792 LOAD_GLOBAL             31 (NULL + sorted)
+                     105     >>  792 LOAD_GLOBAL             31 (NULL + sorted)
                                  804 LOAD_FAST                2 (pCount)
                                  806 PRECALL                  1
                                  810 CALL                     1
                                  820 STORE_FAST               5 (pCountSorted)
                      
-                     106         822 LOAD_FAST                5 (pCountSorted)
+                     107         822 LOAD_FAST                5 (pCountSorted)
                                  824 GET_ITER
                              >>  826 FOR_ITER                75 (to 978)
                                  828 STORE_FAST               6 (count)
                      
-                     107         830 LOAD_FAST                2 (pCount)
+                     108         830 LOAD_FAST                2 (pCount)
                                  832 LOAD_METHOD             16 (index)
                                  854 LOAD_FAST                6 (count)
                                  856 PRECALL                  1
                                  860 CALL                     1
                                  870 STORE_FAST               7 (idx)
                      
-                     108         872 LOAD_GLOBAL              4 (current_app)
+                     109         872 LOAD_GLOBAL              4 (current_app)
                                  884 LOAD_ATTR                3 (config)
                                  894 LOAD_CONST               1 ('CONDITIONS')
                                  896 BINARY_SUBSCR
                                  906 LOAD_FAST                7 (idx)
                                  908 BINARY_SUBSCR
                                  918 STORE_FAST               8 (conditionMeta)
                      
-                     109         920 LOAD_CONST               7 ('enabled')
+                     110         920 LOAD_CONST               7 ('enabled')
                                  922 LOAD_FAST                8 (conditionMeta)
                                  924 CONTAINS_OP              1
                                  926 POP_JUMP_FORWARD_IF_TRUE    12 (to 952)
                                  928 LOAD_FAST                8 (conditionMeta)
                                  930 LOAD_CONST               7 ('enabled')
                                  932 BINARY_SUBSCR
                                  942 LOAD_CONST               8 (True)
                                  944 COMPARE_OP               2 (==)
                                  950 POP_JUMP_FORWARD_IF_FALSE    12 (to 976)
                      
-                     110     >>  952 LOAD_FAST                7 (idx)
+                     111     >>  952 LOAD_FAST                7 (idx)
                                  954 LOAD_CONST               4 (1)
                                  956 BINARY_OP                0 (+)
                                  960 LOAD_FAST                0 (self)
                                  962 STORE_ATTR              10 (condition)
                      
-                     111         972 POP_TOP
+                     112         972 POP_TOP
                                  974 JUMP_FORWARD             1 (to 978)
                      
-                     109     >>  976 JUMP_BACKWARD           76 (to 826)
+                     110     >>  976 JUMP_BACKWARD           76 (to 826)
                      
-                     113     >>  978 LOAD_FAST                3 (printText)
+                     114     >>  978 LOAD_FAST                3 (printText)
                                  980 LOAD_CONST               9 ('User put in condition {}.')
                                  982 LOAD_METHOD              4 (format)
                                 1004 LOAD_FAST                0 (self)
                                 1006 LOAD_ATTR               10 (condition)
                                 1016 PRECALL                  1
                                 1020 CALL                     1
                                 1030 BINARY_OP               13 (+=)
                                 1034 STORE_FAST               3 (printText)
                      
-                     114        1036 LOAD_GLOBAL             35 (NULL + print)
+                     115        1036 LOAD_GLOBAL             35 (NULL + print)
                                 1048 LOAD_FAST                3 (printText)
                                 1050 PRECALL                  1
                                 1054 CALL                     1
                                 1064 POP_TOP
                                 1066 LOAD_CONST               0 (None)
                                 1068 RETURN_VALUE
                      
-                     116     >> 1070 LOAD_CONST               0 (None)
+                     117     >> 1070 LOAD_CONST               0 (None)
                                 1072 LOAD_FAST                0 (self)
                                 1074 STORE_ATTR              10 (condition)
                                 1084 LOAD_CONST               0 (None)
                                 1086 RETURN_VALUE
                      consts
                         None
                         'CONDITIONS'
@@ -988,38 +1021,38 @@
                         'User put in condition {}.'
                      names      ('check_useragent_for_crawler', 'len', 'current_app', 'config', 'format', 'range', 'session', 'query', 'Participant', 'filter', 'condition', 'excludeFromCount', 'count', 'and_', 'is_abandoned', 'sorted', 'index', 'print')
                      varnames   ('self', 'numConditions', 'pCount', 'printText', 'condition', 'pCountSorted', 'count', 'idx', 'conditionMeta')
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'assign_condition'
-                     firstlineno 77
+                     firstlineno 78
                      lnotab
                         0x0401280104023e010e010c022a022c0224013c01340118ff0e0224fd10
                         053c0116013601180118fe0eff0e0424fb0e0746021e0208012a01300120
                         01140104fe02043a012202
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x97007c006a0000000000000000008002640153007c006a000000000000
                         0000007c006a0100000000000000007a0a0000a002000000000000000000
                         0000000000000000000000a6000000ab0000000000000000005300
-                     118           0 RESUME                   0
+                     119           0 RESUME                   0
                      
-                     120           2 LOAD_FAST                0 (self)
+                     121           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (timeEnded)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 20)
                      
-                     121          16 LOAD_CONST               1 (0)
+                     122          16 LOAD_CONST               1 (0)
                                   18 RETURN_VALUE
                      
-                     122     >>   20 LOAD_FAST                0 (self)
+                     123     >>   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (timeEnded)
                                   32 LOAD_FAST                0 (self)
                                   34 LOAD_ATTR                1 (timeStarted)
                                   44 BINARY_OP               10 (-)
                                   48 LOAD_METHOD              2 (total_seconds)
                                   70 PRECALL                  0
                                   74 CALL                     0
@@ -1029,15 +1062,15 @@
                         0
                      names      ('timeEnded', 'timeStarted', 'total_seconds')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'duration'
-                     firstlineno 118
+                     firstlineno 119
                      lnotab 0x02020e010401
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 7
                      flags     : 19
                      code
@@ -1047,27 +1080,27 @@
                         010000000000000000a6010000ab01000000000000000089016a02000000
                         0000000000a00300000000000000000000000000000000000000007c006a
                         040000000000000000a6010000ab0100000000000000007a0a000064017a
                         050000ac02a6020000ab020000000000000000a005000000000000000000
                         00000000000000000000006403a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     124           2 RESUME                   0
+                     125           2 RESUME                   0
                      
-                     126           4 LOAD_DEREF               1 (db)
+                     127           4 LOAD_DEREF               1 (db)
                                    6 LOAD_METHOD              0 (case)
                      
-                     127          28 LOAD_FAST                0 (cls)
+                     128          28 LOAD_FAST                0 (cls)
                                   30 LOAD_ATTR                1 (timeEnded)
                                   40 LOAD_CONST               0 (None)
                                   42 COMPARE_OP               2 (==)
                                   48 LOAD_CONST               0 (None)
                                   50 BUILD_TUPLE              2
                      
-                     128          52 LOAD_DEREF               1 (db)
+                     129          52 LOAD_DEREF               1 (db)
                                   54 LOAD_ATTR                2 (func)
                                   64 LOAD_METHOD              3 (julianday)
                                   86 LOAD_FAST                0 (cls)
                                   88 LOAD_ATTR                1 (timeEnded)
                                   98 PRECALL                  1
                                  102 CALL                     1
                                  112 LOAD_DEREF               1 (db)
@@ -1077,36 +1110,36 @@
                                  148 LOAD_ATTR                4 (timeStarted)
                                  158 PRECALL                  1
                                  162 CALL                     1
                                  172 BINARY_OP               10 (-)
                                  176 LOAD_CONST               1 (86400)
                                  178 BINARY_OP                5 (*)
                      
-                     126         182 KW_NAMES                 2
+                     127         182 KW_NAMES                 2
                                  184 PRECALL                  2
                                  188 CALL                     2
                      
-                     129         198 LOAD_METHOD              5 (label)
+                     130         198 LOAD_METHOD              5 (label)
                                  220 LOAD_CONST               3 ('duration')
                                  222 PRECALL                  1
                                  226 CALL                     1
                      
-                     126         236 RETURN_VALUE
+                     127         236 RETURN_VALUE
                      consts
                         None
                         86400
                         ('else_',)
                         'duration'
                      names      ('case', 'timeEnded', 'func', 'julianday', 'timeStarted', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'duration'
-                     firstlineno 124
+                     firstlineno 125
                      lnotab 0x04021801180182fe100326fd
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 10
                      flags     : 19
                      code
@@ -1119,26 +1152,26 @@
                         000000000000007c006a060000000000000000a6010000ab010000000000
                         0000007a0a00007a050000740e000000000000000000006a080000000000
                         0000006402190000000000000000006b0100000000a6020000ab02000000
                         0000000000a00900000000000000000000000000000000000000006403a6
                         010000ab010000000000000000a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     131           2 RESUME                   0
+                     132           2 RESUME                   0
                      
-                     133           4 LOAD_GLOBAL              1 (NULL + column_property)
+                     134           4 LOAD_GLOBAL              1 (NULL + column_property)
                      
-                     134          16 LOAD_DEREF               1 (db)
+                     135          16 LOAD_DEREF               1 (db)
                                   18 LOAD_METHOD              1 (and_)
                      
-                     135          40 LOAD_FAST                0 (cls)
+                     136          40 LOAD_FAST                0 (cls)
                                   42 LOAD_ATTR                2 (finished)
                                   52 UNARY_INVERT
                      
-                     136          54 LOAD_CONST               1 (1440.0)
+                     137          54 LOAD_CONST               1 (1440.0)
                                   56 LOAD_DEREF               1 (db)
                                   58 LOAD_ATTR                3 (func)
                                   68 LOAD_METHOD              4 (julianday)
                                   90 LOAD_DEREF               1 (db)
                                   92 LOAD_ATTR                3 (func)
                                  102 LOAD_METHOD              5 (current_timestamp)
                                  124 PRECALL                  0
@@ -1151,44 +1184,44 @@
                                  186 LOAD_FAST                0 (cls)
                                  188 LOAD_ATTR                6 (lastActiveOn)
                                  198 PRECALL                  1
                                  202 CALL                     1
                                  212 BINARY_OP               10 (-)
                                  216 BINARY_OP                5 (*)
                      
-                     137         220 LOAD_GLOBAL             14 (current_app)
+                     138         220 LOAD_GLOBAL             14 (current_app)
                                  232 LOAD_ATTR                8 (config)
                                  242 LOAD_CONST               2 ('ABANDONED_MINUTES')
                                  244 BINARY_SUBSCR
                      
-                     136         254 COMPARE_OP               1 (<=)
+                     137         254 COMPARE_OP               1 (<=)
                      
-                     134         260 PRECALL                  2
+                     135         260 PRECALL                  2
                                  264 CALL                     2
                      
-                     138         274 LOAD_METHOD              9 (label)
+                     139         274 LOAD_METHOD              9 (label)
                                  296 LOAD_CONST               3 ('is_in_progress')
                                  298 PRECALL                  1
                                  302 CALL                     1
                      
-                     133         312 PRECALL                  1
+                     134         312 PRECALL                  1
                                  316 CALL                     1
                                  326 RETURN_VALUE
                      consts
                         None
                         1440.0
                         'ABANDONED_MINUTES'
                         'is_in_progress'
                      names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'current_timestamp', 'lastActiveOn', 'current_app', 'config', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'is_in_progress'
-                     firstlineno 131
+                     firstlineno 132
                      lnotab 0x04020c0118010e01a60122ff06fe0e0426fb
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 10
                      flags     : 19
                      code
@@ -1201,26 +1234,26 @@
                         000000000000007c006a060000000000000000a6010000ab010000000000
                         0000007a0a00007a050000740e000000000000000000006a080000000000
                         0000006402190000000000000000006b0400000000a6020000ab02000000
                         0000000000a00900000000000000000000000000000000000000006403a6
                         010000ab010000000000000000a6010000ab0100000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     141           2 RESUME                   0
+                     142           2 RESUME                   0
                      
-                     143           4 LOAD_GLOBAL              1 (NULL + column_property)
+                     144           4 LOAD_GLOBAL              1 (NULL + column_property)
                      
-                     144          16 LOAD_DEREF               1 (db)
+                     145          16 LOAD_DEREF               1 (db)
                                   18 LOAD_METHOD              1 (and_)
                      
-                     145          40 LOAD_FAST                0 (cls)
+                     146          40 LOAD_FAST                0 (cls)
                                   42 LOAD_ATTR                2 (finished)
                                   52 UNARY_INVERT
                      
-                     146          54 LOAD_CONST               1 (1440.0)
+                     147          54 LOAD_CONST               1 (1440.0)
                                   56 LOAD_DEREF               1 (db)
                                   58 LOAD_ATTR                3 (func)
                                   68 LOAD_METHOD              4 (julianday)
                                   90 LOAD_DEREF               1 (db)
                                   92 LOAD_ATTR                3 (func)
                                  102 LOAD_METHOD              5 (current_timestamp)
                                  124 PRECALL                  0
@@ -1233,83 +1266,83 @@
                                  186 LOAD_FAST                0 (cls)
                                  188 LOAD_ATTR                6 (lastActiveOn)
                                  198 PRECALL                  1
                                  202 CALL                     1
                                  212 BINARY_OP               10 (-)
                                  216 BINARY_OP                5 (*)
                      
-                     147         220 LOAD_GLOBAL             14 (current_app)
+                     148         220 LOAD_GLOBAL             14 (current_app)
                                  232 LOAD_ATTR                8 (config)
                                  242 LOAD_CONST               2 ('ABANDONED_MINUTES')
                                  244 BINARY_SUBSCR
                      
-                     146         254 COMPARE_OP               4 (>)
+                     147         254 COMPARE_OP               4 (>)
                      
-                     144         260 PRECALL                  2
+                     145         260 PRECALL                  2
                                  264 CALL                     2
                      
-                     148         274 LOAD_METHOD              9 (label)
+                     149         274 LOAD_METHOD              9 (label)
                                  296 LOAD_CONST               3 ('is_abandoned')
                                  298 PRECALL                  1
                                  302 CALL                     1
                      
-                     143         312 PRECALL                  1
+                     144         312 PRECALL                  1
                                  316 CALL                     1
                                  326 RETURN_VALUE
                      consts
                         None
                         1440.0
                         'ABANDONED_MINUTES'
                         'is_abandoned'
                      names      ('column_property', 'and_', 'finished', 'func', 'julianday', 'current_timestamp', 'lastActiveOn', 'current_app', 'config', 'label')
                      varnames   ('cls',)
                      freevars   ('db',)
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'is_abandoned'
-                     firstlineno 141
+                     firstlineno 142
                      lnotab 0x04020c0118010e01a60122ff06fe0e0426fb
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code
                         0x97007c006a000000000000000000800b7c006a01000000000000000072
                         0264025300640353007c006a0000000000000000007c006a020000000000
                         0000007a0a0000a0030000000000000000000000000000000000000000a6
                         000000ab0000000000000000007d017409000000000000000000007c01a6
                         010000ab0100000000000000005300
-                     151           0 RESUME                   0
+                     152           0 RESUME                   0
                      
-                     157           2 LOAD_FAST                0 (self)
+                     158           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (timeEnded)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE    11 (to 38)
                      
-                     158          16 LOAD_FAST                0 (self)
+                     159          16 LOAD_FAST                0 (self)
                                   18 LOAD_ATTR                1 (is_in_progress)
                                   28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                      
-                     159          30 LOAD_CONST               2 ('In Progress')
+                     160          30 LOAD_CONST               2 ('In Progress')
                                   32 RETURN_VALUE
                      
-                     161     >>   34 LOAD_CONST               3 ('Abandoned')
+                     162     >>   34 LOAD_CONST               3 ('Abandoned')
                                   36 RETURN_VALUE
                      
-                     164     >>   38 LOAD_FAST                0 (self)
+                     165     >>   38 LOAD_FAST                0 (self)
                                   40 LOAD_ATTR                0 (timeEnded)
                                   50 LOAD_FAST                0 (self)
                                   52 LOAD_ATTR                2 (timeStarted)
                                   62 BINARY_OP               10 (-)
                                   66 LOAD_METHOD              3 (total_seconds)
                                   88 PRECALL                  0
                                   92 CALL                     0
                                  102 STORE_FAST               1 (seconds)
                      
-                     165         104 LOAD_GLOBAL              9 (NULL + display_time)
+                     166         104 LOAD_GLOBAL              9 (NULL + display_time)
                                  116 LOAD_FAST                1 (seconds)
                                  118 PRECALL                  1
                                  122 CALL                     1
                                  132 RETURN_VALUE
                      consts
                         '\n            display the time taken or status\n            :return:\n            '
                         None
@@ -1317,74 +1350,74 @@
                         'Abandoned'
                      names      ('timeEnded', 'is_in_progress', 'timeStarted', 'total_seconds', 'display_time')
                      varnames   ('self', 'seconds')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'display_duration'
-                     firstlineno 151
+                     firstlineno 152
                      lnotab 0x02060e010e01040204034201
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x97007400000000000000000000006a010000000000000000a002000000
                         00000000000000000000000000000000007c006a030000000000000000a6
                         010000ab0100000000000000007c005f0200000000000000007c006a0200
                         00000000000000720764017c005f0400000000000000007c006a02000000
                         00000000005300
-                     167           0 RESUME                   0
+                     168           0 RESUME                   0
                      
-                     168           2 LOAD_GLOBAL              0 (current_app)
+                     169           2 LOAD_GLOBAL              0 (current_app)
                                   14 LOAD_ATTR                1 (crawler_detect)
                                   24 LOAD_METHOD              2 (isCrawler)
                                   46 LOAD_FAST                0 (self)
                                   48 LOAD_ATTR                3 (userAgent)
                                   58 PRECALL                  1
                                   62 CALL                     1
                                   72 LOAD_FAST                0 (self)
                                   74 STORE_ATTR               2 (isCrawler)
                      
-                     170          84 LOAD_FAST                0 (self)
+                     171          84 LOAD_FAST                0 (self)
                                   86 LOAD_ATTR                2 (isCrawler)
                                   96 POP_JUMP_FORWARD_IF_FALSE     7 (to 112)
                      
-                     171          98 LOAD_CONST               1 (True)
+                     172          98 LOAD_CONST               1 (True)
                                  100 LOAD_FAST                0 (self)
                                  102 STORE_ATTR               4 (excludeFromCount)
                      
-                     173     >>  112 LOAD_FAST                0 (self)
+                     174     >>  112 LOAD_FAST                0 (self)
                                  114 LOAD_ATTR                2 (isCrawler)
                                  124 RETURN_VALUE
                      consts
                         None
                         True
                      names      ('current_app', 'crawler_detect', 'isCrawler', 'userAgent', 'excludeFromCount')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'check_useragent_for_crawler'
-                     firstlineno 167
+                     firstlineno 168
                      lnotab 0x020152020e010e02
                   ('',)
                   ('return', None)
-               names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'participantID', 'String', 'mTurkID', 'ipAddress', 'userAgent', 'condition', 'DateTime', 'datetime', 'utcnow', 'timeStarted', 'timeEnded', 'Boolean', 'finished', 'isCrawler', 'excludeFromCount', 'code', 'lastActiveOn', 'questionnaire', 'dict', 'questionnaire_log', 'assign_condition', 'hybrid_property', 'int', 'duration', 'expression', 'declared_attr', 'is_in_progress', 'is_abandoned', 'str', 'display_duration', 'check_useragent_for_crawler')
+               names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'participantID', 'String', 'mTurkID', 'ipAddress', 'userAgent', 'condition', 'DateTime', 'datetime', 'utcnow', 'timeStarted', 'timeEnded', 'Boolean', 'finished', 'isCrawler', 'excludeFromCount', 'code', 'lastActiveOn', 'table', 'questionnaire', 'dict', 'questionnaire_log', 'assign_condition', 'hybrid_property', 'int', 'duration', 'expression', 'declared_attr', 'is_in_progress', 'is_abandoned', 'str', 'display_duration', 'check_useragent_for_crawler')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Participant'
                firstlineno 10
                lnotab
-                  0x0c0104023a013a013a013a013a01440138013a013a013a013a01440508
-                  1812180c2902010aff0e0102050c0108ff0e010206020108ff0e01020902
-                  0108ff0e0102090c10
+                  0x0c0104023a013a013a013a013a01440138013a013a013a013a01440206
+                  04081812180c2902010aff0e0102050c0108ff0e010206020108ff0e0102
+                  09020108ff0e0102090c10
             'Participant'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
                code
@@ -1397,75 +1430,75 @@
                   00000000000000000000000000000094006a0a0000000000000000640565
                   0b6a0c0000000000000000ac07a6030000ab0300000000000000005a0d94
                   00a004000000000000000000000000000000000000000094006a0a000000
                   00000000006403ac08a6020000ab0200000000000000005a0e6409650f66
                   02640a84045a10640b5300
                              0 COPY_FREE_VARS           1
                
-               176           2 RESUME                   0
+               177           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Progress')
                             10 STORE_NAME               2 (__qualname__)
                
-               177          12 LOAD_CONST               1 ('progress')
+               178          12 LOAD_CONST               1 ('progress')
                             14 STORE_NAME               3 (__tablename__)
                
-               179          16 LOAD_CLASSDEREF          0 (db)
+               180          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CLASSDEREF          0 (db)
                             54 LOAD_METHOD              6 (ForeignKey)
                             76 LOAD_CONST               2 ('participant.participantID')
                             78 PRECALL                  1
                             82 CALL                     1
                             92 LOAD_CONST               3 (True)
                             94 KW_NAMES                 4
                             96 PRECALL                  3
                            100 CALL                     3
                            110 STORE_NAME               7 (participantID)
                
-               180         112 LOAD_CLASSDEREF          0 (db)
+               181         112 LOAD_CLASSDEREF          0 (db)
                            114 LOAD_METHOD              4 (Column)
                            136 LOAD_CLASSDEREF          0 (db)
                            138 LOAD_ATTR                8 (Text)
                            148 LOAD_CONST               5 (False)
                            150 LOAD_CONST               3 (True)
                            152 KW_NAMES                 6
                            154 PRECALL                  3
                            158 CALL                     3
                            168 STORE_NAME               9 (path)
                
-               181         170 LOAD_CLASSDEREF          0 (db)
+               182         170 LOAD_CLASSDEREF          0 (db)
                            172 LOAD_METHOD              4 (Column)
                            194 LOAD_CLASSDEREF          0 (db)
                            196 LOAD_ATTR               10 (DateTime)
                            206 LOAD_CONST               5 (False)
                            208 LOAD_NAME               11 (datetime)
                            210 LOAD_ATTR               12 (utcnow)
                            220 KW_NAMES                 7
                            222 PRECALL                  3
                            226 CALL                     3
                            236 STORE_NAME              13 (startedOn)
                
-               182         238 LOAD_CLASSDEREF          0 (db)
+               183         238 LOAD_CLASSDEREF          0 (db)
                            240 LOAD_METHOD              4 (Column)
                            262 LOAD_CLASSDEREF          0 (db)
                            264 LOAD_ATTR               10 (DateTime)
                            274 LOAD_CONST               3 (True)
                            276 KW_NAMES                 8
                            278 PRECALL                  2
                            282 CALL                     2
                            292 STORE_NAME              14 (submittedOn)
                
-               184         294 LOAD_CONST               9 ('return')
+               185         294 LOAD_CONST               9 ('return')
                            296 LOAD_NAME               15 (str)
                            298 BUILD_TUPLE              2
-                           300 LOAD_CONST              10 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 184>)
+                           300 LOAD_CONST              10 (<code object display_duration, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 185>)
                            302 MAKE_FUNCTION            4 (annotations)
                            304 STORE_NAME              16 (display_duration)
                            306 LOAD_CONST              11 (None)
                            308 RETURN_VALUE
                consts
                   'create.<locals>.Progress'
                   'progress'
@@ -1487,54 +1520,54 @@
                         0000007c006a0100000000000000007a0a0000a002000000000000000000
                         0000000000000000000000a6000000ab0000000000000000007d017c0164
                         026b040000000072297407000000000000000000006403a6010000ab0100
                         00000000000000a00400000000000000000000000000000000000000007c
                         0164027a0b00007c0164027a060000a6020000ab02000000000000000053
                         00740700000000000000000000740b000000000000000000007c01a60100
                         00ab010000000000000000a6010000ab0100000000000000005300
-                     184           0 RESUME                   0
+                     185           0 RESUME                   0
                      
-                     185           2 LOAD_FAST                0 (self)
+                     186           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (submittedOn)
                                   14 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 20)
                      
-                     186          16 LOAD_CONST               1 ('...')
+                     187          16 LOAD_CONST               1 ('...')
                                   18 RETURN_VALUE
                      
-                     188     >>   20 LOAD_FAST                0 (self)
+                     189     >>   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (submittedOn)
                                   32 LOAD_FAST                0 (self)
                                   34 LOAD_ATTR                1 (startedOn)
                                   44 BINARY_OP               10 (-)
                                   48 LOAD_METHOD              2 (total_seconds)
                                   70 PRECALL                  0
                                   74 CALL                     0
                                   84 STORE_FAST               1 (seconds)
                      
-                     189          86 LOAD_FAST                1 (seconds)
+                     190          86 LOAD_FAST                1 (seconds)
                                   88 LOAD_CONST               2 (60)
                                   90 COMPARE_OP               4 (>)
                                   96 POP_JUMP_FORWARD_IF_FALSE    41 (to 180)
                      
-                     190          98 LOAD_GLOBAL              7 (NULL + str)
+                     191          98 LOAD_GLOBAL              7 (NULL + str)
                                  110 LOAD_CONST               3 ('{:.0f}:{:02.0f}')
                                  112 PRECALL                  1
                                  116 CALL                     1
                                  126 LOAD_METHOD              4 (format)
                                  148 LOAD_FAST                1 (seconds)
                                  150 LOAD_CONST               2 (60)
                                  152 BINARY_OP               11 (/)
                                  156 LOAD_FAST                1 (seconds)
                                  158 LOAD_CONST               2 (60)
                                  160 BINARY_OP                6 (%)
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 RETURN_VALUE
                      
-                     191     >>  180 LOAD_GLOBAL              7 (NULL + str)
+                     192     >>  180 LOAD_GLOBAL              7 (NULL + str)
                                  192 LOAD_GLOBAL             11 (NULL + int)
                                  204 LOAD_FAST                1 (seconds)
                                  206 PRECALL                  1
                                  210 CALL                     1
                                  220 PRECALL                  1
                                  224 CALL                     1
                                  234 RETURN_VALUE
@@ -1545,24 +1578,24 @@
                         '{:.0f}:{:02.0f}'
                      names      ('submittedOn', 'startedOn', 'total_seconds', 'str', 'format', 'int')
                      varnames   ('self', 'seconds')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'display_duration'
-                     firstlineno 184
+                     firstlineno 185
                      lnotab 0x02010e01040242010c015201
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'ForeignKey', 'participantID', 'Text', 'path', 'DateTime', 'datetime', 'utcnow', 'startedOn', 'submittedOn', 'str', 'display_duration')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Progress'
-               firstlineno 176
+               firstlineno 177
                lnotab 0x0c01040260013a0144013802
             'Progress'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1581,93 +1614,93 @@
                   056407ac06a6030000ab0300000000000000005a0f9400a0040000000000
                   00000000000000000000000000000094006a0d0000000000000000640564
                   07ac06a6030000ab0300000000000000005a109400a00400000000000000
                   0000000000000000000000000094006a0d000000000000000064056407ac
                   06a6030000ab0300000000000000005a1164085300
                              0 COPY_FREE_VARS           1
                
-               194           2 RESUME                   0
+               195           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.RadioGridLog')
                             10 STORE_NAME               2 (__qualname__)
                
-               195          12 LOAD_CONST               1 ('radio_grid_log')
+               196          12 LOAD_CONST               1 ('radio_grid_log')
                             14 STORE_NAME               3 (__tablename__)
                
-               197          16 LOAD_CLASSDEREF          0 (db)
+               198          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CONST               2 (True)
                             54 LOAD_CONST               2 (True)
                             56 KW_NAMES                 3
                             58 PRECALL                  3
                             62 CALL                     3
                             72 STORE_NAME               6 (radioGridLog)
                
-               198          74 LOAD_CLASSDEREF          0 (db)
+               199          74 LOAD_CLASSDEREF          0 (db)
                             76 LOAD_METHOD              4 (Column)
                             98 LOAD_CLASSDEREF          0 (db)
                            100 LOAD_ATTR                5 (Integer)
                            110 LOAD_CLASSDEREF          0 (db)
                            112 LOAD_METHOD              7 (ForeignKey)
                            134 LOAD_CONST               4 ('participant.participantID')
                            136 PRECALL                  1
                            140 CALL                     1
                            150 PRECALL                  2
                            154 CALL                     2
                            164 STORE_NAME               8 (participantID)
                
-               199         166 LOAD_CLASSDEREF          0 (db)
+               200         166 LOAD_CLASSDEREF          0 (db)
                            168 LOAD_METHOD              4 (Column)
                            190 LOAD_CLASSDEREF          0 (db)
                            192 LOAD_ATTR                9 (DateTime)
                            202 LOAD_CONST               5 (False)
                            204 LOAD_NAME               10 (datetime)
                            206 LOAD_ATTR               11 (utcnow)
                            216 KW_NAMES                 6
                            218 PRECALL                  3
                            222 CALL                     3
                            232 STORE_NAME              12 (timeClicked)
                
-               200         234 LOAD_CLASSDEREF          0 (db)
+               201         234 LOAD_CLASSDEREF          0 (db)
                            236 LOAD_METHOD              4 (Column)
                            258 LOAD_CLASSDEREF          0 (db)
                            260 LOAD_ATTR               13 (String)
                            270 LOAD_CONST               5 (False)
                            272 LOAD_CONST               7 ('')
                            274 KW_NAMES                 6
                            276 PRECALL                  3
                            280 CALL                     3
                            290 STORE_NAME              14 (questionnaire)
                
-               201         292 LOAD_CLASSDEREF          0 (db)
+               202         292 LOAD_CLASSDEREF          0 (db)
                            294 LOAD_METHOD              4 (Column)
                            316 LOAD_CLASSDEREF          0 (db)
                            318 LOAD_ATTR               13 (String)
                            328 LOAD_CONST               5 (False)
                            330 LOAD_CONST               7 ('')
                            332 KW_NAMES                 6
                            334 PRECALL                  3
                            338 CALL                     3
                            348 STORE_NAME              15 (tag)
                
-               202         350 LOAD_CLASSDEREF          0 (db)
+               203         350 LOAD_CLASSDEREF          0 (db)
                            352 LOAD_METHOD              4 (Column)
                            374 LOAD_CLASSDEREF          0 (db)
                            376 LOAD_ATTR               13 (String)
                            386 LOAD_CONST               5 (False)
                            388 LOAD_CONST               7 ('')
                            390 KW_NAMES                 6
                            392 PRECALL                  3
                            396 CALL                     3
                            406 STORE_NAME              16 (questionID)
                
-               203         408 LOAD_CLASSDEREF          0 (db)
+               204         408 LOAD_CLASSDEREF          0 (db)
                            410 LOAD_METHOD              4 (Column)
                            432 LOAD_CLASSDEREF          0 (db)
                            434 LOAD_ATTR               13 (String)
                            444 LOAD_CONST               5 (False)
                            446 LOAD_CONST               7 ('')
                            448 KW_NAMES                 6
                            450 PRECALL                  3
@@ -1687,15 +1720,15 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'radioGridLog', 'ForeignKey', 'participantID', 'DateTime', 'datetime', 'utcnow', 'timeClicked', 'String', 'questionnaire', 'tag', 'questionID', 'value')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'RadioGridLog'
-               firstlineno 194
+               firstlineno 195
                lnotab 0x0c0104023a015c0144013a013a013a01
             'RadioGridLog'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1714,92 +1747,92 @@
                   0300000000000000005a0c9400a004000000000000000000000000000000
                   000000000094006a05000000000000000064056408ac07a6030000ab0300
                   000000000000005a0d9400a0040000000000000000000000000000000000
                   00000094006a05000000000000000064056408ac07a6030000ab03000000
                   00000000005a0e64095300
                              0 COPY_FREE_VARS           1
                
-               206           2 RESUME                   0
+               207           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.Display')
                             10 STORE_NAME               2 (__qualname__)
                
-               207          12 LOAD_CONST               1 ('display')
+               208          12 LOAD_CONST               1 ('display')
                             14 STORE_NAME               3 (__tablename__)
                
-               209          16 LOAD_CLASSDEREF          0 (db)
+               210          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_ATTR                5 (Integer)
                             52 LOAD_CONST               2 (True)
                             54 LOAD_CONST               2 (True)
                             56 KW_NAMES                 3
                             58 PRECALL                  3
                             62 CALL                     3
                             72 STORE_NAME               6 (logDisplayID)
                
-               210          74 LOAD_CLASSDEREF          0 (db)
+               211          74 LOAD_CLASSDEREF          0 (db)
                             76 LOAD_METHOD              4 (Column)
                             98 LOAD_CLASSDEREF          0 (db)
                            100 LOAD_ATTR                5 (Integer)
                            110 LOAD_CLASSDEREF          0 (db)
                            112 LOAD_METHOD              7 (ForeignKey)
                            134 LOAD_CONST               4 ('participant.participantID')
                            136 PRECALL                  1
                            140 CALL                     1
                            150 PRECALL                  2
                            154 CALL                     2
                            164 STORE_NAME               8 (participantID)
                
-               211         166 LOAD_CLASSDEREF          0 (db)
+               212         166 LOAD_CLASSDEREF          0 (db)
                            168 LOAD_METHOD              4 (Column)
                            190 LOAD_CLASSDEREF          0 (db)
                            192 LOAD_ATTR                9 (Float)
                            202 LOAD_CONST               5 (False)
                            204 LOAD_CONST               6 (0.0)
                            206 KW_NAMES                 7
                            208 PRECALL                  3
                            212 CALL                     3
                            222 STORE_NAME              10 (dppx)
                
-               212         224 LOAD_CLASSDEREF          0 (db)
+               213         224 LOAD_CLASSDEREF          0 (db)
                            226 LOAD_METHOD              4 (Column)
                            248 LOAD_CLASSDEREF          0 (db)
                            250 LOAD_ATTR                5 (Integer)
                            260 LOAD_CONST               5 (False)
                            262 LOAD_CONST               8 (0)
                            264 KW_NAMES                 7
                            266 PRECALL                  3
                            270 CALL                     3
                            280 STORE_NAME              11 (screenWidth)
                
-               213         282 LOAD_CLASSDEREF          0 (db)
+               214         282 LOAD_CLASSDEREF          0 (db)
                            284 LOAD_METHOD              4 (Column)
                            306 LOAD_CLASSDEREF          0 (db)
                            308 LOAD_ATTR                5 (Integer)
                            318 LOAD_CONST               5 (False)
                            320 LOAD_CONST               8 (0)
                            322 KW_NAMES                 7
                            324 PRECALL                  3
                            328 CALL                     3
                            338 STORE_NAME              12 (screenHeight)
                
-               214         340 LOAD_CLASSDEREF          0 (db)
+               215         340 LOAD_CLASSDEREF          0 (db)
                            342 LOAD_METHOD              4 (Column)
                            364 LOAD_CLASSDEREF          0 (db)
                            366 LOAD_ATTR                5 (Integer)
                            376 LOAD_CONST               5 (False)
                            378 LOAD_CONST               8 (0)
                            380 KW_NAMES                 7
                            382 PRECALL                  3
                            386 CALL                     3
                            396 STORE_NAME              13 (innerWidth)
                
-               215         398 LOAD_CLASSDEREF          0 (db)
+               216         398 LOAD_CLASSDEREF          0 (db)
                            400 LOAD_METHOD              4 (Column)
                            422 LOAD_CLASSDEREF          0 (db)
                            424 LOAD_ATTR                5 (Integer)
                            434 LOAD_CONST               5 (False)
                            436 LOAD_CONST               8 (0)
                            438 KW_NAMES                 7
                            440 PRECALL                  3
@@ -1820,15 +1853,15 @@
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'Integer', 'logDisplayID', 'ForeignKey', 'participantID', 'Float', 'dppx', 'screenWidth', 'screenHeight', 'innerWidth', 'innerHeight')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'Display'
-               firstlineno 206
+               firstlineno 207
                lnotab 0x0c0104023a015c013a013a013a013a01
             'Display'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 6
                flags     : 0
@@ -1847,105 +1880,105 @@
                   006a0d0000000000000000a6010000ab0100000000000000005a0e9400a0
                   04000000000000000000000000000000000000000094006a0d0000000000
                   0000006407650f6a100000000000000000ac08a6030000ab030000000000
                   0000005a11640984005a126513640a65146602640b8404a6000000ab0000
                   000000000000005a15640c5300
                              0 COPY_FREE_VARS           1
                
-               218           2 RESUME                   0
+               219           2 RESUME                   0
                              4 LOAD_NAME                0 (__name__)
                              6 STORE_NAME               1 (__module__)
                              8 LOAD_CONST               0 ('create.<locals>.SessionStore')
                             10 STORE_NAME               2 (__qualname__)
                
-               219          12 LOAD_CONST               1 ('session_store')
+               220          12 LOAD_CONST               1 ('session_store')
                             14 STORE_NAME               3 (__tablename__)
                
-               221          16 LOAD_CLASSDEREF          0 (db)
+               222          16 LOAD_CLASSDEREF          0 (db)
                             18 LOAD_METHOD              4 (Column)
                             40 LOAD_CLASSDEREF          0 (db)
                             42 LOAD_METHOD              5 (String)
                             64 LOAD_CONST               2 (255)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 LOAD_CONST               3 (True)
                             82 KW_NAMES                 4
                             84 PRECALL                  2
                             88 CALL                     2
                             98 STORE_NAME               6 (sessionID)
                
-               222         100 LOAD_CLASSDEREF          0 (db)
+               223         100 LOAD_CLASSDEREF          0 (db)
                            102 LOAD_METHOD              4 (Column)
                            124 LOAD_CLASSDEREF          0 (db)
                            126 LOAD_ATTR                7 (Integer)
                            136 LOAD_CLASSDEREF          0 (db)
                            138 LOAD_METHOD              8 (ForeignKey)
                            160 LOAD_CONST               5 ('participant.participantID')
                            162 PRECALL                  1
                            166 CALL                     1
                            176 LOAD_CONST               3 (True)
                            178 KW_NAMES                 6
                            180 PRECALL                  3
                            184 CALL                     3
                            194 STORE_NAME               9 (participantID)
                
-               223         196 LOAD_CLASSDEREF          0 (db)
+               224         196 LOAD_CLASSDEREF          0 (db)
                            198 LOAD_METHOD              4 (Column)
                            220 LOAD_CLASSDEREF          0 (db)
                            222 LOAD_ATTR               10 (Text)
                            232 LOAD_CONST               3 (True)
                            234 KW_NAMES                 6
                            236 PRECALL                  2
                            240 CALL                     2
                            250 STORE_NAME              11 (mTurkID)
                
-               224         252 LOAD_CLASSDEREF          0 (db)
+               225         252 LOAD_CLASSDEREF          0 (db)
                            254 LOAD_METHOD              4 (Column)
                            276 LOAD_CLASSDEREF          0 (db)
                            278 LOAD_ATTR               10 (Text)
                            288 PRECALL                  1
                            292 CALL                     1
                            302 STORE_NAME              12 (data)
                
-               225         304 LOAD_CLASSDEREF          0 (db)
+               226         304 LOAD_CLASSDEREF          0 (db)
                            306 LOAD_METHOD              4 (Column)
                            328 LOAD_CLASSDEREF          0 (db)
                            330 LOAD_ATTR               13 (DateTime)
                            340 PRECALL                  1
                            344 CALL                     1
                            354 STORE_NAME              14 (expiry)
                
-               226         356 LOAD_CLASSDEREF          0 (db)
+               227         356 LOAD_CLASSDEREF          0 (db)
                            358 LOAD_METHOD              4 (Column)
                            380 LOAD_CLASSDEREF          0 (db)
                            382 LOAD_ATTR               13 (DateTime)
                            392 LOAD_CONST               7 (False)
                            394 LOAD_NAME               15 (datetime)
                            396 LOAD_ATTR               16 (utcnow)
                            406 KW_NAMES                 8
                            408 PRECALL                  3
                            412 CALL                     3
                            422 STORE_NAME              17 (createdOn)
                
-               228         424 LOAD_CONST               9 (<code object __repr__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 228>)
+               229         424 LOAD_CONST               9 (<code object __repr__, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 229>)
                            426 MAKE_FUNCTION            0
                            428 STORE_NAME              18 (__repr__)
                
-               231         430 LOAD_NAME               19 (property)
+               232         430 LOAD_NAME               19 (property)
                
-               232         432 LOAD_CONST              10 ('return')
+               233         432 LOAD_CONST              10 ('return')
                            434 LOAD_NAME               20 (bool)
                            436 BUILD_TUPLE              2
-                           438 LOAD_CONST              11 (<code object expired, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 231>)
+                           438 LOAD_CONST              11 (<code object expired, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\models.py", line 232>)
                            440 MAKE_FUNCTION            4 (annotations)
                
-               231         442 PRECALL                  0
+               232         442 PRECALL                  0
                            446 CALL                     0
                
-               232         456 STORE_NAME              21 (expired)
+               233         456 STORE_NAME              21 (expired)
                            458 LOAD_CONST              12 (None)
                            460 RETURN_VALUE
                consts
                   'create.<locals>.SessionStore'
                   'session_store'
                   255
                   True
@@ -1958,17 +1991,17 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x97006401a00000000000000000000000000000000000000000007c006a
                         010000000000000000a6010000ab0100000000000000005300
-                     228           0 RESUME                   0
+                     229           0 RESUME                   0
                      
-                     229           2 LOAD_CONST               1 ('<Session data {0!s}>')
+                     230           2 LOAD_CONST               1 ('<Session data {0!s}>')
                                    4 LOAD_METHOD              0 (format)
                                   26 LOAD_FAST                0 (self)
                                   28 LOAD_ATTR                1 (data)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 RETURN_VALUE
                      consts
@@ -1976,29 +2009,29 @@
                         '<Session data {0!s}>'
                      names      ('format', 'data')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       '__repr__'
-                     firstlineno 228
+                     firstlineno 229
                      lnotab 0x0201
                   'return'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 3
                      flags     : 19
                      code
                         0x97007c006a00000000000000000064007500701b7c006a000000000000
                         0000007403000000000000000000006a020000000000000000a6000000ab
                         0000000000000000006b01000000005300
-                     231           0 RESUME                   0
+                     232           0 RESUME                   0
                      
-                     233           2 LOAD_FAST                0 (self)
+                     234           2 LOAD_FAST                0 (self)
                                    4 LOAD_ATTR                0 (expiry)
                                   14 LOAD_CONST               0 (None)
                                   16 IS_OP                    0
                                   18 JUMP_IF_TRUE_OR_POP     27 (to 74)
                                   20 LOAD_FAST                0 (self)
                                   22 LOAD_ATTR                0 (expiry)
                                   32 LOAD_GLOBAL              3 (NULL + datetime)
@@ -2011,34 +2044,34 @@
                         None
                      names      ('expiry', 'datetime', 'utcnow')
                      varnames   ('self',)
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                      name       'expired'
-                     firstlineno 231
+                     firstlineno 232
                      lnotab 0x0202
                   None
                names      ('__name__', '__module__', '__qualname__', '__tablename__', 'Column', 'String', 'sessionID', 'Integer', 'ForeignKey', 'participantID', 'Text', 'mTurkID', 'data', 'DateTime', 'expiry', 'datetime', 'utcnow', 'createdOn', '__repr__', 'property', 'bool', 'expired')
                varnames   ()
                freevars   ('db',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
                name       'SessionStore'
-               firstlineno 218
+               firstlineno 219
                lnotab 0x0c010402540160013801340134014402060302010aff0e01
             'SessionStore'
          names      ('Model',)
          varnames   ('db', 'Participant', 'Progress', 'RadioGridLog', 'Display', 'SessionStore')
          freevars   ()
          cellvars   ('db',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
          name       'create'
          firstlineno 9
-         lnotab 0x04012a7f00272a122a0c2a0c2a11
+         lnotab 0x04012a7f00282a122a0c2a0c2a11
       None
    names      ('datetime', 'timedelta', 'sqlalchemy.ext.hybrid', 'hybrid_property', 'sqlalchemy.orm', 'column_property', 'sqlalchemy.ext.declarative', 'declared_attr', 'BOFS.util', 'display_time', 'flask', 'current_app', 'create')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\models.py'
    name       '<module>'
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-1.9.3.6/BOFS/default/__pycache__/views.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,79 +1,79 @@
 magic:    0xa70d0d0a
-moddate:  0xb6e71266 (Sun Apr  7 18:36:38 2024 UTC)
-files sz: 17838
+moddate:  0xf8e21e66 (Tue Apr 16 20:43:36 2024 UTC)
+files sz: 18057
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
-      00640064026c066d075a070100640064036c086d095a090100640064046c
-      0a5400640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a1001
-      00640064066c116d125a126d135a1301000200650164076514a6020000ab
-      0200000000000000005a156515a016000000000000000000000000000000
-      00000000006408a6010000ab010000000000000000651764098400a60000
-      00ab000000000000000000a6000000ab0000000000000000005a186515a0
-      160000000000000000000000000000000000000000640a640b640c6702ac
-      0da6020000ab0200000000000000006517640e8400a6000000ab00000000
-      0000000000a6000000ab0000000000000000005a196515a0160000000000
-      000000000000000000000000000000640f640b640c6702ac0da6020000ab
-      020000000000000000651764108400a6000000ab000000000000000000a6
-      000000ab0000000000000000005a1a6515a0160000000000000000000000
-      0000000000000000006411a6010000ab01000000000000000064128400a6
-      000000ab0000000000000000005a1b6515a0160000000000000000000000
-      0000000000000000006413a6010000ab01000000000000000064148400a6
-      000000ab0000000000000000005a1c6515a0160000000000000000000000
-      0000000000000000006415a6010000ab010000000000000000651d651764
-      168400a6000000ab000000000000000000a6000000ab0000000000000000
-      00a6000000ab0000000000000000005a1e6515a016000000000000000000
-      00000000000000000000006417640b640c6702ac0da6020000ab02000000
-      00000000006515a016000000000000000000000000000000000000000064
-      18640b640c6702ac0da6020000ab0200000000000000006515a016000000
-      00000000000000000000000000000000006419640b640c6702ac0da60200
-      00ab0200000000000000006517641a8400a6000000ab0000000000000000
-      00a6000000ab000000000000000000a6000000ab000000000000000000a6
-      000000ab0000000000000000005a1f6515a0160000000000000000000000
-      000000000000000000641b640b640c6702ac0da6020000ab020000000000
-      000000641c8400a6000000ab0000000000000000005a206515a016000000
-      0000000000000000000000000000000000641d640b640c6702ac0da60200
-      00ab0200000000000000006515a016000000000000000000000000000000
-      0000000000641e640b640c6702ac0da6020000ab02000000000000000065
-      17643b64208401a6000000ab000000000000000000a6000000ab00000000
-      0000000000a6000000ab0000000000000000005a216515a0160000000000
-      0000000000000000000000000000006421640b6701ac0da6020000ab0200
-      0000000000000064226522660264238404a6000000ab0000000000000000
-      005a236515a01600000000000000000000000000000000000000006424a6
-      010000ab01000000000000000064258400a6000000ab0000000000000000
-      005a246515a01600000000000000000000000000000000000000006426a6
-      010000ab01000000000000000064278400a6000000ab0000000000000000
-      005a256515a01600000000000000000000000000000000000000006428a6
-      010000ab01000000000000000064298400a6000000ab0000000000000000
-      005a266515a0160000000000000000000000000000000000000000642aa6
-      010000ab010000000000000000642b8400a6000000ab0000000000000000
-      005a276515a0160000000000000000000000000000000000000000642ca6
-      010000ab0100000000000000006517651d642d8400a6000000ab00000000
-      0000000000a6000000ab000000000000000000a6000000ab000000000000
-      0000005a286515a016000000000000000000000000000000000000000064
-      2ea6010000ab010000000000000000642f8400a6000000ab000000000000
-      0000005a296515a016000000000000000000000000000000000000000064
-      30a6010000ab01000000000000000064318400a6000000ab000000000000
-      0000005a2a6515a016000000000000000000000000000000000000000064
-      32a6010000ab01000000000000000064338400a6000000ab000000000000
-      0000005a2b6515a016000000000000000000000000000000000000000064
-      34640b6701ac0da6020000ab02000000000000000064358400a6000000ab
-      0000000000000000005a2c6515a016000000000000000000000000000000
-      00000000006436640b640c6702ac0da6020000ab02000000000000000065
-      17651d64378400a6000000ab000000000000000000a6000000ab00000000
-      0000000000a6000000ab0000000000000000005a2d6515a0160000000000
-      0000000000000000000000000000006438640b640c6702ac0da6020000ab
-      0200000000000000006517651d64398400a6000000ab0000000000000000
-      00a6000000ab000000000000000000a6000000ab0000000000000000005a
-      2e643a5300
+      00640064026c066d075a070100640064036c085a08640064046c096d0a5a
+      0a0100640064056c0b5400640064066c0c6d0d5a0d6d0e5a0e6d0f5a0f6d
+      105a106d115a110100640064076c126d135a136d145a1401000200650164
+      086515a6020000ab0200000000000000005a166516a01700000000000000
+      000000000000000000000000006409a6010000ab01000000000000000065
+      18640a8400a6000000ab000000000000000000a6000000ab000000000000
+      0000005a196516a017000000000000000000000000000000000000000064
+      0b640c640d6702ac0ea6020000ab0200000000000000006518640f8400a6
+      000000ab000000000000000000a6000000ab0000000000000000005a1a65
+      16a01700000000000000000000000000000000000000006410640c640d67
+      02ac0ea6020000ab020000000000000000651864118400a6000000ab0000
+      00000000000000a6000000ab0000000000000000005a1b6516a017000000
+      00000000000000000000000000000000006412a6010000ab010000000000
+      00000064138400a6000000ab0000000000000000005a1c6516a017000000
+      00000000000000000000000000000000006414a6010000ab010000000000
+      00000064158400a6000000ab0000000000000000005a1d6516a017000000
+      00000000000000000000000000000000006416a6010000ab010000000000
+      000000651e651864178400a6000000ab000000000000000000a6000000ab
+      000000000000000000a6000000ab0000000000000000005a1f6516a01700
+      000000000000000000000000000000000000006418640c640d6702ac0ea6
+      020000ab0200000000000000006516a01700000000000000000000000000
+      000000000000006419640c640d6702ac0ea6020000ab0200000000000000
+      006516a0170000000000000000000000000000000000000000641a640c64
+      0d6702ac0ea6020000ab0200000000000000006518641b8400a6000000ab
+      000000000000000000a6000000ab000000000000000000a6000000ab0000
+      00000000000000a6000000ab0000000000000000005a206516a017000000
+      0000000000000000000000000000000000641c640c640d6702ac0ea60200
+      00ab020000000000000000641d8400a6000000ab0000000000000000005a
+      216516a0170000000000000000000000000000000000000000641e640c64
+      0d6702ac0ea6020000ab0200000000000000006516a01700000000000000
+      00000000000000000000000000641f640c640d6702ac0ea6020000ab0200
+      000000000000006518643b64218401a6000000ab000000000000000000a6
+      000000ab000000000000000000a6000000ab0000000000000000005a2265
+      16a01700000000000000000000000000000000000000006422640c6701ac
+      0ea6020000ab02000000000000000064236523660264248404a6000000ab
+      0000000000000000005a246516a017000000000000000000000000000000
+      00000000006425a6010000ab01000000000000000064268400a6000000ab
+      0000000000000000005a256516a017000000000000000000000000000000
+      00000000006427a6010000ab01000000000000000064288400a6000000ab
+      0000000000000000005a266516a017000000000000000000000000000000
+      00000000006429a6010000ab010000000000000000642a8400a6000000ab
+      0000000000000000005a276516a017000000000000000000000000000000
+      0000000000642ba6010000ab010000000000000000642c8400a6000000ab
+      0000000000000000005a286516a017000000000000000000000000000000
+      0000000000642da6010000ab0100000000000000006518651e642e8400a6
+      000000ab000000000000000000a6000000ab000000000000000000a60000
+      00ab0000000000000000005a296516a01700000000000000000000000000
+      00000000000000642fa6010000ab01000000000000000064308400a60000
+      00ab0000000000000000005a2a6516a01700000000000000000000000000
+      000000000000006431a6010000ab01000000000000000064328400a60000
+      00ab0000000000000000005a2b6516a01700000000000000000000000000
+      000000000000006433a6010000ab01000000000000000064348400a60000
+      00ab0000000000000000005a2c6516a01700000000000000000000000000
+      000000000000006435640c6701ac0ea6020000ab02000000000000000064
+      368400a6000000ab0000000000000000005a2d6516a01700000000000000
+      000000000000000000000000006437640c640d6702ac0ea6020000ab0200
+      000000000000006518651e64388400a6000000ab000000000000000000a6
+      000000ab000000000000000000a6000000ab0000000000000000005a2e65
+      16a01700000000000000000000000000000000000000006439640c640d67
+      02ac0ea6020000ab0200000000000000006518651e643a8400a6000000ab
+      000000000000000000a6000000ab000000000000000000a6000000ab0000
+      000000000000005a2f64035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Blueprint', 'render_template', 'current_app', 'request', 'make_response'))
                  6 IMPORT_NAME              0 (flask)
                  8 IMPORT_FROM              1 (Blueprint)
                 10 STORE_NAME               1 (Blueprint)
@@ -90,499 +90,505 @@
      2          30 LOAD_CONST               0 (0)
                 32 LOAD_CONST               2 (('urlsplit',))
                 34 IMPORT_NAME              6 (urllib.parse)
                 36 IMPORT_FROM              7 (urlsplit)
                 38 STORE_NAME               7 (urlsplit)
                 40 POP_TOP
    
-     4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('JSONTable',))
-                46 IMPORT_NAME              8 (BOFS.JSONTable)
-                48 IMPORT_FROM              9 (JSONTable)
-                50 STORE_NAME               9 (JSONTable)
-                52 POP_TOP
-   
-     5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('*',))
-                58 IMPORT_NAME             10 (BOFS.util)
-                60 IMPORT_STAR
-   
-     6          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('db', 'referrer', 'page_list', 'questionnaires', 'tables'))
-                66 IMPORT_NAME             11 (BOFS.globals)
-                68 IMPORT_FROM             12 (db)
-                70 STORE_NAME              12 (db)
-                72 IMPORT_FROM             13 (referrer)
-                74 STORE_NAME              13 (referrer)
-                76 IMPORT_FROM             14 (page_list)
-                78 STORE_NAME              14 (page_list)
-                80 IMPORT_FROM             15 (questionnaires)
-                82 STORE_NAME              15 (questionnaires)
-                84 IMPORT_FROM             16 (tables)
-                86 STORE_NAME              16 (tables)
-                88 POP_TOP
-   
-     7          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               6 (('BOFSSessionInterface', 'BOFSSession'))
-                94 IMPORT_NAME             17 (BOFS.BOFSSession)
-                96 IMPORT_FROM             18 (BOFSSessionInterface)
-                98 STORE_NAME              18 (BOFSSessionInterface)
-               100 IMPORT_FROM             19 (BOFSSession)
-               102 STORE_NAME              19 (BOFSSession)
-               104 POP_TOP
-   
-    10         106 PUSH_NULL
-               108 LOAD_NAME                1 (Blueprint)
-               110 LOAD_CONST               7 ('default')
-               112 LOAD_NAME               20 (__name__)
-               114 PRECALL                  2
-               118 CALL                     2
-               128 STORE_NAME              21 (default)
-   
-    13         130 LOAD_NAME               21 (default)
-               132 LOAD_METHOD             22 (route)
-               154 LOAD_CONST               8 ('/')
-               156 PRECALL                  1
-               160 CALL                     1
-   
-    14         170 LOAD_NAME               23 (verify_correct_page)
-   
-    15         172 LOAD_CONST               9 (<code object route_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 13>)
-               174 MAKE_FUNCTION            0
-   
-    14         176 PRECALL                  0
-               180 CALL                     0
-   
-    13         190 PRECALL                  0
-               194 CALL                     0
-   
-    15         204 STORE_NAME              24 (route_index)
-   
-    19         206 LOAD_NAME               21 (default)
-               208 LOAD_METHOD             22 (route)
-               230 LOAD_CONST              10 ('/consent')
-               232 LOAD_CONST              11 ('POST')
-               234 LOAD_CONST              12 ('GET')
-               236 BUILD_LIST               2
-               238 KW_NAMES                13
-               240 PRECALL                  2
-               244 CALL                     2
-   
-    20         254 LOAD_NAME               23 (verify_correct_page)
-   
-    21         256 LOAD_CONST              14 (<code object route_consent, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 19>)
-               258 MAKE_FUNCTION            0
-   
-    20         260 PRECALL                  0
-               264 CALL                     0
-   
-    19         274 PRECALL                  0
-               278 CALL                     0
-   
-    21         288 STORE_NAME              25 (route_consent)
-   
-    45         290 LOAD_NAME               21 (default)
-               292 LOAD_METHOD             22 (route)
-               314 LOAD_CONST              15 ('/consent_nc')
-               316 LOAD_CONST              11 ('POST')
-               318 LOAD_CONST              12 ('GET')
-               320 BUILD_LIST               2
-               322 KW_NAMES                13
-               324 PRECALL                  2
-               328 CALL                     2
-   
-    46         338 LOAD_NAME               23 (verify_correct_page)
-   
-    47         340 LOAD_CONST              16 (<code object route_consent_nc, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 45>)
-               342 MAKE_FUNCTION            0
-   
-    46         344 PRECALL                  0
-               348 CALL                     0
-   
-    45         358 PRECALL                  0
-               362 CALL                     0
-   
-    47         372 STORE_NAME              26 (route_consent_nc)
-   
-    60         374 LOAD_NAME               21 (default)
-               376 LOAD_METHOD             22 (route)
-               398 LOAD_CONST              17 ('/create_participant')
-               400 PRECALL                  1
-               404 CALL                     1
-   
-    61         414 LOAD_CONST              18 (<code object route_create_participant, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 60>)
-               416 MAKE_FUNCTION            0
-   
-    60         418 PRECALL                  0
-               422 CALL                     0
-   
-    61         432 STORE_NAME              27 (route_create_participant)
-   
-    73         434 LOAD_NAME               21 (default)
-               436 LOAD_METHOD             22 (route)
-               458 LOAD_CONST              19 ('/create_participant_nc')
-               460 PRECALL                  1
-               464 CALL                     1
-   
-    74         474 LOAD_CONST              20 (<code object route_create_participant_nc, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 73>)
-               476 MAKE_FUNCTION            0
-   
-    73         478 PRECALL                  0
-               482 CALL                     0
-   
-    74         492 STORE_NAME              28 (route_create_participant_nc)
-   
-    88         494 LOAD_NAME               21 (default)
-               496 LOAD_METHOD             22 (route)
-               518 LOAD_CONST              21 ('/assign_condition')
-               520 PRECALL                  1
-               524 CALL                     1
-   
-    89         534 LOAD_NAME               29 (verify_session_valid)
-   
-    90         536 LOAD_NAME               23 (verify_correct_page)
-   
-    91         538 LOAD_CONST              22 (<code object route_assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 88>)
-               540 MAKE_FUNCTION            0
-   
-    90         542 PRECALL                  0
-               546 CALL                     0
-   
-    89         556 PRECALL                  0
-               560 CALL                     0
-   
-    88         570 PRECALL                  0
-               574 CALL                     0
-   
-    91         584 STORE_NAME              30 (route_assign_condition)
-   
-   111         586 LOAD_NAME               21 (default)
-               588 LOAD_METHOD             22 (route)
-               610 LOAD_CONST              23 ('/startMTurk')
-               612 LOAD_CONST              11 ('POST')
-               614 LOAD_CONST              12 ('GET')
-               616 BUILD_LIST               2
-               618 KW_NAMES                13
-               620 PRECALL                  2
-               624 CALL                     2
-   
-   112         634 LOAD_NAME               21 (default)
-               636 LOAD_METHOD             22 (route)
-               658 LOAD_CONST              24 ('/start_mturk')
-               660 LOAD_CONST              11 ('POST')
-               662 LOAD_CONST              12 ('GET')
-               664 BUILD_LIST               2
-               666 KW_NAMES                13
-               668 PRECALL                  2
-               672 CALL                     2
-   
-   113         682 LOAD_NAME               21 (default)
-               684 LOAD_METHOD             22 (route)
-               706 LOAD_CONST              25 ('/external_id')
-               708 LOAD_CONST              11 ('POST')
-               710 LOAD_CONST              12 ('GET')
-               712 BUILD_LIST               2
-               714 KW_NAMES                13
-               716 PRECALL                  2
-               720 CALL                     2
-   
-   114         730 LOAD_NAME               23 (verify_correct_page)
-   
-   115         732 LOAD_CONST              26 (<code object route_external_id, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 111>)
-               734 MAKE_FUNCTION            0
-   
-   114         736 PRECALL                  0
-               740 CALL                     0
-   
-   113         750 PRECALL                  0
-               754 CALL                     0
-   
-   112         764 PRECALL                  0
-               768 CALL                     0
-   
-   111         778 PRECALL                  0
-               782 CALL                     0
-   
-   115         792 STORE_NAME              31 (route_external_id)
-   
-   186         794 LOAD_NAME               21 (default)
-               796 LOAD_METHOD             22 (route)
-               818 LOAD_CONST              27 ('/table/<tableName>')
-               820 LOAD_CONST              11 ('POST')
-               822 LOAD_CONST              12 ('GET')
-               824 BUILD_LIST               2
-               826 KW_NAMES                13
-               828 PRECALL                  2
-               832 CALL                     2
-   
-   187         842 LOAD_CONST              28 (<code object route_table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 186>)
-               844 MAKE_FUNCTION            0
-   
-   186         846 PRECALL                  0
-               850 CALL                     0
-   
-   187         860 STORE_NAME              32 (route_table)
-   
-   204         862 LOAD_NAME               21 (default)
-               864 LOAD_METHOD             22 (route)
-               886 LOAD_CONST              29 ('/questionnaire/<questionnaireName>')
-               888 LOAD_CONST              11 ('POST')
-               890 LOAD_CONST              12 ('GET')
-               892 BUILD_LIST               2
-               894 KW_NAMES                13
-               896 PRECALL                  2
-               900 CALL                     2
-   
-   205         910 LOAD_NAME               21 (default)
-               912 LOAD_METHOD             22 (route)
-               934 LOAD_CONST              30 ('/questionnaire/<questionnaireName>/<tag>')
-               936 LOAD_CONST              11 ('POST')
-               938 LOAD_CONST              12 ('GET')
-               940 BUILD_LIST               2
-               942 KW_NAMES                13
-               944 PRECALL                  2
-               948 CALL                     2
-   
-   206         958 LOAD_NAME               23 (verify_correct_page)
-   
-   207         960 LOAD_CONST              59 (('',))
-               962 LOAD_CONST              32 (<code object route_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 204>)
-               964 MAKE_FUNCTION            1 (defaults)
-   
-   206         966 PRECALL                  0
-               970 CALL                     0
-   
-   205         980 PRECALL                  0
-               984 CALL                     0
-   
-   204         994 PRECALL                  0
-               998 CALL                     0
-   
-   207        1008 STORE_NAME              33 (route_questionnaire)
-   
-   234        1010 LOAD_NAME               21 (default)
-              1012 LOAD_METHOD             22 (route)
-              1034 LOAD_CONST              33 ('/questionnaire_question/<questionType>')
-              1036 LOAD_CONST              11 ('POST')
-              1038 BUILD_LIST               1
-              1040 KW_NAMES                13
-              1042 PRECALL                  2
-              1046 CALL                     2
-   
-   235        1056 LOAD_CONST              34 ('questionType')
-              1058 LOAD_NAME               34 (str)
-              1060 BUILD_TUPLE              2
-              1062 LOAD_CONST              35 (<code object route_questionnaire_question, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 234>)
-              1064 MAKE_FUNCTION            4 (annotations)
-   
-   234        1066 PRECALL                  0
-              1070 CALL                     0
-   
-   235        1080 STORE_NAME              35 (route_questionnaire_question)
-   
-   255        1082 LOAD_NAME               21 (default)
-              1084 LOAD_METHOD             22 (route)
-              1106 LOAD_CONST              36 ('/redirect_previous_page')
-              1108 PRECALL                  1
-              1112 CALL                     1
-   
-   256        1122 LOAD_CONST              37 (<code object route_redirect_previous_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 255>)
-              1124 MAKE_FUNCTION            0
-   
-   255        1126 PRECALL                  0
-              1130 CALL                     0
-   
-   256        1140 STORE_NAME              36 (route_redirect_previous_page)
-   
-   268        1142 LOAD_NAME               21 (default)
-              1144 LOAD_METHOD             22 (route)
-              1166 LOAD_CONST              38 ('/redirect_next_page')
-              1168 PRECALL                  1
-              1172 CALL                     1
-   
-   269        1182 LOAD_CONST              39 (<code object route_redirect_next_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 268>)
-              1184 MAKE_FUNCTION            0
-   
-   268        1186 PRECALL                  0
-              1190 CALL                     0
-   
-   269        1200 STORE_NAME              37 (route_redirect_next_page)
-   
-   292        1202 LOAD_NAME               21 (default)
-              1204 LOAD_METHOD             22 (route)
-              1226 LOAD_CONST              40 ('/redirect_from_page/<path:page>')
-              1228 PRECALL                  1
-              1232 CALL                     1
-   
-   293        1242 LOAD_CONST              41 (<code object route_redirect_from_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 292>)
-              1244 MAKE_FUNCTION            0
-   
-   292        1246 PRECALL                  0
-              1250 CALL                     0
-   
-   293        1260 STORE_NAME              38 (route_redirect_from_page)
-   
-   307        1262 LOAD_NAME               21 (default)
-              1264 LOAD_METHOD             22 (route)
-              1286 LOAD_CONST              42 ('/redirect_to_page/<path:page>')
-              1288 PRECALL                  1
-              1292 CALL                     1
-   
-   308        1302 LOAD_CONST              43 (<code object route_redirect_to_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 307>)
-              1304 MAKE_FUNCTION            0
-   
-   307        1306 PRECALL                  0
-              1310 CALL                     0
-   
-   308        1320 STORE_NAME              39 (route_redirect_to_page)
-   
-   322        1322 LOAD_NAME               21 (default)
-              1324 LOAD_METHOD             22 (route)
-              1346 LOAD_CONST              44 ('/end')
-              1348 PRECALL                  1
-              1352 CALL                     1
-   
-   323        1362 LOAD_NAME               23 (verify_correct_page)
-   
-   324        1364 LOAD_NAME               29 (verify_session_valid)
-   
-   325        1366 LOAD_CONST              45 (<code object route_end, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 322>)
-              1368 MAKE_FUNCTION            0
-   
-   324        1370 PRECALL                  0
-              1374 CALL                     0
-   
-   323        1384 PRECALL                  0
-              1388 CALL                     0
-   
-   322        1398 PRECALL                  0
-              1402 CALL                     0
-   
-   325        1412 STORE_NAME              40 (route_end)
-   
-   345        1414 LOAD_NAME               21 (default)
-              1416 LOAD_METHOD             22 (route)
-              1438 LOAD_CONST              46 ('/user_active')
-              1440 PRECALL                  1
-              1444 CALL                     1
-   
-   346        1454 LOAD_CONST              47 (<code object route_user_active, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 345>)
-              1456 MAKE_FUNCTION            0
-   
-   345        1458 PRECALL                  0
-              1462 CALL                     0
-   
-   346        1472 STORE_NAME              41 (route_user_active)
-   
-   354        1474 LOAD_NAME               21 (default)
-              1476 LOAD_METHOD             22 (route)
-              1498 LOAD_CONST              48 ('/current_url')
-              1500 PRECALL                  1
-              1504 CALL                     1
-   
-   355        1514 LOAD_CONST              49 (<code object route_current_url, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 354>)
-              1516 MAKE_FUNCTION            0
-   
-   354        1518 PRECALL                  0
-              1522 CALL                     0
-   
-   355        1532 STORE_NAME              42 (route_current_url)
-   
-   367        1534 LOAD_NAME               21 (default)
-              1536 LOAD_METHOD             22 (route)
-              1558 LOAD_CONST              50 ('/restart')
-              1560 PRECALL                  1
-              1564 CALL                     1
-   
-   368        1574 LOAD_CONST              51 (<code object route_restart, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 367>)
-              1576 MAKE_FUNCTION            0
-   
-   367        1578 PRECALL                  0
-              1582 CALL                     0
-   
-   368        1592 STORE_NAME              43 (route_restart)
-   
-   402        1594 LOAD_NAME               21 (default)
-              1596 LOAD_METHOD             22 (route)
-              1618 LOAD_CONST              52 ('/submit')
-              1620 LOAD_CONST              11 ('POST')
-              1622 BUILD_LIST               1
-              1624 KW_NAMES                13
-              1626 PRECALL                  2
-              1630 CALL                     2
-   
-   403        1640 LOAD_CONST              53 (<code object submit, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 402>)
-              1642 MAKE_FUNCTION            0
-   
-   402        1644 PRECALL                  0
-              1648 CALL                     0
-   
-   403        1658 STORE_NAME              44 (submit)
-   
-   416        1660 LOAD_NAME               21 (default)
-              1662 LOAD_METHOD             22 (route)
-              1684 LOAD_CONST              54 ('/instructions/<pageName>')
-              1686 LOAD_CONST              11 ('POST')
-              1688 LOAD_CONST              12 ('GET')
-              1690 BUILD_LIST               2
-              1692 KW_NAMES                13
-              1694 PRECALL                  2
-              1698 CALL                     2
-   
-   417        1708 LOAD_NAME               23 (verify_correct_page)
-   
-   418        1710 LOAD_NAME               29 (verify_session_valid)
-   
-   419        1712 LOAD_CONST              55 (<code object route_instructions, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 416>)
-              1714 MAKE_FUNCTION            0
-   
-   418        1716 PRECALL                  0
-              1720 CALL                     0
-   
-   417        1730 PRECALL                  0
-              1734 CALL                     0
-   
-   416        1744 PRECALL                  0
-              1748 CALL                     0
-   
-   419        1758 STORE_NAME              45 (route_instructions)
-   
-   445        1760 LOAD_NAME               21 (default)
-              1762 LOAD_METHOD             22 (route)
-              1784 LOAD_CONST              56 ('/simple/<pageName>')
-              1786 LOAD_CONST              11 ('POST')
-              1788 LOAD_CONST              12 ('GET')
-              1790 BUILD_LIST               2
-              1792 KW_NAMES                13
-              1794 PRECALL                  2
-              1798 CALL                     2
-   
-   446        1808 LOAD_NAME               23 (verify_correct_page)
-   
-   447        1810 LOAD_NAME               29 (verify_session_valid)
-   
-   448        1812 LOAD_CONST              57 (<code object route_simple_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 445>)
-              1814 MAKE_FUNCTION            0
-   
-   447        1816 PRECALL                  0
-              1820 CALL                     0
-   
-   446        1830 PRECALL                  0
-              1834 CALL                     0
-   
-   445        1844 PRECALL                  0
-              1848 CALL                     0
-   
-   448        1858 STORE_NAME              46 (route_simple_html)
-              1860 LOAD_CONST              58 (None)
-              1862 RETURN_VALUE
+     3          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               3 (None)
+                46 IMPORT_NAME              8 (traceback)
+                48 STORE_NAME               8 (traceback)
+   
+     4          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               4 (('JSONTable',))
+                54 IMPORT_NAME              9 (BOFS.JSONTable)
+                56 IMPORT_FROM             10 (JSONTable)
+                58 STORE_NAME              10 (JSONTable)
+                60 POP_TOP
+   
+     5          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('*',))
+                66 IMPORT_NAME             11 (BOFS.util)
+                68 IMPORT_STAR
+   
+     6          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('db', 'referrer', 'page_list', 'questionnaires', 'tables'))
+                74 IMPORT_NAME             12 (BOFS.globals)
+                76 IMPORT_FROM             13 (db)
+                78 STORE_NAME              13 (db)
+                80 IMPORT_FROM             14 (referrer)
+                82 STORE_NAME              14 (referrer)
+                84 IMPORT_FROM             15 (page_list)
+                86 STORE_NAME              15 (page_list)
+                88 IMPORT_FROM             16 (questionnaires)
+                90 STORE_NAME              16 (questionnaires)
+                92 IMPORT_FROM             17 (tables)
+                94 STORE_NAME              17 (tables)
+                96 POP_TOP
+   
+     7          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               7 (('BOFSSessionInterface', 'BOFSSession'))
+               102 IMPORT_NAME             18 (BOFS.BOFSSession)
+               104 IMPORT_FROM             19 (BOFSSessionInterface)
+               106 STORE_NAME              19 (BOFSSessionInterface)
+               108 IMPORT_FROM             20 (BOFSSession)
+               110 STORE_NAME              20 (BOFSSession)
+               112 POP_TOP
+   
+    10         114 PUSH_NULL
+               116 LOAD_NAME                1 (Blueprint)
+               118 LOAD_CONST               8 ('default')
+               120 LOAD_NAME               21 (__name__)
+               122 PRECALL                  2
+               126 CALL                     2
+               136 STORE_NAME              22 (default)
+   
+    13         138 LOAD_NAME               22 (default)
+               140 LOAD_METHOD             23 (route)
+               162 LOAD_CONST               9 ('/')
+               164 PRECALL                  1
+               168 CALL                     1
+   
+    14         178 LOAD_NAME               24 (verify_correct_page)
+   
+    15         180 LOAD_CONST              10 (<code object route_index, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 13>)
+               182 MAKE_FUNCTION            0
+   
+    14         184 PRECALL                  0
+               188 CALL                     0
+   
+    13         198 PRECALL                  0
+               202 CALL                     0
+   
+    15         212 STORE_NAME              25 (route_index)
+   
+    19         214 LOAD_NAME               22 (default)
+               216 LOAD_METHOD             23 (route)
+               238 LOAD_CONST              11 ('/consent')
+               240 LOAD_CONST              12 ('POST')
+               242 LOAD_CONST              13 ('GET')
+               244 BUILD_LIST               2
+               246 KW_NAMES                14
+               248 PRECALL                  2
+               252 CALL                     2
+   
+    20         262 LOAD_NAME               24 (verify_correct_page)
+   
+    21         264 LOAD_CONST              15 (<code object route_consent, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 19>)
+               266 MAKE_FUNCTION            0
+   
+    20         268 PRECALL                  0
+               272 CALL                     0
+   
+    19         282 PRECALL                  0
+               286 CALL                     0
+   
+    21         296 STORE_NAME              26 (route_consent)
+   
+    45         298 LOAD_NAME               22 (default)
+               300 LOAD_METHOD             23 (route)
+               322 LOAD_CONST              16 ('/consent_nc')
+               324 LOAD_CONST              12 ('POST')
+               326 LOAD_CONST              13 ('GET')
+               328 BUILD_LIST               2
+               330 KW_NAMES                14
+               332 PRECALL                  2
+               336 CALL                     2
+   
+    46         346 LOAD_NAME               24 (verify_correct_page)
+   
+    47         348 LOAD_CONST              17 (<code object route_consent_nc, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 45>)
+               350 MAKE_FUNCTION            0
+   
+    46         352 PRECALL                  0
+               356 CALL                     0
+   
+    45         366 PRECALL                  0
+               370 CALL                     0
+   
+    47         380 STORE_NAME              27 (route_consent_nc)
+   
+    60         382 LOAD_NAME               22 (default)
+               384 LOAD_METHOD             23 (route)
+               406 LOAD_CONST              18 ('/create_participant')
+               408 PRECALL                  1
+               412 CALL                     1
+   
+    61         422 LOAD_CONST              19 (<code object route_create_participant, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 60>)
+               424 MAKE_FUNCTION            0
+   
+    60         426 PRECALL                  0
+               430 CALL                     0
+   
+    61         440 STORE_NAME              28 (route_create_participant)
+   
+    73         442 LOAD_NAME               22 (default)
+               444 LOAD_METHOD             23 (route)
+               466 LOAD_CONST              20 ('/create_participant_nc')
+               468 PRECALL                  1
+               472 CALL                     1
+   
+    74         482 LOAD_CONST              21 (<code object route_create_participant_nc, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 73>)
+               484 MAKE_FUNCTION            0
+   
+    73         486 PRECALL                  0
+               490 CALL                     0
+   
+    74         500 STORE_NAME              29 (route_create_participant_nc)
+   
+    88         502 LOAD_NAME               22 (default)
+               504 LOAD_METHOD             23 (route)
+               526 LOAD_CONST              22 ('/assign_condition')
+               528 PRECALL                  1
+               532 CALL                     1
+   
+    89         542 LOAD_NAME               30 (verify_session_valid)
+   
+    90         544 LOAD_NAME               24 (verify_correct_page)
+   
+    91         546 LOAD_CONST              23 (<code object route_assign_condition, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 88>)
+               548 MAKE_FUNCTION            0
+   
+    90         550 PRECALL                  0
+               554 CALL                     0
+   
+    89         564 PRECALL                  0
+               568 CALL                     0
+   
+    88         578 PRECALL                  0
+               582 CALL                     0
+   
+    91         592 STORE_NAME              31 (route_assign_condition)
+   
+   111         594 LOAD_NAME               22 (default)
+               596 LOAD_METHOD             23 (route)
+               618 LOAD_CONST              24 ('/startMTurk')
+               620 LOAD_CONST              12 ('POST')
+               622 LOAD_CONST              13 ('GET')
+               624 BUILD_LIST               2
+               626 KW_NAMES                14
+               628 PRECALL                  2
+               632 CALL                     2
+   
+   112         642 LOAD_NAME               22 (default)
+               644 LOAD_METHOD             23 (route)
+               666 LOAD_CONST              25 ('/start_mturk')
+               668 LOAD_CONST              12 ('POST')
+               670 LOAD_CONST              13 ('GET')
+               672 BUILD_LIST               2
+               674 KW_NAMES                14
+               676 PRECALL                  2
+               680 CALL                     2
+   
+   113         690 LOAD_NAME               22 (default)
+               692 LOAD_METHOD             23 (route)
+               714 LOAD_CONST              26 ('/external_id')
+               716 LOAD_CONST              12 ('POST')
+               718 LOAD_CONST              13 ('GET')
+               720 BUILD_LIST               2
+               722 KW_NAMES                14
+               724 PRECALL                  2
+               728 CALL                     2
+   
+   114         738 LOAD_NAME               24 (verify_correct_page)
+   
+   115         740 LOAD_CONST              27 (<code object route_external_id, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 111>)
+               742 MAKE_FUNCTION            0
+   
+   114         744 PRECALL                  0
+               748 CALL                     0
+   
+   113         758 PRECALL                  0
+               762 CALL                     0
+   
+   112         772 PRECALL                  0
+               776 CALL                     0
+   
+   111         786 PRECALL                  0
+               790 CALL                     0
+   
+   115         800 STORE_NAME              32 (route_external_id)
+   
+   186         802 LOAD_NAME               22 (default)
+               804 LOAD_METHOD             23 (route)
+               826 LOAD_CONST              28 ('/table/<tableName>')
+               828 LOAD_CONST              12 ('POST')
+               830 LOAD_CONST              13 ('GET')
+               832 BUILD_LIST               2
+               834 KW_NAMES                14
+               836 PRECALL                  2
+               840 CALL                     2
+   
+   187         850 LOAD_CONST              29 (<code object route_table, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 186>)
+               852 MAKE_FUNCTION            0
+   
+   186         854 PRECALL                  0
+               858 CALL                     0
+   
+   187         868 STORE_NAME              33 (route_table)
+   
+   204         870 LOAD_NAME               22 (default)
+               872 LOAD_METHOD             23 (route)
+               894 LOAD_CONST              30 ('/questionnaire/<questionnaireName>')
+               896 LOAD_CONST              12 ('POST')
+               898 LOAD_CONST              13 ('GET')
+               900 BUILD_LIST               2
+               902 KW_NAMES                14
+               904 PRECALL                  2
+               908 CALL                     2
+   
+   205         918 LOAD_NAME               22 (default)
+               920 LOAD_METHOD             23 (route)
+               942 LOAD_CONST              31 ('/questionnaire/<questionnaireName>/<tag>')
+               944 LOAD_CONST              12 ('POST')
+               946 LOAD_CONST              13 ('GET')
+               948 BUILD_LIST               2
+               950 KW_NAMES                14
+               952 PRECALL                  2
+               956 CALL                     2
+   
+   206         966 LOAD_NAME               24 (verify_correct_page)
+   
+   207         968 LOAD_CONST              59 (('',))
+               970 LOAD_CONST              33 (<code object route_questionnaire, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 204>)
+               972 MAKE_FUNCTION            1 (defaults)
+   
+   206         974 PRECALL                  0
+               978 CALL                     0
+   
+   205         988 PRECALL                  0
+               992 CALL                     0
+   
+   204        1002 PRECALL                  0
+              1006 CALL                     0
+   
+   207        1016 STORE_NAME              34 (route_questionnaire)
+   
+   234        1018 LOAD_NAME               22 (default)
+              1020 LOAD_METHOD             23 (route)
+              1042 LOAD_CONST              34 ('/questionnaire_question/<questionType>')
+              1044 LOAD_CONST              12 ('POST')
+              1046 BUILD_LIST               1
+              1048 KW_NAMES                14
+              1050 PRECALL                  2
+              1054 CALL                     2
+   
+   235        1064 LOAD_CONST              35 ('questionType')
+              1066 LOAD_NAME               35 (str)
+              1068 BUILD_TUPLE              2
+              1070 LOAD_CONST              36 (<code object route_questionnaire_question, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 234>)
+              1072 MAKE_FUNCTION            4 (annotations)
+   
+   234        1074 PRECALL                  0
+              1078 CALL                     0
+   
+   235        1088 STORE_NAME              36 (route_questionnaire_question)
+   
+   260        1090 LOAD_NAME               22 (default)
+              1092 LOAD_METHOD             23 (route)
+              1114 LOAD_CONST              37 ('/redirect_previous_page')
+              1116 PRECALL                  1
+              1120 CALL                     1
+   
+   261        1130 LOAD_CONST              38 (<code object route_redirect_previous_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 260>)
+              1132 MAKE_FUNCTION            0
+   
+   260        1134 PRECALL                  0
+              1138 CALL                     0
+   
+   261        1148 STORE_NAME              37 (route_redirect_previous_page)
+   
+   273        1150 LOAD_NAME               22 (default)
+              1152 LOAD_METHOD             23 (route)
+              1174 LOAD_CONST              39 ('/redirect_next_page')
+              1176 PRECALL                  1
+              1180 CALL                     1
+   
+   274        1190 LOAD_CONST              40 (<code object route_redirect_next_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 273>)
+              1192 MAKE_FUNCTION            0
+   
+   273        1194 PRECALL                  0
+              1198 CALL                     0
+   
+   274        1208 STORE_NAME              38 (route_redirect_next_page)
+   
+   297        1210 LOAD_NAME               22 (default)
+              1212 LOAD_METHOD             23 (route)
+              1234 LOAD_CONST              41 ('/redirect_from_page/<path:page>')
+              1236 PRECALL                  1
+              1240 CALL                     1
+   
+   298        1250 LOAD_CONST              42 (<code object route_redirect_from_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 297>)
+              1252 MAKE_FUNCTION            0
+   
+   297        1254 PRECALL                  0
+              1258 CALL                     0
+   
+   298        1268 STORE_NAME              39 (route_redirect_from_page)
+   
+   312        1270 LOAD_NAME               22 (default)
+              1272 LOAD_METHOD             23 (route)
+              1294 LOAD_CONST              43 ('/redirect_to_page/<path:page>')
+              1296 PRECALL                  1
+              1300 CALL                     1
+   
+   313        1310 LOAD_CONST              44 (<code object route_redirect_to_page, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 312>)
+              1312 MAKE_FUNCTION            0
+   
+   312        1314 PRECALL                  0
+              1318 CALL                     0
+   
+   313        1328 STORE_NAME              40 (route_redirect_to_page)
+   
+   327        1330 LOAD_NAME               22 (default)
+              1332 LOAD_METHOD             23 (route)
+              1354 LOAD_CONST              45 ('/end')
+              1356 PRECALL                  1
+              1360 CALL                     1
+   
+   328        1370 LOAD_NAME               24 (verify_correct_page)
+   
+   329        1372 LOAD_NAME               30 (verify_session_valid)
+   
+   330        1374 LOAD_CONST              46 (<code object route_end, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 327>)
+              1376 MAKE_FUNCTION            0
+   
+   329        1378 PRECALL                  0
+              1382 CALL                     0
+   
+   328        1392 PRECALL                  0
+              1396 CALL                     0
+   
+   327        1406 PRECALL                  0
+              1410 CALL                     0
+   
+   330        1420 STORE_NAME              41 (route_end)
+   
+   350        1422 LOAD_NAME               22 (default)
+              1424 LOAD_METHOD             23 (route)
+              1446 LOAD_CONST              47 ('/user_active')
+              1448 PRECALL                  1
+              1452 CALL                     1
+   
+   351        1462 LOAD_CONST              48 (<code object route_user_active, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 350>)
+              1464 MAKE_FUNCTION            0
+   
+   350        1466 PRECALL                  0
+              1470 CALL                     0
+   
+   351        1480 STORE_NAME              42 (route_user_active)
+   
+   359        1482 LOAD_NAME               22 (default)
+              1484 LOAD_METHOD             23 (route)
+              1506 LOAD_CONST              49 ('/current_url')
+              1508 PRECALL                  1
+              1512 CALL                     1
+   
+   360        1522 LOAD_CONST              50 (<code object route_current_url, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 359>)
+              1524 MAKE_FUNCTION            0
+   
+   359        1526 PRECALL                  0
+              1530 CALL                     0
+   
+   360        1540 STORE_NAME              43 (route_current_url)
+   
+   372        1542 LOAD_NAME               22 (default)
+              1544 LOAD_METHOD             23 (route)
+              1566 LOAD_CONST              51 ('/restart')
+              1568 PRECALL                  1
+              1572 CALL                     1
+   
+   373        1582 LOAD_CONST              52 (<code object route_restart, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 372>)
+              1584 MAKE_FUNCTION            0
+   
+   372        1586 PRECALL                  0
+              1590 CALL                     0
+   
+   373        1600 STORE_NAME              44 (route_restart)
+   
+   407        1602 LOAD_NAME               22 (default)
+              1604 LOAD_METHOD             23 (route)
+              1626 LOAD_CONST              53 ('/submit')
+              1628 LOAD_CONST              12 ('POST')
+              1630 BUILD_LIST               1
+              1632 KW_NAMES                14
+              1634 PRECALL                  2
+              1638 CALL                     2
+   
+   408        1648 LOAD_CONST              54 (<code object submit, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 407>)
+              1650 MAKE_FUNCTION            0
+   
+   407        1652 PRECALL                  0
+              1656 CALL                     0
+   
+   408        1666 STORE_NAME              45 (submit)
+   
+   421        1668 LOAD_NAME               22 (default)
+              1670 LOAD_METHOD             23 (route)
+              1692 LOAD_CONST              55 ('/instructions/<pageName>')
+              1694 LOAD_CONST              12 ('POST')
+              1696 LOAD_CONST              13 ('GET')
+              1698 BUILD_LIST               2
+              1700 KW_NAMES                14
+              1702 PRECALL                  2
+              1706 CALL                     2
+   
+   422        1716 LOAD_NAME               24 (verify_correct_page)
+   
+   423        1718 LOAD_NAME               30 (verify_session_valid)
+   
+   424        1720 LOAD_CONST              56 (<code object route_instructions, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 421>)
+              1722 MAKE_FUNCTION            0
+   
+   423        1724 PRECALL                  0
+              1728 CALL                     0
+   
+   422        1738 PRECALL                  0
+              1742 CALL                     0
+   
+   421        1752 PRECALL                  0
+              1756 CALL                     0
+   
+   424        1766 STORE_NAME              46 (route_instructions)
+   
+   450        1768 LOAD_NAME               22 (default)
+              1770 LOAD_METHOD             23 (route)
+              1792 LOAD_CONST              57 ('/simple/<pageName>')
+              1794 LOAD_CONST              12 ('POST')
+              1796 LOAD_CONST              13 ('GET')
+              1798 BUILD_LIST               2
+              1800 KW_NAMES                14
+              1802 PRECALL                  2
+              1806 CALL                     2
+   
+   451        1816 LOAD_NAME               24 (verify_correct_page)
+   
+   452        1818 LOAD_NAME               30 (verify_session_valid)
+   
+   453        1820 LOAD_CONST              58 (<code object route_simple_html, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\default\views.py", line 450>)
+              1822 MAKE_FUNCTION            0
+   
+   452        1824 PRECALL                  0
+              1828 CALL                     0
+   
+   451        1838 PRECALL                  0
+              1842 CALL                     0
+   
+   450        1852 PRECALL                  0
+              1856 CALL                     0
+   
+   453        1866 STORE_NAME              47 (route_simple_html)
+              1868 LOAD_CONST               3 (None)
+              1870 RETURN_VALUE
    consts
       0
       ('Blueprint', 'render_template', 'current_app', 'request', 'make_response')
       ('urlsplit',)
+      None
       ('JSONTable',)
       ('*',)
       ('db', 'referrer', 'page_list', 'questionnaires', 'tables')
       ('BOFSSessionInterface', 'BOFSSession')
       'default'
       '/'
       code
@@ -1392,28 +1398,33 @@
          name       'route_questionnaire'
          firstlineno 204
          lnotab 0x02111a0220012a024e020e0102010c013afd
       '/questionnaire_question/<questionType>'
       'questionType'
       code
          argcount  : 1
-         nlocals   : 3
-         stacksize : 5
+         nlocals   : 4
+         stacksize : 6
          flags     : 3
          code
             0x970064017400000000000000000000007601720f740300000000000000
             0000006402a6010000ab0100000000000000008201740400000000000000
             0000006a0300000000000000006a040000000000000000a0050000000000
             000000000000000000000000000000740000000000000000000000640119
             000000000000000000a6010000ab0100000000000000007d010900740d00
             00000000000000000064037c009b0064049d03740e000000000000000000
             006a0800000000000000007c01ac05a6030000ab03000000000000000053
-            002300740200000000000000000000240072127d0264067c009b0064077c
-            029b009d046302590064087d027e02530064087d027e0277017700780359
-            007701
+            002300740200000000000000000000240072647d02741200000000000000
+            0000006a0a000000000000000072377417000000000000000000007c02a6
+            010000ab01000000000000000064067a0000007417000000000000000000
+            007419000000000000000000006a0d0000000000000000a6000000ab0000
+            00000000000000a6010000ab0100000000000000007a00000064077a0000
+            007d036e0f7417000000000000000000007c02a6010000ab010000000000
+            0000007d0364087c009b0064097c039b009d0463025900640a7d027e0253
+            00640a7d027e0277017700780359007701
          234           0 RESUME                   0
          
          242           2 LOAD_CONST               1 ('participantID')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              1
                       18 POP_JUMP_FORWARD_IF_FALSE    15 (to 50)
          
@@ -1452,103 +1463,134 @@
                      194 PRECALL                  3
                      198 CALL                     3
                      208 RETURN_VALUE
                  >>  210 PUSH_EXC_INFO
          
          251         212 LOAD_GLOBAL              2 (Exception)
                      224 CHECK_EXC_MATCH
-                     226 POP_JUMP_FORWARD_IF_FALSE    18 (to 264)
+                     226 POP_JUMP_FORWARD_IF_FALSE   100 (to 428)
                      228 STORE_FAST               2 (ex)
          
-         252         230 LOAD_CONST               6 ('Exception in <b>')
-                     232 LOAD_FAST                0 (questionType)
-                     234 FORMAT_VALUE             0
-                     236 LOAD_CONST               7 ('.html</b>: ')
-                     238 LOAD_FAST                2 (ex)
-                     240 FORMAT_VALUE             0
-                     242 BUILD_STRING             4
-                     244 SWAP                     2
-                     246 POP_EXCEPT
-                     248 LOAD_CONST               8 (None)
-                     250 STORE_FAST               2 (ex)
-                     252 DELETE_FAST              2 (ex)
-                     254 RETURN_VALUE
-                 >>  256 LOAD_CONST               8 (None)
-                     258 STORE_FAST               2 (ex)
-                     260 DELETE_FAST              2 (ex)
-                     262 RERAISE                  1
-         
-         251     >>  264 RERAISE                  0
-                 >>  266 COPY                     3
-                     268 POP_EXCEPT
-                     270 RERAISE                  1
+         252         230 LOAD_GLOBAL             18 (current_app)
+                     242 LOAD_ATTR               10 (run_with_debugging)
+                     252 POP_JUMP_FORWARD_IF_FALSE    55 (to 364)
+         
+         253         254 LOAD_GLOBAL             23 (NULL + str)
+                     266 LOAD_FAST                2 (ex)
+                     268 PRECALL                  1
+                     272 CALL                     1
+                     282 LOAD_CONST               6 ('<p><pre>')
+                     284 BINARY_OP                0 (+)
+                     288 LOAD_GLOBAL             23 (NULL + str)
+                     300 LOAD_GLOBAL             25 (NULL + traceback)
+                     312 LOAD_ATTR               13 (format_exc)
+                     322 PRECALL                  0
+                     326 CALL                     0
+                     336 PRECALL                  1
+                     340 CALL                     1
+                     350 BINARY_OP                0 (+)
+                     354 LOAD_CONST               7 ('</pre>')
+                     356 BINARY_OP                0 (+)
+                     360 STORE_FAST               3 (debugging_info)
+                     362 JUMP_FORWARD            15 (to 394)
+         
+         255     >>  364 LOAD_GLOBAL             23 (NULL + str)
+                     376 LOAD_FAST                2 (ex)
+                     378 PRECALL                  1
+                     382 CALL                     1
+                     392 STORE_FAST               3 (debugging_info)
+         
+         257     >>  394 LOAD_CONST               8 ('Exception in <b>')
+                     396 LOAD_FAST                0 (questionType)
+                     398 FORMAT_VALUE             0
+                     400 LOAD_CONST               9 ('.html</b>: ')
+                     402 LOAD_FAST                3 (debugging_info)
+                     404 FORMAT_VALUE             0
+                     406 BUILD_STRING             4
+                     408 SWAP                     2
+                     410 POP_EXCEPT
+                     412 LOAD_CONST              10 (None)
+                     414 STORE_FAST               2 (ex)
+                     416 DELETE_FAST              2 (ex)
+                     418 RETURN_VALUE
+                 >>  420 LOAD_CONST              10 (None)
+                     422 STORE_FAST               2 (ex)
+                     424 DELETE_FAST              2 (ex)
+                     426 RERAISE                  1
+         
+         251     >>  428 RERAISE                  0
+                 >>  430 COPY                     3
+                     432 POP_EXCEPT
+                     434 RERAISE                  1
          ExceptionTable:
            146 to 206 -> 210 [0]
-           210 to 228 -> 266 [1] lasti
-           230 to 242 -> 256 [1] lasti
-           244 to 244 -> 266 [1] lasti
-           256 to 264 -> 266 [1] lasti
+           210 to 228 -> 430 [1] lasti
+           230 to 406 -> 420 [1] lasti
+           408 to 408 -> 430 [1] lasti
+           420 to 428 -> 430 [1] lasti
          consts
             '\n    ``/questionnaire_question/<questionType>``\n\n    Render a specific question type for the questionnaire. Only accepts POST requests.\n    Data posted to this route must be a JSON object of the question data.\n    '
             'participantID'
             'Error: No participantID in session. Did you forget /consent or /create_participant, etc.?'
             'questions/'
             '.html'
             ('question', 'participant')
+            '<p><pre>'
+            '</pre>'
             'Exception in <b>'
             '.html</b>: '
             None
-         names      ('session', 'Exception', 'db', 'Participant', 'query', 'get', 'render_template', 'request', 'json')
-         varnames   ('questionType', 'participant', 'ex')
+         names      ('session', 'Exception', 'db', 'Participant', 'query', 'get', 'render_template', 'request', 'json', 'current_app', 'run_with_debugging', 'str', 'traceback', 'format_exc')
+         varnames   ('questionType', 'participant', 'ex', 'debugging_info')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_questionnaire_question'
          firstlineno 234
-         lnotab 0x020812011e025e0202011601160102fe1403120122ff
+         lnotab 0x020812011e025e0202011601160102fe1403120118016e021e0222fa
       '/redirect_previous_page'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007404000000
             00000000000000640119000000000000000000a6010000ab010000000000
             00000074040000000000000000000064013c000000740600000000000000
             0000006a04000000000000000064021900000000000000000064037a0000
             007404000000000000000000006401190000000000000000007a0000007d
             00740b000000000000000000007c00a6010000ab01000000000000000053
             00
-         255           0 RESUME                   0
+         260           0 RESUME                   0
          
-         262           2 LOAD_GLOBAL              1 (NULL + page_list)
+         267           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (previous_path)
                       24 LOAD_GLOBAL              4 (session)
                       36 LOAD_CONST               1 ('currentUrl')
                       38 BINARY_SUBSCR
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_GLOBAL              4 (session)
                       74 LOAD_CONST               1 ('currentUrl')
                       76 STORE_SUBSCR
          
-         263          80 LOAD_GLOBAL              6 (current_app)
+         268          80 LOAD_GLOBAL              6 (current_app)
                       92 LOAD_ATTR                4 (config)
                      102 LOAD_CONST               2 ('APPLICATION_ROOT')
                      104 BINARY_SUBSCR
                      114 LOAD_CONST               3 ('/')
                      116 BINARY_OP                0 (+)
                      120 LOAD_GLOBAL              4 (session)
                      132 LOAD_CONST               1 ('currentUrl')
                      134 BINARY_SUBSCR
                      144 BINARY_OP                0 (+)
                      148 STORE_FAST               0 (nextUrl)
          
-         265         150 LOAD_GLOBAL             11 (NULL + redirect)
+         270         150 LOAD_GLOBAL             11 (NULL + redirect)
                      162 LOAD_FAST                0 (nextUrl)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 RETURN_VALUE
          consts
             '\n    ``/redirect_previous_page``\n\n    Sends a user to the previous page. This is intended primarily for debugging purposes.\n    '
             'currentUrl'
@@ -1556,15 +1598,15 @@
             '/'
          names      ('page_list', 'previous_path', 'session', 'current_app', 'config', 'redirect')
          varnames   ('nextUrl',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_previous_page'
-         firstlineno 255
+         firstlineno 260
          lnotab 0x02074e014602
       '/redirect_next_page'
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 4
          flags     : 3
@@ -1578,77 +1620,77 @@
             041900000000000000000064057a000000a6010000ab0100000000000000
             0053007411000000000000000000006a0900000000000000007c01a60100
             00ab01000000000000000074080000000000000000000064023c00000074
             0c000000000000000000006a070000000000000000640419000000000000
             00000064067a000000740800000000000000000000640219000000000000
             0000007a0000007d02740b000000000000000000007c02a6010000ab0100
             000000000000005300
-         268           0 RESUME                   0
+         273           0 RESUME                   0
          
-         275           2 LOAD_GLOBAL              0 (request)
+         280           2 LOAD_GLOBAL              0 (request)
                       14 POP_JUMP_FORWARD_IF_NONE    45 (to 106)
                       16 LOAD_GLOBAL              0 (request)
                       28 LOAD_ATTR                1 (referrer)
                       38 POP_JUMP_FORWARD_IF_NONE    33 (to 106)
          
-         276          40 LOAD_GLOBAL              5 (NULL + urlsplit)
+         281          40 LOAD_GLOBAL              5 (NULL + urlsplit)
                       52 LOAD_GLOBAL              0 (request)
                       64 LOAD_ATTR                1 (referrer)
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               0 (parsed)
          
-         277          90 LOAD_FAST                0 (parsed)
+         282          90 LOAD_FAST                0 (parsed)
                       92 LOAD_ATTR                3 (path)
                      102 STORE_FAST               1 (current_page)
                      104 JUMP_FORWARD            13 (to 132)
          
-         281     >>  106 LOAD_GLOBAL              8 (session)
+         286     >>  106 LOAD_GLOBAL              8 (session)
                      118 LOAD_CONST               2 ('currentUrl')
                      120 BINARY_SUBSCR
                      130 STORE_FAST               1 (current_page)
          
-         283     >>  132 LOAD_FAST                1 (current_page)
+         288     >>  132 LOAD_FAST                1 (current_page)
                      134 LOAD_CONST               3 ('end')
                      136 COMPARE_OP               2 (==)
                      142 POP_JUMP_FORWARD_IF_FALSE    34 (to 212)
          
-         284         144 LOAD_GLOBAL             11 (NULL + redirect)
+         289         144 LOAD_GLOBAL             11 (NULL + redirect)
                      156 LOAD_GLOBAL             12 (current_app)
                      168 LOAD_ATTR                7 (config)
                      178 LOAD_CONST               4 ('APPLICATION_ROOT')
                      180 BINARY_SUBSCR
                      190 LOAD_CONST               5 ('/end')
                      192 BINARY_OP                0 (+)
                      196 PRECALL                  1
                      200 CALL                     1
                      210 RETURN_VALUE
          
-         286     >>  212 LOAD_GLOBAL             17 (NULL + page_list)
+         291     >>  212 LOAD_GLOBAL             17 (NULL + page_list)
                      224 LOAD_ATTR                9 (next_path)
                      234 LOAD_FAST                1 (current_page)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_GLOBAL              8 (session)
                      262 LOAD_CONST               2 ('currentUrl')
                      264 STORE_SUBSCR
          
-         287         268 LOAD_GLOBAL             12 (current_app)
+         292         268 LOAD_GLOBAL             12 (current_app)
                      280 LOAD_ATTR                7 (config)
                      290 LOAD_CONST               4 ('APPLICATION_ROOT')
                      292 BINARY_SUBSCR
                      302 LOAD_CONST               6 ('/')
                      304 BINARY_OP                0 (+)
                      308 LOAD_GLOBAL              8 (session)
                      320 LOAD_CONST               2 ('currentUrl')
                      322 BINARY_SUBSCR
                      332 BINARY_OP                0 (+)
                      336 STORE_FAST               2 (nextUrl)
          
-         289         338 LOAD_GLOBAL             11 (NULL + redirect)
+         294         338 LOAD_GLOBAL             11 (NULL + redirect)
                      350 LOAD_FAST                2 (nextUrl)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 RETURN_VALUE
          consts
             '\n    ``/redirect_next_page``\n\n    This is the preferred way of sending a user to the next page.\n    '
             None
@@ -1659,53 +1701,53 @@
             '/'
          names      ('request', 'referrer', 'urlsplit', 'path', 'session', 'redirect', 'current_app', 'config', 'page_list', 'next_path')
          varnames   ('parsed', 'current_page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_next_page'
-         firstlineno 268
+         firstlineno 273
          lnotab 0x02072601320110041a020c01440238014602
       '/redirect_from_page/<path:page>'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a60100
             00ab01000000000000000074040000000000000000000064013c00000074
             06000000000000000000006a040000000000000000640219000000000000
             00000064037a000000740400000000000000000000640119000000000000
             0000007a0000007d01740b000000000000000000007c01a6010000ab0100
             000000000000005300
-         292           0 RESUME                   0
+         297           0 RESUME                   0
          
-         301           2 LOAD_GLOBAL              1 (NULL + page_list)
+         306           2 LOAD_GLOBAL              1 (NULL + page_list)
                       14 LOAD_ATTR                1 (next_path)
                       24 LOAD_FAST                0 (page)
                       26 PRECALL                  1
                       30 CALL                     1
                       40 LOAD_GLOBAL              4 (session)
                       52 LOAD_CONST               1 ('currentUrl')
                       54 STORE_SUBSCR
          
-         302          58 LOAD_GLOBAL              6 (current_app)
+         307          58 LOAD_GLOBAL              6 (current_app)
                       70 LOAD_ATTR                4 (config)
                       80 LOAD_CONST               2 ('APPLICATION_ROOT')
                       82 BINARY_SUBSCR
                       92 LOAD_CONST               3 ('/')
                       94 BINARY_OP                0 (+)
                       98 LOAD_GLOBAL              4 (session)
                      110 LOAD_CONST               1 ('currentUrl')
                      112 BINARY_SUBSCR
                      122 BINARY_OP                0 (+)
                      126 STORE_FAST               1 (nextUrl)
          
-         304         128 LOAD_GLOBAL             11 (NULL + redirect)
+         309         128 LOAD_GLOBAL             11 (NULL + redirect)
                      140 LOAD_FAST                1 (nextUrl)
                      142 PRECALL                  1
                      146 CALL                     1
                      156 RETURN_VALUE
          consts
             '\n    ``/redirect_from_page/<path:page>``\n\n    Redirect the user from a specific page.\n\n    :param page: The page to start from, the user will be sent to next page in the list\n    '
             'currentUrl'
@@ -1713,48 +1755,48 @@
             '/'
          names      ('page_list', 'next_path', 'session', 'current_app', 'config', 'redirect')
          varnames   ('page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_from_page'
-         firstlineno 292
+         firstlineno 297
          lnotab 0x020938014602
       '/redirect_to_page/<path:page>'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007c0074000000000000000000000064013c00000074020000000000
             00000000006a02000000000000000064021900000000000000000064037a
             0000007400000000000000000000006401190000000000000000007a0000
             007d017407000000000000000000007c01a6010000ab0100000000000000
             005300
-         307           0 RESUME                   0
+         312           0 RESUME                   0
          
-         316           2 LOAD_FAST                0 (page)
+         321           2 LOAD_FAST                0 (page)
                        4 LOAD_GLOBAL              0 (session)
                       16 LOAD_CONST               1 ('currentUrl')
                       18 STORE_SUBSCR
          
-         317          22 LOAD_GLOBAL              2 (current_app)
+         322          22 LOAD_GLOBAL              2 (current_app)
                       34 LOAD_ATTR                2 (config)
                       44 LOAD_CONST               2 ('APPLICATION_ROOT')
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               3 ('/')
                       58 BINARY_OP                0 (+)
                       62 LOAD_GLOBAL              0 (session)
                       74 LOAD_CONST               1 ('currentUrl')
                       76 BINARY_SUBSCR
                       86 BINARY_OP                0 (+)
                       90 STORE_FAST               1 (nextUrl)
          
-         319          92 LOAD_GLOBAL              7 (NULL + redirect)
+         324          92 LOAD_GLOBAL              7 (NULL + redirect)
                      104 LOAD_FAST                1 (nextUrl)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 RETURN_VALUE
          consts
             '\n    ``/redirect_to_page/<path:page>``\n\n    Redirect the user to a specific page path in ``PAGE_LIST``\n\n    :param page:\n    '
             'currentUrl'
@@ -1762,15 +1804,15 @@
             '/'
          names      ('session', 'current_app', 'config', 'redirect')
          varnames   ('page', 'nextUrl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_redirect_to_page'
-         firstlineno 307
+         firstlineno 312
          lnotab 0x020914014602
       '/end'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 5
          flags     : 3
@@ -1787,71 +1829,71 @@
             0b0000000000000000760072317414000000000000000000006a0b000000
             0000000000640419000000000000000000811f7419000000000000000000
             007414000000000000000000006a0b000000000000000064041900000000
             0000000000a6010000ab0100000000000000005300741b00000000000000
             000000640564067408000000000000000000007600720d74080000000000
             00000000006406190000000000000000006e016402ac07a6020000ab0200
             000000000000005300
-         322           0 RESUME                   0
+         327           0 RESUME                   0
          
-         332           2 LOAD_GLOBAL              0 (db)
+         337           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (Participant)
                       24 LOAD_ATTR                2 (query)
                       34 LOAD_METHOD              3 (get)
                       56 LOAD_GLOBAL              8 (session)
                       68 LOAD_CONST               1 ('participantID')
                       70 BINARY_SUBSCR
                       80 PRECALL                  1
                       84 CALL                     1
                       94 STORE_FAST               0 (p)
          
-         333          96 LOAD_FAST                0 (p)
+         338          96 LOAD_FAST                0 (p)
                       98 LOAD_ATTR                5 (timeEnded)
                      108 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 180)
          
-         334         110 LOAD_GLOBAL             12 (datetime)
+         339         110 LOAD_GLOBAL             12 (datetime)
                      122 LOAD_ATTR                6 (datetime)
                      132 LOAD_METHOD              7 (utcnow)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 LOAD_FAST                0 (p)
                      170 STORE_ATTR               5 (timeEnded)
          
-         335     >>  180 LOAD_CONST               3 (True)
+         340     >>  180 LOAD_CONST               3 (True)
                      182 LOAD_FAST                0 (p)
                      184 STORE_ATTR               8 (finished)
          
-         337         194 LOAD_GLOBAL              0 (db)
+         342         194 LOAD_GLOBAL              0 (db)
                      206 LOAD_ATTR                4 (session)
                      216 LOAD_METHOD              9 (commit)
                      238 PRECALL                  0
                      242 CALL                     0
                      252 POP_TOP
          
-         339         254 LOAD_CONST               4 ('OUTGOING_URL')
+         344         254 LOAD_CONST               4 ('OUTGOING_URL')
                      256 LOAD_GLOBAL             20 (current_app)
                      268 LOAD_ATTR               11 (config)
                      278 CONTAINS_OP              0
                      280 POP_JUMP_FORWARD_IF_FALSE    49 (to 380)
                      282 LOAD_GLOBAL             20 (current_app)
                      294 LOAD_ATTR               11 (config)
                      304 LOAD_CONST               4 ('OUTGOING_URL')
                      306 BINARY_SUBSCR
                      316 POP_JUMP_FORWARD_IF_NONE    31 (to 380)
          
-         340         318 LOAD_GLOBAL             25 (NULL + redirect)
+         345         318 LOAD_GLOBAL             25 (NULL + redirect)
                      330 LOAD_GLOBAL             20 (current_app)
                      342 LOAD_ATTR               11 (config)
                      352 LOAD_CONST               4 ('OUTGOING_URL')
                      354 BINARY_SUBSCR
                      364 PRECALL                  1
                      368 CALL                     1
                      378 RETURN_VALUE
          
-         342     >>  380 LOAD_GLOBAL             27 (NULL + render_template)
+         347     >>  380 LOAD_GLOBAL             27 (NULL + render_template)
                      392 LOAD_CONST               5 ('end.html')
                      394 LOAD_CONST               6 ('code')
                      396 LOAD_GLOBAL              8 (session)
                      408 CONTAINS_OP              0
                      410 POP_JUMP_FORWARD_IF_FALSE    13 (to 438)
                      412 LOAD_GLOBAL              8 (session)
                      424 LOAD_CONST               6 ('code')
@@ -1873,15 +1915,15 @@
             ('code',)
          names      ('db', 'Participant', 'query', 'get', 'session', 'timeEnded', 'datetime', 'utcnow', 'finished', 'commit', 'current_app', 'config', 'redirect', 'render_template')
          varnames   ('p',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_end'
-         firstlineno 322
+         firstlineno 327
          lnotab 0x020a5e010e0146010e023c0240013e02
       '/user_active'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
@@ -1892,99 +1934,99 @@
             00ab010000000000000000a0040000000000000000000000000000000000
             000000740000000000000000000000640119000000000000000000a60100
             00ab0100000000000000007d00740a000000000000000000006a05000000
             0000000000a0060000000000000000000000000000000000000000a60000
             00ab0000000000000000007c005f07000000000000000074020000000000
             00000000006a000000000000000000a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000010064025300
-         345           0 RESUME                   0
+         350           0 RESUME                   0
          
-         347           2 LOAD_CONST               1 ('participantID')
+         352           2 LOAD_CONST               1 ('participantID')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              0
                       18 POP_JUMP_FORWARD_IF_FALSE   136 (to 292)
          
-         348          20 LOAD_GLOBAL              2 (db)
+         353          20 LOAD_GLOBAL              2 (db)
                       32 LOAD_ATTR                0 (session)
                       42 LOAD_METHOD              2 (query)
                       64 LOAD_GLOBAL              2 (db)
                       76 LOAD_ATTR                3 (Participant)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_METHOD              4 (get)
                      122 LOAD_GLOBAL              0 (session)
                      134 LOAD_CONST               1 ('participantID')
                      136 BINARY_SUBSCR
                      146 PRECALL                  1
                      150 CALL                     1
                      160 STORE_FAST               0 (participant)
          
-         349         162 LOAD_GLOBAL             10 (datetime)
+         354         162 LOAD_GLOBAL             10 (datetime)
                      174 LOAD_ATTR                5 (datetime)
                      184 LOAD_METHOD              6 (utcnow)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 LOAD_FAST                0 (participant)
                      222 STORE_ATTR               7 (lastActiveOn)
          
-         350         232 LOAD_GLOBAL              2 (db)
+         355         232 LOAD_GLOBAL              2 (db)
                      244 LOAD_ATTR                0 (session)
                      254 LOAD_METHOD              8 (commit)
                      276 PRECALL                  0
                      280 CALL                     0
                      290 POP_TOP
          
-         351     >>  292 LOAD_CONST               2 ('')
+         356     >>  292 LOAD_CONST               2 ('')
                      294 RETURN_VALUE
          consts
             None
             'participantID'
             ''
          names      ('session', 'db', 'query', 'Participant', 'get', 'datetime', 'utcnow', 'lastActiveOn', 'commit')
          varnames   ('participant',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_user_active'
-         firstlineno 345
+         firstlineno 350
          lnotab 0x020212018e0146013c01
       '/current_url'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 3
          code
             0x970064017400000000000000000000007600720d740000000000000000
             000000640119000000000000000000530064025300
-         354           0 RESUME                   0
+         359           0 RESUME                   0
          
-         361           2 LOAD_CONST               1 ('currentUrl')
+         366           2 LOAD_CONST               1 ('currentUrl')
                        4 LOAD_GLOBAL              0 (session)
                       16 CONTAINS_OP              0
                       18 POP_JUMP_FORWARD_IF_FALSE    13 (to 46)
          
-         362          20 LOAD_GLOBAL              0 (session)
+         367          20 LOAD_GLOBAL              0 (session)
                       32 LOAD_CONST               1 ('currentUrl')
                       34 BINARY_SUBSCR
                       44 RETURN_VALUE
          
-         364     >>   46 LOAD_CONST               2 ('/')
+         369     >>   46 LOAD_CONST               2 ('/')
                       48 RETURN_VALUE
          consts
             '\n    ``/current_url``\n\n    :return: The current URL of the user. For a new user, it returns "/".\n    '
             'currentUrl'
             '/'
          names      ('session',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_current_url'
-         firstlineno 354
+         firstlineno 359
          lnotab 0x020712011a02
       '/restart'
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 6
          flags     : 3
@@ -2003,110 +2045,110 @@
             0000000000a00a0000000000000000000000000000000000000000a60000
             00ab00000000000000000001007416000000000000000000006a0b000000
             000000000044005d417d0364047c03760172018c077c0364041900000000
             00000000007d047c04a00c00000000000000000000000000000000000000
             006401a6010000ab010000000000000000730564017c047a0000007d047c
             00a00d0000000000000000000000000000000000000000640264057c04ac
             06a6030000ab03000000000000000001008c427c005300
-         367           0 RESUME                   0
+         372           0 RESUME                   0
          
-         376           2 LOAD_GLOBAL              1 (NULL + make_response)
+         381           2 LOAD_GLOBAL              1 (NULL + make_response)
                       14 LOAD_GLOBAL              3 (NULL + redirect)
                       26 LOAD_CONST               1 ('/')
                       28 PRECALL                  1
                       32 CALL                     1
                       42 PRECALL                  1
                       46 CALL                     1
                       56 STORE_FAST               0 (response)
          
-         377          58 LOAD_GLOBAL              4 (request)
+         382          58 LOAD_GLOBAL              4 (request)
                       70 LOAD_ATTR                3 (cookies)
                       80 LOAD_METHOD              4 (get)
                      102 LOAD_CONST               2 ('session')
                      104 LOAD_CONST               3 (None)
                      106 PRECALL                  2
                      110 CALL                     2
                      120 STORE_FAST               1 (sessionID)
          
-         379         122 LOAD_FAST                1 (sessionID)
+         384         122 LOAD_FAST                1 (sessionID)
                      124 POP_JUMP_FORWARD_IF_FALSE   123 (to 372)
          
-         381         126 LOAD_GLOBAL             10 (db)
+         386         126 LOAD_GLOBAL             10 (db)
                      138 LOAD_ATTR                6 (session)
                      148 LOAD_METHOD              7 (query)
                      170 LOAD_GLOBAL             10 (db)
                      182 LOAD_ATTR                8 (SessionStore)
                      192 PRECALL                  1
                      196 CALL                     1
                      206 LOAD_METHOD              4 (get)
                      228 LOAD_FAST                1 (sessionID)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 STORE_FAST               2 (ss)
          
-         383         246 LOAD_FAST                2 (ss)
+         388         246 LOAD_FAST                2 (ss)
                      248 POP_JUMP_FORWARD_IF_FALSE    61 (to 372)
          
-         384         250 LOAD_GLOBAL             10 (db)
+         389         250 LOAD_GLOBAL             10 (db)
                      262 LOAD_ATTR                6 (session)
                      272 LOAD_METHOD              9 (delete)
                      294 LOAD_FAST                2 (ss)
                      296 PRECALL                  1
                      300 CALL                     1
                      310 POP_TOP
          
-         385         312 LOAD_GLOBAL             10 (db)
+         390         312 LOAD_GLOBAL             10 (db)
                      324 LOAD_ATTR                6 (session)
                      334 LOAD_METHOD             10 (commit)
                      356 PRECALL                  0
                      360 CALL                     0
                      370 POP_TOP
          
-         388     >>  372 LOAD_GLOBAL             22 (page_list)
+         393     >>  372 LOAD_GLOBAL             22 (page_list)
                      384 LOAD_ATTR               11 (page_list)
                      394 GET_ITER
                  >>  396 FOR_ITER                65 (to 528)
                      398 STORE_FAST               3 (page)
          
-         390         400 LOAD_CONST               4 ('path')
+         395         400 LOAD_CONST               4 ('path')
                      402 LOAD_FAST                3 (page)
                      404 CONTAINS_OP              1
                      406 POP_JUMP_FORWARD_IF_FALSE     1 (to 410)
          
-         391         408 JUMP_BACKWARD            7 (to 396)
+         396         408 JUMP_BACKWARD            7 (to 396)
          
-         393     >>  410 LOAD_FAST                3 (page)
+         398     >>  410 LOAD_FAST                3 (page)
                      412 LOAD_CONST               4 ('path')
                      414 BINARY_SUBSCR
                      424 STORE_FAST               4 (path)
          
-         394         426 LOAD_FAST                4 (path)
+         399         426 LOAD_FAST                4 (path)
                      428 LOAD_METHOD             12 (startswith)
                      450 LOAD_CONST               1 ('/')
                      452 PRECALL                  1
                      456 CALL                     1
                      466 POP_JUMP_FORWARD_IF_TRUE     5 (to 478)
          
-         395         468 LOAD_CONST               1 ('/')
+         400         468 LOAD_CONST               1 ('/')
                      470 LOAD_FAST                4 (path)
                      472 BINARY_OP                0 (+)
                      476 STORE_FAST               4 (path)
          
-         397     >>  478 LOAD_FAST                0 (response)
+         402     >>  478 LOAD_FAST                0 (response)
                      480 LOAD_METHOD             13 (set_cookie)
                      502 LOAD_CONST               2 ('session')
                      504 LOAD_CONST               5 (0)
                      506 LOAD_FAST                4 (path)
                      508 KW_NAMES                 6
                      510 PRECALL                  3
                      514 CALL                     3
                      524 POP_TOP
                      526 JUMP_BACKWARD           66 (to 396)
          
-         399     >>  528 LOAD_FAST                0 (response)
+         404     >>  528 LOAD_FAST                0 (response)
                      530 RETURN_VALUE
          consts
             '\n    ``/restart``\n\n    Use this if you ever need to the user to start the experiment over for any reason.\n    This tries to clear out all the cookies.\n    '
             '/'
             'session'
             None
             'path'
@@ -2114,44 +2156,44 @@
             ('expires', 'path')
          names      ('make_response', 'redirect', 'request', 'cookies', 'get', 'db', 'session', 'query', 'SessionStore', 'delete', 'commit', 'page_list', 'startswith', 'set_cookie')
          varnames   ('response', 'sessionID', 'ss', 'page', 'path')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_restart'
-         firstlineno 367
+         firstlineno 372
          lnotab
             0x0209380140020402780204013e013c031c020801020210012a010a0232
             02
       '/submit'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         402           0 RESUME                   0
+         407           0 RESUME                   0
          
-         410           2 LOAD_GLOBAL              1 (NULL + redirect)
+         415           2 LOAD_GLOBAL              1 (NULL + redirect)
                       14 LOAD_CONST               1 ('/redirect_next_page')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             '\n    ``/submit``\n\n    Use this if you simply need to submit a form that redirects to the next page without doing anything with\n    the form data.\n    '
             '/redirect_next_page'
          names      ('redirect',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'submit'
-         firstlineno 402
+         firstlineno 407
          lnotab 0x0208
       '/instructions/<pageName>'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -2161,53 +2203,53 @@
             027400000000000000000000006a040000000000000000a6020000ab0200
             00000000000000a6010000ab0100000000000000005300740a0000000000
             00000000006a0600000000000000007d017c01a007000000000000000000
             000000000000000000000064037c007a060000a6010000ab010000000000
             0000007d027c02a0080000000000000000000000000000000000000000a6
             000000ab0000000000000000007d0374130000000000000000000064047c
             03ac05a6020000ab0200000000000000005300
-         416           0 RESUME                   0
+         421           0 RESUME                   0
          
-         435           2 LOAD_GLOBAL              0 (request)
+         440           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 POP_JUMP_FORWARD_IF_FALSE    39 (to 112)
          
-         436          34 LOAD_GLOBAL              5 (NULL + redirect)
+         441          34 LOAD_GLOBAL              5 (NULL + redirect)
                       46 LOAD_GLOBAL              7 (NULL + join_urls)
                       58 LOAD_CONST               2 ('/redirect_from_page')
                       60 LOAD_GLOBAL              0 (request)
                       72 LOAD_ATTR                4 (path)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 PRECALL                  1
                      100 CALL                     1
                      110 RETURN_VALUE
          
-         438     >>  112 LOAD_GLOBAL             10 (current_app)
+         443     >>  112 LOAD_GLOBAL             10 (current_app)
                      124 LOAD_ATTR                6 (jinja_env)
                      134 STORE_FAST               1 (jinja)
          
-         439         136 LOAD_FAST                1 (jinja)
+         444         136 LOAD_FAST                1 (jinja)
                      138 LOAD_METHOD              7 (get_or_select_template)
                      160 LOAD_CONST               3 ('instructions/%s.html')
                      162 LOAD_FAST                0 (pageName)
                      164 BINARY_OP                6 (%)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               2 (instructionsTemplate)
          
-         440         184 LOAD_FAST                2 (instructionsTemplate)
+         445         184 LOAD_FAST                2 (instructionsTemplate)
                      186 LOAD_METHOD              8 (render)
                      208 PRECALL                  0
                      212 CALL                     0
                      222 STORE_FAST               3 (instructionsHtml)
          
-         442         224 LOAD_GLOBAL             19 (NULL + render_template)
+         447         224 LOAD_GLOBAL             19 (NULL + render_template)
                      236 LOAD_CONST               4 ('instructions.html')
                      238 LOAD_FAST                3 (instructionsHtml)
                      240 KW_NAMES                 5
                      242 PRECALL                  2
                      246 CALL                     2
                      256 RETURN_VALUE
          consts
@@ -2219,15 +2261,15 @@
             ('instructions',)
          names      ('request', 'method', 'redirect', 'join_urls', 'path', 'current_app', 'jinja_env', 'get_or_select_template', 'render', 'render_template')
          varnames   ('pageName', 'jinja', 'instructionsTemplate', 'instructionsHtml')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_instructions'
-         firstlineno 416
+         firstlineno 421
          lnotab 0x021320014e02180130012802
       '/simple/<pageName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -2237,50 +2279,50 @@
             027400000000000000000000006a040000000000000000a6020000ab0200
             00000000000000a6010000ab0100000000000000005300740a0000000000
             00000000006a0600000000000000007d017c01a007000000000000000000
             000000000000000000000064037c007a060000a6010000ab010000000000
             000000a0080000000000000000000000000000000000000000a6000000ab
             0000000000000000007d0274130000000000000000000064047c02ac05a6
             020000ab0200000000000000005300
-         445           0 RESUME                   0
+         450           0 RESUME                   0
          
-         467           2 LOAD_GLOBAL              0 (request)
+         472           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 POP_JUMP_FORWARD_IF_FALSE    39 (to 112)
          
-         468          34 LOAD_GLOBAL              5 (NULL + redirect)
+         473          34 LOAD_GLOBAL              5 (NULL + redirect)
                       46 LOAD_GLOBAL              7 (NULL + join_urls)
                       58 LOAD_CONST               2 ('/redirect_from_page')
                       60 LOAD_GLOBAL              0 (request)
                       72 LOAD_ATTR                4 (path)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 PRECALL                  1
                      100 CALL                     1
                      110 RETURN_VALUE
          
-         470     >>  112 LOAD_GLOBAL             10 (current_app)
+         475     >>  112 LOAD_GLOBAL             10 (current_app)
                      124 LOAD_ATTR                6 (jinja_env)
                      134 STORE_FAST               1 (jinja)
          
-         471         136 LOAD_FAST                1 (jinja)
+         476         136 LOAD_FAST                1 (jinja)
                      138 LOAD_METHOD              7 (get_or_select_template)
                      160 LOAD_CONST               3 ('simple/%s.html')
                      162 LOAD_FAST                0 (pageName)
                      164 BINARY_OP                6 (%)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 LOAD_METHOD              8 (render)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 STORE_FAST               2 (simple_html)
          
-         473         220 LOAD_GLOBAL             19 (NULL + render_template)
+         478         220 LOAD_GLOBAL             19 (NULL + render_template)
                      232 LOAD_CONST               4 ('simple.html')
                      234 LOAD_FAST                2 (simple_html)
                      236 KW_NAMES                 5
                      238 PRECALL                  2
                      242 CALL                     2
                      252 RETURN_VALUE
          consts
@@ -2292,28 +2334,27 @@
             ('simple_contents',)
          names      ('request', 'method', 'redirect', 'join_urls', 'path', 'current_app', 'jinja_env', 'get_or_select_template', 'render', 'render_template')
          varnames   ('pageName', 'jinja', 'simple_html')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_simple_html'
-         firstlineno 445
+         firstlineno 450
          lnotab 0x021620014e0218015402
-      None
       ('',)
-   names      ('flask', 'Blueprint', 'render_template', 'current_app', 'request', 'make_response', 'urllib.parse', 'urlsplit', 'BOFS.JSONTable', 'JSONTable', 'BOFS.util', 'BOFS.globals', 'db', 'referrer', 'page_list', 'questionnaires', 'tables', 'BOFS.BOFSSession', 'BOFSSessionInterface', 'BOFSSession', '__name__', 'default', 'route', 'verify_correct_page', 'route_index', 'route_consent', 'route_consent_nc', 'route_create_participant', 'route_create_participant_nc', 'verify_session_valid', 'route_assign_condition', 'route_external_id', 'route_table', 'route_questionnaire', 'str', 'route_questionnaire_question', 'route_redirect_previous_page', 'route_redirect_next_page', 'route_redirect_from_page', 'route_redirect_to_page', 'route_end', 'route_user_active', 'route_current_url', 'route_restart', 'submit', 'route_instructions', 'route_simple_html')
+   names      ('flask', 'Blueprint', 'render_template', 'current_app', 'request', 'make_response', 'urllib.parse', 'urlsplit', 'traceback', 'BOFS.JSONTable', 'JSONTable', 'BOFS.util', 'BOFS.globals', 'db', 'referrer', 'page_list', 'questionnaires', 'tables', 'BOFS.BOFSSession', 'BOFSSessionInterface', 'BOFSSession', '__name__', 'default', 'route', 'verify_correct_page', 'route_index', 'route_consent', 'route_consent_nc', 'route_create_participant', 'route_create_participant_nc', 'verify_session_valid', 'route_assign_condition', 'route_external_id', 'route_table', 'route_questionnaire', 'str', 'route_questionnaire_question', 'route_redirect_previous_page', 'route_redirect_next_page', 'route_redirect_from_page', 'route_redirect_to_page', 'route_end', 'route_user_active', 'route_current_url', 'route_restart', 'submit', 'route_instructions', 'route_simple_html')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02011c010c020c0108011c01100318032801020104ff0eff0e0202
-      043001020104ff0eff0e0202183001020104ff0eff0e02020d280104ff0e
-      01020c280104ff0e01020e28010201020104ff0eff0eff0e030214300130
-      013001020104ff0eff0eff0eff0e040247300104ff0e0102113001300102
-      0106ff0eff0eff0e03021b2e010aff0e010214280104ff0e01020c280104
-      ff0e010217280104ff0e01020e280104ff0e01020e28010201020104ff0e
-      ff0eff0e030214280104ff0e010208280104ff0e01020c280104ff0e0102
-      222e0104ff0e01020d30010201020104ff0eff0eff0e03021a3001020102
-      0104ff0eff0eff0e03
+      0x00ff02011c010c0108010c0108011c01100318032801020104ff0eff0e
+      0202043001020104ff0eff0e0202183001020104ff0eff0e02020d280104
+      ff0e01020c280104ff0e01020e28010201020104ff0eff0eff0e03021430
+      0130013001020104ff0eff0eff0eff0e040247300104ff0e010211300130
+      01020106ff0eff0eff0e03021b2e010aff0e010219280104ff0e01020c28
+      0104ff0e010217280104ff0e01020e280104ff0e01020e28010201020104
+      ff0eff0eff0e030214280104ff0e010208280104ff0e01020c280104ff0e
+      0102222e0104ff0e01020d30010201020104ff0eff0eff0e03021a300102
+      01020104ff0eff0eff0e03
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/models.py` & `bride-of-frankensystem-1.9.3.6/BOFS/default/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,27 @@
         timeStarted = db.Column(db.DateTime, nullable=False, default=datetime.utcnow)  # Starts after consent
         timeEnded = db.Column(db.DateTime, nullable=True)
         finished = db.Column(db.Boolean, nullable=False, default=False)
         isCrawler = db.Column(db.Boolean, nullable=False, default=False)
         excludeFromCount = db.Column(db.Boolean, nullable=False, default=False)
         code = db.Column(db.String, nullable=False, default=0)
         lastActiveOn = db.Column(db.DateTime, nullable=False, default=datetime.utcnow)
+        notes = db.Column(db.String, nullable=False, default="")
+
+        def table(self, name):
+            return getattr(self, "table_" + name)
 
-        #def table(self, name):
-        #    from BOFS.globals import tables
 
         def questionnaire(self, name, tag=""):
             from BOFS.globals import questionnaires
-            qResults = getattr(self, "questionnaire_" + name)
+            q_results = getattr(self, "questionnaire_" + name)
 
             toConsider = []
 
-            for result in qResults:
+            for result in q_results:
                 if result.tag == tag or (result.tag == u'0' and tag == ''):
                     toConsider.append(result)
 
             if len(toConsider) == 1:
                 return toConsider[0]
 
             if len(toConsider) > 1:
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/default/views.py` & `bride-of-frankensystem-1.9.3.6/BOFS/default/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from flask import Blueprint, render_template, current_app, request, make_response
 from urllib.parse import urlsplit
-
+import traceback
 from BOFS.JSONTable import JSONTable
 from BOFS.util import *
 from BOFS.globals import db, referrer, page_list, questionnaires, tables
 from BOFS.BOFSSession import BOFSSessionInterface, BOFSSession
 
 
 default = Blueprint('default', __name__)
@@ -245,15 +245,20 @@
     participant = db.Participant.query.get(session['participantID'])
 
     try:
         return render_template(f'questions/{questionType}.html',
                                question=request.json,
                                participant=participant)
     except Exception as ex:
-        return f"Exception in <b>{questionType}.html</b>: {ex}"
+        if current_app.run_with_debugging:
+            debugging_info = str(ex) + "<p><pre>" + str(traceback.format_exc()) + "</pre>"
+        else:
+            debugging_info = str(ex)
+
+        return f"Exception in <b>{questionType}.html</b>: {debugging_info}"
 
 
 @default.route("/redirect_previous_page")
 def route_redirect_previous_page():
     """
     ``/redirect_previous_page``
```

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/globals.py` & `bride-of-frankensystem-1.9.3.6/BOFS/globals.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/all.min.css` & `bride-of-frankensystem-1.9.3.6/BOFS/static/all.min.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/bootstrap.min.css` & `bride-of-frankensystem-1.9.3.6/BOFS/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/img/check.png` & `bride-of-frankensystem-1.9.3.6/BOFS/static/img/check.png`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/img/spinner32.gif` & `bride-of-frankensystem-1.9.3.6/BOFS/static/img/spinner32.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/js/bootstrap.bundle.min.js` & `bride-of-frankensystem-1.9.3.6/BOFS/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/js/htmx.min.js` & `bride-of-frankensystem-1.9.3.6/BOFS/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/js/jquery-3.7.1.min.js` & `bride-of-frankensystem-1.9.3.6/BOFS/static/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/loading.gif` & `bride-of-frankensystem-1.9.3.6/BOFS/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/style.css` & `bride-of-frankensystem-1.9.3.6/BOFS/static/style.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/static/style_admin.css` & `bride-of-frankensystem-1.9.3.6/BOFS/static/style_admin.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/consent.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/consent.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/end.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/end.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/external_id.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/external_id.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/questionnaire_macro.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/questionnaire_macro.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/radiogrid.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/radiogrid.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/radiolist.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/radiolist.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/questions/slider.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/questions/slider.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/template.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/template.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/unity_webgl.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/unity_webgl.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/templates/unity_webgl_fullscreen.html` & `bride-of-frankensystem-1.9.3.6/BOFS/templates/unity_webgl_fullscreen.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/BOFS/util.py` & `bride-of-frankensystem-1.9.3.6/BOFS/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/LICENSE` & `bride-of-frankensystem-1.9.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/PKG-INFO` & `bride-of-frankensystem-1.9.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.5
+Version: 1.9.3.6
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.5/README.md` & `bride-of-frankensystem-1.9.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.5
+Version: 1.9.3.6
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.5/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-1.9.3.6/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,23 @@
 BOFS/__pycache__/PageList.cpython-311.pyc
 BOFS/__pycache__/__init__.cpython-311.pyc
 BOFS/__pycache__/__main__.cpython-311.pyc
 BOFS/__pycache__/cli.cpython-311.pyc
 BOFS/__pycache__/create_app.cpython-311.pyc
 BOFS/__pycache__/globals.cpython-311.pyc
 BOFS/__pycache__/util.cpython-311.pyc
-BOFS/admin/QuestionnaireResults.py
+BOFS/admin/Results.py
+BOFS/admin/SummaryStats.py
 BOFS/admin/__init__.py
-BOFS/admin/export_helpers.py
 BOFS/admin/util.py
 BOFS/admin/views.py
-BOFS/admin/__pycache__/QuestionnaireResults.cpython-310.pyc
-BOFS/admin/__pycache__/QuestionnaireResults.cpython-311.pyc
+BOFS/admin/__pycache__/Results.cpython-311.pyc
+BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc
 BOFS/admin/__pycache__/__init__.cpython-310.pyc
 BOFS/admin/__pycache__/__init__.cpython-311.pyc
-BOFS/admin/__pycache__/export_helpers.cpython-311.pyc
 BOFS/admin/__pycache__/util.cpython-310.pyc
 BOFS/admin/__pycache__/util.cpython-311.pyc
 BOFS/admin/__pycache__/views.cpython-310.pyc
 BOFS/admin/__pycache__/views.cpython-311.pyc
 BOFS/admin/templates/database_delete.html
 BOFS/admin/templates/export.html
 BOFS/admin/templates/export_csv.html
@@ -45,14 +44,15 @@
 BOFS/admin/templates/preview_questionnaire.html
 BOFS/admin/templates/preview_questionnaire_simple.html
 BOFS/admin/templates/progress.html
 BOFS/admin/templates/progress_ajax.html
 BOFS/admin/templates/progress_summary_ajax.html
 BOFS/admin/templates/questionnaire_results.html
 BOFS/admin/templates/results.html
+BOFS/admin/templates/results_boxplot.html
 BOFS/admin/templates/table_ajax.html
 BOFS/admin/templates/table_view.html
 BOFS/admin/templates/template_admin.html
 BOFS/admin/templates/template_admin_head.html
 BOFS/bride_of_frankensystem.egg-info/PKG-INFO
 BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
 BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
```

### Comparing `bride-of-frankensystem-1.9.3.5/pyproject.toml` & `bride-of-frankensystem-1.9.3.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bride-of-frankensystem"
-version = "1.9.3.5"
+version = "1.9.3.6"
 description = "A framework that allows for the development of custom online experiments and surveys."
 readme = "README.md"
 authors = [{ name = "Colby Johanson", email = "colby.johanson@usask.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
@@ -18,15 +18,16 @@
 dependencies = [
     "flask>=2.3.0",
     "eventlet",
     "sqlalchemy>=1.4.18",
     "flask-sqlalchemy>=3.0.0",
     "flask-compress",
     "toml",
-    "crawlerdetect"
+    "crawlerdetect",
+    "pandas"
 ]
 requires-python = ">=3.9"
 
 [tool.setuptools.packages.find]
 where = [""]
 
 [project.urls]
```

