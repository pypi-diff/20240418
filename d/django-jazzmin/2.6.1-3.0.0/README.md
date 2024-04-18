# Comparing `tmp/django_jazzmin-2.6.1.tar.gz` & `tmp/django_jazzmin-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jazzmin-2.6.1.tar", max compression
+gzip compressed data, was "django_jazzmin-3.0.0.tar", max compression
```

## Comparing `django_jazzmin-2.6.1.tar` & `django_jazzmin-3.0.0.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0     1056 2024-03-23 08:35:29.437913 django_jazzmin-2.6.1/LICENSE
--rw-r--r--   0        0        0     3881 2024-03-23 08:35:29.437913 django_jazzmin-2.6.1/README.md
--rw-r--r--   0        0        0      116 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/__init__.py
--rw-r--r--   0        0        0      210 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/apps.py
--rw-r--r--   0        0        0      176 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/compat.py
--rw-r--r--   0        0        0     9666 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17953 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1536 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2486 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1572 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2518 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3080 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3379 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2967 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5327 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2862 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4142 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1323 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2085 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1325 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2088 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13753 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/settings.py
--rw-r--r--   0        0        0      564 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/static/admin/js/cancel.js
--rw-r--r--   0        0        0     1946 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/static/admin/js/popup_response.js
--rw-r--r--   0        0        0    16969 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/css/main.css
--rw-r--r--   0        0        0     1094 2024-03-23 08:35:29.449913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/calendar-icons.svg
--rw-r--r--   0        0        0   223437 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/default-log.svg
--rw-r--r--   0        0        0     7070 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/default.jpg
--rw-r--r--   0        0        0     1086 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/icon-calendar.svg
--rw-r--r--   0        0        0      380 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/icon-changelink.svg
--rw-r--r--   0        0        0     3291 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/selector-icons.svg
--rw-r--r--   0        0        0     6052 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/change_form.js
--rw-r--r--   0        0        0     2252 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/change_list.js
--rw-r--r--   0        0        0     2391 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/main.js
--rw-r--r--   0        0        0     6258 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/related-modal.js
--rw-r--r--   0        0        0    13873 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/ui-builder.js
--rw-r--r--   0        0        0     2756 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
--rw-r--r--   0        0        0  1382975 2024-03-23 08:35:29.453913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/css/adminlte.min.css
--rw-r--r--   0        0        0  3783134 2024-03-23 08:35:29.461913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/css/adminlte.min.css.map
--rw-r--r--   0        0        0     2637 2024-03-23 08:35:29.461913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/AdminLTELogo.png
--rw-r--r--   0        0        0     1139 2024-03-23 08:35:29.461913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/icons.png
--rw-r--r--   0        0        0     5357 2024-03-23 08:35:29.461913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/user2-160x160.jpg
--rw-r--r--   0        0        0    44244 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/js/adminlte.min.js
--rw-r--r--   0        0        0   129651 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/js/adminlte.min.js.map
--rw-r--r--   0        0        0    62440 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   187646 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0   163350 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cerulean/bootstrap.min.css
--rw-r--r--   0        0        0   154456 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cosmo/bootstrap.min.css
--rw-r--r--   0        0        0   164597 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cyborg/bootstrap.min.css
--rw-r--r--   0        0        0   164202 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/darkly/bootstrap.min.css
--rw-r--r--   0        0        0   161972 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/default/bootstrap.min.css
--rw-r--r--   0        0        0   164819 2024-03-23 08:35:29.465913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/flatly/bootstrap.min.css
--rw-r--r--   0        0        0   161735 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/journal/bootstrap.min.css
--rw-r--r--   0        0        0   165148 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/litera/bootstrap.min.css
--rw-r--r--   0        0        0   167943 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/lumen/bootstrap.min.css
--rw-r--r--   0        0        0   155932 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/lux/bootstrap.min.css
--rw-r--r--   0        0        0   194473 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/materia/bootstrap.min.css
--rw-r--r--   0        0        0   165946 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/minty/bootstrap.min.css
--rw-r--r--   0        0        0   155889 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/pulse/bootstrap.min.css
--rw-r--r--   0        0        0   163543 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/sandstone/bootstrap.min.css
--rw-r--r--   0        0        0   163234 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/simplex/bootstrap.min.css
--rw-r--r--   0        0        0   167043 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/sketchy/bootstrap.min.css
--rw-r--r--   0        0        0   171632 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/slate/bootstrap.min.css
--rw-r--r--   0        0        0   169219 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/solar/bootstrap.min.css
--rw-r--r--   0        0        0   164894 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/spacelab/bootstrap.min.css
--rw-r--r--   0        0        0   164559 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/superhero/bootstrap.min.css
--rw-r--r--   0        0        0   161367 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/united/bootstrap.min.css
--rw-r--r--   0        0        0   168497 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/yeti/bootstrap.min.css
--rw-r--r--   0        0        0    59344 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/css/all.min.css
--rw-r--r--   0        0        0   134346 2024-03-23 08:35:29.469913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   747545 2024-03-23 08:35:29.473913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   134040 2024-03-23 08:35:29.473913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    90060 2024-03-23 08:35:29.473913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    76764 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34034 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   144714 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    33736 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16276 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13276 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   203030 2024-03-23 08:35:29.477913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   918991 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   202744 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   101652 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    78196 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    16264 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/select2/css/select2.min.css
--rw-r--r--   0        0        0    73170 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/static/vendor/select2/js/select2.min.js
--rw-r--r--   0        0        0     1519 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/actions.html
--rw-r--r--   0        0        0      517 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/app_index.html
--rw-r--r--   0        0        0      364 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/auth/user/add_form.html
--rw-r--r--   0        0        0     5448 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/auth/user/change_password.html
--rw-r--r--   0        0        0    20234 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/base.html
--rw-r--r--   0        0        0       31 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/base_site.html
--rw-r--r--   0        0        0     5658 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/change_form.html
--rw-r--r--   0        0        0      545 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/change_form_object_tools.html
--rw-r--r--   0        0        0     4903 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/change_list.html
--rw-r--r--   0        0        0      516 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/change_list_object_tools.html
--rw-r--r--   0        0        0     2108 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/change_list_results.html
--rw-r--r--   0        0        0      956 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/date_hierarchy.html
--rw-r--r--   0        0        0     4104 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/delete_confirmation.html
--rw-r--r--   0        0        0     4180 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0        0        0     4246 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/edit_inline/stacked.html
--rw-r--r--   0        0        0     6424 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/edit_inline/tabular.html
--rw-r--r--   0        0        0     1800 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/breadcrumbs.html
--rw-r--r--   0        0        0      983 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/change_form.html
--rw-r--r--   0        0        0     4142 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/delete_selected_files_confirmation.html
--rw-r--r--   0        0        0     1555 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/file/change_form.html
--rw-r--r--   0        0        0     1817 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/folder/change_form.html
--rw-r--r--   0        0        0    14677 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/folder/directory_listing.html
--rw-r--r--   0        0        0     1539 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/image/change_form.html
--rw-r--r--   0        0        0     2743 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filer/tools/detail_info.html
--rw-r--r--   0        0        0      592 2024-03-23 08:35:29.481913 django_jazzmin-2.6.1/jazzmin/templates/admin/filter.html
--rw-r--r--   0        0        0      916 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/base.html
--rw-r--r--   0        0        0      391 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list.html
--rw-r--r--   0        0        0      187 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list_export.html
--rw-r--r--   0        0        0      286 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0        0        0      187 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list_import.html
--rw-r--r--   0        0        0      323 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0        0        0      301 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0        0        0     3191 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/export.html
--rw-r--r--   0        0        0    13270 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/import.html
--rw-r--r--   0        0        0     2725 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/includes/fieldset.html
--rw-r--r--   0        0        0      302 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0        0        0     6784 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/index.html
--rw-r--r--   0        0        0     3075 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/login.html
--rw-r--r--   0        0        0      645 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/mptt_filter.html
--rw-r--r--   0        0        0     3268 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/object_history.html
--rw-r--r--   0        0        0     1036 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/pagination.html
--rw-r--r--   0        0        0      605 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/popup_response.html
--rw-r--r--   0        0        0     1928 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/search_form.html
--rw-r--r--   0        0        0      937 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/solo/change_form.html
--rw-r--r--   0        0        0      572 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/solo/object_history.html
--rw-r--r--   0        0        0     1821 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin/submit_line.html
--rw-r--r--   0        0        0      678 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/base_docs.html
--rw-r--r--   0        0        0     1644 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/bookmarklets.html
--rw-r--r--   0        0        0     1619 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/index.html
--rw-r--r--   0        0        0      809 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/missing_docutils.html
--rw-r--r--   0        0        0     2973 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/model_detail.html
--rw-r--r--   0        0        0     2083 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/model_index.html
--rw-r--r--   0        0        0     1159 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_detail.html
--rw-r--r--   0        0        0     2802 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_filter_index.html
--rw-r--r--   0        0        0     2286 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_tag_index.html
--rw-r--r--   0        0        0     1387 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/view_detail.html
--rw-r--r--   0        0        0     2797 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/admin_doc/view_index.html
--rw-r--r--   0        0        0     1803 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/carousel.html
--rw-r--r--   0        0        0     1152 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/collapsible.html
--rw-r--r--   0        0        0     1321 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/horizontal_tabs.html
--rw-r--r--   0        0        0      610 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/related_modal.html
--rw-r--r--   0        0        0      862 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/single.html
--rw-r--r--   0        0        0    14972 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/ui_builder_panel.html
--rw-r--r--   0        0        0     1449 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/vertical_tabs.html
--rw-r--r--   0        0        0      468 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/jazzmin/widgets/select.html
--rw-r--r--   0        0        0     3045 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/base.html
--rw-r--r--   0        0        0      428 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/logged_out.html
--rw-r--r--   0        0        0      880 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_change_done.html
--rw-r--r--   0        0        0     5870 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_change_form.html
--rw-r--r--   0        0        0      450 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_complete.html
--rw-r--r--   0        0        0     2640 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_confirm.html
--rw-r--r--   0        0        0      590 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_done.html
--rw-r--r--   0        0        0     1634 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_form.html
--rw-r--r--   0        0        0        0 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templatetags/__init__.py
--rw-r--r--   0        0        0    17332 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/templatetags/jazzmin.py
--rw-r--r--   0        0        0     7813 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/utils.py
--rw-r--r--   0        0        0      803 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/jazzmin/widgets.py
--rw-r--r--   0        0        0     5260 2024-03-23 08:35:29.485913 django_jazzmin-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     5865 1970-01-01 00:00:00.000000 django_jazzmin-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-18 18:29:42.880035 django_jazzmin-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-18 18:29:42.880035 django_jazzmin-3.0.0/README.md
+-rw-r--r--   0        0        0      564 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/__init__.py
+-rw-r--r--   0        0        0      210 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/apps.py
+-rw-r--r--   0        0        0      176 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/compat.py
+-rw-r--r--   0        0        0     9666 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17953 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1536 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2486 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1572 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2518 2024-04-18 18:29:42.888036 django_jazzmin-3.0.0/jazzmin/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3080 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3379 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2967 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5327 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2862 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4142 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1323 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2085 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1325 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2088 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13768 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/settings.py
+-rw-r--r--   0        0        0      564 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/admin/js/cancel.js
+-rw-r--r--   0        0        0     1535 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/admin/js/popup_response.js
+-rw-r--r--   0        0        0    16969 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/css/main.css
+-rw-r--r--   0        0        0     1094 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/calendar-icons.svg
+-rw-r--r--   0        0        0   223437 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/default-log.svg
+-rw-r--r--   0        0        0     7070 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/default.jpg
+-rw-r--r--   0        0        0     1086 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/icon-calendar.svg
+-rw-r--r--   0        0        0      380 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/icon-changelink.svg
+-rw-r--r--   0        0        0     3291 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/selector-icons.svg
+-rw-r--r--   0        0        0     6052 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/change_form.js
+-rw-r--r--   0        0        0     2252 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/change_list.js
+-rw-r--r--   0        0        0     2391 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/main.js
+-rw-r--r--   0        0        0     6258 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/related-modal.js
+-rw-r--r--   0        0        0    13873 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/ui-builder.js
+-rw-r--r--   0        0        0     2756 2024-04-18 18:29:42.892036 django_jazzmin-3.0.0/jazzmin/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js
+-rw-r--r--   0        0        0  1382975 2024-04-18 18:29:42.896036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/css/adminlte.min.css
+-rw-r--r--   0        0        0  3783134 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/css/adminlte.min.css.map
+-rw-r--r--   0        0        0     2637 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/AdminLTELogo.png
+-rw-r--r--   0        0        0     1139 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/icons.png
+-rw-r--r--   0        0        0     5357 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/user2-160x160.jpg
+-rw-r--r--   0        0        0    44244 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/js/adminlte.min.js
+-rw-r--r--   0        0        0   129651 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/js/adminlte.min.js.map
+-rw-r--r--   0        0        0    62440 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   187646 2024-04-18 18:29:42.904036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0   163350 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cerulean/bootstrap.min.css
+-rw-r--r--   0        0        0   154456 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cosmo/bootstrap.min.css
+-rw-r--r--   0        0        0   164597 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cyborg/bootstrap.min.css
+-rw-r--r--   0        0        0   164202 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/darkly/bootstrap.min.css
+-rw-r--r--   0        0        0   161972 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/default/bootstrap.min.css
+-rw-r--r--   0        0        0   164819 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/flatly/bootstrap.min.css
+-rw-r--r--   0        0        0   161735 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/journal/bootstrap.min.css
+-rw-r--r--   0        0        0   165148 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/litera/bootstrap.min.css
+-rw-r--r--   0        0        0   167943 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/lumen/bootstrap.min.css
+-rw-r--r--   0        0        0   155932 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/lux/bootstrap.min.css
+-rw-r--r--   0        0        0   194473 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/materia/bootstrap.min.css
+-rw-r--r--   0        0        0   165946 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/minty/bootstrap.min.css
+-rw-r--r--   0        0        0   155889 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/pulse/bootstrap.min.css
+-rw-r--r--   0        0        0   163543 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/sandstone/bootstrap.min.css
+-rw-r--r--   0        0        0   163234 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/simplex/bootstrap.min.css
+-rw-r--r--   0        0        0   167043 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/sketchy/bootstrap.min.css
+-rw-r--r--   0        0        0   171632 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/slate/bootstrap.min.css
+-rw-r--r--   0        0        0   169219 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/solar/bootstrap.min.css
+-rw-r--r--   0        0        0   164894 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/spacelab/bootstrap.min.css
+-rw-r--r--   0        0        0   164559 2024-04-18 18:29:42.908036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/superhero/bootstrap.min.css
+-rw-r--r--   0        0        0   161367 2024-04-18 18:29:42.912036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/united/bootstrap.min.css
+-rw-r--r--   0        0        0   168497 2024-04-18 18:29:42.912036 django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/yeti/bootstrap.min.css
+-rw-r--r--   0        0        0    59344 2024-04-18 18:29:42.912036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/css/all.min.css
+-rw-r--r--   0        0        0   134346 2024-04-18 18:29:42.912036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   747545 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   134040 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    90060 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    76764 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34034 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   144714 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    33736 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16276 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13276 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   203030 2024-04-18 18:29:42.916036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   918991 2024-04-18 18:29:42.920036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   202744 2024-04-18 18:29:42.920036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   101652 2024-04-18 18:29:42.920036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    78196 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    16264 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/static/vendor/select2/css/select2.min.css
+-rw-r--r--   0        0        0    73170 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/static/vendor/select2/js/select2.min.js
+-rw-r--r--   0        0        0     1519 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/actions.html
+-rw-r--r--   0        0        0      517 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/app_index.html
+-rw-r--r--   0        0        0      364 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     5448 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/auth/user/change_password.html
+-rw-r--r--   0        0        0    20353 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/base.html
+-rw-r--r--   0        0        0       31 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/base_site.html
+-rw-r--r--   0        0        0     5658 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/change_form.html
+-rw-r--r--   0        0        0      545 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/change_form_object_tools.html
+-rw-r--r--   0        0        0     4903 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/change_list.html
+-rw-r--r--   0        0        0      516 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0        0        0     2108 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/change_list_results.html
+-rw-r--r--   0        0        0      956 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/date_hierarchy.html
+-rw-r--r--   0        0        0     4104 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/delete_confirmation.html
+-rw-r--r--   0        0        0     4180 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     4246 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0        0        0     6424 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0        0        0     1800 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/breadcrumbs.html
+-rw-r--r--   0        0        0      983 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/change_form.html
+-rw-r--r--   0        0        0     4142 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/delete_selected_files_confirmation.html
+-rw-r--r--   0        0        0     1555 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/file/change_form.html
+-rw-r--r--   0        0        0     1817 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/folder/change_form.html
+-rw-r--r--   0        0        0    14682 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/folder/directory_listing.html
+-rw-r--r--   0        0        0     1539 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/image/change_form.html
+-rw-r--r--   0        0        0     2743 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filer/tools/detail_info.html
+-rw-r--r--   0        0        0      592 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/filter.html
+-rw-r--r--   0        0        0      916 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/base.html
+-rw-r--r--   0        0        0      391 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list.html
+-rw-r--r--   0        0        0      187 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0        0        0      286 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0        0        0      187 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0        0        0      323 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0        0        0      301 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0        0        0     3191 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/export.html
+-rw-r--r--   0        0        0    13270 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/import.html
+-rw-r--r--   0        0        0     2725 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0      302 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0        0        0     6784 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/index.html
+-rw-r--r--   0        0        0     3075 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/login.html
+-rw-r--r--   0        0        0      645 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/mptt_filter.html
+-rw-r--r--   0        0        0     3268 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/object_history.html
+-rw-r--r--   0        0        0     1036 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/pagination.html
+-rw-r--r--   0        0        0      605 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/popup_response.html
+-rw-r--r--   0        0        0     1928 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/search_form.html
+-rw-r--r--   0        0        0      937 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/solo/change_form.html
+-rw-r--r--   0        0        0      572 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/solo/object_history.html
+-rw-r--r--   0        0        0     1821 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin/submit_line.html
+-rw-r--r--   0        0        0      678 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/base_docs.html
+-rw-r--r--   0        0        0     1644 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/bookmarklets.html
+-rw-r--r--   0        0        0     1619 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/index.html
+-rw-r--r--   0        0        0      809 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/missing_docutils.html
+-rw-r--r--   0        0        0     2973 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/model_detail.html
+-rw-r--r--   0        0        0     2083 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/model_index.html
+-rw-r--r--   0        0        0     1159 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_detail.html
+-rw-r--r--   0        0        0     2802 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_filter_index.html
+-rw-r--r--   0        0        0     2286 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_tag_index.html
+-rw-r--r--   0        0        0     1387 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/view_detail.html
+-rw-r--r--   0        0        0     2797 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/admin_doc/view_index.html
+-rw-r--r--   0        0        0     1803 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/carousel.html
+-rw-r--r--   0        0        0     1152 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/collapsible.html
+-rw-r--r--   0        0        0     1321 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/horizontal_tabs.html
+-rw-r--r--   0        0        0      610 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/related_modal.html
+-rw-r--r--   0        0        0      862 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/single.html
+-rw-r--r--   0        0        0    14972 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/ui_builder_panel.html
+-rw-r--r--   0        0        0     1449 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/vertical_tabs.html
+-rw-r--r--   0        0        0      468 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/jazzmin/widgets/select.html
+-rw-r--r--   0        0        0     3045 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/base.html
+-rw-r--r--   0        0        0      428 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/logged_out.html
+-rw-r--r--   0        0        0      880 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_change_done.html
+-rw-r--r--   0        0        0     5870 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_change_form.html
+-rw-r--r--   0        0        0      450 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_complete.html
+-rw-r--r--   0        0        0     2640 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_confirm.html
+-rw-r--r--   0        0        0      590 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_done.html
+-rw-r--r--   0        0        0     1634 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_form.html
+-rw-r--r--   0        0        0        0 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templatetags/__init__.py
+-rw-r--r--   0        0        0    17378 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/templatetags/jazzmin.py
+-rw-r--r--   0        0        0     7815 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/utils.py
+-rw-r--r--   0        0        0      803 2024-04-18 18:29:42.924036 django_jazzmin-3.0.0/jazzmin/widgets.py
+-rw-r--r--   0        0        0     5133 2024-04-18 18:29:54.384049 django_jazzmin-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6160 1970-01-01 00:00:00.000000 django_jazzmin-3.0.0/PKG-INFO
```

### Comparing `django_jazzmin-2.6.1/LICENSE` & `django_jazzmin-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/README.md` & `django_jazzmin-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 
 # Django jazzmin (Jazzy Admin)
 
+## Project Status
+
+This project is being actively maintained, though with a reduced feature set, we are looking for contributors to help
+maintain and improve the project, please get in touch if you would like to help.
+
+Help needed with:
+
+- Triaging issues
+- Frontend fixes and UI improvements
+- Testing
+- Documentation
+
+Pull requests are welcome, though ive been pre-occupied with other projects lately, so have not been able to review
+them as quickly as I would like, but im trying to get through them all now, hopefully with some outside help.
+
 [![Docs](https://readthedocs.org/projects/django-jazzmin/badge/?version=latest)](https://django-jazzmin.readthedocs.io)
 ![PyPI download month](https://img.shields.io/pypi/dm/django-jazzmin.svg)
 [![PyPI version](https://badge.fury.io/py/django-jazzmin.svg)](https://pypi.python.org/pypi/django-jazzmin/)
-![Python versions](https://img.shields.io/badge/python-%3E%3D3.6-brightgreen)
-![Django Versions](https://img.shields.io/badge/django-%3E%3D2-brightgreen)
+![Python versions](https://img.shields.io/badge/python-%3E=3.8-brightgreen)
+![Django Versions](https://img.shields.io/badge/django-%3E=4.2-brightgreen)
 [![Coverage Status](https://coveralls.io/repos/github/farridav/django-jazzmin/badge.svg?branch=master)](https://coveralls.io/github/farridav/django-jazzmin?branch=master)
 
 Drop-in theme for django admin, that utilises AdminLTE 3 & Bootstrap 4 to make yo' admin look jazzy
 
 ## Installation
-```
+
+```bash
 pip install django-jazzmin
 ```
 
 ## Documentation
-See [Documentation](https://django-jazzmin.readthedocs.io) or [Test App](https://github.com/farridav/django-jazzmin/tree/master/tests/test_app/library/settings.py)
 
-## Demo
-Live demo https://django-jazzmin.herokuapp.com/admin
-
-**Username**: test@test.com
-
-**Password**: test
-
-*Note: Data resets nightly*
+See [Documentation](https://django-jazzmin.readthedocs.io) or [Test App](https://github.com/farridav/django-jazzmin/tree/master/tests/test_app/library/settings.py)
 
 ## Features
+
 - Drop-in admin skin, all configuration optional
 - Customisable side menu
 - Customisable top menu
 - Customisable user menu
 - 4 different Change form templates (horizontal tabs, vertical tabs, carousel, collapsible)
 - Bootstrap 4 modal (instead of the old popup window, optional)
 - Search bar for any given model admin
@@ -40,63 +49,79 @@
 - Select2 drop-downs
 - Bootstrap 4 & AdminLTE UI components
 - Using the latest [adminlte](https://adminlte.io/) + [bootstrap](https://getbootstrap.com/)
 
 ## Screenshots
 
 ## Dashboard
+
 ![dashboard](https://django-jazzmin.readthedocs.io/img/dashboard.png)
 
 ## List view
+
 ![table list](https://django-jazzmin.readthedocs.io/img/list_view.png)
 
 ## Change form templates
 
 ### Collapsed side menu
+
 ![form page](https://django-jazzmin.readthedocs.io/img/detail_view.png)
 
 ### Expanded side menu
+
 ![Single](https://django-jazzmin.readthedocs.io/img/changeform_single.png)
 
 ### Horizontal tabs
+
 ![Horizontal tabs](https://django-jazzmin.readthedocs.io/img/changeform_horizontal_tabs.png)
 
 ### Vertical tabs
+
 ![Vertical tabs](https://django-jazzmin.readthedocs.io/img/changeform_vertical_tabs.png)
 
 ### Collapsible
+
 ![Collapsible](https://django-jazzmin.readthedocs.io/img/changeform_collapsible.png)
 
 ### Carousel
+
 ![Carousel](https://django-jazzmin.readthedocs.io/img/changeform_carousel.png)
 
 ### Related modal
+
 ![Related modal](https://django-jazzmin.readthedocs.io/img/related_modal_bootstrap.png)
 
 ## History page
+
 ![form page](https://django-jazzmin.readthedocs.io/img/history_page.png)
 
 ## Login view
+
 ![login](https://django-jazzmin.readthedocs.io/img/login.png)
 
 ## UI Customiser
+
 ![ui_customiser](https://django-jazzmin.readthedocs.io/img/ui_customiser.png)
 
 ## Mobile layout
+
 ![mobile](https://django-jazzmin.readthedocs.io/img/dashboard_mobile.png)
 
 ## Tablet layout
+
 ![tablet](https://django-jazzmin.readthedocs.io/img/dashboard_tablet.png)
 
 ## Admin Docs (if installed)
+
 ![admin_docs](https://django-jazzmin.readthedocs.io/img/admin_docs.png)
 
 ## Thanks
-This was initially a Fork of https://github.com/wuyue92tree/django-adminlte-ui that we refactored so much we thought it
+
+This was initially a Fork of <https://github.com/wuyue92tree/django-adminlte-ui> that we refactored so much we thought it
 deserved its own package, big thanks to @wuyue92tree for all of his initial hard work, we are still patching into that
 project were possible, but this project has taken a different direction.
 
 The javascript modal implementation uses some code from [django-admin-interface](https://github.com/fabiocaccamo/django-admin-interface/blob/master/admin_interface/static/admin/js/popup_response.js), so thanks to @fabiocaccamo for original work
 
-- Based on AdminLTE 3: https://adminlte.io/
-- Using Bootstrap 4: https://getbootstrap.com/
-- Using Font Awesome 5: https://fontawesome.com/
+- Based on AdminLTE 3: <https://adminlte.io/>
+- Using Bootstrap 4: <https://getbootstrap.com/>
+- Using Font Awesome 5: <https://fontawesome.com/>
```

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/bg/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/bg/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/de/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/de/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/es/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/es/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/fr/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/fr/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/hu/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/hu/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/ru/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/ru/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/zh_Hans/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/zh_Hant/LC_MESSAGES/django.mo` & `django_jazzmin-3.0.0/jazzmin/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/locale/zh_Hant/LC_MESSAGES/django.po` & `django_jazzmin-3.0.0/jazzmin/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/settings.py` & `django_jazzmin-3.0.0/jazzmin/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import logging
-from typing import Dict, Any
+from typing import Any, Dict
 
 from django.conf import settings
 from django.templatetags.static import static
 
 from .utils import get_admin_url, get_model_meta
 
 logger = logging.getLogger(__name__)
@@ -57,15 +57,16 @@
     "hide_models": [],
     # List of apps to base side menu ordering off of
     "order_with_respect_to": [],
     # Custom links to append to side menu app groups, keyed on app name
     "custom_links": {},
     # Custom icons for side menu apps/models See the link below
     # https://fontawesome.com/icons?d=gallery&m=free&v=5.0.0,5.0.1,5.0.10,5.0.11,5.0.12,5.0.13,5.0.2,5.0.3,5.0.4,5.0.5,5.0.6,5.0.7,5.0.8,5.0.9,5.1.0,
-    # 5.1.1,5.2.0,5.3.0,5.3.1,5.4.0,5.4.1,5.4.2,5.13.0,5.12.0,5.11.2,5.11.1,5.10.0,5.9.0,5.8.2,5.8.1,5.7.2,5.7.1,5.7.0,5.6.3,5.5.0,5.4.2
+    # 5.1.1,5.2.0,5.3.0,5.3.1,5.4.0,5.4.1,5.4.2,5.13.0,5.12.0,
+    # 5.11.2,5.11.1,5.10.0,5.9.0,5.8.2,5.8.1,5.7.2,5.7.1,5.7.0,5.6.3,5.5.0,5.4.2
     # for the full list of 5.13.0 free icon classes
     "icons": {"auth": "fas fa-users-cog", "auth.user": "fas fa-user", "auth.Group": "fas fa-users"},
     # Icons that are used when one is not manually specified
     "default_icon_parents": "fas fa-chevron-circle-right",
     "default_icon_children": "fas fa-circle",
     #################
     # Related Modal #
@@ -225,19 +226,19 @@
             if model_meta:
                 jazzmin_search_model["search_name"] = model_meta.verbose_name_plural.title()
             else:
                 jazzmin_search_model["search_name"] = search_model.split(".")[-1] + "s"
             jazzmin_settings["search_models_parsed"].append(jazzmin_search_model)
 
     # Deal with single strings in hide_apps/hide_models and make sure we lower case 'em
-    if type(jazzmin_settings["hide_apps"]) == str:
+    if isinstance(jazzmin_settings["hide_apps"], str):
         jazzmin_settings["hide_apps"] = [jazzmin_settings["hide_apps"]]
     jazzmin_settings["hide_apps"] = [x.lower() for x in jazzmin_settings["hide_apps"]]
 
-    if type(jazzmin_settings["hide_models"]) == str:
+    if isinstance(jazzmin_settings["hide_models"], str):
         jazzmin_settings["hide_models"] = [jazzmin_settings["hide_models"]]
     jazzmin_settings["hide_models"] = [x.lower() for x in jazzmin_settings["hide_models"]]
 
     # Ensure icon model names and classes are lower case
     jazzmin_settings["icons"] = {x.lower(): y.lower() for x, y in jazzmin_settings.get("icons", {}).items()}
 
     # Default the site icon using the site logo
```

### Comparing `django_jazzmin-2.6.1/jazzmin/static/admin/js/cancel.js` & `django_jazzmin-3.0.0/jazzmin/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/admin/js/popup_response.js` & `django_jazzmin-3.0.0/jazzmin/static/admin/js/popup_response.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -7,18 +7,14 @@
     var windowName, widgetName;
     var openerRef = windowRef.opener;
     if (!openerRef) {
         // related modal is active
         openerRef = windowRef.parent;
         windowName = windowRef.name;
         widgetName = windowName.replace(/^(change|add|delete|lookup)_/, '');
-        if (typeof(openerRef.id_to_windowname) === 'function') {
-            // django < 3.1 compatibility
-            widgetName = openerRef.id_to_windowname(widgetName);
-        }
         windowRefProxy = {
             name: widgetName,
             location: windowRef.location,
             close: function() {
                 openerRef.dismissRelatedObjectModal();
             }
         };
@@ -37,15 +33,12 @@
             if (typeof(openerRef.dismissDeleteRelatedObjectPopup) === 'function') {
                 openerRef.dismissDeleteRelatedObjectPopup(windowRef, initData.value);
             }
             break;
         default:
             if (typeof(openerRef.dismissAddRelatedObjectPopup) === 'function') {
                 openerRef.dismissAddRelatedObjectPopup(windowRef, initData.value, initData.obj);
-            } else if (typeof(openerRef.dismissAddAnotherPopup) === 'function') {
-                // django 1.7 compatibility
-                openerRef.dismissAddAnotherPopup(windowRef, initData.value, initData.obj);
             }
             break;
     }
 
 })();
```

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/css/main.css` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/css/main.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/calendar-icons.svg` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/default-log.svg` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/default-log.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/default.jpg` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/default.jpg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/icon-calendar.svg` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/img/selector-icons.svg` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/change_form.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/change_list.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/change_list.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/main.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/main.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/related-modal.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/related-modal.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/js/ui-builder.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/js/ui-builder.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js` & `django_jazzmin-3.0.0/jazzmin/static/jazzmin/plugins/bootstrap-show-modal/bootstrap-show-modal.min.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/css/adminlte.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/css/adminlte.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/css/adminlte.min.css.map` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/css/adminlte.min.css.map`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/AdminLTELogo.png` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/AdminLTELogo.png`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/icons.png` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/icons.png`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/img/user2-160x160.jpg` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/img/user2-160x160.jpg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/js/adminlte.min.js` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/js/adminlte.min.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/adminlte/js/adminlte.min.js.map` & `django_jazzmin-3.0.0/jazzmin/static/vendor/adminlte/js/adminlte.min.js.map`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js.map` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cerulean/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cerulean/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cosmo/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cosmo/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/cyborg/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/cyborg/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/darkly/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/default/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/default/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/flatly/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/journal/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/journal/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/litera/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/litera/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/lumen/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/lumen/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/lux/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/lux/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/materia/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/minty/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/minty/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/pulse/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/pulse/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/sandstone/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/sandstone/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/simplex/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/simplex/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/sketchy/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/sketchy/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/slate/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/solar/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/solar/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/spacelab/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/spacelab/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/superhero/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/superhero/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/united/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/united/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/bootswatch/yeti/bootstrap.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/bootswatch/yeti/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/css/all.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django_jazzmin-3.0.0/jazzmin/static/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/select2/css/select2.min.css` & `django_jazzmin-3.0.0/jazzmin/static/vendor/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/static/vendor/select2/js/select2.min.js` & `django_jazzmin-3.0.0/jazzmin/static/vendor/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/actions.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/app_index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/auth/user/change_password.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/base.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,18 @@
                     <div class="dropdown-menu dropdown-menu-lg dropdown-menu-left" id="jazzy-usermenu">
                         <span class="dropdown-header">{% trans 'Account' %}</span>
                         <div class="dropdown-divider"></div>
                         <a href="{% url 'admin:password_change' %}" class="dropdown-item">
                             <i class="fas fa-key mr-2"></i> {% trans 'Change password' %}
                         </a>
                         <div class="dropdown-divider"></div>
-                        <a href="{% url 'admin:logout' %}" class="dropdown-item">
-                            <i class="fas fa-users mr-2"></i> {% trans 'Log out' %}
-                        </a>
+                        <form id="logout-form" method="post" action="{% url 'admin:logout' %}">
+                            {% csrf_token %}
+                            <button type="submit" class="dropdown-item"><i class="fas fa-users mr-2"></i> {% translate 'Log out' %}</button>
+                        </form>
                         {% get_user_menu user request.current_app|default:"admin" as user_menu %}
                         {% for link in user_menu %}
                             <div class="dropdown-divider"></div>
                             <a href="{{ link.url }}" class="dropdown-item" {% if link.new_window %}target="_blank"{% endif %}>
                                 <i class="{{ link.icon }} mr-2"></i> {% trans link.name %}
                             </a>
                         {% endfor %}
```

#### html2text {}

```diff
@@ -37,15 +37,15 @@
       get_available_languages as LANGUAGES %} {% get_language_info_list for
       LANGUAGES as languages %}
     * {% csrf_token %} {% for language in languages %} {
       { language.name_local|title }} {% endfor %}
     * {% endif %}
     * {% trans 'Account' %}
       _{_%_ _t_r_a_n_s_ _'_C_h_a_n_g_e_ _p_a_s_s_w_o_r_d_'_ _%_}
-      _{_%_ _t_r_a_n_s_ _'_L_o_g_ _o_u_t_'_ _%_}
+      {% csrf_token %} {% translate 'Log out' %}
       {% get_user_menu user request.current_app|default:"admin" as user_menu %}
       {% for link in user_menu %}
       % if link.new_window %}target="_blank"{% endif %}> {% trans link.name %}
 {% endfor %}
 {% if perms|can_view_self %}
 }" class="dropdown-item dropdown-footer">{% trans 'See Profile' %}
  {% endif %}
```

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/change_form_object_tools.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/change_list.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/change_list_object_tools.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/change_list_results.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/date_hierarchy.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/delete_confirmation.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/delete_selected_confirmation.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/edit_inline/stacked.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/edit_inline/tabular.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/breadcrumbs.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/delete_selected_files_confirmation.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/delete_selected_files_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/file/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/file/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/folder/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/folder/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/folder/directory_listing.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/folder/directory_listing.html`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         <div class="js-navigator navigator{% if not actions_on_top and not actions_on_bottom %}navigator-no-actions{% endif %}">
             <form class="js-navigator-form" method="post">
                 {% csrf_token %}
                 {% filer_admin_context_hidden_formfields %}
                 {% if action_form and actions_on_top and paginator.count and not is_popup %}
                     {% filer_actions %}
                 {% endif %}
-                {% include "admin/filer/folder/directory_table.html" %}
+                {% include "admin/filer/folder/directory_table_list.html" %}
                 {% if action_form and actions_on_bottom and paginator.count and not is_popup %}
                     {% filer_actions %}
                 {% endif %}
             </form>
         </div>
     </div>
 {% endblock %}
```

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/image/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/image/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filer/tools/detail_info.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filer/tools/detail_info.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/filter.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/base.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/export.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/import_export/import.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/includes/fieldset.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/login.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/mptt_filter.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/mptt_filter.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/object_history.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/pagination.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/popup_response.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/search_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/solo/change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/solo/change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/solo/object_history.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/solo/object_history.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin/submit_line.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/base_docs.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/base_docs.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/bookmarklets.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/bookmarklets.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/missing_docutils.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/missing_docutils.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/model_detail.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/model_detail.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/model_index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/model_index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_detail.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_detail.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_filter_index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_filter_index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/template_tag_index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/template_tag_index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/view_detail.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/view_detail.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/admin_doc/view_index.html` & `django_jazzmin-3.0.0/jazzmin/templates/admin_doc/view_index.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/carousel.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/carousel.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/collapsible.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/collapsible.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/horizontal_tabs.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/horizontal_tabs.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/related_modal.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/related_modal.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/single.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/single.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/ui_builder_panel.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/ui_builder_panel.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/jazzmin/includes/vertical_tabs.html` & `django_jazzmin-3.0.0/jazzmin/templates/jazzmin/includes/vertical_tabs.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/base.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/base.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/password_change_done.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/password_change_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_confirm.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_done.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templates/registration/password_reset_form.html` & `django_jazzmin-3.0.0/jazzmin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/jazzmin/templatetags/jazzmin.py` & `django_jazzmin-3.0.0/jazzmin/templatetags/jazzmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,21 @@
 from django.utils.html import escape, format_html
 from django.utils.safestring import SafeText, mark_safe
 from django.utils.text import get_text_list, slugify
 from django.utils.translation import gettext
 
 from .. import version
 from ..settings import CHANGEFORM_TEMPLATES, get_settings, get_ui_tweaks
-from ..utils import get_admin_url, get_filter_id, has_fieldsets_check, make_menu, order_with_respect_to
+from ..utils import (
+    get_admin_url,
+    get_filter_id,
+    has_fieldsets_check,
+    make_menu,
+    order_with_respect_to,
+)
 
 User = get_user_model()
 register = Library()
 logger = logging.getLogger(__name__)
 
 
 @register.simple_tag(takes_context=True)
@@ -114,15 +120,21 @@
 
 @register.simple_tag
 def get_user_menu(user: AbstractUser, admin_site: str = "admin") -> List[Dict]:
     """
     Produce the menu for the user dropdown
     """
     options = get_settings()
-    return make_menu(user, options.get("usermenu_links", []), options, allow_appmenus=False, admin_site=admin_site)
+    return make_menu(
+        user,
+        options.get("usermenu_links", []),
+        options,
+        allow_appmenus=False,
+        admin_site=admin_site,
+    )
 
 
 @register.simple_tag
 def get_jazzmin_settings(request: WSGIRequest) -> Dict:
     """
     Get Jazzmin settings, update any defaults from the request, and return
     """
@@ -174,23 +186,25 @@
         return no_avatar
 
     if callable(avatar_field_name):
         return avatar_field_name(user)
 
     # If we find the property directly on the user model (imagefield or URLfield)
     avatar_field = getattr(user, avatar_field_name, None)
-    if avatar_field:
-        if type(avatar_field) == str:
+    if avatar_field is not None:
+        if not avatar_field:
+            return no_avatar
+        if isinstance(avatar_field, str):
             return avatar_field
         elif hasattr(avatar_field, "url"):
             return avatar_field.url
         elif callable(avatar_field):
             return avatar_field()
 
-    logger.warning("avatar field must be an ImageField/URLField on the user model, or a callable")
+    logger.warning("Avatar field must be an ImageField/URLField on the user model, or a callable")
 
     return no_avatar
 
 
 @register.simple_tag
 def jazzmin_paginator_number(change_list: ChangeList, i: int) -> SafeText:
     """
@@ -204,63 +218,55 @@
 
     if start:
         link = change_list.get_query_string({PAGE_VAR: change_list.page_num - 1}) if change_list.page_num > 1 else "#"
         html_str += """
         <li class="page-item previous {disabled}">
             <a class="page-link" href="{link}" data-dt-idx="0" tabindex="0">«</a>
         </li>
-        """.format(
-            link=link, disabled="disabled" if link == "#" else ""
-        )
+        """.format(link=link, disabled="disabled" if link == "#" else "")
 
     if current_page:
         html_str += """
         <li class="page-item active">
             <a class="page-link" href="javascript:void(0);" data-dt-idx="3" tabindex="0">{num}</a>
         </li>
-        """.format(
-            num=i
-        )
+        """.format(num=i)
     elif spacer:
         html_str += """
         <li class="page-item">
             <a class="page-link" href="javascript:void(0);" data-dt-idx="3" tabindex="0">… </a>
         </li>
         """
     else:
         query_string = change_list.get_query_string({PAGE_VAR: i})
         end = "end" if end else ""
         html_str += """
             <li class="page-item">
             <a href="{query_string}" class="page-link {end}" data-dt-idx="3" tabindex="0">{num}</a>
             </li>
-        """.format(
-            num=i, query_string=query_string, end=end
-        )
+        """.format(num=i, query_string=query_string, end=end)
 
     if end:
         link = change_list.get_query_string({PAGE_VAR: change_list.page_num + 1}) if change_list.page_num < i else "#"
         html_str += """
         <li class="page-item next {disabled}">
             <a class="page-link" href="{link}" data-dt-idx="7" tabindex="0">»</a>
         </li>
-        """.format(
-            link=link, disabled="disabled" if link == "#" else ""
-        )
+        """.format(link=link, disabled="disabled" if link == "#" else "")
 
     return format_html(html_str)
 
 
 @register.simple_tag
 def admin_extra_filters(cl: ChangeList) -> Dict:
     """
     Return the dict of used filters which is not included in list_filters form
     """
     used_parameters = list(itertools.chain(*(s.used_parameters.keys() for s in cl.filter_specs)))
-    return dict((k, v) for k, v in cl.params.items() if k not in used_parameters)
+    return {k: v for k, v in cl.params.items() if k not in used_parameters}
 
 
 @register.simple_tag
 def jazzmin_list_filter(cl: ChangeList, spec: ListFilter) -> SafeText:
     """
     Render out our list filter in a dropdown friendly format, for use by filter.html, see original implementation here
 
@@ -326,15 +332,15 @@
 @register.simple_tag
 def get_sections(
     admin_form: AdminForm, inline_admin_formsets: List[InlineAdminFormSet]
 ) -> List[Union[Fieldset, InlineAdminFormSet]]:
     """
     Get and sort all of the sections that need rendering out in a change form
     """
-    fieldsets = [x for x in admin_form]
+    fieldsets = list(admin_form)
 
     # Make inlines behave like formsets
     for fieldset in inline_admin_formsets:
         fieldset.name = capfirst(fieldset.opts.verbose_name_plural)
         fieldset.is_inline = True
         fieldsets.append(fieldset)
 
@@ -453,15 +459,15 @@
     """
     Checks if an app has been installed under INSTALLED_APPS on the project settings
     """
     return app in settings.INSTALLED_APPS
 
 
 @register.simple_tag
-def action_message_to_list(action: LogEntry) -> List[Dict]:
+def action_message_to_list(action: LogEntry) -> List[Dict]:  # noqa: C901
     """
     Retrieves a formatted list with all actions taken by a user given a log entry object
     """
     messages = []
 
     def added(x: str) -> Dict:
         return {
@@ -524,15 +530,15 @@
     message_words = escape(message).split()
 
     if not len(message_words):
         return ""
 
     message_words[0] = "<strong>{}</strong>".format(message_words[0])
 
-    message = " ".join([word for word in message_words])
+    message = " ".join(list(message_words))
 
     return mark_safe(message)
 
 
 @register.filter
 def unicode_slugify(message: str) -> str:
     return slugify(message, allow_unicode=True)
```

### Comparing `django_jazzmin-2.6.1/jazzmin/utils.py` & `django_jazzmin-3.0.0/jazzmin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
-from typing import List, Union, Dict, Set, Callable, Any
+from typing import Any, Callable, Dict, List, Set, Union
 from urllib.parse import urlencode
 
 from django.apps import apps
 from django.contrib.admin import ListFilter
 from django.contrib.admin.helpers import AdminForm
 from django.contrib.auth.models import AbstractUser
-from django.db.models.base import ModelBase, Model
+from django.db.models.base import Model, ModelBase
 from django.db.models.options import Options
 from django.utils.translation import gettext
 
 from jazzmin.compat import NoReverseMatch, reverse
 
 logger = logging.getLogger(__name__)
 
@@ -36,16 +36,15 @@
 def get_admin_url(instance: Any, admin_site: str = "admin", from_app: bool = False, **kwargs: str) -> str:
     """
     Return the admin URL for the given instance, model class or <app>.<model> string
     """
     url = "#"
 
     try:
-
-        if type(instance) == str:
+        if isinstance(instance, str):
             app_label, model_name = instance.split(".")
             model_name = model_name.lower()
             url = reverse(
                 "admin:{app_label}_{model_name}_changelist".format(app_label=app_label, model_name=model_name),
                 current_app=admin_site,
             )
 
@@ -161,15 +160,14 @@
     if not user:
         return []
 
     model_permissions = get_view_permissions(user)
 
     menu = []
     for link in links:
-
         perm_matches = []
         for perm in link.get("permissions", []):
             perm_matches.append(user.has_perm(perm))
 
         if not all(perm_matches):
             continue
```

### Comparing `django_jazzmin-2.6.1/jazzmin/widgets.py` & `django_jazzmin-3.0.0/jazzmin/widgets.py`

 * *Files identical despite different names*

### Comparing `django_jazzmin-2.6.1/PKG-INFO` & `django_jazzmin-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,86 @@
 Metadata-Version: 2.1
 Name: django-jazzmin
-Version: 2.6.1
+Version: 3.0.0
 Summary: Drop-in theme for django admin, that utilises AdminLTE 3 & Bootstrap 4 to make yo' admin look jazzy
 Home-page: https://github.com/farridav/django-jazzmin
 License: MIT
 Keywords: django,dashboard,theme,admin,jazzmin
 Author: Shipit
 Author-email: packages@shipit.ltd
 Maintainer: Shipit
 Maintainer-email: packages@shipit.ltd
-Requires-Python: >=3.6.2
+Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: django (>=2.2)
+Requires-Dist: django (>=4.2)
 Project-URL: All Releases, https://github.com/farridav/django-jazzmin/releases
 Project-URL: Bug Tracker, https://github.com/farridav/django-jazzmin/issues
 Project-URL: Documentation, https://django-jazzmin.readthedocs.io
 Project-URL: Latest Release, https://github.com/farridav/django-jazzmin/releases/latest
 Project-URL: Repository, https://github.com/farridav/django-jazzmin
 Project-URL: Source, https://github.com/farridav/django-jazzmin
 Description-Content-Type: text/markdown
 
 
 # Django jazzmin (Jazzy Admin)
 
+## Project Status
+
+This project is being actively maintained, though with a reduced feature set, we are looking for contributors to help
+maintain and improve the project, please get in touch if you would like to help.
+
+Help needed with:
+
+- Triaging issues
+- Frontend fixes and UI improvements
+- Testing
+- Documentation
+
+Pull requests are welcome, though ive been pre-occupied with other projects lately, so have not been able to review
+them as quickly as I would like, but im trying to get through them all now, hopefully with some outside help.
+
 [![Docs](https://readthedocs.org/projects/django-jazzmin/badge/?version=latest)](https://django-jazzmin.readthedocs.io)
 ![PyPI download month](https://img.shields.io/pypi/dm/django-jazzmin.svg)
 [![PyPI version](https://badge.fury.io/py/django-jazzmin.svg)](https://pypi.python.org/pypi/django-jazzmin/)
-![Python versions](https://img.shields.io/badge/python-%3E%3D3.6-brightgreen)
-![Django Versions](https://img.shields.io/badge/django-%3E%3D2-brightgreen)
+![Python versions](https://img.shields.io/badge/python-%3E=3.8-brightgreen)
+![Django Versions](https://img.shields.io/badge/django-%3E=4.2-brightgreen)
 [![Coverage Status](https://coveralls.io/repos/github/farridav/django-jazzmin/badge.svg?branch=master)](https://coveralls.io/github/farridav/django-jazzmin?branch=master)
 
 Drop-in theme for django admin, that utilises AdminLTE 3 & Bootstrap 4 to make yo' admin look jazzy
 
 ## Installation
-```
+
+```bash
 pip install django-jazzmin
 ```
 
 ## Documentation
-See [Documentation](https://django-jazzmin.readthedocs.io) or [Test App](https://github.com/farridav/django-jazzmin/tree/master/tests/test_app/library/settings.py)
 
-## Demo
-Live demo https://django-jazzmin.herokuapp.com/admin
-
-**Username**: test@test.com
-
-**Password**: test
-
-*Note: Data resets nightly*
+See [Documentation](https://django-jazzmin.readthedocs.io) or [Test App](https://github.com/farridav/django-jazzmin/tree/master/tests/test_app/library/settings.py)
 
 ## Features
+
 - Drop-in admin skin, all configuration optional
 - Customisable side menu
 - Customisable top menu
 - Customisable user menu
 - 4 different Change form templates (horizontal tabs, vertical tabs, carousel, collapsible)
 - Bootstrap 4 modal (instead of the old popup window, optional)
 - Search bar for any given model admin
@@ -83,64 +89,80 @@
 - Select2 drop-downs
 - Bootstrap 4 & AdminLTE UI components
 - Using the latest [adminlte](https://adminlte.io/) + [bootstrap](https://getbootstrap.com/)
 
 ## Screenshots
 
 ## Dashboard
+
 ![dashboard](https://django-jazzmin.readthedocs.io/img/dashboard.png)
 
 ## List view
+
 ![table list](https://django-jazzmin.readthedocs.io/img/list_view.png)
 
 ## Change form templates
 
 ### Collapsed side menu
+
 ![form page](https://django-jazzmin.readthedocs.io/img/detail_view.png)
 
 ### Expanded side menu
+
 ![Single](https://django-jazzmin.readthedocs.io/img/changeform_single.png)
 
 ### Horizontal tabs
+
 ![Horizontal tabs](https://django-jazzmin.readthedocs.io/img/changeform_horizontal_tabs.png)
 
 ### Vertical tabs
+
 ![Vertical tabs](https://django-jazzmin.readthedocs.io/img/changeform_vertical_tabs.png)
 
 ### Collapsible
+
 ![Collapsible](https://django-jazzmin.readthedocs.io/img/changeform_collapsible.png)
 
 ### Carousel
+
 ![Carousel](https://django-jazzmin.readthedocs.io/img/changeform_carousel.png)
 
 ### Related modal
+
 ![Related modal](https://django-jazzmin.readthedocs.io/img/related_modal_bootstrap.png)
 
 ## History page
+
 ![form page](https://django-jazzmin.readthedocs.io/img/history_page.png)
 
 ## Login view
+
 ![login](https://django-jazzmin.readthedocs.io/img/login.png)
 
 ## UI Customiser
+
 ![ui_customiser](https://django-jazzmin.readthedocs.io/img/ui_customiser.png)
 
 ## Mobile layout
+
 ![mobile](https://django-jazzmin.readthedocs.io/img/dashboard_mobile.png)
 
 ## Tablet layout
+
 ![tablet](https://django-jazzmin.readthedocs.io/img/dashboard_tablet.png)
 
 ## Admin Docs (if installed)
+
 ![admin_docs](https://django-jazzmin.readthedocs.io/img/admin_docs.png)
 
 ## Thanks
-This was initially a Fork of https://github.com/wuyue92tree/django-adminlte-ui that we refactored so much we thought it
+
+This was initially a Fork of <https://github.com/wuyue92tree/django-adminlte-ui> that we refactored so much we thought it
 deserved its own package, big thanks to @wuyue92tree for all of his initial hard work, we are still patching into that
 project were possible, but this project has taken a different direction.
 
 The javascript modal implementation uses some code from [django-admin-interface](https://github.com/fabiocaccamo/django-admin-interface/blob/master/admin_interface/static/admin/js/popup_response.js), so thanks to @fabiocaccamo for original work
 
-- Based on AdminLTE 3: https://adminlte.io/
-- Using Bootstrap 4: https://getbootstrap.com/
-- Using Font Awesome 5: https://fontawesome.com/
+- Based on AdminLTE 3: <https://adminlte.io/>
+- Using Bootstrap 4: <https://getbootstrap.com/>
+- Using Font Awesome 5: <https://fontawesome.com/>
```

