# Comparing `tmp/esanom-0.7.12.11.tar.gz` & `tmp/esanom-0.7.12.7720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-0.7.12.11.tar", max compression
+gzip compressed data, was "esanom-0.7.12.7720.tar", max compression
```

## Comparing `esanom-0.7.12.11.tar` & `esanom-0.7.12.7720.tar`

### file list

```diff
@@ -1,218 +1,220 @@
--rw-r--r--   0        0        0        0 2024-04-18 14:42:38.051798 esanom-0.7.12.11/README.md
--rw-r--r--   0        0        0      144 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/CHANGELOG.txt
--rw-r--r--   0        0        0      388 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/COPYRIGHT.txt
--rw-r--r--   0        0        0    17260 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/LICENCE.txt
--rw-r--r--   0        0        0     1413 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/__init__.py
--rw-r--r--   0        0        0     5950 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/client.py
--rw-r--r--   0        0        0     5156 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/config.py
--rw-r--r--   0        0        0    47586 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/database.py
--rw-r--r--   0        0        0     1125 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/engine.py
--rw-r--r--   0        0        0     2496 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/monitor.py
--rw-r--r--   0        0        0    10320 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/orchestrator.py
--rw-r--r--   0        0        0    12985 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/pipeline.py
--rw-r--r--   0        0        0     1665 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/account.sql
--rw-r--r--   0        0        0     1828 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/api.sql
--rw-r--r--   0        0        0     1352 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/api_group.sql
--rw-r--r--   0        0        0     1326 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/api_role.sql
--rw-r--r--   0        0        0     1226 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/claim.sql
--rw-r--r--   0        0        0     1215 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/group.sql
--rw-r--r--   0        0        0     1828 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/io.sql
--rw-r--r--   0        0        0     1416 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/ioblock.sql
--rw-r--r--   0        0        0     1680 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/log.sql
--rw-r--r--   0        0        0     1950 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/mpin.sql
--rw-r--r--   0        0        0     1921 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/mport.sql
--rw-r--r--   0        0        0     1536 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/pin.sql
--rw-r--r--   0        0        0     1842 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/pipeline.sql
--rw-r--r--   0        0        0     1514 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/pipeline_task.sql
--rw-r--r--   0        0        0     1501 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/port.sql
--rw-r--r--   0        0        0     1388 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/port_pin.sql
--rw-r--r--   0        0        0     1126 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/role.sql
--rw-r--r--   0        0        0     1250 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/roleadmin.sql
--rw-r--r--   0        0        0     1257 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/roledashboard.sql
--rw-r--r--   0        0        0     2173 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/rolemodel.sql
--rw-r--r--   0        0        0     1655 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/roleuser.sql
--rw-r--r--   0        0        0     1319 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/schedule.sql
--rw-r--r--   0        0        0     1156 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/session.sql
--rw-r--r--   0        0        0     1236 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/system.sql
--rw-r--r--   0        0        0     1914 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/task.sql
--rw-r--r--   0        0        0     5741 2024-04-18 14:42:38.519804 esanom-0.7.12.11/esanom/resources/database/triggers.sql
--rw-r--r--   0        0        0     1497 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/resources/database/unit.sql
--rw-r--r--   0        0        0    11022 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/roleadmin.py
--rw-r--r--   0        0        0     4208 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/rolemodel.py
--rw-r--r--   0        0        0     3456 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/roleuser.py
--rw-r--r--   0        0        0      790 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/__init__.py
--rw-r--r--   0        0        0    38001 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/api.py
--rw-r--r--   0        0        0    40721 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/api.py-bak1
--rw-r--r--   0        0        0     8952 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/common.py
--rw-r--r--   0        0        0    80721 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   232803 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/bootstrap.min.css
--rw-r--r--   0        0        0      639 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/dashboard.css
--rw-r--r--   0        0        0    20832 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/routes/v3/static/datatables.min.css
--rw-r--r--   0        0        0   197654 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/routes/v3/static/datatables.min.js
--rw-r--r--   0        0        0      318 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/favicon.ico
--rw-r--r--   0        0        0    48036 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/htmx.min.js
--rw-r--r--   0        0        0       97 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/main.css
--rw-r--r--   0        0        0      422 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/main.js
--rw-r--r--   0        0        0     1723 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/nom-logo.png
--rw-r--r--   0        0        0  3620840 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/routes/v3/static/plotly.min.js
--rw-r--r--   0        0        0     1741 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/static/theme.css
--rw-r--r--   0        0        0      717 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/admin_db_pipeline_row.html
--rw-r--r--   0        0        0      627 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/admin_db_pipeline_rows.html
--rw-r--r--   0        0        0     1542 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/base.html
--rw-r--r--   0        0        0     1000 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/db_rolemodel_row.html
--rw-r--r--   0        0        0      633 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/db_rolemodel_rows.html
--rw-r--r--   0        0        0      140 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/dummy.html
--rw-r--r--   0        0        0      153 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/error_404.html
--rw-r--r--   0        0        0      114 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/error_500.html
--rw-r--r--   0        0        0       82 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
--rw-r--r--   0        0        0      731 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_model_io.html
--rw-r--r--   0        0        0     1331 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_model_io_port.html
--rw-r--r--   0        0        0      808 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_models.html
--rw-r--r--   0        0        0      836 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_pipelines.html
--rw-r--r--   0        0        0     2019 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_debug.html
--rw-r--r--   0        0        0      248 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_loggedin_nav.html
--rw-r--r--   0        0        0      586 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
--rw-r--r--   0        0        0      300 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
--rw-r--r--   0        0        0      282 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_loggedin_nav_member.html
--rw-r--r--   0        0        0      182 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_footer.html
--rw-r--r--   0        0        0      628 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_head.html
--rw-r--r--   0        0        0     1332 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_header.html
--rw-r--r--   0        0        0      173 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_header_logo.html
--rw-r--r--   0        0        0      487 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_header_nav.html
--rw-r--r--   0        0        0      240 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_header_toggle.html
--rw-r--r--   0        0        0      153 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/navigation.html
--rw-r--r--   0        0        0      327 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_admin_pipelines.html
--rw-r--r--   0        0        0      921 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_dashboard_tasks.html
--rw-r--r--   0        0        0      115 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_docs.html
--rw-r--r--   0        0        0      116 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_index.html
--rw-r--r--   0        0        0      121 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_interfaces.html
--rw-r--r--   0        0        0      516 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_model.html
--rw-r--r--   0        0        0      157 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/templates/page_models.html
--rw-r--r--   0        0        0      128 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin/main.html
--rw-r--r--   0        0        0       94 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
--rw-r--r--   0        0        0     1378 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
--rw-r--r--   0        0        0      188 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_account_create/main.html
--rw-r--r--   0        0        0        5 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
--rw-r--r--   0        0        0      110 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
--rw-r--r--   0        0        0      429 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
--rw-r--r--   0        0        0      299 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
--rw-r--r--   0        0        0      315 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/main.html
--rw-r--r--   0        0        0      272 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/read.html
--rw-r--r--   0        0        0      114 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
--rw-r--r--   0        0        0      248 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
--rw-r--r--   0        0        0      207 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/update.html
--rw-r--r--   0        0        0     1887 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
--rw-r--r--   0        0        0      113 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
--rw-r--r--   0        0        0      544 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_read/main.html
--rw-r--r--   0        0        0        6 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
--rw-r--r--   0        0        0     1221 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
--rw-r--r--   0        0        0      474 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
--rw-r--r--   0        0        0      256 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_update/main.html
--rw-r--r--   0        0        0      421 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
--rw-r--r--   0        0        0      369 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
--rw-r--r--   0        0        0      240 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_apis/main.html
--rw-r--r--   0        0        0       94 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
--rw-r--r--   0        0        0      324 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
--rw-r--r--   0        0        0      263 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_create/main.html
--rw-r--r--   0        0        0      111 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
--rw-r--r--   0        0        0      278 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_read/main.html
--rw-r--r--   0        0        0        6 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
--rw-r--r--   0        0        0      718 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
--rw-r--r--   0        0        0      352 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_update/main.html
--rw-r--r--   0        0        0       87 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
--rw-r--r--   0        0        0      425 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_groups/main.html
--rw-r--r--   0        0        0      111 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
--rw-r--r--   0        0        0      332 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_read/main.html
--rw-r--r--   0        0        0       24 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
--rw-r--r--   0        0        0      897 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
--rw-r--r--   0        0        0      403 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_update/main.html
--rw-r--r--   0        0        0      425 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_models/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
--rw-r--r--   0        0        0      245 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_models/main.html
--rw-r--r--   0        0        0       40 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
--rw-r--r--   0        0        0      413 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
--rw-r--r--   0        0        0      463 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
--rw-r--r--   0        0        0      260 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_settings/main.html
--rw-r--r--   0        0        0       82 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
--rw-r--r--   0        0        0       82 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
--rw-r--r--   0        0        0      118 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/main.html
--rw-r--r--   0        0        0      895 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/pipelines.html
--rw-r--r--   0        0        0      891 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/tasks.html
--rw-r--r--   0        0        0      640 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
--rw-r--r--   0        0        0     1218 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
--rw-r--r--   0        0        0       26 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
--rw-r--r--   0        0        0      770 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
--rw-r--r--   0        0        0      128 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/main.html
--rw-r--r--   0        0        0       60 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/login/hx_login.html
--rw-r--r--   0        0        0      766 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/login/main.html
--rw-r--r--   0        0        0      133 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/logout/main.html
--rw-r--r--   0        0        0      128 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member/main.html
--rw-r--r--   0        0        0      617 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
--rw-r--r--   0        0        0      789 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
--rw-r--r--   0        0        0      182 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_api_create/main.html
--rw-r--r--   0        0        0      347 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
--rw-r--r--   0        0        0      423 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/inc_table.html
--rw-r--r--   0        0        0      367 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
--rw-r--r--   0        0        0      416 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/main.html
--rw-r--r--   0        0        0      256 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/read.html
--rw-r--r--   0        0        0      129 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/update.html
--rw-r--r--   0        0        0      637 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
--rw-r--r--   0        0        0      347 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
--rw-r--r--   0        0        0      442 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/inc_table.html
--rw-r--r--   0        0        0      163 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
--rw-r--r--   0        0        0      241 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/main.html
--rw-r--r--   0        0        0      256 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/read.html
--rw-r--r--   0        0        0      129 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/update.html
--rw-r--r--   0        0        0      637 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
--rw-r--r--   0        0        0      428 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read.html
--rw-r--r--   0        0        0      160 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_info.html
--rw-r--r--   0        0        0     1331 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_port.html
--rw-r--r--   0        0        0     1331 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
--rw-r--r--   0        0        0      733 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_ports.html
--rw-r--r--   0        0        0      238 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/rows.html
--rw-r--r--   0        0        0      424 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/rows_inc_table.html
--rw-r--r--   0        0        0      607 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
--rw-r--r--   0        0        0      322 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/read.html
--rw-r--r--   0        0        0       92 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/read_inc_info.html
--rw-r--r--   0        0        0      174 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
--rw-r--r--   0        0        0      130 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
--rw-r--r--   0        0        0      432 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
--rw-r--r--   0        0        0      234 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/rows.html
--rw-r--r--   0        0        0      420 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
--rw-r--r--   0        0        0      339 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 14:42:38.535804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/read.html
--rw-r--r--   0        0        0       92 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/read_inc_info.html
--rw-r--r--   0        0        0      422 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/read_inc_table.html
--rw-r--r--   0        0        0      309 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
--rw-r--r--   0        0        0      125 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
--rw-r--r--   0        0        0      236 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/rows.html
--rw-r--r--   0        0        0      422 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
--rw-r--r--   0        0        0      340 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 14:42:38.531804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
--rw-r--r--   0        0        0      265 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/register/hx_form.html
--rw-r--r--   0        0        0      387 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/register/main.html
--rw-r--r--   0        0        0     1037 2024-04-18 14:42:38.527804 esanom-0.7.12.11/esanom/routes/v3/templates/pages/register/main_inc_form.html
--rw-r--r--   0        0        0    49163 2024-04-18 14:42:38.523804 esanom-0.7.12.11/esanom/routes/v3/web.py
--rw-r--r--   0        0        0     1693 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/sample_gunicorn_config.py
--rw-r--r--   0        0        0      753 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/sample_nom_config.json
--rw-r--r--   0        0        0     5050 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/scheduler.py
--rw-r--r--   0        0        0     3661 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/server.py
--rw-r--r--   0        0        0    12199 2024-04-18 14:42:38.539804 esanom-0.7.12.11/esanom/util.py
--rw-r--r--   0        0        0      443 2024-04-18 14:42:44.155867 esanom-0.7.12.11/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 esanom-0.7.12.11/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 16:51:07.558558 esanom-0.7.12.7720/README.md
+-rw-r--r--   0        0        0      144 2024-04-18 16:51:08.006550 esanom-0.7.12.7720/esanom/CHANGELOG.txt
+-rw-r--r--   0        0        0      388 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/COPYRIGHT.txt
+-rw-r--r--   0        0        0    17260 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/LICENCE.txt
+-rw-r--r--   0        0        0     1413 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/__init__.py
+-rw-r--r--   0        0        0     5950 2024-04-18 16:51:08.006550 esanom-0.7.12.7720/esanom/client.py
+-rw-r--r--   0        0        0     5156 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/config.py
+-rw-r--r--   0        0        0    47586 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/database.py
+-rw-r--r--   0        0        0     1125 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/engine.py
+-rw-r--r--   0        0        0     2496 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/monitor.py
+-rw-r--r--   0        0        0    10320 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/orchestrator.py
+-rw-r--r--   0        0        0    12985 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/pipeline.py
+-rw-r--r--   0        0        0     1665 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/account.sql
+-rw-r--r--   0        0        0     1828 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/api.sql
+-rw-r--r--   0        0        0     1352 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/api_group.sql
+-rw-r--r--   0        0        0     1326 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/api_role.sql
+-rw-r--r--   0        0        0     1226 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/claim.sql
+-rw-r--r--   0        0        0     1215 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/group.sql
+-rw-r--r--   0        0        0     1828 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/io.sql
+-rw-r--r--   0        0        0     1416 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/ioblock.sql
+-rw-r--r--   0        0        0     1680 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/log.sql
+-rw-r--r--   0        0        0     1950 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/mpin.sql
+-rw-r--r--   0        0        0     1921 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/mport.sql
+-rw-r--r--   0        0        0     1536 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/pin.sql
+-rw-r--r--   0        0        0     1842 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/pipeline.sql
+-rw-r--r--   0        0        0     1514 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/pipeline_task.sql
+-rw-r--r--   0        0        0     1501 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/port.sql
+-rw-r--r--   0        0        0     1388 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/port_pin.sql
+-rw-r--r--   0        0        0     1126 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/role.sql
+-rw-r--r--   0        0        0     1250 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/roleadmin.sql
+-rw-r--r--   0        0        0     1257 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/roledashboard.sql
+-rw-r--r--   0        0        0     2173 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/rolemodel.sql
+-rw-r--r--   0        0        0     1655 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/roleuser.sql
+-rw-r--r--   0        0        0     1319 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/schedule.sql
+-rw-r--r--   0        0        0     1156 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/session.sql
+-rw-r--r--   0        0        0     1236 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/system.sql
+-rw-r--r--   0        0        0     1914 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/task.sql
+-rw-r--r--   0        0        0     5741 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/triggers.sql
+-rw-r--r--   0        0        0     1497 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/resources/database/unit.sql
+-rw-r--r--   0        0        0    11022 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/roleadmin.py
+-rw-r--r--   0        0        0     4208 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/rolemodel.py
+-rw-r--r--   0        0        0     3456 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/roleuser.py
+-rw-r--r--   0        0        0      790 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/__init__.py
+-rw-r--r--   0        0        0    38001 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/api.py
+-rw-r--r--   0        0        0    40721 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/api.py-bak1
+-rw-r--r--   0        0        0     8952 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/common.py
+-rw-r--r--   0        0        0    80721 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   232803 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/bootstrap.min.css
+-rw-r--r--   0        0        0      639 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/dashboard.css
+-rw-r--r--   0        0        0    20832 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/routes/v3/static/datatables.min.css
+-rw-r--r--   0        0        0   197654 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/routes/v3/static/datatables.min.js
+-rw-r--r--   0        0        0      318 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/favicon.ico
+-rw-r--r--   0        0        0    48036 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/htmx.min.js
+-rw-r--r--   0        0        0       97 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/main.css
+-rw-r--r--   0        0        0      422 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/main.js
+-rw-r--r--   0        0        0     1723 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/nom-logo.png
+-rw-r--r--   0        0        0  3620840 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/routes/v3/static/plotly.min.js
+-rw-r--r--   0        0        0     1741 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/static/theme.css
+-rw-r--r--   0        0        0      717 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/admin_db_pipeline_row.html
+-rw-r--r--   0        0        0      627 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/admin_db_pipeline_rows.html
+-rw-r--r--   0        0        0     1542 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/base.html
+-rw-r--r--   0        0        0     1000 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/db_rolemodel_row.html
+-rw-r--r--   0        0        0      633 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/db_rolemodel_rows.html
+-rw-r--r--   0        0        0      140 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/dummy.html
+-rw-r--r--   0        0        0      153 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/error_404.html
+-rw-r--r--   0        0        0      114 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/error_500.html
+-rw-r--r--   0        0        0       82 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
+-rw-r--r--   0        0        0      731 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_model_io.html
+-rw-r--r--   0        0        0     1331 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_model_io_port.html
+-rw-r--r--   0        0        0      808 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_models.html
+-rw-r--r--   0        0        0      836 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_pipelines.html
+-rw-r--r--   0        0        0     2019 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_debug.html
+-rw-r--r--   0        0        0      248 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_loggedin_nav.html
+-rw-r--r--   0        0        0      586 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
+-rw-r--r--   0        0        0      300 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
+-rw-r--r--   0        0        0      282 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_loggedin_nav_member.html
+-rw-r--r--   0        0        0      182 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_footer.html
+-rw-r--r--   0        0        0      628 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_head.html
+-rw-r--r--   0        0        0     1332 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_header.html
+-rw-r--r--   0        0        0      173 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_header_logo.html
+-rw-r--r--   0        0        0      487 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_header_nav.html
+-rw-r--r--   0        0        0      240 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_header_toggle.html
+-rw-r--r--   0        0        0      153 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/navigation.html
+-rw-r--r--   0        0        0      327 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_admin_pipelines.html
+-rw-r--r--   0        0        0      921 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_dashboard_tasks.html
+-rw-r--r--   0        0        0      115 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_docs.html
+-rw-r--r--   0        0        0      116 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_index.html
+-rw-r--r--   0        0        0      121 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_interfaces.html
+-rw-r--r--   0        0        0      516 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_model.html
+-rw-r--r--   0        0        0      157 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/page_models.html
+-rw-r--r--   0        0        0      128 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin/main.html
+-rw-r--r--   0        0        0       94 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
+-rw-r--r--   0        0        0     1378 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
+-rw-r--r--   0        0        0      188 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_account_create/main.html
+-rw-r--r--   0        0        0        5 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
+-rw-r--r--   0        0        0      110 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
+-rw-r--r--   0        0        0      429 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
+-rw-r--r--   0        0        0      299 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
+-rw-r--r--   0        0        0      315 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/main.html
+-rw-r--r--   0        0        0      272 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/read.html
+-rw-r--r--   0        0        0      114 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
+-rw-r--r--   0        0        0      248 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
+-rw-r--r--   0        0        0      207 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/update.html
+-rw-r--r--   0        0        0     1887 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
+-rw-r--r--   0        0        0      113 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
+-rw-r--r--   0        0        0      544 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
+-rw-r--r--   0        0        0     1221 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
+-rw-r--r--   0        0        0      474 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
+-rw-r--r--   0        0        0      256 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_update/main.html
+-rw-r--r--   0        0        0      421 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
+-rw-r--r--   0        0        0      369 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
+-rw-r--r--   0        0        0      240 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_apis/main.html
+-rw-r--r--   0        0        0       94 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
+-rw-r--r--   0        0        0      324 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
+-rw-r--r--   0        0        0      263 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_create/main.html
+-rw-r--r--   0        0        0      111 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
+-rw-r--r--   0        0        0      278 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
+-rw-r--r--   0        0        0      718 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
+-rw-r--r--   0        0        0      352 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_update/main.html
+-rw-r--r--   0        0        0       87 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
+-rw-r--r--   0        0        0      425 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_groups/main.html
+-rw-r--r--   0        0        0      111 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
+-rw-r--r--   0        0        0      332 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_read/main.html
+-rw-r--r--   0        0        0       24 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
+-rw-r--r--   0        0        0      897 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
+-rw-r--r--   0        0        0      403 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_update/main.html
+-rw-r--r--   0        0        0      425 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_models/inc_table.html
+-rw-r--r--   0        0        0      296 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
+-rw-r--r--   0        0        0      245 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_models/main.html
+-rw-r--r--   0        0        0       40 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
+-rw-r--r--   0        0        0      307 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/inc_form_pins.html
+-rw-r--r--   0        0        0      311 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/inc_form_ports.html
+-rw-r--r--   0        0        0      413 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
+-rw-r--r--   0        0        0      463 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
+-rw-r--r--   0        0        0      380 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_settings/main.html
+-rw-r--r--   0        0        0       82 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
+-rw-r--r--   0        0        0       82 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
+-rw-r--r--   0        0        0      118 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/main.html
+-rw-r--r--   0        0        0      895 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/pipelines.html
+-rw-r--r--   0        0        0      891 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/tasks.html
+-rw-r--r--   0        0        0      640 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
+-rw-r--r--   0        0        0     1218 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
+-rw-r--r--   0        0        0       26 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
+-rw-r--r--   0        0        0      770 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
+-rw-r--r--   0        0        0      128 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/main.html
+-rw-r--r--   0        0        0       60 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/login/hx_login.html
+-rw-r--r--   0        0        0      766 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/login/main.html
+-rw-r--r--   0        0        0      133 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/logout/main.html
+-rw-r--r--   0        0        0      128 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member/main.html
+-rw-r--r--   0        0        0      617 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
+-rw-r--r--   0        0        0      789 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
+-rw-r--r--   0        0        0      182 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_api_create/main.html
+-rw-r--r--   0        0        0      347 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
+-rw-r--r--   0        0        0      423 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/inc_table.html
+-rw-r--r--   0        0        0      367 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
+-rw-r--r--   0        0        0      416 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/main.html
+-rw-r--r--   0        0        0      256 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/read.html
+-rw-r--r--   0        0        0      129 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/update.html
+-rw-r--r--   0        0        0      637 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
+-rw-r--r--   0        0        0      347 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/hx_form.html
+-rw-r--r--   0        0        0      111 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/inc_button_update.html
+-rw-r--r--   0        0        0      103 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/inc_create_button.html
+-rw-r--r--   0        0        0      442 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/inc_table.html
+-rw-r--r--   0        0        0      163 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/inc_table_head.html
+-rw-r--r--   0        0        0      241 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/main.html
+-rw-r--r--   0        0        0      256 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/read.html
+-rw-r--r--   0        0        0      129 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/read_inc_info.html
+-rw-r--r--   0        0        0      199 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/update.html
+-rw-r--r--   0        0        0      637 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html
+-rw-r--r--   0        0        0      428 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read.html
+-rw-r--r--   0        0        0      160 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_info.html
+-rw-r--r--   0        0        0     1331 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_port.html
+-rw-r--r--   0        0        0     1331 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
+-rw-r--r--   0        0        0      733 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_ports.html
+-rw-r--r--   0        0        0      238 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/rows.html
+-rw-r--r--   0        0        0      424 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/rows_inc_table.html
+-rw-r--r--   0        0        0      607 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-18 16:51:08.018550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
+-rw-r--r--   0        0        0      322 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/read.html
+-rw-r--r--   0        0        0       92 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/read_inc_info.html
+-rw-r--r--   0        0        0      174 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
+-rw-r--r--   0        0        0      130 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
+-rw-r--r--   0        0        0      432 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
+-rw-r--r--   0        0        0      234 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/rows.html
+-rw-r--r--   0        0        0      420 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
+-rw-r--r--   0        0        0      339 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/read.html
+-rw-r--r--   0        0        0       92 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/read_inc_info.html
+-rw-r--r--   0        0        0      422 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/read_inc_table.html
+-rw-r--r--   0        0        0      309 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
+-rw-r--r--   0        0        0      125 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
+-rw-r--r--   0        0        0      236 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/rows.html
+-rw-r--r--   0        0        0      422 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
+-rw-r--r--   0        0        0      340 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-18 16:51:08.022550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
+-rw-r--r--   0        0        0      265 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/register/hx_form.html
+-rw-r--r--   0        0        0      387 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/register/main.html
+-rw-r--r--   0        0        0     1037 2024-04-18 16:51:08.014550 esanom-0.7.12.7720/esanom/routes/v3/templates/pages/register/main_inc_form.html
+-rw-r--r--   0        0        0    53912 2024-04-18 16:51:08.010550 esanom-0.7.12.7720/esanom/routes/v3/web.py
+-rw-r--r--   0        0        0     1693 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/sample_gunicorn_config.py
+-rw-r--r--   0        0        0      753 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/sample_nom_config.json
+-rw-r--r--   0        0        0     5050 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/scheduler.py
+-rw-r--r--   0        0        0     3698 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/server.py
+-rw-r--r--   0        0        0    12199 2024-04-18 16:51:08.026550 esanom-0.7.12.7720/esanom/util.py
+-rw-r--r--   0        0        0      445 2024-04-18 16:51:12.190477 esanom-0.7.12.7720/pyproject.toml
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 esanom-0.7.12.7720/PKG-INFO
```

### Comparing `esanom-0.7.12.11/esanom/LICENCE.txt` & `esanom-0.7.12.7720/esanom/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/__init__.py` & `esanom-0.7.12.7720/esanom/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/client.py` & `esanom-0.7.12.7720/esanom/client.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/config.py` & `esanom-0.7.12.7720/esanom/config.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/database.py` & `esanom-0.7.12.7720/esanom/database.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/engine.py` & `esanom-0.7.12.7720/esanom/engine.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/monitor.py` & `esanom-0.7.12.7720/esanom/monitor.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/orchestrator.py` & `esanom-0.7.12.7720/esanom/orchestrator.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/pipeline.py` & `esanom-0.7.12.7720/esanom/pipeline.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/account.sql` & `esanom-0.7.12.7720/esanom/resources/database/account.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/api.sql` & `esanom-0.7.12.7720/esanom/resources/database/api.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/api_group.sql` & `esanom-0.7.12.7720/esanom/resources/database/api_group.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/api_role.sql` & `esanom-0.7.12.7720/esanom/resources/database/api_role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/claim.sql` & `esanom-0.7.12.7720/esanom/resources/database/claim.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/group.sql` & `esanom-0.7.12.7720/esanom/resources/database/group.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/io.sql` & `esanom-0.7.12.7720/esanom/resources/database/io.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/ioblock.sql` & `esanom-0.7.12.7720/esanom/resources/database/ioblock.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/log.sql` & `esanom-0.7.12.7720/esanom/resources/database/log.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/mpin.sql` & `esanom-0.7.12.7720/esanom/resources/database/mpin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/mport.sql` & `esanom-0.7.12.7720/esanom/resources/database/mport.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/pin.sql` & `esanom-0.7.12.7720/esanom/resources/database/pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/pipeline.sql` & `esanom-0.7.12.7720/esanom/resources/database/pipeline.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/pipeline_task.sql` & `esanom-0.7.12.7720/esanom/resources/database/pipeline_task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/port.sql` & `esanom-0.7.12.7720/esanom/resources/database/port.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/port_pin.sql` & `esanom-0.7.12.7720/esanom/resources/database/port_pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/role.sql` & `esanom-0.7.12.7720/esanom/resources/database/role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/roleadmin.sql` & `esanom-0.7.12.7720/esanom/resources/database/roleadmin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/roledashboard.sql` & `esanom-0.7.12.7720/esanom/resources/database/roledashboard.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/rolemodel.sql` & `esanom-0.7.12.7720/esanom/resources/database/rolemodel.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/roleuser.sql` & `esanom-0.7.12.7720/esanom/resources/database/roleuser.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/schedule.sql` & `esanom-0.7.12.7720/esanom/resources/database/schedule.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/session.sql` & `esanom-0.7.12.7720/esanom/resources/database/session.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/system.sql` & `esanom-0.7.12.7720/esanom/resources/database/system.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/task.sql` & `esanom-0.7.12.7720/esanom/resources/database/task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/triggers.sql` & `esanom-0.7.12.7720/esanom/resources/database/triggers.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/resources/database/unit.sql` & `esanom-0.7.12.7720/esanom/resources/database/unit.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/roleadmin.py` & `esanom-0.7.12.7720/esanom/roleadmin.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/rolemodel.py` & `esanom-0.7.12.7720/esanom/rolemodel.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/roleuser.py` & `esanom-0.7.12.7720/esanom/roleuser.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/__init__.py` & `esanom-0.7.12.7720/esanom/routes/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/api.py` & `esanom-0.7.12.7720/esanom/routes/v3/api.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/api.py-bak1` & `esanom-0.7.12.7720/esanom/routes/v3/api.py-bak1`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/common.py` & `esanom-0.7.12.7720/esanom/routes/v3/common.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/bootstrap.bundle.min.js` & `esanom-0.7.12.7720/esanom/routes/v3/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/bootstrap.min.css` & `esanom-0.7.12.7720/esanom/routes/v3/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/dashboard.css` & `esanom-0.7.12.7720/esanom/routes/v3/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/datatables.min.css` & `esanom-0.7.12.7720/esanom/routes/v3/static/datatables.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/datatables.min.js` & `esanom-0.7.12.7720/esanom/routes/v3/static/datatables.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/htmx.min.js` & `esanom-0.7.12.7720/esanom/routes/v3/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/nom-logo.png` & `esanom-0.7.12.7720/esanom/routes/v3/static/nom-logo.png`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/plotly.min.js` & `esanom-0.7.12.7720/esanom/routes/v3/static/plotly.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/static/theme.css` & `esanom-0.7.12.7720/esanom/routes/v3/static/theme.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/admin_db_pipeline_row.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/admin_db_pipeline_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/admin_db_pipeline_rows.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/admin_db_pipeline_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/base.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/base.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/db_rolemodel_row.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/db_rolemodel_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/db_rolemodel_rows.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/db_rolemodel_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_model_io.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_model_io.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_model_io_port.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_model_io_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_models.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_models.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_content_pipelines.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_content_pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_debug.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_debug.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_loggedin_nav_admin.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_loggedin_nav_admin.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_head.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_head.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/inc_page_header.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/inc_page_header.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/page_dashboard_tasks.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/page_dashboard_tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/page_model.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/page_model.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_read/main.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_read/main.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/pipelines.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/dashboard/tasks.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/login/main.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/login/main.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_api_create/hx_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_api_create/hx_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_api_create/inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_api_create/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/member_logs/update_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_port.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/read_inc_ports.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/read_inc_ports.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/templates/pages/register/main_inc_form.html` & `esanom-0.7.12.7720/esanom/routes/v3/templates/pages/register/main_inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/routes/v3/web.py` & `esanom-0.7.12.7720/esanom/routes/v3/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import time
 import json
 import html
 import random
 from datetime import datetime
 from importlib.metadata import version
 from flask import Blueprint , render_template , request , g as _g , redirect , url_for , make_response
+from werkzeug.utils import secure_filename
 from esanom import database as _database , util as _util , config as _config
 from . import common as _common 
 
 #####################################################################
 
 ROUTES = Blueprint( "routes" , __name__ , template_folder = "templates" , static_folder='static' )
 
@@ -1566,14 +1567,151 @@
     row_data = {
         "val_str" : val_str
     }
     _database.update_fromdict( "system" , "system/id" , row_data , cid = "key" )
 
     return( render_template( "pages/admin_settings/hx_form.html" ) )
 
+
+@ROUTES.route( "/hx_admin_settings_ports" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_settings_ports( ) :
+
+    f = request.files['file']
+    f.save("/tmp/"+secure_filename(f.filename))
+
+    with open("/tmp/ports.json") as f:
+        ports = json.loads(f.read())
+
+    port_ids = [ ]
+
+    for port_i , ( port_name , port_val ) in enumerate( ports.items( ) ) :
+
+        row_data = { "name" : port_name , "description" : port_val.get( "description" ) }
+
+        port = _database.db_query_select_row( "SELECT * from `port` where `name`=%s LIMIT 1" , [ port_name ] )
+
+        if port is None :
+            port_id = _database.insert_fromdict( "port" , row_data )
+            print( f"CREATED {port_name=}" )
+        else :
+            port_id = port[ "id" ]
+            _database.update_fromdict( "port" , port_id , row_data )
+            print( f"UPDATED {port_name=}" )
+
+        port_ids.append( port_id )
+
+        _database.db_query_delete( "DELETE FROM `port_pin` WHERE `port_id`=%s" , [ port_id ] )
+
+        print( f"{port_id=}" )
+
+        if "pins" not in port_val : continue
+
+        for pin_i , ( pin_name , pin_val ) in enumerate( port_val["pins"].items( ) ) :
+            pin_row = _database.db_query_select_row( "SELECT * from `pin` where `name`=%s LIMIT 1" , [ pin_name ] )
+            if pin_row is None :
+                raise Exception( f"ERROR: PIN NOT FOUND {pin_name=}" )
+
+            port_pin_data = { "port_id" : port_id , "pin_id" : pin_row[ "id" ] , "cardinal" : pin_val.get( "cardinal" , 1 ) }
+            _database.insert_fromdict( "port_pin" , port_pin_data )
+
+
+    ####
+
+    rows = _database.db_query_select_rows( "SELECT * from `port`" )
+    for row in rows :
+        if row[ "id" ] not in port_ids :
+            _database.db_query_delete( "DELETE FROM `port` WHERE `id`=%s LIMIT 1" , [ row[ "id" ] ] )
+
+    ####
+
+    return( render_template( "pages/admin_settings/hx_form.html" ) )
+
+
+@ROUTES.route( "/hx_admin_settings_pins" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_settings_pins( ) :
+
+    f = request.files['file']
+    f.save("/tmp/"+secure_filename(f.filename))
+
+    with open("/tmp/pins.json") as f:
+        pins = json.loads(f.read())
+
+    pin_ids = [ ]
+
+    for pin_i , ( pin_name , pin_val ) in enumerate( pins.items( ) ) :
+
+        row_data = { "name" : pin_name , "description" : pin_val.get( "description" ) , "type" : pin_val.get( "type" ) }
+
+        pin = _database.db_query_select_row( "SELECT * from `pin` where `name`=%s LIMIT 1" , [ pin_name ] )
+
+        if pin is None :
+            pin_id = _database.insert_fromdict( "pin" , row_data )
+            print( f"CREATED {pin_name=}" )
+        else :
+            pin_id = pin[ "id" ]
+            _database.update_fromdict( "pin" , pin_id , row_data )
+            print( f"UPDATED {pin_name=}" )
+
+        pin_ids.append( pin_id )
+
+        print( f"{pin_id=}" )
+
+        ####
+
+        flag_default_unit_i = 0
+        for unit_i , ( unit_name , unit_val ) in enumerate( pin_val[ "units" ].items( ) ) :
+            if unit_val.get( "default" , 0 ) == 1 :
+                flag_default_unit_i = unit_i
+                break
+
+        ####
+
+        unit_ids = [ ]
+
+        for unit_i , ( unit_name , unit_val ) in enumerate( pin_val[ "units" ].items( ) ) :
+
+            unit_default = unit_i == flag_default_unit_i
+
+            row_data = { "pin_id" : pin_id , "name" : unit_name , "description" : unit_val.get( "description" ) , "symbol" : unit_val.get( "symbol" ) , "default" : unit_default }
+
+            unit = _database.db_query_select_row( "SELECT * from `unit` where pin_id=%s and `name`=%s LIMIT 1" , [ pin_id, unit_name ] )
+
+            if unit is None :
+                unit_id = _database.insert_fromdict( "unit" , row_data )
+                print( f"CREATED {unit_name=}" )
+            else :
+                unit_id = unit[ "id" ]
+                _database.update_fromdict( "unit" , unit_id , row_data )
+                print( f"UPDATED {unit_name=}" )
+
+            unit_ids.append( unit_id )
+
+        ####
+
+        rows = _database.db_query_select_rows( "SELECT * from `unit` where `pin_id`=%s" , [ pin_id ] )
+        for row in rows :
+            if row[ "id" ] not in unit_ids :
+                _database.db_query_delete( "DELETE FROM `unit` WHERE `id`=%s LIMIT 1" , [ row[ "id" ] ] )
+
+        ####
+
+
+    ####
+
+    rows = _database.db_query_select_rows( "SELECT * from `pin`" )
+    for row in rows :
+        if row[ "id" ] not in pin_ids :
+            _database.db_query_delete( "DELETE FROM `pin` WHERE `id`=%s LIMIT 1" , [ row[ "id" ] ] )
+
+    ####
+
+    return( render_template( "pages/admin_settings/hx_form.html" ) )
+
 @ROUTES.route( "/hx_admin_settings_form_system_registration" , methods = [ "POST" ] )
 @_common.decorator_web_login_required( "_admin" )
 def hx_admin_settings_form_system_registration( ) :
 
     form = request.form.to_dict( flat = False )
     print( form )
```

### Comparing `esanom-0.7.12.11/esanom/sample_gunicorn_config.py` & `esanom-0.7.12.7720/esanom/sample_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/sample_nom_config.json` & `esanom-0.7.12.7720/esanom/sample_nom_config.json`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/scheduler.py` & `esanom-0.7.12.7720/esanom/scheduler.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/esanom/server.py` & `esanom-0.7.12.7720/esanom/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 app.wsgi_app = ProxyFix( app.wsgi_app , x_for = 1 , x_host = 1 , x_port = 1 , x_proto = 1 , x_prefix = 1 )
 Compress( app )
 
 #####################################################################
 
 app.config[ "SEND_FILE_MAX_AGE_DEFAULT" ] = 31622400
 app.config[ "MAX_CONTENT_LENGTH" ] = 16 * 1024 * 1024
+app.config['UPLOAD_FOLDER'] = '/tmp'
 
 #####################################################################
 
 from esanom.routes.v3.api import ROUTES as routes_v3_api
 app.register_blueprint( routes_v3_api , name = "routes_v3_api" , url_prefix = "/v3/api" )
 
 from esanom.routes.v3.web import ROUTES as routes_v3_web
```

### Comparing `esanom-0.7.12.11/esanom/util.py` & `esanom-0.7.12.7720/esanom/util.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.11/PKG-INFO` & `esanom-0.7.12.7720/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanom
-Version: 0.7.12.11
+Version: 0.7.12.7720
 Summary: ESANOM
 Author: Zafar Iqbal
 Author-email: zaf@sparc.space
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

