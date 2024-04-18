# Comparing `tmp/esanom-0.7.12.30.tar.gz` & `tmp/esanom-0.7.9.3232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanom-0.7.12.30.tar", max compression
+gzip compressed data, was "esanom-0.7.9.3232.tar", max compression
```

## Comparing `esanom-0.7.12.30.tar` & `esanom-0.7.9.3232.tar`

### file list

```diff
@@ -1,207 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-18 10:43:45.566382 esanom-0.7.12.30/README.md
--rw-r--r--   0        0        0      144 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/CHANGELOG.txt
--rw-r--r--   0        0        0      388 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/COPYRIGHT.txt
--rw-r--r--   0        0        0    17260 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/LICENCE.txt
--rw-r--r--   0        0        0     1413 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/__init__.py
--rw-r--r--   0        0        0     5950 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/client.py
--rw-r--r--   0        0        0     5156 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/config.py
--rw-r--r--   0        0        0    47586 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/database.py
--rw-r--r--   0        0        0     1125 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/engine.py
--rw-r--r--   0        0        0     2496 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/monitor.py
--rw-r--r--   0        0        0    10303 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/orchestrator.py
--rw-r--r--   0        0        0    13068 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/pipeline.py
--rw-r--r--   0        0        0     1665 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/account.sql
--rw-r--r--   0        0        0     1828 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/api.sql
--rw-r--r--   0        0        0     1352 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/api_group.sql
--rw-r--r--   0        0        0     1326 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/api_role.sql
--rw-r--r--   0        0        0     1226 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/resources/database/claim.sql
--rw-r--r--   0        0        0     1215 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/group.sql
--rw-r--r--   0        0        0     1828 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/io.sql
--rw-r--r--   0        0        0     1416 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/ioblock.sql
--rw-r--r--   0        0        0     1596 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/log.sql
--rw-r--r--   0        0        0     1950 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/mpin.sql
--rw-r--r--   0        0        0     1921 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/mport.sql
--rw-r--r--   0        0        0     1536 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/pin.sql
--rw-r--r--   0        0        0     1842 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/pipeline.sql
--rw-r--r--   0        0        0     1514 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/pipeline_task.sql
--rw-r--r--   0        0        0     1501 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/port.sql
--rw-r--r--   0        0        0     1388 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/port_pin.sql
--rw-r--r--   0        0        0     1126 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/role.sql
--rw-r--r--   0        0        0     1250 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/roleadmin.sql
--rw-r--r--   0        0        0     1257 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/roledashboard.sql
--rw-r--r--   0        0        0     2173 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/rolemodel.sql
--rw-r--r--   0        0        0     1655 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/roleuser.sql
--rw-r--r--   0        0        0     1319 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/resources/database/schedule.sql
--rw-r--r--   0        0        0     1156 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/session.sql
--rw-r--r--   0        0        0     1236 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/resources/database/system.sql
--rw-r--r--   0        0        0     1914 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/task.sql
--rw-r--r--   0        0        0     5741 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/triggers.sql
--rw-r--r--   0        0        0     1497 2024-04-18 10:43:46.042383 esanom-0.7.12.30/esanom/resources/database/unit.sql
--rw-r--r--   0        0        0    11022 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/roleadmin.py
--rw-r--r--   0        0        0     4208 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/rolemodel.py
--rw-r--r--   0        0        0     3456 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/roleuser.py
--rw-r--r--   0        0        0      790 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/__init__.py
--rw-r--r--   0        0        0    38001 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/api.py
--rw-r--r--   0        0        0    40721 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/api.py-bak1
--rw-r--r--   0        0        0     8952 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/common.py
--rw-r--r--   0        0        0    80721 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   232803 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/static/bootstrap.min.css
--rw-r--r--   0        0        0      639 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/static/dashboard.css
--rw-r--r--   0        0        0    20832 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/datatables.min.css
--rw-r--r--   0        0        0   197654 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/datatables.min.js
--rw-r--r--   0        0        0      318 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/static/favicon.ico
--rw-r--r--   0        0        0    48036 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/static/htmx.min.js
--rw-r--r--   0        0        0       97 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/static/main.css
--rw-r--r--   0        0        0      422 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/main.js
--rw-r--r--   0        0        0     1723 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/nom-logo.png
--rw-r--r--   0        0        0  3620840 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/plotly.min.js
--rw-r--r--   0        0        0     1741 2024-04-18 10:43:46.058383 esanom-0.7.12.30/esanom/routes/v3/static/theme.css
--rw-r--r--   0        0        0      717 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/admin_db_pipeline_row.html
--rw-r--r--   0        0        0      627 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/admin_db_pipeline_rows.html
--rw-r--r--   0        0        0     1542 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/base.html
--rw-r--r--   0        0        0     1000 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/db_rolemodel_row.html
--rw-r--r--   0        0        0      633 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/db_rolemodel_rows.html
--rw-r--r--   0        0        0      140 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/dummy.html
--rw-r--r--   0        0        0      153 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/error_404.html
--rw-r--r--   0        0        0      114 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/error_500.html
--rw-r--r--   0        0        0       82 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
--rw-r--r--   0        0        0      731 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_model_io.html
--rw-r--r--   0        0        0     1331 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_model_io_port.html
--rw-r--r--   0        0        0      808 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_models.html
--rw-r--r--   0        0        0      836 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_pipelines.html
--rw-r--r--   0        0        0     2019 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_debug.html
--rw-r--r--   0        0        0      248 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_loggedin_nav.html
--rw-r--r--   0        0        0      586 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
--rw-r--r--   0        0        0      300 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_loggedin_nav_dashboard.html
--rw-r--r--   0        0        0      197 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_loggedin_nav_member.html
--rw-r--r--   0        0        0      152 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_footer.html
--rw-r--r--   0        0        0      628 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_head.html
--rw-r--r--   0        0        0     1332 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_header.html
--rw-r--r--   0        0        0      173 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_header_logo.html
--rw-r--r--   0        0        0      487 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_header_nav.html
--rw-r--r--   0        0        0      240 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_header_toggle.html
--rw-r--r--   0        0        0      153 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/navigation.html
--rw-r--r--   0        0        0      327 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_admin_pipelines.html
--rw-r--r--   0        0        0      921 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_dashboard_tasks.html
--rw-r--r--   0        0        0      115 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_docs.html
--rw-r--r--   0        0        0      116 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_index.html
--rw-r--r--   0        0        0      121 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_interfaces.html
--rw-r--r--   0        0        0      516 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_model.html
--rw-r--r--   0        0        0      157 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/page_models.html
--rw-r--r--   0        0        0      128 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin/main.html
--rw-r--r--   0        0        0       94 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
--rw-r--r--   0        0        0     1378 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
--rw-r--r--   0        0        0      188 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_account_create/main.html
--rw-r--r--   0        0        0        5 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/hx_form.html
--rw-r--r--   0        0        0      110 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
--rw-r--r--   0        0        0      429 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
--rw-r--r--   0        0        0      299 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
--rw-r--r--   0        0        0      315 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/main.html
--rw-r--r--   0        0        0      272 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/read.html
--rw-r--r--   0        0        0      114 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/read_inc_button_update.html
--rw-r--r--   0        0        0      248 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/read_inc_info.html
--rw-r--r--   0        0        0      207 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/update.html
--rw-r--r--   0        0        0     1887 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_accounts/update_inc_form.html
--rw-r--r--   0        0        0      113 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
--rw-r--r--   0        0        0      544 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_read/main.html
--rw-r--r--   0        0        0        6 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
--rw-r--r--   0        0        0     1221 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
--rw-r--r--   0        0        0      474 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
--rw-r--r--   0        0        0      489 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_update/main.html
--rw-r--r--   0        0        0      421 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
--rw-r--r--   0        0        0      369 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
--rw-r--r--   0        0        0      240 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_apis/main.html
--rw-r--r--   0        0        0       94 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
--rw-r--r--   0        0        0      324 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
--rw-r--r--   0        0        0      263 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_create/main.html
--rw-r--r--   0        0        0      111 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
--rw-r--r--   0        0        0      278 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_read/main.html
--rw-r--r--   0        0        0        6 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
--rw-r--r--   0        0        0      718 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
--rw-r--r--   0        0        0      352 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_update/main.html
--rw-r--r--   0        0        0       87 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
--rw-r--r--   0        0        0      425 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_groups/main.html
--rw-r--r--   0        0        0      111 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
--rw-r--r--   0        0        0      332 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_read/main.html
--rw-r--r--   0        0        0       24 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
--rw-r--r--   0        0        0      897 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
--rw-r--r--   0        0        0      403 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_update/main.html
--rw-r--r--   0        0        0      425 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_models/inc_table.html
--rw-r--r--   0        0        0      296 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
--rw-r--r--   0        0        0      245 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_models/main.html
--rw-r--r--   0        0        0       40 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_settings/hx_form.html
--rw-r--r--   0        0        0      413 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_id.html
--rw-r--r--   0        0        0      463 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_registration.html
--rw-r--r--   0        0        0      260 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_settings/main.html
--rw-r--r--   0        0        0       82 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/dashboard/hx_pipelines.html
--rw-r--r--   0        0        0       82 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/dashboard/hx_tasks.html
--rw-r--r--   0        0        0      118 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/dashboard/main.html
--rw-r--r--   0        0        0      895 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/dashboard/pipelines.html
--rw-r--r--   0        0        0      891 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/dashboard/tasks.html
--rw-r--r--   0        0        0      640 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
--rw-r--r--   0        0        0     1218 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
--rw-r--r--   0        0        0       26 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
--rw-r--r--   0        0        0      770 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
--rw-r--r--   0        0        0      128 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/main.html
--rw-r--r--   0        0        0       60 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/login/hx_login.html
--rw-r--r--   0        0        0      766 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/login/main.html
--rw-r--r--   0        0        0      133 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/logout/main.html
--rw-r--r--   0        0        0      128 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member/main.html
--rw-r--r--   0        0        0      617 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
--rw-r--r--   0        0        0      789 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
--rw-r--r--   0        0        0      182 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_api_create/main.html
--rw-r--r--   0        0        0      347 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/hx_form.html
--rw-r--r--   0        0        0      111 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/inc_button_update.html
--rw-r--r--   0        0        0      103 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
--rw-r--r--   0        0        0      423 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/inc_table.html
--rw-r--r--   0        0        0      367 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
--rw-r--r--   0        0        0      185 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
--rw-r--r--   0        0        0      416 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/main.html
--rw-r--r--   0        0        0      256 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/read.html
--rw-r--r--   0        0        0      129 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/read_inc_info.html
--rw-r--r--   0        0        0      199 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/update.html
--rw-r--r--   0        0        0      637 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_apis/update_inc_form.html
--rw-r--r--   0        0        0      428 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read.html
--rw-r--r--   0        0        0      160 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_info.html
--rw-r--r--   0        0        0     1331 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_port.html
--rw-r--r--   0        0        0     1331 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
--rw-r--r--   0        0        0      733 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_ports.html
--rw-r--r--   0        0        0      238 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/rows.html
--rw-r--r--   0        0        0      424 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/rows_inc_table.html
--rw-r--r--   0        0        0      607 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
--rw-r--r--   0        0        0      322 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/read.html
--rw-r--r--   0        0        0       92 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/read_inc_info.html
--rw-r--r--   0        0        0      174 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/read_inc_table_body_units.html
--rw-r--r--   0        0        0      130 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/read_inc_table_head_units.html
--rw-r--r--   0        0        0      432 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/read_inc_table_units.html
--rw-r--r--   0        0        0      234 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/rows.html
--rw-r--r--   0        0        0      420 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
--rw-r--r--   0        0        0      339 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
--rw-r--r--   0        0        0      320 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/read.html
--rw-r--r--   0        0        0       92 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/read_inc_info.html
--rw-r--r--   0        0        0      422 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/read_inc_table.html
--rw-r--r--   0        0        0      309 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
--rw-r--r--   0        0        0      125 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
--rw-r--r--   0        0        0      236 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/rows.html
--rw-r--r--   0        0        0      422 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
--rw-r--r--   0        0        0      340 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
--rw-r--r--   0        0        0      209 2024-04-18 10:43:46.054383 esanom-0.7.12.30/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
--rw-r--r--   0        0        0      265 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/register/hx_form.html
--rw-r--r--   0        0        0      387 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/register/main.html
--rw-r--r--   0        0        0     1037 2024-04-18 10:43:46.050382 esanom-0.7.12.30/esanom/routes/v3/templates/pages/register/main_inc_form.html
--rw-r--r--   0        0        0    48540 2024-04-18 10:43:46.046383 esanom-0.7.12.30/esanom/routes/v3/web.py
--rw-r--r--   0        0        0     1693 2024-04-18 10:43:46.062383 esanom-0.7.12.30/esanom/sample_gunicorn_config.py
--rw-r--r--   0        0        0      753 2024-04-18 10:43:46.062383 esanom-0.7.12.30/esanom/sample_nom_config.json
--rw-r--r--   0        0        0     5050 2024-04-18 10:43:46.062383 esanom-0.7.12.30/esanom/scheduler.py
--rw-r--r--   0        0        0     3661 2024-04-18 10:43:46.062383 esanom-0.7.12.30/esanom/server.py
--rw-r--r--   0        0        0    12199 2024-04-18 10:43:46.062383 esanom-0.7.12.30/esanom/util.py
--rw-r--r--   0        0        0      443 2024-04-18 10:43:50.814388 esanom-0.7.12.30/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 esanom-0.7.12.30/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 16:37:06.484637 esanom-0.7.9.3232/README.md
+-rw-r--r--   0        0        0      144 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/CHANGELOG.txt
+-rw-r--r--   0        0        0      388 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/COPYRIGHT.txt
+-rw-r--r--   0        0        0    17260 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/LICENCE.txt
+-rw-r--r--   0        0        0     1412 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/__init__.py
+-rw-r--r--   0        0        0     6229 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/client.py
+-rw-r--r--   0        0        0     5123 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/config.py
+-rw-r--r--   0        0        0    43836 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/database.py
+-rw-r--r--   0        0        0     1125 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/engine.py
+-rw-r--r--   0        0        0     2496 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/monitor.py
+-rw-r--r--   0        0        0    10303 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/orchestrator.py
+-rw-r--r--   0        0        0    13068 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/pipeline.py
+-rw-r--r--   0        0        0     1613 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/account.sql
+-rw-r--r--   0        0        0     1828 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api.sql
+-rw-r--r--   0        0        0     1352 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api_group.sql
+-rw-r--r--   0        0        0     1326 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/api_role.sql
+-rw-r--r--   0        0        0     1226 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/resources/database/claim.sql
+-rw-r--r--   0        0        0     1131 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/group.sql
+-rw-r--r--   0        0        0     1828 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/io.sql
+-rw-r--r--   0        0        0     1416 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/ioblock.sql
+-rw-r--r--   0        0        0     1596 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/log.sql
+-rw-r--r--   0        0        0     1950 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/mpin.sql
+-rw-r--r--   0        0        0     1921 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/mport.sql
+-rw-r--r--   0        0        0     1451 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pin.sql
+-rw-r--r--   0        0        0     1842 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pipeline.sql
+-rw-r--r--   0        0        0     1514 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/pipeline_task.sql
+-rw-r--r--   0        0        0     1501 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/port.sql
+-rw-r--r--   0        0        0     1388 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/port_pin.sql
+-rw-r--r--   0        0        0     1126 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/role.sql
+-rw-r--r--   0        0        0     1250 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roleadmin.sql
+-rw-r--r--   0        0        0     1257 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roledashboard.sql
+-rw-r--r--   0        0        0     2173 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/rolemodel.sql
+-rw-r--r--   0        0        0     1655 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/roleuser.sql
+-rw-r--r--   0        0        0     1319 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/schedule.sql
+-rw-r--r--   0        0        0     1156 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/session.sql
+-rw-r--r--   0        0        0     1236 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/system.sql
+-rw-r--r--   0        0        0     1914 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/task.sql
+-rw-r--r--   0        0        0     4725 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/triggers.sql
+-rw-r--r--   0        0        0     1432 2024-04-15 16:37:06.892635 esanom-0.7.9.3232/esanom/resources/database/unit.sql
+-rw-r--r--   0        0        0     9732 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleadmin.py
+-rw-r--r--   0        0        0    11371 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleadmin.py-bak1
+-rw-r--r--   0        0        0     4192 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/rolemodel.py
+-rw-r--r--   0        0        0     3456 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/roleuser.py
+-rw-r--r--   0        0        0      790 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/__init__.py
+-rw-r--r--   0        0        0    40473 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/api.py
+-rw-r--r--   0        0        0     8676 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/common.py
+-rw-r--r--   0        0        0    80721 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   232803 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.min.css
+-rw-r--r--   0        0        0      639 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/dashboard.css
+-rw-r--r--   0        0        0    20832 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.css
+-rw-r--r--   0        0        0   197654 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.js
+-rw-r--r--   0        0        0      318 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/favicon.ico
+-rw-r--r--   0        0        0    48036 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/htmx.min.js
+-rw-r--r--   0        0        0       97 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/main.css
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/main.js
+-rw-r--r--   0        0        0     1723 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/nom-logo.png
+-rw-r--r--   0        0        0  3620840 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/routes/v3/static/plotly.min.js
+-rw-r--r--   0        0        0     1741 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/static/theme.css
+-rw-r--r--   0        0        0      717 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_row.html
+-rw-r--r--   0        0        0      627 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_rows.html
+-rw-r--r--   0        0        0     1542 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/base.html
+-rw-r--r--   0        0        0     1000 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_row.html
+-rw-r--r--   0        0        0      633 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_rows.html
+-rw-r--r--   0        0        0      140 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/dummy.html
+-rw-r--r--   0        0        0      153 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/error_404.html
+-rw-r--r--   0        0        0      114 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/error_500.html
+-rw-r--r--   0        0        0       82 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/hx_dashboard_tasks_taskcount.html
+-rw-r--r--   0        0        0      731 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io_port.html
+-rw-r--r--   0        0        0      808 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_models.html
+-rw-r--r--   0        0        0      836 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_pipelines.html
+-rw-r--r--   0        0        0     1827 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_debug.html
+-rw-r--r--   0        0        0      149 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav.html
+-rw-r--r--   0        0        0      586 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_admin.html
+-rw-r--r--   0        0        0      197 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_member.html
+-rw-r--r--   0        0        0      152 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_footer.html
+-rw-r--r--   0        0        0      628 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_head.html
+-rw-r--r--   0        0        0     1332 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header.html
+-rw-r--r--   0        0        0      173 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_logo.html
+-rw-r--r--   0        0        0      487 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_nav.html
+-rw-r--r--   0        0        0      240 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header_toggle.html
+-rw-r--r--   0        0        0      153 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/navigation.html
+-rw-r--r--   0        0        0      327 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_admin_pipelines.html
+-rw-r--r--   0        0        0      921 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_dashboard_tasks.html
+-rw-r--r--   0        0        0      115 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_docs.html
+-rw-r--r--   0        0        0      116 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_index.html
+-rw-r--r--   0        0        0      121 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_interfaces.html
+-rw-r--r--   0        0        0      516 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_model.html
+-rw-r--r--   0        0        0      157 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/page_models.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin/main.html
+-rw-r--r--   0        0        0       94 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/hx_form.html
+-rw-r--r--   0        0        0     1381 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html
+-rw-r--r--   0        0        0      188 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/main.html
+-rw-r--r--   0        0        0      110 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_create_button.html
+-rw-r--r--   0        0        0      429 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table.html
+-rw-r--r--   0        0        0      336 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/inc_table_head.html
+-rw-r--r--   0        0        0      315 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_accounts/main.html
+-rw-r--r--   0        0        0      113 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/inc_button_update.html
+-rw-r--r--   0        0        0      544 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/hx_form.html
+-rw-r--r--   0        0        0     1221 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html
+-rw-r--r--   0        0        0      474 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form_groups.html
+-rw-r--r--   0        0        0      492 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/main.html
+-rw-r--r--   0        0        0      421 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table.html
+-rw-r--r--   0        0        0      369 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/inc_table_head.html
+-rw-r--r--   0        0        0      241 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_apis/main.html
+-rw-r--r--   0        0        0       94 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/hx_form.html
+-rw-r--r--   0        0        0      324 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/inc_form.html
+-rw-r--r--   0        0        0      263 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_create/main.html
+-rw-r--r--   0        0        0      109 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_read/inc_button_update.html
+-rw-r--r--   0        0        0      278 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_read/main.html
+-rw-r--r--   0        0        0        6 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/hx_form.html
+-rw-r--r--   0        0        0      716 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html
+-rw-r--r--   0        0        0      352 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/main.html
+-rw-r--r--   0        0        0       87 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_button_create.html
+-rw-r--r--   0        0        0      425 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table.html
+-rw-r--r--   0        0        0      293 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table_body.html
+-rw-r--r--   0        0        0      184 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_groups/main.html
+-rw-r--r--   0        0        0      109 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_read/inc_button_update.html
+-rw-r--r--   0        0        0      332 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_read/main.html
+-rw-r--r--   0        0        0       24 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/hx_form.html
+-rw-r--r--   0        0        0      895 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html
+-rw-r--r--   0        0        0      421 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/main.html
+-rw-r--r--   0        0        0      425 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table.html
+-rw-r--r--   0        0        0      364 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table_body.html
+-rw-r--r--   0        0        0      184 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/inc_table_head.html
+-rw-r--r--   0        0        0      245 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_models/main.html
+-rw-r--r--   0        0        0       40 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/hx_form_system_mailer.html
+-rw-r--r--   0        0        0      445 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/inc_form_system_mailer.html
+-rw-r--r--   0        0        0      199 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_settings/main.html
+-rw-r--r--   0        0        0      640 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html
+-rw-r--r--   0        0        0     1218 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html
+-rw-r--r--   0        0        0       26 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create_form_submit.html
+-rw-r--r--   0        0        0      770 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/main.html
+-rw-r--r--   0        0        0       60 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/login/hx_login.html
+-rw-r--r--   0        0        0      702 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/login/main.html
+-rw-r--r--   0        0        0      117 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/logout/main.html
+-rw-r--r--   0        0        0      128 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member/main.html
+-rw-r--r--   0        0        0      432 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/hx_form.html
+-rw-r--r--   0        0        0      792 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/inc_form.html
+-rw-r--r--   0        0        0      182 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/main.html
+-rw-r--r--   0        0        0      103 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_create_button.html
+-rw-r--r--   0        0        0      423 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table.html
+-rw-r--r--   0        0        0      407 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table_body.html
+-rw-r--r--   0        0        0      185 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/inc_table_head.html
+-rw-r--r--   0        0        0      416 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_apis/main.html
+-rw-r--r--   0        0        0      428 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read.html
+-rw-r--r--   0        0        0      160 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_info.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html
+-rw-r--r--   0        0        0     1331 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1
+-rw-r--r--   0        0        0      733 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_ports.html
+-rw-r--r--   0        0        0      238 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows.html
+-rw-r--r--   0        0        0      424 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table.html
+-rw-r--r--   0        0        0      607 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_head.html
+-rw-r--r--   0        0        0      189 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/read.html
+-rw-r--r--   0        0        0       92 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/read_inc_info.html
+-rw-r--r--   0        0        0      234 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows.html
+-rw-r--r--   0        0        0      420 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table.html
+-rw-r--r--   0        0        0      337 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/pins/rows_inc_table_head.html
+-rw-r--r--   0        0        0      243 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read.html
+-rw-r--r--   0        0        0       92 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_info.html
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table.html
+-rw-r--r--   0        0        0      163 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table_body.html
+-rw-r--r--   0        0        0      125 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/read_inc_table_head.html
+-rw-r--r--   0        0        0      236 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows.html
+-rw-r--r--   0        0        0      422 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table.html
+-rw-r--r--   0        0        0      340 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table_body.html
+-rw-r--r--   0        0        0      209 2024-04-15 16:37:06.904635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/ports/rows_inc_table_head.html
+-rw-r--r--   0        0        0      320 2024-04-15 16:37:06.900635 esanom-0.7.9.3232/esanom/routes/v3/templates/pages/register/main.html
+-rw-r--r--   0        0        0    39183 2024-04-15 16:37:06.896635 esanom-0.7.9.3232/esanom/routes/v3/web.py
+-rw-r--r--   0        0        0     1693 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/sample_gunicorn_config.py
+-rw-r--r--   0        0        0      753 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/sample_nom_config.json
+-rw-r--r--   0        0        0     5050 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/scheduler.py
+-rw-r--r--   0        0        0     2887 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/server.py
+-rw-r--r--   0        0        0    12199 2024-04-15 16:37:06.908635 esanom-0.7.9.3232/esanom/util.py
+-rw-r--r--   0        0        0      444 2024-04-15 16:37:23.952531 esanom-0.7.9.3232/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 esanom-0.7.9.3232/PKG-INFO
```

### Comparing `esanom-0.7.12.30/esanom/LICENCE.txt` & `esanom-0.7.9.3232/esanom/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/__init__.py` & `esanom-0.7.9.3232/esanom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # This file is subject to the terms and conditions defined in file 'LICENCE.txt', 
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 
-__version__ = "0.7.12"
+__version__ = "0.7.9"
 
 #####################################################################
 
 from importlib.metadata import version
 
 print( f"NoM v{version('esanom')} Copyright 2024 © European Space Agency. All rights reserved." )
```

### Comparing `esanom-0.7.12.30/esanom/client.py` & `esanom-0.7.9.3232/esanom/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -187,21 +187,21 @@
 
 def user_pipeline_submit( pipeline ) :
 
     if pipeline.submitted : raise Exception( "Already submitted" )
 
     user_pipeline_submit_reserve_messages = _roleuser.pipeline_submit_reserve( pipeline )
 
-    #print( user_pipeline_submit_reserve_messages )
+    print( user_pipeline_submit_reserve_messages )
 
     task_uids = user_pipeline_submit_reserve_messages[ "task_uids" ]
 
     pipeline_io_uids = _roleuser.pipeline_submit_io( pipeline , task_uids )
 
-    #print(f"{pipeline_io_uids=}")
+    print(f"{pipeline_io_uids=}")
 
     _roleuser.pipeline_submit_io_blocks( pipeline , pipeline_io_uids )
 
     _roleuser.pipeline_submit( pipeline )
 
     pipeline.submitted = True
 
@@ -211,33 +211,41 @@
     #print(messages)
 
     return( True )
 
 def user_pipeline_await( pipeline ) :
 
     pipeline_name = pipeline.name
-
-    t0 = time.time( )
+    t0=time.time()
 
     while not pipeline.done :
-        dt = int( time.time( ) - t0 )
+        dt=int(time.time()-t0)
         print( f"[{dt}] awaiting {pipeline_name}")
-        time.sleep( 5 )
+        time.sleep(1)
         pipeline = user_pipeline( pipeline_name )
 
-    if pipeline.done :
-        print( "PIPELINE DONE" )
-    else :
-        print( "PIPELINE NOT DONE" )
-
     return( pipeline )
 
 
 def user_pipeline_archive( pipeline_name ) :
+
     return( _roleuser.pipeline_archive( pipeline_name ) )
 
 
 def user_pipeline_cancel( pipeline_name ) :
+
     return( _roleuser.pipeline_cancel( pipeline_name ) )
 
+def user_sample_workload( ) :
+
+    pipeline = user_pipeline( f"sample_workload {time.time()}" )
+
+    pipeline.add( "test_model0" , "m0" )
+
+    for i in range( 1 , 10 ) :
+        pipeline.add( f"test_model0" , f"m{i}" )
+        pipeline.connect( f"m{i}" , "m0" )
+        pipeline.io( f"/m{i}/inputs/test_model0:p1/0/test_model0:q1/0" , f"M{i}_{time.time()}" )
+
+    user_pipeline_submit( pipeline )
```

### Comparing `esanom-0.7.12.30/esanom/config.py` & `esanom-0.7.9.3232/esanom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,15 @@
     config_fp = f"{NOM_CONFIG_PATH}"
     if not NOM_CONFIG_PATH.startswith( "/" ) :
         config_fp = f"{cwd_fp}/{NOM_CONFIG_PATH}"
 
     ####
 
     if load_from_filepath( config_fp ) == None : load_from_env( )
-    if "_load_from_env" not in DATA :
-        DATA[ "_load_from_env" ] = False 
-        DATA[ "_config_fp" ] = NOM_CONFIG_PATH
+    if "_load_from_env" not in DATA : DATA[ "_load_from_env" ] = False 
 
     ####
 
     DATA[ "_package_fp" ] = os.path.abspath( os.path.dirname( __file__ ) )
     DATA[ "_cwd_fp" ] = cwd_fp
     DATA[ "_time_created" ] = time.time( )
 
@@ -74,15 +72,15 @@
 
     config_init_default_boolean( "server_debug" )
     config_init_default_boolean( "server_security_lax" )
     config_init_default_boolean( "database_disable_init" )
 
     ####
 
-    #_util.print_debug( DATA )
+    _util.print_debug( DATA )
 
     return
 
 #####################################################################
 
 def config_init_default_boolean( k , v = False ) :
     global DATA
@@ -95,27 +93,26 @@
         DATA[ k ] = True
     else :
         DATA[ k ] = False
 
 #####################################################################
 
 def load_from_filepath( config_fp ) :
-
     global DATA
 
     if not os.path.isfile( config_fp ) :
-        print( f"CONFIG FILE NOT FOUND {config_fp=}" )
+        print( f"WARNING CONFIG FILE NOT FOUND {config_fp=}" )
         return( None )
 
     ####
 
     with open( config_fp ) as f :
         try :
             DATA = json.loads( f.read( ) )
-            print( f"CONFIG FILE FOUND {config_fp=}" )
+            print( f"Config loaded from file config_fp = {config_fp}" )
             return( True )
         except json.decoder.JSONDecodeError as e :
             print( f"ERROR JSONDecodeError {e.msg}" )
             sys.exit( 4 )
 
 
 def env_get( k ) :
@@ -148,18 +145,19 @@
         "fs_storage_path" : env_get( "NOM_CONFIG_FS_STORAGE_PATH" ),
         "database_disable_init" : env_get( "NOM_CONFIG_DATABASE_DISABLE_INIT" ),
         "server_debug" : env_get( "NOM_CONFIG_SERVER_DEBUG" ),
         "server_security_lax" : env_get( "NOM_CONFIG_SERVER_SECURITY_LAX" ) 
 
     }
 
-    print( "CONFIG loaded from ENV" )
+    print("CONFIG loaded from ENV")
 
     #_util.print_debug( DATA , "Config loaded from ENV" )
 
+
     #if db_host == None or db_port == None : return( None )
     #if db_user == None or db_passwd == None : return( None )
     #if db_database == None : return( None )
 
     #if admin_api_email == None : return( None )
 
     return
```

### Comparing `esanom-0.7.12.30/esanom/database.py` & `esanom-0.7.9.3232/esanom/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,18 +55,18 @@
     if _config.DATA[ "database_disable_init" ] : return
 
     # FIXME TODO find a better way to detect that we don't want database init
     if _config.DATA[ "database" ][ "port" ].startswith( "_" ) : return
     if _config.DATA[ "database" ][ "host" ] == "" : return
 
     print( "ATTEMPT DB INIT" )
+    time.sleep(10)
 
     try :
         db = mysql.connect( **_config.DATA[ "database" ] )
-        db.autocommit = True
         cursor = db.cursor( )
     except Exception as e :
         print( f"database create_tables connect exception {e}" )
         sys.exit( 4 )
 
     ####
 
@@ -89,25 +89,24 @@
         ####
 
         with open( sql_fp , "r" ) as f : sql = f.read( )
 
         try :
 
             cursor.execute( sql )
-            #print(f"{sql_fp=}")
 
         except Error as err :
 
             cursor.close( )
             db.close( )
 
             # FIXME TODO check if this is "client" run and bypass database stuff
             # FIXME TODO keep account as first table to create otherwise it fails
             if err.errno == errorcode.ER_TABLE_EXISTS_ERROR and sql_file == "account" :
-                print( "DATABASE SETUP SKIPPING" )
+                #print( "DATABASE SETUP SKIPPING" )
                 return
 
             print( f"create_tables {sql_file} {err.msg}" )
             sys.exit( 4 )
 
         ####
 
@@ -118,31 +117,27 @@
 
     insert_fromdict( "system" , { "key" : "database/version" , "val_str" : version( "esanom" ) } )
 
     insert_fromdict( "system" , { "key" : "orchestrator/time" , "val_int" : 0 } )
     insert_fromdict( "system" , { "key" : "scheduler/time" , "val_int" : 0 } )
 
     insert_fromdict( "system" , { "key" : "system/mailer/token" } )
-    insert_fromdict( "system" , { "key" : "system/id" , "val_str" : "SPARC" } )
-    insert_fromdict( "system" , { "key" : "system/registration" , "val_int" : 0 } )
 
     print( "DB INIT OK" )
 
 #####################################################################
 
 def init_tables( ) :
 
     # Default group
     insert_fromdict( "group" , { "name" : "default" , "enable" : 1 } )
     system_group_id = insert_fromdict( "group" , { "name" : "system" , "enable" : 1 } )
 
     admin_role_id = insert_fromdict( "role" , { "name" : "admin" , "enable" : 1 } )
     user_role_id = insert_fromdict( "role" , { "name" : "user" , "enable" : 1 } )
-    model_role_id = insert_fromdict( "role" , { "name" : "model" , "enable" : 1 } )
-    dashboard_role_id = insert_fromdict( "role" , { "name" : "dashboard" , "enable" : 1 } )
 
     ####
 
     if _config.get( "admin_account_email" ) != "" :
 
         admin_account_password = _config.get( "admin_account_password" ) 
         if admin_account_password == "" :
@@ -159,14 +154,18 @@
         admin_api_id = insert_fromdict( "api" , { "account_id" : admin_account_id , "name" : "_admin_system_user" , "ip" : "127." , "enable" : 1  } )
         insert_fromdict( "api_role" , { "api_id" : admin_api_id , "role_id" : user_role_id } )
         insert_fromdict( "api_group" , { "api_id" : admin_api_id , "group_id" : system_group_id } )
         insert_fromdict( "roleuser" , { "api_id" : admin_api_id  } )
 
     #####
 
+    # model/dashboard role
+    insert_fromdict( "role" , { "name" : "model" , "enable" : 1 } )
+    insert_fromdict( "role" , { "name" : "dashboard" , "enable" : 1 } )
+
 #####################################################################
 
 def wait_until_ready( retries = 20 ) :
 
     counter_databaseready_retries = retries
     while ready_check( ) == None :
         print( "Waiting for database ready" )
@@ -674,44 +673,15 @@
     rows = db_query_select_rows( f"SELECT name from `port`" )
     if rows == None : return( port_names )
 
     for row in rows : port_names.append( row[ "name" ] )
 
     return( port_names )
 
-
-def verify_portpinunit( io_name , io_val ) :
-
-    row = db_query_select_row( f"SELECT id from `port` where name=%s LIMIT 1" , [ io_name ] )
-    if row == None : raise Exception( f"no port found {io_name=}" )
-
-    if not "pins" in io_val : return( )
-
-    port_id = row[ "id" ]
-
-    ####
-
-    for pin_i , ( pin_name , pin_val ) in enumerate( io_val[ "pins" ].items( ) ) :
-
-        row = db_query_select_row( f"SELECT id from `pin` where name=%s LIMIT 1" , [ pin_name ] )
-        if row == None : raise Exception( f"no pin found {io_name=} {pin_name=}" )
-
-        pin_id = row[ "id" ]
-
-        row = db_query_select_row( f"SELECT id from `port_pin` where port_id=%s AND pin_id=%s LIMIT 1" , [ port_id , pin_id ] )
-        if row == None : raise Exception( f"no port_pin row {io_name=} {pin_name=}" )
-
-        if not "unit" in pin_val : continue
-
-        row = db_query_select_row( f"SELECT id from `unit` where pin_id=%s and name=%s LIMIT 1" , [ pin_id , pin_val[ "unit" ] ] )
-        if row == None : raise Exception( f"no unit row {io_name=} {pin_name=} {pin_val['unit']=}" )
-
-
-
-def xxxverify_portpinunit( specs_io ) :
+def verify_portpinunit( specs_io ) :
 
     if not "name" in specs_io : return( None )
 
     ####
 
     row = db_query_select_row( f"SELECT id from `port` where name=%s LIMIT 1" , [ specs_io[ "name" ] ] )
     if row == None :
@@ -766,62 +736,16 @@
 
     for unit in units :
         if unit[ "default" ] == 1 :
             return( unit[ "id" ] )
 
     return( None )
 
-def process_specs_io( io_name , io_val , rolemodel_id , direction ) :
-            
-    port_row = db_query_select_row( "SELECT id,name from port where name=%s" , [ io_name ] )
-    if port_row == None : raise Exception( f"port_row None {io_name}" )
-
-    ####
-
-    row_data = { "rolemodel_id" : rolemodel_id , "port_id" : port_row[ "id" ] , "direction" : direction }
-
-    row_data.update( _util.dict_scan( io_val , [ "enable" , "visible" , "cardinal" , "pipeline" , "download" , "read" , "write" ] ) )
-
-    mport_id = insert_fromdict( "mport" , row_data )
-    if mport_id == None : raise Exception( f"process_specs_io mport_id None {io_name} {row_data}" )
-
-    ####
 
-    pins = db_query_select_rows( f"SELECT pin.id as pin_id , pin.name as pin_name FROM port_pin,pin WHERE port_id={port_row['id']} AND port_pin.pin_id = pin.id" )
-
-    for pin in pins :
-
-        # Init with default unit (if any)
-        # FIXME TODO maybe use a faster query rather than the same generic one when unit name is given
-        pin_unit = unit_get_bypin( pin[ "pin_id" ] )
-        if pin_unit == None : raise Exception( f"no unit? {pin['pin_name']}" )
-
-        mpin_row = { "mport_id" : mport_id , "pin_id" : pin[ "pin_id" ] , "unit_id" : pin_unit }
-
-        ####
-
-        if "pins" in io_val :
-            for pin_i , ( pin_name , pin_v ) in enumerate( io_val[ "pins" ].items( ) ) :
-                if pin_name == pin[ "pin_name" ] :
-                    mpin_row.update( _util.dict_scan( pin_v , [ "override" , "enable" , "visible" , "pipeline" , "download" , "read" , "write" ] ) )
-
-                    pin_unit = unit_get_bypin( pin[ "pin_id" ] , pin_v.get( "unit" , None ) )
-                    if pin_unit == None : raise Exception( "no unit?" )
-
-                    mpin_row[ "unit_id" ] = pin_unit
-
-                    break
-
-        ####
-
-        insert_fromdict( "mpin" , mpin_row )
-
-
-
-def xxxprocess_specs_io( specs_io , rolemodel_id , direction ) :
+def process_specs_io( specs_io , rolemodel_id , direction ) :
             
     if not "name" in specs_io : return( None )
 
     port_row = db_query_select_row( "SELECT id,name from port where name=%s" , [ specs_io[ "name" ] ] )
     if port_row == None :
         print( f"port_row None {specs_io['name']}")
         return( None )
@@ -1267,27 +1191,24 @@
 
     #print( ports )
 
     rolemodel_row = db_query_select_row( "SELECT * from rolemodel WHERE id=%s LIMIT 1" , [ rolemodel_id ] )
     if rolemodel_row == None : raise Exception("rolemodel_row None" ) 
 
     interface_namespace = f"{rolemodel_row['name']}:"
-    if interfaces_global :
-        rolemodel_id=None
-        interface_namespace = ""
+    if interfaces_global : interface_namespace = ""
 
     for port_data in ports :
         if "name" not in port_data : raise Exception( f"name not in port" )
         if "pins" not in port_data : raise Exception( f"pins not in port" )
 
         port_name = f"{interface_namespace}{port_data['name']}"
 
         port_row = db_query_select_row( "SELECT * from port where name=%s LIMIT 1" , [ port_name ] )
-        #if port_row != None : raise Exception( f"port {port_name} already exists" )
-        if port_row != None : continue
+        if port_row != None : raise Exception( f"port {port_name} already exists" )
 
         port_id = insert_fromdict( "port" , { "name" : port_name , "rolemodel_id" : rolemodel_id , "visible" : 0 } )
 
         print( f"{port_name=} {port_id=}" )
 
         for pin_data in port_data[ "pins" ] :
             if "name" not in pin_data : raise Exception( f"name not in pin" )
@@ -1327,16 +1248,15 @@
             ####
 
             for unit_data in pin_data[ "units" ] :
                 default = 0
                 if not flag_unit_default_found :
                     default = 1
                     flag_unit_default_found = True
-                # FIXME TODO once default is seen, do not process any future defaults
-                if "default" in pin_data : default = pin_data[ "default" ]
+                if "default" in pin_data : default = pin_data["default"]
                 unit_name = f"{unit_data['name']}"
                 insert_fromdict( "unit" , { "name" : unit_name , "pin_id" : pin_id , "default" : default , "visible" : 0 } )
 
 ####
 
 def handle_overrides( task_uid ) :
     #print( f"handle_overrides {task_uid=}" )
@@ -1344,15 +1264,15 @@
 
     rolemodel_id = task_row[ "rolemodel_id" ]
     mport_rows = db_query_select_rows( "SELECT * from mport where rolemodel_id=%s" , [ rolemodel_id ] )
 
     for mport_row in mport_rows :
         mpin_rows = db_query_select_rows( "SELECT * from mpin where mport_id=%s and override IS NOT NULL" , [ mport_row[ "id" ] ] )
         for mpin_row in mpin_rows :
-            io_row = db_query_select_row( "SELECT * from io where task_id=%s AND mpin_id=%s LIMIT 1" , [ task_row[ "id" ] , mpin_row[ "id" ] ] )
+            io_row = db_query_select_row( "SELECT * from io where task_id=%s AND mpin_id=%s LIMIT 1" , [ task_row["id"],mpin_row["id"] ] )
             if io_row is None : handle_override( task_row[ "id" ] , mpin_row[ "id" ] , mpin_row[ "override" ] )
 
 
 def handle_override( task_id , mpin_id , mpin_override ) :
 
     override_sections = mpin_override.split( "," )
 
@@ -1380,15 +1300,15 @@
         file_data = dumps( cmd_val )
         file_hash = sha256( file_data ).hexdigest( ) 
         file_path = _util.get_io_hash_filepath( file_hash )
         with open( file_path , "wb" ) as f : f.write( file_data )
         file_size = os.path.getsize( file_path )
         #dtype = type( cmd_val ).__name__ 
 
-        #print( f"{file_path=}" )
+        print(f"{file_path=}")
 
         ####
         # FIXME TODO handle if data is > than block limit (8MB)
 
         io_data = {
             "task_id" : task_id ,
             "mpin_id" : mpin_id ,
@@ -1447,32 +1367,28 @@
     if override_key == "api_name" :
 
         pipeline_task_row = db_query_select_row( "SELECT * from pipeline_task WHERE task_id=%s OR next_task_id=%s LIMIT 1" , [ task_id , task_id ] )
         pipeline_row = db_query_select_row( "SELECT * from pipeline WHERE id=%s LIMIT 1" , [ pipeline_task_row[ "pipeline_id" ] ] )
         roleuser_row = db_query_select_row( "SELECT * from roleuser WHERE id=%s LIMIT 1" , [ pipeline_row[ "roleuser_id" ] ] )
         api_row = db_query_select_row( "SELECT * from api WHERE id=%s LIMIT 1" , [ roleuser_row[ "api_id" ] ] )
 
-        system_row = db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "system/id" ] )
-        v = f"{system_row['val_str']}/api/name : {api_row['name']}"
+        v = api_row['name']
         #print(f"{v=}")
         return( v )
         #return( pipeline_row[ "name" ] )
 
     ####
 
     if override_key == "pipeline_status" :
 
         pipeline_task_row = db_query_select_row( "SELECT * from pipeline_task WHERE task_id=%s OR next_task_id=%s LIMIT 1" , [ task_id , task_id ] )
         pipeline_row = db_query_select_row( "SELECT * from pipeline WHERE id=%s LIMIT 1" , [ pipeline_task_row[ "pipeline_id" ] ] )
 
-        task_row = db_query_select_row( "SELECT * from `task` WHERE `id`=%s LIMIT 1" , [ task_id ] )
-
-        system_row = db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "system/id" ] )
-
-        dt=round(time.time()-task_row['created_at'].timestamp(),1)
-        msg = f"{system_row['val_str']} -> {pipeline_row['name']} -> {dt}s"
-        return( msg )
+        v = pipeline_row['name']
+        #print(f"{v=}")
+        return( v )
+        #return( pipeline_row[ "name" ] )
 
     return( None )
 
 ####
```

### Comparing `esanom-0.7.12.30/esanom/engine.py` & `esanom-0.7.9.3232/esanom/engine.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/monitor.py` & `esanom-0.7.9.3232/esanom/monitor.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/orchestrator.py` & `esanom-0.7.9.3232/esanom/orchestrator.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/pipeline.py` & `esanom-0.7.9.3232/esanom/pipeline.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/account.sql` & `esanom-0.7.9.3232/esanom/resources/database/account.sql`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,19 @@
     
     `email` varchar(255) NOT NULL CHECK (`email` <> ""),
     `password` varchar(255) DEFAULT NULL,
     `name` varchar(255) DEFAULT NULL,
 
     `enable` BOOLEAN DEFAULT 0,
 
-    `email_confirm_code` varchar(255) DEFAULT NULL,
     `email_confirmsent_at` DATETIME DEFAULT NULL,
     `email_confirmed` BOOLEAN DEFAULT 0,
     `email_confirmed_at` DATETIME DEFAULT NULL,
     
-    `api_max` int UNSIGNED DEFAULT 1,
+    `api_max` int UNSIGNED DEFAULT 2,
     
     `uid` varchar(255) NOT NULL CHECK (`uid` <> ""),
 
     `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
     `accessed_at` DATETIME DEFAULT NULL,
```

### Comparing `esanom-0.7.12.30/esanom/resources/database/api.sql` & `esanom-0.7.9.3232/esanom/resources/database/api.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/api_group.sql` & `esanom-0.7.9.3232/esanom/resources/database/api_group.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/api_role.sql` & `esanom-0.7.9.3232/esanom/resources/database/api_role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/claim.sql` & `esanom-0.7.9.3232/esanom/resources/database/claim.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/group.sql` & `esanom-0.7.9.3232/esanom/resources/database/group.sql`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 CREATE TABLE `group` (
 
     `id` INT UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` VARCHAR(255) NOT NULL CHECK (`name` <> ""),
     `description` VARCHAR(255) DEFAULT "",
     `enable` BOOLEAN DEFAULT 0,
-    `uid` varchar(255) NOT NULL CHECK (`uid` <> ""),
     
     PRIMARY KEY (`id`),
     
     UNIQUE KEY `name` (`name`),
-    UNIQUE KEY `uid` (`uid`) ,
     KEY `enable` (`enable`) 
 
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.12.30/esanom/resources/database/io.sql` & `esanom-0.7.9.3232/esanom/resources/database/io.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/ioblock.sql` & `esanom-0.7.9.3232/esanom/resources/database/ioblock.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/log.sql` & `esanom-0.7.9.3232/esanom/resources/database/log.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/mpin.sql` & `esanom-0.7.9.3232/esanom/resources/database/mpin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/mport.sql` & `esanom-0.7.9.3232/esanom/resources/database/mport.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/pin.sql` & `esanom-0.7.9.3232/esanom/resources/database/port.sql`

 * *Files 9% similar despite different names*

```diff
@@ -16,37 +16,35 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-CREATE TABLE `pin` (
+CREATE TABLE `port` (
 
     `id` int UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` varchar(255) NOT NULL CHECK (`name` <> ""),
     `description` TEXT ,
     
     `visible` BOOLEAN DEFAULT 1,
     `rolemodel_id` INT UNSIGNED DEFAULT NULL,
-    
-    `type` varchar(255) DEFAULT "",
     `uid` varchar(255) NOT NULL CHECK (`uid` <> "") ,
 
     `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
 
     PRIMARY KEY (`id`) ,
 
     UNIQUE KEY `name` (`name`) ,
     UNIQUE KEY `uid` (`uid`) ,
 
     KEY `rolemodel_id` (`rolemodel_id`),
-    CONSTRAINT `pin_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
-
+    CONSTRAINT `port_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
+    
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.12.30/esanom/resources/database/pipeline.sql` & `esanom-0.7.9.3232/esanom/resources/database/pipeline.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/pipeline_task.sql` & `esanom-0.7.9.3232/esanom/resources/database/pipeline_task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/port.sql` & `esanom-0.7.9.3232/esanom/resources/database/pin.sql`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-CREATE TABLE `port` (
+CREATE TABLE `pin` (
 
     `id` int UNSIGNED NOT NULL AUTO_INCREMENT,
 
     `name` varchar(255) NOT NULL CHECK (`name` <> ""),
     `description` TEXT ,
     
     `visible` BOOLEAN DEFAULT 1,
     `rolemodel_id` INT UNSIGNED DEFAULT NULL,
-    `uid` varchar(255) NOT NULL CHECK (`uid` <> "") ,
+    
+    `type` varchar(255) DEFAULT "",
 
     `created_at` DATETIME DEFAULT CURRENT_TIMESTAMP,
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
 
     PRIMARY KEY (`id`) ,
 
     UNIQUE KEY `name` (`name`) ,
-    UNIQUE KEY `uid` (`uid`) ,
 
     KEY `rolemodel_id` (`rolemodel_id`),
-    CONSTRAINT `port_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
-    
+    CONSTRAINT `pin_rolemodel_id` FOREIGN KEY (`rolemodel_id`) REFERENCES `rolemodel` (`id`) ON DELETE CASCADE 
+
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.12.30/esanom/resources/database/port_pin.sql` & `esanom-0.7.9.3232/esanom/resources/database/port_pin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/role.sql` & `esanom-0.7.9.3232/esanom/resources/database/role.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/roleadmin.sql` & `esanom-0.7.9.3232/esanom/resources/database/roleadmin.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/roledashboard.sql` & `esanom-0.7.9.3232/esanom/resources/database/roledashboard.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/rolemodel.sql` & `esanom-0.7.9.3232/esanom/resources/database/rolemodel.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/roleuser.sql` & `esanom-0.7.9.3232/esanom/resources/database/roleuser.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/schedule.sql` & `esanom-0.7.9.3232/esanom/resources/database/schedule.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/session.sql` & `esanom-0.7.9.3232/esanom/resources/database/session.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/system.sql` & `esanom-0.7.9.3232/esanom/resources/database/system.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/task.sql` & `esanom-0.7.9.3232/esanom/resources/database/task.sql`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/resources/database/triggers.sql` & `esanom-0.7.9.3232/esanom/resources/database/triggers.sql`

 * *Files 12% similar despite different names*

```diff
@@ -16,61 +16,36 @@
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 */
 
-
-CREATE TRIGGER group_insert BEFORE INSERT ON `group` FOR EACH ROW BEGIN
-
-    SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
-
-END ;
-
-/******************************************************************/
-
 CREATE TRIGGER account_insert BEFORE INSERT ON account FOR EACH ROW BEGIN
 
     IF ( NEW.email_confirmed = 1 ) THEN
         SET NEW.email_confirmsent_at = NOW( ) ;
         SET NEW.email_confirmed_at = NOW( ) ;
     END IF ;
 
     SET NEW.password = SHA2( NEW.password , 256 ) ;
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-CREATE TRIGGER account_update BEFORE UPDATE ON account FOR EACH ROW BEGIN
-
-    IF NEW.password <> OLD.password THEN
-        SET NEW.password = SHA2( NEW.password , 256 ) ;
-    END IF ;
-
-END ;
-
 /******************************************************************/
 
 CREATE TRIGGER api_insert BEFORE INSERT ON api FOR EACH ROW BEGIN
 
     SET NEW.token = CONCAT( "NOM" , SUBSTRING( SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) , 4 , 64 ) ) ;
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-CREATE TRIGGER api_update BEFORE UPDATE ON api FOR EACH ROW BEGIN
-
-    IF NEW.token <> OLD.token THEN
-        SET NEW.token = CONCAT( "NOM" , SUBSTRING( SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) , 4 , 64 ) ) ;
-    END IF ;
-
-END ;
-
 /******************************************************************/
 
 CREATE TRIGGER pipeline_insert BEFORE INSERT ON pipeline FOR EACH ROW BEGIN
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
@@ -179,19 +154,7 @@
 
 CREATE TRIGGER port_insert BEFORE INSERT ON port FOR EACH ROW BEGIN
 
     SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
 
 END ;
 
-/******************************************************************/
-
-CREATE TRIGGER pin_insert BEFORE INSERT ON pin FOR EACH ROW BEGIN
-
-    SET NEW.uid = SHA2( CONCAT( NOW( ) , RAND( ) , UUID( ) , NEW.id , "7F6I12APOL" ) , 256 ) ;
-
-END ;
-
-/**WARNING-DO-NOT-DB-INIT-GROUP-TRIGGERS-AT-THE-BOTTOM-WTF*********/
-
-
-
```

### Comparing `esanom-0.7.12.30/esanom/resources/database/unit.sql` & `esanom-0.7.9.3232/esanom/resources/database/unit.sql`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     `updated_at` DATETIME DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
 
     PRIMARY KEY (`id`) ,
 
     KEY `pin_id` (`pin_id`),
     KEY `default` (`default`),
 
-    CONSTRAINT `unit_pin_id` FOREIGN KEY (`pin_id`) REFERENCES `pin` (`id`) ON DELETE CASCADE ,
-    CONSTRAINT `unit_unique_pinidname` UNIQUE (`pin_id`,`name`)
+    CONSTRAINT `unit_pin_id` FOREIGN KEY (`pin_id`) REFERENCES `pin` (`id`) ON DELETE CASCADE 
     
 ) ENGINE=InnoDB,AUTO_INCREMENT=101;
```

### Comparing `esanom-0.7.12.30/esanom/roleadmin.py` & `esanom-0.7.9.3232/esanom/roleadmin.py-bak1`

 * *Files 8% similar despite different names*

```diff
@@ -298,101 +298,125 @@
     delete_testdata( "group" )
 
     delete_testdata( "port" )
     delete_testdata( "pin" )
     delete_testdata( "unit" )
 
     ####
-
+    
     config = { }
 
-    # GROUPS
-    for i in range( 10 ) :
+    config[ "group_total" ] = 10
+
+    for i in range( config[ "group_total" ] ) :
         config[ f"group{i}_name" ] = _util.get_test_uid( postfix = f"{i}_GROUP" )
         row_data = { "name" : config[ f"group{i}_name" ] , "enable" : 1 }
         create( "group" , row_data )
 
     ####
 
-    # USERS
-    for i in range( 10 ) :
-        account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 , "email" :  f"nom_user_test{i}@sparc.space" , "password" : f"{i}_USER" , "email_confirmed" : 1 } )
+    test_models = [
+        "TESTNOTIFICATIONEMAIL_MODEL" ,
+        "TESTMATHINCREMENT_MODEL" ,
+        "TESTNOP_MODEL" , "TESTSLEEP_MODEL" , "TESTFAILURE_MODEL" ,
+        "TESTNAND_MODEL" , "TESTREBOUND_MODEL" ,"TESTXLSX_MODEL" ,"TESTPLOT_MODEL" ,
+        "TESTPILLOW_MODEL" , "TESTDATETIME_MODEL" ,
+        "TRAJECTORY_MODEL"
+    ]
+
+    for test_model in test_models :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{test_model}" ) , "enable" : 1 } ,
+            "group" : [ config[ f"group0_name" ] ] 
+        } 
+        create_model( options )
+
+    ####
+
+    config[ "user_total" ] = 10
+    for i in range( config[ "user_total" ] ) :
+
+        api_email = f"nomserver_user_{i}@sparc.space"
         
         options = {
-            "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 } ,
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_USER" ) , "enable" : 1 , "email" : api_email } ,
             "group" : [ config[ f"group0_name" ] ] 
         } 
         create_user( options )
 
     ####
-    # MODELS
-    for i in range( 10 ) :
-        account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 , "email" :  f"nom_model_test{i}@sparc.space" , "password" : f"{i}_MODEL" , "email_confirmed" : 1 } )
-        
+
+    config[ "model_total" ] = 10
+    for i in range( config[ "model_total" ] ) :
         options = {
-            "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 } ,
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_MODEL" ) , "enable" : 1 } ,
             "group" : [ config[ f"group0_name" ] ] 
         } 
         create_model( options )
 
+    ####
 
-    # DASHBOARD (Single)
-    account_id = create( "account" , { "name" : _util.get_test_uid( postfix = f"0_DASHBOARD" ) , "enable" : 1 , "email" :  f"nom_dashboard_test0@sparc.space" , "password" : f"0_DASHBOARD" , "email_confirmed" : 1 } )
-    
-    options = {
-        "api" : { "account_id" : account_id , "name" : _util.get_test_uid( postfix = f"0_DASHBOARD" ) , "enable" : 1 } ,
-        "group" : [ ] ,
-        "role" : "dashboard"
-    } 
-    create_api_with_rolegroup( options )
+    config[ "admin_total" ] = 10
+    for i in range( config[ "admin_total" ] ) :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_ADMIN" ) , "enable" : 1 } ,
+            "group" : [ ] ,
+            "role" : "admin"
+        } 
+        create_api_with_rolegroup( options )
 
+    ####
 
+    config[ "dashboard_total" ] = 10
+    for i in range( config[ "dashboard_total" ] ) :
+        options = {
+            "api" : { "name" : _util.get_test_uid( postfix = f"{i}_DASHBOARD" ) , "enable" : 1 } ,
+            "group" : [ ] ,
+            "role" : "dashboard"
+        } 
+        create_api_with_rolegroup( options )
+
+    ####
 
     port_prefixes = [ ]
     for chi in range( 26 ) : port_prefixes.append( f"test_port_{chr(97+chi)}_")
 
-    ####
-
     data_rows_unit = [ ] 
     data_rows_port_pin = [ ] 
 
-    ####
-
     for port_prefix in port_prefixes :
 
         for i in range( 3 ) :
 
             port_name = f"{port_prefix}{i}"
             port_id = create( "port" , { "name" : port_name } )
             
             ####
 
             for j in range( 3 ) :
 
                 pin_name = f"{port_name}_pin_{j}"
-                pin_id = create( "pin" , { "name" : pin_name , "type" : "str" } )
+                pin_id = create( "pin" , { "name" : pin_name } )
 
                 ####
 
                 for k in range( 3 ) :
 
                     unit_default = 0
-                    #if k == 0 and j == 1 : unit_default = 1
                     if k == 0 : unit_default = 1
 
                     row_data = { "name" : f"{pin_name}_unit_{k}" , "pin_id" : pin_id , "default" : unit_default }
 
                     data_rows_unit.append( row_data )
 
                 ####
 
                 cardinal = j
-                #if i == 0 : cardinal = j
 
-                row_data = { "port_id" : port_id , "pin_id" : pin_id ,"cardinal" : cardinal }
+                row_data = { "port_id" : port_id , "pin_id" : pin_id , "cardinal" : cardinal }
                 data_rows_port_pin.append( row_data )
 
     ####
 
     create_bulk( "unit" , data_rows_unit )
     create_bulk( "port_pin" , data_rows_port_pin )
```

### Comparing `esanom-0.7.12.30/esanom/rolemodel.py` & `esanom-0.7.9.3232/esanom/rolemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     return( _util.request_get( "/model_state" ) )
 
 
 def specs( specs_in ) :
 
     res = _util.request_post( "/model_specs" , data = specs_in )
-    print(res)
     return( isinstance( res , dict ) )
 
 def model_pipeline( ) :
 
     model_schedule_messages = _util.request_get( "/model_schedule" )
     #print(model_schedule_messages)
 
@@ -62,15 +61,15 @@
     if model_claim_set_messages[ "claim_status" ] == "NO" : raise Exception( "claim_status NO" )
     ####
 
     claim_uid = model_claim_set_messages[ "claim_uid" ]
     for i in range( 6 ) :
         time.sleep( 5 )
         model_claim_get_messages = _util.request_post( "/model_claim_get" , params = { "claim_uid" : claim_uid } )
-        #_util.print_debug( model_claim_get_messages )
+        _util.print_debug( model_claim_get_messages )
         if model_claim_get_messages[ "claim_status" ] == "NO" : raise Exception( "claim_status NO" )
         if model_claim_get_messages[ "claim_status" ] == "YES" : break
         print(f"model_pipeline model_claim_get WAIT {i}/15")
 
     if model_claim_get_messages[ "claim_status" ] != "YES" :
         _util.request_post( "/model_claim_release" , params = { "claim_uid" : claim_uid } )
         raise Exception( "claim_status NO... Claim released." )
```

### Comparing `esanom-0.7.12.30/esanom/roleuser.py` & `esanom-0.7.9.3232/esanom/roleuser.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/__init__.py` & `esanom-0.7.9.3232/esanom/routes/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/api.py` & `esanom-0.7.9.3232/esanom/routes/v3/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -263,55 +263,105 @@
 
 @ROUTES.route( "/model_specs" , methods = [ "POST" ] )
 @_common.decorator_token_required
 @_common.decorator_role_required( "model" )
 @_common.decorator_request_json
 def model_specs( ) :
 
-    api_id = _g.api[ "id" ]
-    specs = request.json
+    if not "name" in request.json : return( _common.response_error( e_msg = "not name"  ) )
 
-    rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE api_id=%s LIMIT 1" , [ api_id ] )
+    ####
+
+    rolemodel_enable = 0
+    if _config.DATA[ "server_security_lax" ] : rolemodel_enable = 1
+
+    ####
 
-    rolemodel_data = {
-        "api_id" : api_id ,
-        "name" : specs[ "name" ] ,
-        "specs" : json.dumps( specs ) ,
-        "category" : specs.get( "category" ) ,
-        "description" : specs.get( "desc" ) ,
-        "ignore_pred_fail" : specs.get( "ignore_pred_fail" , 0 ) 
-    }
+    rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
 
     if rolemodel_row == None :
-        try : rolemodel_id = _database.insert_fromdict( "rolemodel" , rolemodel_data )
-        except Exception as e : raise Exception( f"verify specs {e}" )
+        rolemodel_data = {
+            "api_id" : _g.api[ "id" ] ,
+            "name" : request.json[ "name" ] ,
+            "specs" : json.dumps( request.json ) ,
+            "category" : request.json.get( "category" ) ,
+            "description" : request.json.get( "desc" ) ,
+            "type" : request.json.get( "type" ) ,
+            "user_api_ip_prefix" : request.json.get( "user_api_ip_prefix" , "127.,192.168.,172.,10." ) ,
+            "user_api_email_postfix" : request.json.get( "user_api_email_postfix" , "sparc.gr,esa.int,aeronomie.be" ) ,
+            "input_size_max" : request.json.get( "input_size_max" , 10485760 ) ,
+            "ignore_pred_fail" : request.json.get( "ignore_pred_fail" ) ,
+            "enable" : rolemodel_enable
+        }
+        rolemodel_id = _database.insert_fromdict( "rolemodel" , rolemodel_data )
     else :
-        if rolemodel_row[ "updateable" ] == 0 : raise Exception( f"not updateable" )
+        if rolemodel_row[ "updateable" ] == 0 :
+            if not _config.DATA[ "server_security_lax" ]  :
+                return( _common.response_error( e_msg = "not updateable"  ) )
+        if json.loads( rolemodel_row[ "specs" ] ) == request.json : return( _common.response_default( ) )
         rolemodel_id = rolemodel_row[ "id" ]
+        rolemodel_data = {
+            "name" : request.json[ "name" ] ,
+            "specs" : json.dumps( request.json ) ,
+            "category" : request.json.get( "category" ) ,
+            "description" : request.json.get( "desc" ) ,
+            "type" : request.json.get( "type" ) ,
+            "user_api_ip_prefix" : request.json.get( "user_api_ip_prefix" , "127.,192.168.,172.,10." ) ,
+            "user_api_email_postfix" : request.json.get( "user_api_email_postfix" , "sparc.gr,esa.int,aeronomie.be" ) ,
+            "input_size_max" : request.json.get( "input_size_max" , 10485760 ) ,
+            "ignore_pred_fail" : request.json.get( "ignore_pred_fail" ) ,
+            "enable" : rolemodel_enable
+        }
         _database.update_fromdict( "rolemodel" , rolemodel_id , rolemodel_data )
 
     ####
 
     _database.model_flush_ports( rolemodel_id ) 
+    # FIXME TODO is this required?
     _database.db_query_delete( f"DELETE from `mport` WHERE rolemodel_id=%s" , [ rolemodel_id ] )    
 
-    if "inputs" in specs :
-        for io_i , ( io_name , io_val ) in enumerate( specs[ "inputs" ].items( ) ) :
-            _database.verify_portpinunit( io_name , io_val )
-            _database.process_specs_io( io_name , io_val , rolemodel_id , "inputs" )
-
-    if "outputs" in specs :
-        for io_i , ( io_name , io_val ) in enumerate( specs[ "outputs" ].items( ) ) :
-            _database.verify_portpinunit( io_name , io_val )
-            _database.process_specs_io( io_name , io_val , rolemodel_id , "outputs" )
+
+    interfaces_global = request.json.get( "interfaces_global" , 0 ) == 1
+
+    if "ports" in request.json : _database.model_load_ports( rolemodel_id , request.json[ "ports" ] , interfaces_global = interfaces_global )
+
+    ####
+
+    if "inputs" in request.json :
+        for specs_io in request.json[ "inputs" ] :
+            if not "name" in specs_io : return( _common.response_error( e_msg = "not name in specs_input"  ) )
+            if _database.verify_portpinunit( specs_io ) == None :
+                return( _common.response_error( e_msg = f"verify {specs_io['name']}"  ) )
+
+    if "outputs" in request.json :
+        for specs_io in request.json[ "outputs" ] :
+            if not "name" in specs_io : return( _common.response_error( e_msg = "not name in specs_output"  ) )
+            if _database.verify_portpinunit( specs_io ) == None :
+                return( _common.response_error( e_msg = f"verify {specs_io['name']}"  ) )
+
+    ####
+
+    if "inputs" in request.json :
+        for specs_io in request.json[ "inputs" ] :
+            if _database.process_specs_io( specs_io , rolemodel_id , "inputs" ) == None :
+                return( _common.response_error( e_msg = f"process_specs_io inputs" ) )
+
+    if "outputs" in request.json :
+        for specs_io in request.json[ "outputs" ] :
+            if _database.process_specs_io( specs_io , rolemodel_id , "outputs" ) == None :
+                return( _common.response_error( e_msg = f"process_specs_io outputs" ) )
 
     ####
 
     return( _common.response_default( ) )
 
+
+
+
+
 @ROUTES.route( "/model_pipeline_failed" , methods = [ "POST" ] )
 @_common.decorator_token_required
 @_common.decorator_role_required( "model" )
 @_common.decorator_request_json
 def model_pipeline_failed( ) :
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/api.py-bak1` & `esanom-0.7.9.3232/esanom/routes/v3/web.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,1104 +14,1235 @@
 # This file is subject to the terms and conditions defined in file 'LICENCE.txt', 
 # which is part of this source code package. No part of the package, including 
 # this file, may be copied, modified, propagated, or distributed except 
 # according to the terms contained in the file ‘LICENCE.txt’.“ 
 #
 #################################################################################
 
-from flask import Blueprint , request , g as _g , send_file
-import json
-import copy
 import os
 import time
+import json
+import html
 from datetime import datetime
-
-from esanom import database as _database , util as _util , pipeline as _pipeline , config as _config
-
-from . import common as _common
+from importlib.metadata import version
+from flask import Blueprint , render_template , request , g as _g , redirect , url_for , make_response
+from esanom import database as _database , util as _util , config as _config
+from . import common as _common 
 
 #####################################################################
 
-ROUTES = Blueprint( "routes" , __name__ )
+ROUTES = Blueprint( "routes" , __name__ , template_folder = "templates" , static_folder='static' )
 
-####
+#####################################################################
 
+@ROUTES.before_request
+def before_request_func( ) :
+    _g._benchmark_before_request = time.time( )
 
 @ROUTES.after_request
 def after_request_func( resp ) :
 
-    #print(f"after_request_func{request.url_rule}")
-    #/v3/api/model_schedule
+#    resp.cache_control.max_age = 600
 
-    ####
-    NoM_Client_Wait = 0
-    if "/admin" not in request.url_rule.rule : NoM_Client_Wait = 0.5
-    if request.remote_addr.startswith( "127." ): NoM_Client_Wait = 0.01
-    resp.headers[ "NoM_Client_Wait" ] = NoM_Client_Wait
-    ####
+#    resp.cache_control.no_cache = True
+#    resp.cache_control.no_store = True
+    #resp.cache_control.must_revalidate = False
+    #resp.cache_control.proxy_revalidate = False
 
-    #if 'Cache-Control' not in response.headers:
-    #    response.headers['Cache-Control'] = 'no-store'
+    if "text/html" not in resp.headers[ "Content-Type" ] : return( resp )
 
-    #if "text/html" not in resp.headers[ "Content-Type" ] : return( resp )
-    #cookie_key = request.cookies.get( "key" , "" )
+    cookie_key = request.cookies.get( "key" , "" )
     #if cookie_key.strip( ) != "" : return( resp )
-    #resp.set_cookie( "key" , session_key , secure = True , samesite = "Strict" )
+    if len( cookie_key ) == 64 : return( resp )
+
+    ####
+
+    session_key = _util.generate_rhash( )
+    resp.set_cookie( "key" , session_key , secure = True , samesite = "Strict" )
 
     ####
 
     return( resp )
 
+@ROUTES.app_template_filter( "filter_self_basename" )
+def filter_self_basename( s ):
+    # <TemplateReference 'pages/account/inc_admin_nav.html'>
+    parts = str( s ).split( "'" )
+    if len( parts ) != 3 : return( None )
+    return( os.path.basename( parts[ 1 ] ).removesuffix( ".html" ) )
 
-@ROUTES.route( "/admin_state" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-def admin_state( ) :
+#####################################################################
 
-    messages = { }
+@ROUTES.route( "/error_404" , methods = [ "GET" ] )
+def page_error_404( ) :
+    return( render_template( "error_404.html" ) , 404 )
+
+@ROUTES.route( "/error_500" , methods = [ "GET" ] )
+def page_error_500( ) :
+    return( render_template( "error_500.html" ) , 500 )
 
-    ####
+#####################################################################
 
-    table = request.args.get( "table" , default = "" ) 
-    if table.strip( ) != "" :
+@ROUTES.app_context_processor
+def app_context_processor( ) :
 
-        row_id_str = request.args.get( "row_id" , default = "" )
-        if row_id_str.strip( ) == "" or ( not row_id_str.lstrip( "-" ).isdigit( ) ) : 
-            row_id = None
-        else :
-            row_id = int( float( row_id_str ) )
-            if not row_id > 0 : row_id = None
+    session_data = { }
+    session_key = request.cookies.get( "key" , "" ).strip( )
+    if len( session_key ) == 64 :
+        session_row = _database.db_query_select_row( "SELECT * from `session` WHERE `key`=%s LIMIT 1" , [ session_key ] )
+        if session_row != None :
+            session_data = json.loads( session_row[ "data" ] ) 
 
-        messages[ table ] = _database.admin_state( table , row_id = row_id )
-        return( _common.response_default( messages ) )
 
-    ####
 
-    for t in _database.NOMTABLES : messages[ t ] = _database.admin_state( t )
+    # FIXME TODO should be optimized
+    system_databaseversion_row = _database.db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "database/version" ] )
+    system_orchestratortime_row = _database.db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "orchestrator/time" ] )
+    system_schedulertime_row = _database.db_query_select_row( "SELECT * from `system` WHERE `key`=%s LIMIT 1" , [ "scheduler/time" ] )
 
-    return( _common.response_default( messages ) )
+    orchestrator_time_dt = round( time.time( ) - system_orchestratortime_row[ "val_int" ] )
+    scheduler_time_dt = round( time.time( ) - system_schedulertime_row[ "val_int" ] )
 
-@ROUTES.route( "/admin_create" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_create( ) :
+    ####
 
-    if not "table" in request.args : return( _common.response_error( e_msg = "request args"  ) )
+    api_row = _database.db_query_select_row( "SELECT * from `api` WHERE `name` LIKE '%0_USER' LIMIT 1" )
 
-    id = _database.insert_fromdict( request.args.get( "table" ).strip( ) , request.json )
+    flag_sampledata = False 
+    if api_row != None : flag_sampledata = True
 
-    if id == None : return( _common.response_error( e_msg = "id none"  ) )
+    ####
 
-    messages = { "id" : id }
+    is_admin = False
+    is_loggedin = False
+    if session_data.get( "account_row" ) :
+        is_loggedin = True
+        is_admin = ( session_data["account_row"]["name"]=="_admin" )
 
-    return( _common.response_default( messages ) )
+    data = {
+        "config_data" : _config.DATA ,
+        "admin_account_email" : "".join(f"&#{ord(c)};" for c in _config.DATA[ "admin_account_email" ] ) ,
+        "nom_version" : version( "esanom" ) ,
+        "database_version" : system_databaseversion_row[ "val_str" ] ,
+        "orchestrator_time_dt" : orchestrator_time_dt ,
+        "scheduler_time_dt" : scheduler_time_dt ,
+        "year" : datetime.now( ).strftime( "%Y" ) ,
+        "flag_sampledata" : flag_sampledata ,
+        "benchmark" : round( time.time( ) - _g._benchmark_before_request , 3 ) ,
+        "session_data" : session_data ,
+        "is_loggedin" : is_loggedin ,
+        "is_admin" : is_admin 
+    }
 
-@ROUTES.route( "/admin_create_bulk" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_create_bulk( ) :
+    #print(data)
 
-    if not "table" in request.args : return( _common.response_error( e_msg = "request args"  ) )
+    return( dict( _tdata = data ) )
 
-    if not "rows" in request.json : return( _common.response_error( e_msg = "request json rows"  ) )
+@ROUTES.app_template_global( "test" )
+def app_template_global_test( n ) :
+    return( f"{n}." )
 
-    ids = [ ]
+#####################################################################
 
-    table = _common.request_arg_str( "table" )
+@ROUTES.route( "/" , methods = [ "GET" ] )
+def page_index( ) :
 
-    for r in request.json[ "rows" ] :
-        id = _database.insert_fromdict( table , r )
-        if id == None : return( _common.response_error( e_msg = "id none"  ) )
-        ids.append( id )
+    return( render_template( "page_index.html" ) )
 
-    messages = { "ids" : ids }
+@ROUTES.route( "/models" , methods = [ "GET" ] )
+def page_models( ) :
 
-    return( _common.response_default( messages ) )
+    rolemodel_rows = _database.db_query_select_rows( "SELECT * from `rolemodel` where enable=1" )
 
-@ROUTES.route( "/admin_update" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_update( ) :
+    for rolemodel_row in rolemodel_rows :
+        if rolemodel_row[ "heartbeat_at" ] != None :
+            rolemodel_row[ "[heartbeat_last]" ] = round( time.time( ) - rolemodel_row[ "heartbeat_at" ].timestamp( ) )
+        else :
+            rolemodel_row[ "[heartbeat_last]" ] = 99999
 
-    if not "table" in request.args : return( _common.response_error( e_msg = "request args"  ) )
-    if not "id" in request.args : return( _common.response_error( e_msg = "request args"  ) )
+    columns = [ "uid" , "name" , "category" , "description" , "[heartbeat_last]" ]
 
-    table = request.args.get( "table" , default = "" ) 
-    if table.strip( ) == "" : return( _common.response_error( e_msg = "table blank" ) )
+    tdata = {
+        "rows" : rolemodel_rows ,
+        "columns" : columns
+    }
 
-    id_str = request.args.get( "id" , default = "" ) 
-    if not id_str.isdigit( ): return( _common.response_error( e_msg = "id not isdigit" ) )
-    id = int( float( id_str ) )
-    if not id > 0 : return( _common.response_error( e_msg = "not id" ) )
+    return( render_template( "pages/models/rows.html" , tdata = tdata ) )
 
-    res = _database.update_fromdict( table , id , request.json )
 
-    if res == None : return( _common.response_error( e_msg = "res none" ) )
 
-    return( _common.response_default( ) )
 
-@ROUTES.route( "/admin_delete" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_delete( ) :
+@ROUTES.route( "/models_read" , methods = [ "GET" ] )
+def page_models_read( ) :
 
-    if not "table" in request.args : return( _common.response_error( e_msg = "request args"  ) )
-    if not "id" in request.args : return( _common.response_error( e_msg = "request args"  ) )
+    rolemodel_uid = _common.request_arg_str( "uid" )
 
-    table = request.args.get( "table" , default = "" ) 
-    if table.strip( ) == "" : return( _common.response_error( e_msg = "table blank" ) )
+    rolemodel_row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE uid=%s LIMIT 1" , [ rolemodel_uid ] )
 
-    id_str = request.args.get( "id" , default = "" ) 
-    if not id_str.isdigit( ) : return( _common.response_error( e_msg = "id not isdigit" ) )
-    id = int( float( id_str ) )
-    if not id > 0 : return( _common.response_error( e_msg = "not id" ) )
+    if rolemodel_row == None : return( render_template( "error_500.html" ) )
 
-    res = _database.delete_fromid( table , id )
+    ####
 
-    if res == None : return( _common.response_error( e_msg = "res none" ) )
+    mport_rows = _database.db_query_select_rows( "SELECT id,port_id,direction,enable,cardinal from mport where rolemodel_id=%s order by id" , [ rolemodel_row[ "id" ] ] )
 
-    return( _common.response_default( ) )
+    ####
 
+    has_inputs = False
+    has_outputs = False
 
-@ROUTES.route( "/admin_delete_bulk" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_delete_bulk( ) :
+    mpins = [ ]
 
-    table = request.args.get( "table" , default = "" ) 
-    if table.strip( ) == "" : return( _common.response_error( e_msg = "table blank" ) )
+    for mport_row in mport_rows :
 
-    if not "rows" in request.json : return( _common.response_error( e_msg = "request json rows"  ) )
+        if mport_row["direction"] == "inputs" : has_inputs = True 
+        if mport_row["direction"] == "outputs" : has_outputs = True 
+        
+        port_row = _database.db_query_select_row( "SELECT * from port where id=%s LIMIT 1" , [ mport_row[ "port_id" ] ] )
 
-    for row_id in request.json[ "rows" ] :
-        _database.delete_fromid( table , row_id )
-        # == None : return( _common.response_error( e_msg = f"delete_fromid {table} {row_id}"  ) )
+        mport_row[ "[port_name]"] = port_row[ "name" ]
+        mport_row[ "[port_uid]"] = port_row[ "uid" ]
 
-    return( _common.response_default( ) )
+        mpin_rows = _database.db_query_select_rows( "SELECT id,mport_id,unit_id from mpin where mport_id=%s order by id" , [ mport_row["id"] ] )
 
-@ROUTES.route( "/admin_model_enable" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_model_enable( ) :
 
-    api_token = request.json.get( "api_token" , "" )
-    if api_token.strip( ) == "" : return( _common.response_error( e_msg = "no api_token" ) )
+        for mpin_row in mpin_rows :
+            unit_row = _database.db_query_select_row( "SELECT * from unit where id=%s LIMIT 1" , [ mpin_row["unit_id"]] )
+            pin_row = _database.db_query_select_row( "SELECT * from pin where id=%s LIMIT 1" , [ unit_row["pin_id"]] )
+            port_pin_row = _database.db_query_select_row( "SELECT * from port_pin where port_id=%s and pin_id=%s LIMIT 1" , [port_row[ "id" ] , pin_row[ "id" ] ] )
+            mpin_row[ "cardinal" ] = port_pin_row[ "cardinal" ]
+            mpin_row[ "id" ] = pin_row[ "id" ]
+            mpin_row[ "name" ] = pin_row[ "name" ]
+            mpin_row[ "type" ] = pin_row[ "type" ]
+            mpin_row[ "unit_name" ] = unit_row[ "name" ]
+            mpin_row[ "port_name/pin_name(unit_name)" ] = port_row[ "name" ] + "/" + pin_row[ "name" ] + "(" + unit_row[ "name" ] + ")"
 
-    api_row = _database.db_query_select_row( "SELECT id from api WHERE token=%s LIMIT 1" , [ api_token ] )
-    if api_row == None : return( _common.response_error( e_msg = "api_row" ) )
 
-    sql = "UPDATE rolemodel SET enable = 1 , updateable = 0 WHERE api_id=%s LIMIT 1"
-    params = [ api_row[ "id" ] ]
+        mpins.append( mpin_rows )
 
-    _database.db_query_update( sql , params )
+        mport_row[ "[mpin_rows]" ] = mpin_rows
 
-    return( _common.response_default( ) )
 
+    mpin_columns = [ "name" , "cardinal" , "type" , "unit_name" ]
 
-@ROUTES.route( "/admin_model_updateable" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_model_updateable( ) :
+    tdata = {
+        "row" : rolemodel_row ,
+        "mport_rows" : mport_rows ,
+        "has_inputs" : has_inputs ,
+        "has_outputs" : has_outputs ,
+        "mpin_columns" : mpin_columns
+    }
 
-    api_token = request.json.get( "api_token" , "" )
-    if api_token.strip( ) == "" : return( _common.response_error( e_msg = "no api_token" ) )
+    return( render_template( "pages/models/read.html" , tdata = tdata ) )
 
-    api_row = _database.db_query_select_row( "SELECT id from api WHERE token=%s LIMIT 1" , [ api_token ] )
-    if api_row == None : return( _common.response_error( e_msg = "api_row" ) )
 
-    sql = "UPDATE rolemodel SET enable=0,updateable=1 WHERE api_id=%s LIMIT 1"
-    params = [ api_row[ "id" ] ]
 
-    res = _database.db_query_update( sql , params )
-    if res == None : return( _common.response_error( e_msg = "db_query_update none" ) )
+@ROUTES.route( "/ports" , methods = [ "GET" ] )
+def page_ports( ) :
 
-    return( _common.response_default( ) )
 
+    rows = _database.db_query_select_rows( "SELECT * from `port`" )
 
-@ROUTES.route( "/admin_group_flush" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "admin" )
-@_common.decorator_request_json
-def admin_group_flush( ) :
+    columns = [ "uid" , "name" , "description" ]
 
-    api_id = _common.request_arg_int( "api_id" )
-    if api_id == None : return( _common.response_error( e_msg = "api_id bad" ) )
+    tdata = {
+        "rows" : rows ,
+        "columns" : columns
+    }
 
-    _database.db_query_delete( "DELETE FROM api_group WHERE api_id=%s" , [ api_id ] )
+    return( render_template( "pages/ports/rows.html" , tdata = tdata ) )
 
-    return( _common.response_default( ) )
 
-#####################################################################
 
-@ROUTES.route( "/model_state" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-def model_state( ) :
+@ROUTES.route( "/ports_read" , methods = [ "GET" ] )
+def page_ports_read( ) :
 
-    messages = { }
+    uid = _common.request_arg_str( "uid" )
 
-    messages[ "model" ] = _database.model_state_rolemodel( api_id = _g.api[ "id" ] )
-    messages[ "group" ] = _database.model_state_group( api_id = _g.api[ "id" ] )
+    row = _database.db_query_select_row( "SELECT * from `port` WHERE uid=%s LIMIT 1" , [ uid ] )
+    if row == None : return( render_template( "error_500.html" ) )
 
-    return( _common.response_default( messages ) )
+    port_pin_rows = _database.db_query_select_rows( "SELECT * from `port_pin` WHERE port_id=%s" , [ row["id"]] )
 
-@ROUTES.route( "/model_specs" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_specs( ) :
+    for port_pin_row in port_pin_rows :
+        pin_row = _database.db_query_select_row( "SELECT * from `pin` WHERE id=%s LIMIT 1" , [ port_pin_row["pin_id"]] )
+        port_pin_row["[pin_name]"]=pin_row["name"]
+        port_pin_row["[pin_type]"]=pin_row["type"]
 
-    if not "name" in request.json : return( _common.response_error( e_msg = "not name"  ) )
+    columns = ["[pin_name]","[pin_type]","cardinal"]
 
     ####
 
-    rolemodel_enable = 0
-    if _config.DATA[ "server_security_lax" ] : rolemodel_enable = 1
 
-    ####
+    tdata = {
+        "row" : row ,
+        "rows" : port_pin_rows,
+        "columns" : columns
+    }
 
-    rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
+    return( render_template( "pages/ports/read.html" , tdata = tdata ) )
 
-    if rolemodel_row == None :
-        rolemodel_data = {
-            "api_id" : _g.api[ "id" ] ,
-            "name" : request.json[ "name" ] ,
-            "specs" : json.dumps( request.json ) ,
-            "category" : request.json.get( "category" ) ,
-            "description" : request.json.get( "desc" ) ,
-            "type" : request.json.get( "type" ) ,
-            "user_api_ip_prefix" : request.json.get( "user_api_ip_prefix" , "127.,192.168.,172.,10." ) ,
-            "user_api_email_postfix" : request.json.get( "user_api_email_postfix" , "sparc.gr,esa.int,aeronomie.be" ) ,
-            "input_size_max" : request.json.get( "input_size_max" , 10485760 ) ,
-            "ignore_pred_fail" : request.json.get( "ignore_pred_fail" ) ,
-            "enable" : rolemodel_enable
-        }
-        try :
-            rolemodel_id = _database.insert_fromdict( "rolemodel" , rolemodel_data )
-        except Exception as e :
-            return( _common.response_error( e_msg = f"verify specs {e}"  ) )
-    else :
-        if rolemodel_row[ "updateable" ] == 0 :
-            if not _config.DATA[ "server_security_lax" ]  :
-                return( _common.response_error( e_msg = "not updateable"  ) )
-        if json.loads( rolemodel_row[ "specs" ] ) == request.json : return( _common.response_default( ) )
-        rolemodel_id = rolemodel_row[ "id" ]
-        rolemodel_data = {
-            "name" : request.json[ "name" ] ,
-            "specs" : json.dumps( request.json ) ,
-            "category" : request.json.get( "category" ) ,
-            "description" : request.json.get( "desc" ) ,
-            "type" : request.json.get( "type" ) ,
-            "user_api_ip_prefix" : request.json.get( "user_api_ip_prefix" , "127.,192.168.,172.,10." ) ,
-            "user_api_email_postfix" : request.json.get( "user_api_email_postfix" , "sparc.gr,esa.int,aeronomie.be" ) ,
-            "input_size_max" : request.json.get( "input_size_max" , 10485760 ) ,
-            "ignore_pred_fail" : request.json.get( "ignore_pred_fail" ) ,
-            "enable" : rolemodel_enable
-        }
-        _database.update_fromdict( "rolemodel" , rolemodel_id , rolemodel_data )
 
-    ####
+####
 
-    interfaces_global = request.json.get( "interfaces_global" , 0 ) == 1
+@ROUTES.route( "/pins" , methods = [ "GET" ] )
+def page_pins( ) :
 
-    # FIXEM TODO disabled - make sure to remove
-    interfaces_global = 0
 
+    rows = _database.db_query_select_rows( "SELECT * from `pin`" )
 
-    if interfaces_global == 0 :
-        _database.model_flush_ports( rolemodel_id ) 
-        # FIXME TODO is this required?
-        _database.db_query_delete( f"DELETE from `mport` WHERE rolemodel_id=%s" , [ rolemodel_id ] )    
+    columns = [ "uid" , "name" , "description" ]
 
+    tdata = {
+        "rows" : rows ,
+        "columns" : columns
+    }
 
+    return( render_template( "pages/pins/rows.html" , tdata = tdata ) )
 
-    if "ports" in request.json : _database.model_load_ports( rolemodel_id , request.json[ "ports" ] , interfaces_global = interfaces_global )
 
-    ####
 
-    if "inputs" in request.json :
-        for specs_io in request.json[ "inputs" ] :
-            if not "name" in specs_io : return( _common.response_error( e_msg = "not name in specs_input"  ) )
-            if _database.verify_portpinunit( specs_io ) == None :
-                return( _common.response_error( e_msg = f"verify {specs_io['name']}"  ) )
+@ROUTES.route( "/pins_read" , methods = [ "GET" ] )
+def page_pins_read( ) :
 
-    if "outputs" in request.json :
-        for specs_io in request.json[ "outputs" ] :
-            if not "name" in specs_io : return( _common.response_error( e_msg = "not name in specs_output"  ) )
-            if _database.verify_portpinunit( specs_io ) == None :
-                return( _common.response_error( e_msg = f"verify {specs_io['name']}"  ) )
+    id = _common.request_arg_str( "id" )
+
+    row = _database.db_query_select_row( "SELECT * from `pin` WHERE id=%s LIMIT 1" , [ id ] )
+    if row == None : return( render_template( "error_500.html" ) )
 
     ####
 
-    if "inputs" in request.json :
-        for specs_io in request.json[ "inputs" ] :
-            if _database.process_specs_io( specs_io , rolemodel_id , "inputs" ) == None :
-                return( _common.response_error( e_msg = f"process_specs_io inputs" ) )
+    tdata = {
+        "row" : row 
+    }
 
-    if "outputs" in request.json :
-        for specs_io in request.json[ "outputs" ] :
-            if _database.process_specs_io( specs_io , rolemodel_id , "outputs" ) == None :
-                return( _common.response_error( e_msg = f"process_specs_io outputs" ) )
+    return( render_template( "pages/pins/read.html" , tdata = tdata ) )
+####
 
-    ####
+@ROUTES.route( "/docs" , methods = [ "GET" ] )
+def page_docs( ) :
+    return( render_template( "page_docs.html" ) )
 
-    return( _common.response_default( ) )
 
+@ROUTES.route( "/login" , methods = [ "GET" ] )
+def page_login( ) :
+    return( render_template( "pages/login/main.html" ) )
 
+@ROUTES.route( "/logout" , methods = [ "GET" ] )
+def page_logout( ) :
+    session_key = request.cookies.get( "key" , "" ).strip( )
+    if len( session_key ) == 64 :
+        _database.db_query_delete( "DELETE FROM session WHERE `key`=%s LIMIT 1" , [ session_key ] )
+    return( render_template( "pages/logout/main.html" ) )
 
+@ROUTES.route( "/register" , methods = [ "GET" ] )
+def page_register( ) :
+    return( render_template( "pages/register/main.html" ) )
 
 
-@ROUTES.route( "/model_pipeline_failed" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_pipeline_failed( ) :
+@ROUTES.route( "/admin" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin( ) :
+    return( render_template( "/pages/admin/main.html" ) )
 
+@ROUTES.route( "/member" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( )
+def page_member( ) :
 
-    task_uid = _common.request_arg_str( "task_uid" )
-    exit_code = _common.request_arg_int( "exit_code" )
+    #session_data = _common.session_get( )
 
-    task_row = _database.db_query_select_row( "SELECT * from task WHERE uid=%s LIMIT 1" , [ task_uid ] )
+    #account_row = session_data.get("account_row")
+    #if not account_row : raise Exception( f"account_row None" )
 
-    if task_row[ "status" ] == "RUNNING" :
-        _database.update_fromdict( "task" , task_row[ "id" ] , { "status" : "FAILED" , "exit_code" : exit_code } )
+    #api_rows = _database.db_query_select_rows( "SELECT * from api WHERE account_id=%s LIMIT 1" , [ account_row["id"] ] )
 
+    #cols = ["name"]
 
-    return( _common.response_default( ) )
+    #tdata = {
+    #    "rows" : api_rows ,
+    #    "cols" : cols
+    #}
 
-@ROUTES.route( "/model_schedule" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-def model_schedule( ) :
 
-    rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if rolemodel_row == None : return( _common.response_error( e_msg = "rolemodel_row None" ) )
 
-    rolemodel_id = rolemodel_row[ "id" ]
 
-    _database.update_fromdict( "rolemodel" , rolemodel_id , { "heartbeat_at" : datetime.now( ) } )
+    return( render_template( "/pages/member/main.html" ) )
 
-    schedule_row = _database.db_query_select_row( "SELECT * from schedule WHERE rolemodel_id=%s LIMIT 1" , [ rolemodel_id ] )
+#####################################################################
 
-    messages = { }
+@ROUTES.route( "/admin_pipelines" , methods = [ "GET" ] )
+def page_admin_pipelines( ) :
 
-    if schedule_row != None : messages[ "schedule_data_json" ] = schedule_row[ "data" ] 
+    pipeline_rows = _database.db_query_select_rows( "SELECT * from pipeline ORDER by id DESC" )
 
-    return( _common.response_default( messages ) )
+    #print(pipeline_rows)
 
+    for pipeline_row in pipeline_rows :
+        pipeline_obj = _database.pipeline_object( pipeline_row )
+        #pipeline_obj.print_debug( )
+        pipeline_row[ "[nodes]" ] = pipeline_obj.nodes
 
-@ROUTES.route( "/model_claim_set" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_claim_set( ) :
 
-    task_uid = _common.request_arg_str( "task_uid" )
 
-    ####
+    cols = [ "uid" , "name" , "status" , "done" , "archived" , "[nodes]" ]
 
-    messages = {
-        "claim_uid" : "" ,
-        "claim_status" : "NO"
+    tdata = {
+        "rows" : pipeline_rows ,
+        "cols" : cols
     }
 
-    ####
 
-    # Another claim with status YES?
-    claim_row = _database.db_query_select_row( "SELECT * from claim WHERE task_uid=%s AND status=%s LIMIT 1" , [ task_uid , "YES" ] )
-    if claim_row != None : return( _common.response_default( messages ) )
+    return( render_template( "page_admin_pipelines.html" , tdata = tdata ) )
 
-    ####
 
-    row_data = { "task_uid" : task_uid }
-    claim_id = _database.insert_fromdict( "claim" , row_data )
-    if claim_id == None : return( _common.response_error( e_msg = "claim_id none"  ) )
+@ROUTES.route( "/dashboard_tasks" , methods = [ "GET" ] )
+def page_dashboard_tasks( ) :
 
-    ####
+    tdata = {
+    }
 
-    claim_row = _database.db_query_select_row( "SELECT * from claim WHERE id=%s LIMIT 1" , [ claim_id ] )
 
-    messages[ "claim_uid" ] = claim_row[ "uid" ]
-    messages[ "claim_status" ] = claim_row[ "status" ]
+    return( render_template( "page_dashboard_tasks.html" , tdata = tdata ) )
 
-    ####
 
-    return( _common.response_default( messages ) )
+#####################################################################
 
+@ROUTES.route( "/admin/db_rolemodel_rows" , methods = [ "GET" ] )
+def admin_db_rolemodel_rows( ) :
 
-@ROUTES.route( "/model_claim_release" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_claim_release( ) :
+    rolemodel_rows = _database.db_query_select_rows( "SELECT id,api_id,name,enable,updateable from rolemodel order by id" )
 
-    claim_uid = _common.request_arg_str( "claim_uid" )
-    _database.db_query_delete( "DELETE from claim WHERE uid=%s LIMIT 1;" , [ claim_uid ] )
+    print(rolemodel_rows)
 
-    return( _common.response_default( ) )
+    for rolemodel_row in rolemodel_rows :
 
-    ####
+        rolemodel_api_id = rolemodel_row[ "api_id" ]
+
+        if rolemodel_api_id == None : continue
 
+        api_row = _database.db_query_select_row( "SELECT * from api where id=%s LIMIT 1" , [ rolemodel_api_id ] )
+        api_name = api_row[ "name" ]
+        if api_name.startswith( "test_" ) : api_name = api_name[ -10: ]
+
+        rolemodel_row[ "[api_name]" ] = api_name
+        rolemodel_row[ "[api_enable]" ] = api_row[ "enable" ]
+
+    tdata = {
+        "rolemodel_rows" : rolemodel_rows
+    }
+    #print(tdata)
 
-@ROUTES.route( "/model_claim_get" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_claim_get( ) :
+    return( render_template( "db_rolemodel_rows.html" , tdata = tdata ) )
 
-    claim_uid = _common.request_arg_str( "claim_uid" )
+@ROUTES.route( "/admin/db_rolemodel_row" , methods = [ "GET" ] )
+def admin_db_rolemodel_row( ) :
+
+    rolemodel_id = _common.request_arg_int( "rolemodel_id" )
 
     ####
 
-    messages = {
-        "claim_status" : "NO" ,
-        "pipeline" : False
+    rolemodel_row = _database.db_query_select_row( "SELECT id,api_id,name,enable,updateable from rolemodel where id=%s" , [ rolemodel_id ] )
+
+    mport_rows = _database.db_query_select_rows( "SELECT id,port_id,direction,enable,cardinal from mport where rolemodel_id=%s order by id" , [ rolemodel_id ] )
+
+    mpins = [ ]
+    for mport_row in mport_rows :
+        port_row = _database.db_query_select_row( "SELECT * from port where id=%s LIMIT 1" , [ mport_row["port_id"]] )
+        port_name = port_row[ "name" ]
+        mport_row[ "[port_name]" ] = port_name
+
+        mpin_rows = _database.db_query_select_rows( "SELECT id,mport_id,unit_id from mpin where mport_id=%s order by id" , [ mport_row["id"] ] )
+
+        for mpin_row in mpin_rows :
+            unit_row = _database.db_query_select_row( "SELECT * from unit where id=%s LIMIT 1" , [ mpin_row["unit_id"]] )
+            pin_row = _database.db_query_select_row( "SELECT * from pin where id=%s LIMIT 1" , [ unit_row["pin_id"]] )
+            port_pin_row = _database.db_query_select_row( "SELECT * from port_pin where port_id=%s and pin_id=%s LIMIT 1" , [port_row[ "id" ] , pin_row[ "id" ] ] )
+            mpin_row[ "[direction]" ] = mport_row[ "direction" ]
+            mpin_row[ "[port_pin_cardinal]" ] = port_pin_row[ "cardinal" ]
+            mpin_row[ "[pin_id]" ] = pin_row[ "id" ]
+            mpin_row[ "[port_name/pin_name(unit_name)]" ] = port_row[ "name" ] + "/" + pin_row[ "name" ] + "(" + unit_row[ "name" ] + ")"
+
+
+        mpins.append( mpin_rows)
+
+
+    tdata = {
+        "rolemodel_row" : rolemodel_row ,
+        "mport_rows" : mport_rows ,
+        "mpins" : mpins
     }
 
-    ####
+    return( render_template( "db_rolemodel_row.html" , tdata = tdata ) )
 
-    claim_row = _database.db_query_select_row( "SELECT * from claim WHERE uid=%s LIMIT 1" , [ claim_uid ] )
-    if claim_row == None : return( _common.response_default( messages ) )
+####
 
-    ####
+@ROUTES.route( "/admin/db_pipeline_rows" , methods = [ "GET" ] )
+def admin_db_pipeline_rows( ) :
 
-    task_uid = claim_row[ "task_uid" ]
+    pipeline_rows = _database.db_query_select_rows( "SELECT id,roleuser_id,name,status,done,archived,created_at,updated_at from pipeline order by id DESC" )
 
-    ####
+    tdata = {
+        "pipeline_rows" : pipeline_rows
+    }
 
-    check_yes_claim_row = _database.db_query_select_row( "SELECT * from claim WHERE task_uid=%s AND status=%s LIMIT 1" , [ task_uid , "YES" ] )
-    # Make sure to check if the claim uid is not the input
-    another_yesclaim_exists = ( check_yes_claim_row != None ) and ( check_yes_claim_row[ "uid" ] != claim_uid )
-    if another_yesclaim_exists :
-        _database.db_query_delete( "DELETE from claim WHERE uid=%s LIMIT 1;" , [ claim_uid ] )
-        return( _common.response_default( messages ) )
+    return( render_template( "admin_db_pipeline_rows.html" , tdata = tdata ) )
 
-    ####
+@ROUTES.route( "/admin/db_pipeline_row" , methods = [ "GET" ] )
+def admin_db_pipeline_row( ) :
+    pipeline_id = _common.request_arg_int( "pipeline_id" )
+    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline where id=%s" , [pipeline_id] )
+
+    pipeline_object = _database.pipeline_object(pipeline_row)
+
+    tdata = {
+        "pipeline_row" : pipeline_row ,
+        "pipeline" : pipeline_object
+    }
+    pipeline_object.print_debug()
+    return( render_template( "admin_db_pipeline_row.html" , tdata = tdata ) )
 
-    if claim_row[ "status" ] == "WAIT" :
-        messages[ "claim_status" ] = claim_row[ "status" ]
-        return( _common.response_default( messages ) )
 
-    ####
+@ROUTES.route( "/admin_accounts" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_accounts( ) :
+
+    rows = _database.db_query_select_rows( "SELECT * from account order by email" )
+    columns = ["uid" , "email" , "name","enable","email_confirm_at","email_confirmed","email_confirmed_at"]
+
+    tdata = {
+        "time" : time.time( ) ,
+        "rows" : rows ,
+        "columns" : columns 
+    }
+
+    return( render_template( "pages/admin_accounts/main.html" , tdata = tdata ) )
+
+@ROUTES.route( "/admin_account_create" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_account_create( ) :
+
+
+    tdata = {
+        "time" : time.time( ) 
+    }
+
+    return( render_template( "pages/admin_account_create/main.html" , tdata = tdata ) )
+
+@ROUTES.route( "/admin_group_create" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_group_create( ) :
 
-    task_row = _database.db_query_select_row( "SELECT * from task WHERE uid=%s LIMIT 1" , [ task_uid ] )
 
-    # Check if task is scheduled
-    if task_row[ "status" ] != "SCHEDULED" :
-        _database.db_query_delete( "DELETE from claim WHERE uid=%s LIMIT 1;" , [ claim_uid ] )
-        return( _common.response_default( messages ) )
+    tdata = {
+        "time" : time.time( ) 
+    }
+
+    return( render_template( "pages/admin_group_create/main.html" , tdata = tdata ) )
+
+@ROUTES.route( "/hx_admin_group_create" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_group_create( ) :
+
+    form = request.form.to_dict( flat = False )
+    print(form)
+
+    error_msgs = [ ]
+
+    try : input_name = _common.request_form_str( form , "name" , 3 )
+    except Exception as e : error_msgs.append( f"{e}" )
+
+    try : input_enable = _common.request_form_checkbox_single( form , "enable" )
+    except Exception as e : error_msgs.append( f"{e}" )
 
     ####
+    id = False
+    if len( error_msgs ) == 0 :
+        try :
+            id = _database.insert_fromdict( "group" , { "name" : input_name , "enable" : input_enable } )
+        except Exception as e : error_msgs.append( f"{e}" )
 
-    rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if rolemodel_row == None : return( _common.response_error( e_msg = "rolemodel_row None" ) )
 
     ####
 
-    pipeline = _pipeline.Pipeline( )
+    tdata = {
+        "time" : time.time( ) ,
+        "error_msgs" : error_msgs ,
+        "id" : id
+    }
 
-    pipeline.task_uid = claim_row[ "task_uid" ]
+    response = make_response( render_template( "pages/admin_group_create/hx_form.html" , tdata = tdata ) )
 
-    pipeline.status = "RUNNING"
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_groups" )
 
-    pipeline.current_role_name = _g.api[ "role_name" ]
+    return( response )
 
-    pipeline.io_info[ "_" ] = _database.io_info( rolemodel_row[ "name" ] )
-    
-    pipeline.io_data = _database.io_data( task_row[ "id" ] )
 
-    pipeline.nodes = {
-        "_": {
-            "name" : "_" ,
-            "task_uid" : task_uid
-        }
-    }
+@ROUTES.route( "/hx_admin_account_create" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_account_create( ) :
+
+    form = request.form.to_dict( flat = False )
+    print(form)
 
-    #####
+    error_msgs = [ ]
 
-    _database.update_fromdict( "task" , task_row[ "id" ] , { "status" : "RUNNING" } )
+    try : account_email = _common.request_form_email( form , "account_email" )
+    except Exception as e : error_msgs.append( f"{e}" )
 
-    pipeline_task_row = _database.db_query_select_row( "SELECT * from pipeline_task WHERE task_id=%s OR next_task_id=%s LIMIT 1" , [ task_row[ "id" ] , task_row[ "id" ] ] )
-    if pipeline_task_row == None : return( _common.response_error( e_msg = "pipeline_task_row None" ) )
+    try : account_password = _common.request_form_str( form , "account_password" )
+    except Exception as e : error_msgs.append( f"{e}" )
+
+    try : account_name = _common.request_form_str( form , "account_name" , 3 )
+    except Exception as e : error_msgs.append( f"{e}" )
+
+    try : account_enable = _common.request_form_checkbox_single( form , "account_enable" )
+    except Exception as e : error_msgs.append( f"{e}" )
+
+    try : account_email_confirmed = _common.request_form_checkbox_single( form , "account_email_confirmed" )
+    except Exception as e : error_msgs.append( f"{e}" )
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE id=%s LIMIT 1" , [ pipeline_task_row["pipeline_id"] ] )
-    if pipeline_row == None : return( _common.response_error( e_msg = "pipeline_row None" ) )
 
-    # Is pipeline scheduled (first task to be running) or not running?
-    if pipeline_row[ "status" ] == "SCHEDULED" :
-        _database.update_fromdict( "pipeline" , pipeline_row[ "id" ] , { "status" : "RUNNING" } )
-    elif pipeline_row[ "status" ] != "RUNNING" :
-        _database.db_query_delete( "DELETE from claim WHERE uid=%s LIMIT 1;" , [ claim_uid ] )
-        return( _common.response_default( messages ) )
 
     ####
+    account_id = False
+    if len( error_msgs ) == 0 :
+        try :
+            account_id = _database.insert_fromdict( "account" , { "email" : account_email , "password" : account_password , "name" : account_name , "enable" : account_enable , "email_confirmed" : account_email_confirmed  })
+        except Exception as e : error_msgs.append( f"{e}" )
 
-    messages[ "pipeline" ] = _util.object_encode( pipeline )
-    messages[ "claim_status" ] = claim_row[ "status" ]
 
     ####
 
-    return( _common.response_default( messages ) )
+    tdata = {
+        "time" : time.time( ) ,
+        "error_msgs" : error_msgs ,
+        "account_id" : account_id
+    }
 
+    return( render_template( "pages/admin_account_create/hx_form.html" , tdata = tdata ) )
 
 
-@ROUTES.route( "/model_task_heartbeat" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_task_heartbeat( ) :
+@ROUTES.route( "/hx_dashboard_tasks_taskcount" , methods = [ "GET" ] )
+def hx_dashboard_tasks_taskcount( ) :
 
-    task_uid = _common.request_arg_str( "task_uid" )
+    task_rows = _database.db_query_select_rows( "SELECT * from task where done=%s" , [ 0 ] )
 
-    task_row = _database.db_query_select_row( "SELECT * from task WHERE uid=%s LIMIT 1" , [ task_uid ] )
+    tdata = {
+        "x" : datetime.now( ).isoformat( ) ,
+        "y" : len( task_rows )
+    }
+    return( render_template( "hx_dashboard_tasks_taskcount.html" , tdata = tdata ) )
 
-    if task_row[ "status" ] == "RUNNING" :
-        _database.update_fromdict( "task" , task_row[ "id" ] , { "heartbeat_at" : datetime.now( ) } )
 
-    pipeline_task_row = _database.db_query_select_row( "SELECT * from pipeline_task WHERE task_id=%s OR next_task_id=%s LIMIT 1" , [ task_row[ "id" ] , task_row[ "id" ] ] )
+@ROUTES.route( "/hx_login" , methods = [ "POST" ] )
+def hx_login( ) :
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE id=%s LIMIT 1" , [ pipeline_task_row[ "pipeline_id" ] ] )
+    form = request.form.to_dict( flat = False )
 
+    error_msgs = [ ]
 
-    messages = {
-        "pipeline_status" : pipeline_row["status"]
-    }
+    if "account_email" not in form : error_msgs.append( "email not found" )
+    if len( form[ "account_email" ] ) != 1 : error_msgs.append( "email count != 1" )
+    account_email = form[ "account_email" ][ 0 ].strip( )
+    if len( account_email ) < 5 : error_msgs.append( "email to short" )
+
+    if "account_password" not in form : error_msgs.append( "password not found" )
+    if len( form[ "account_password" ] ) != 1 : error_msgs.append( "password count != 1" )
+    account_password = form[ "account_password" ][ 0 ].strip( )
+    if len( account_password ) < 5 : error_msgs.append( "password to short" )
+
+    ####
+
+    account_row = { }
+    account_name = None
+    if len( error_msgs ) == 0 :
+        password = _util.hash_str( account_password )
+        account_row = _database.db_query_select_row( "SELECT * from account WHERE email=%s AND password=%s LIMIT 1" , [ account_email , password ] )
+        if account_row == None :
+            error_msgs.append( "An error occurred. Please try again later." )
+        else :
+            account_name = account_row[ "name" ]
+
+
+    session_data = { }
+    if len( error_msgs ) == 0 :
+        session_key = request.cookies.get( "key" , "" ).strip( )
+        if len( session_key ) == 64 :
+            _database.db_query_delete( "DELETE FROM session WHERE `key`=%s LIMIT 1" , [ session_key ] )
 
-    return( _common.response_default( messages ) )
+            remote_ip = request.headers.get( "X-Forwarded-For" )
+            if not remote_ip : remote_ip = request.remote_addr
 
+            session_data = {
+                "time" : time.time( ) ,
+                "ip" : remote_ip ,
+                "ua" : request.headers.get( "User-Agent" ) ,
+                "loggedin" : True ,
+                "account_row" : account_row
+            }
+            _database.insert_fromdict( "session" , { "key" : session_key , "data" : json.dumps( session_data , default = str ) })
 
-@ROUTES.route( "/model_ioblock" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-def model_ioblock( ) :  
+    ####
 
-    io_uid = _common.request_arg_str( "io_uid" ) 
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
+    tdata = {
+        "k1" : time.time( ) ,
+        "error_msgs" : error_msgs ,
+        "account_name" : account_name
+    }
 
-    ioblock_block = _common.request_arg_int( "ioblock_block" )
-    if ioblock_block == None : return( _common.response_error( e_msg = "ioblock_block bad" ) )
+    response = make_response( render_template( "pages/login/hx_login.html" , tdata = tdata ) )
 
     ####
 
-    io_row = _database.db_query_select_row( "SELECT * from io WHERE uid=%s LIMIT 1" , [ io_uid ] )
-    if io_row == None : _common.response_error( e_msg = f"io_row not found" )
-    io_id = io_row[ "id" ]
+    if session_data.get( "loggedin" , False ) :
 
-    ioblock_row = _database.db_query_select_row( "SELECT * from ioblock WHERE io_id=%s AND block=%s LIMIT 1" , [ io_id , ioblock_block ] )
-    if ioblock_row == None : _common.response_error( e_msg = f"ioblock_row not found" )
+        if account_name == "_admin" :
+            url_redirect = url_for( ".page_admin" )
+        else :
+            url_redirect = url_for( ".page_member" )
 
-    #print(ioblock_row)
+        response.headers[ "HX-Redirect" ] = url_redirect
+
+    ####
+
+    return( response )
 
-    io_hash_filepath = _util.get_io_hash_filepath( ioblock_row[ "hash" ] )
- 
-    #print( io_hash_filepath )
 
-    return( send_file( io_hash_filepath ) )
+@ROUTES.route( "/hx_register" , methods = [ "POST" ] )
+def hx_register( ) :
 
+    form = request.form.to_dict( flat = False )
 
-@ROUTES.route( "/model_ioblock_status" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-def model_ioblock_status( ) :
+    error_msgs = [ ]
 
-    io_uid = _common.request_arg_str( "io_uid" )
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
+    try : account_email = _common.request_form_str( form , "account_email" )
+    except Exception as e : error_msgs.append( f"{e}" )
 
-    io_row = _database.db_query_select_row( "SELECT * from io WHERE uid=%s LIMIT 1" , [ io_uid ] )
-    if io_row == None : return( _common.response_error( e_msg = "io_row none" ) )
-    io_id = io_row["id"]
+    if not _util.email_check( account_email ) :
+        error_msgs.append( "Invalid email address" )
+
+    ####
 
-    ioblock_row = _database.db_query_select_row( "SELECT * from ioblock WHERE io_id=%s order by block DESC LIMIT 1" , [io_id ] )
-    if ioblock_row == None :
-        block_current = 0
-    else :
-        block_current = ioblock_row[ "block" ] + 1
+    #if len( error_msgs ) == 0 :
+    #    password = _util.hash_str( account_password )
+    #    account_row = _database.db_query_select_row( "SELECT * from account WHERE email=%s LIMIT 1" , [ account_email ] )
 
-    messages = {
-        "blocks_total" : io_row[ "blocks" ] ,
-        "blocks_current" : block_current
+    tdata = {
+        "k1" : time.time( ) ,
+        "error_msgs" : error_msgs 
     }
+    return( render_template( "hx_register.html" , tdata = tdata ) )
 
-    return( _common.response_default( messages ) )
+@ROUTES.route( "/hx_admin_account" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_account( ) :
 
+    account_uid = _common.request_arg_str( "account_uid" )
+    if account_uid == "" : raise Exception( f"account_uid blank" )
 
+    account_row = _database.db_query_select_row( "SELECT * from account WHERE uid=%s LIMIT 1" , [ account_uid ] )
+    if account_row is None : raise Exception( f"account_row None" )
 
-@ROUTES.route( "/model_ioblock_upload_block" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-#@_common.decorator_request_json
-def model_ioblock_upload_block( ) :
+    api_rows = _database.db_query_select_rows( "SELECT * from api WHERE account_id=%s" , [ account_row["id"] ] )
 
-    io_uid = _common.request_arg_str( "io_uid" )
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
+    columns = ["uid","name","enable"]
 
-    # FIXME TODO check all incoming parameters before doing db queries?
-    io_row = _database.db_query_select_row( "SELECT * from io WHERE uid=%s LIMIT 1" , [ io_uid ] )
-    if io_row == None : return( _common.response_error( e_msg = "io_row none" ) )
-    io_id = io_row[ "id" ]
+    tdata = {
+        "k1" : time.time( ) ,
+        "account_row" : account_row ,
+        "rows" : api_rows ,
+        "columns" : columns
+    }
 
-    block_str = request.args.get( "block" , default = "" ) 
-    if not block_str.isdigit( ): return( _common.response_error( e_msg = "block_str not isdigit" ) )
-    block = int( float( block_str ) )
+    #print(tdata)
 
-    file_hash = _common.request_arg_str( "hash" )
-    if file_hash == "" : return( _common.response_error( e_msg = "file_hash blank" ) )
+    return( render_template( "pages/admin/hx_admin_account.html" , tdata = tdata ) )
 
-    file_compressor = _common.request_arg_str( "compressor" )
-    if file_compressor == "" : return( _common.response_error( e_msg = "file_compressor blank" ) )
 
-    #print(request.data)
+@ROUTES.route( "/member_apis" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( )
+def page_member_apis( ) :
 
-    request_data_hash = _util.filedata_hash( request.data )
-    if request_data_hash != file_hash: return( _common.response_error( e_msg = "hash mismatch" ) )
+    session_data = _common.session_get( )
 
-    file_path = _util.get_io_hash_filepath( file_hash )
+    account_row = session_data.get("account_row")
+    if not account_row : raise Exception( f"account_row None" )
 
-    # FIXME TODO what if another process is doing the same file write? Do write then move?
-    if not os.path.isfile( file_path ) : 
-        with open( file_path , "wb" ) as f : f.write( request.data )
+    api_rows = _database.db_query_select_rows( "SELECT * from `api` where `account_id`=%s ORDER by `name`",[account_row["id"]] )
 
-    ioblock_row = {
-        "io_id" : io_id ,
-        "block" : block ,
-        "size" : len(request.data),
-        "hash" : file_hash ,
-        "compressor" : file_compressor
-    }
+    for api_row in api_rows :
+        api_role_row = _database.db_query_select_row( "SELECT * from `api_role` WHERE api_id=%s LIMIT 1" , [api_row["id"]])
+        role_row = _database.db_query_select_row( "SELECT * from `role` WHERE id=%s LIMIT 1" , [api_role_row["role_id"]])
+        api_row["[role_name]"]=role_row["name"]
+
+    columns = ["uid","[role_name]","name","token","enable"]
 
-    _database.insert_fromdict( "ioblock" , ioblock_row )
-    if id == None : return( _common.response_error( e_msg = "id none"  ) )
+    flag_apimax = len( api_rows ) >= account_row[ "api_max" ]
 
-    return( _common.response_default( ) )
+    tdata = {
+        "k1" : time.time( ) ,
+        "rows" : api_rows ,
+        "columns" : columns ,
+        "flag_apimax" : flag_apimax
+    }
+
+    #print(tdata)
 
+    return( render_template( "pages/member_apis/main.html" , tdata = tdata ) )
 
 
-@ROUTES.route( "/model_pipeline_submit_io" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_pipeline_submit_io( ) :    
+@ROUTES.route( "/admin_models" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_models( ) :
 
-    task_uid = _common.request_arg_str( "task_uid" )
-    if task_uid == "" : return( _common.response_error( e_msg = "task_uid blank" ) )
+    rows = _database.db_query_select_rows( "SELECT * from `rolemodel`" )
 
-    #print(request.json)
+    columns = [ "id" , "name" , "category" , "enable" , "updateable" ]
 
-    messages = {
-        "io_uid" : _database.io_insert( task_uid , request.json )
+    tdata = {
+        "k1" : time.time( ) ,
+        "rows" : rows ,
+        "columns" : columns
     }
 
-    return( _common.response_default( messages ) )
+    #print(tdata)
 
+    return( render_template( "pages/admin_models/main.html" , tdata = tdata ) )
 
-@ROUTES.route( "/model_pipeline_submit" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "model" )
-@_common.decorator_request_json
-def model_pipeline_submit( ) :    
+@ROUTES.route( "/admin_model_read" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_model_read( ) :
 
-    task_uid = _common.request_arg_str( "task_uid" )
-    if task_uid == "" : return( _common.response_error( e_msg = "task_uid blank" ) )
+    id = _common.request_arg_str( "id" )
 
-    task_row = _database.db_query_select_row( "SELECT * from task WHERE uid=%s AND status=%s LIMIT 1" , [ task_uid , "RUNNING" ] )
-    if task_row == None : _common.response_error( e_msg = f"task_row not found" )
+    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE id=%s LIMIT 1" , [id])
+    if row is None : raise Exception( f"row None" )
 
-    _database.update_fromdict( "task" , task_row[ "id" ] , { "status" : "COMPLETED" , "status_code" : 0 } )
+    tdata = {
+        "row" : row 
+    }
 
-    return( _common.response_default( ) )
+    #print(tdata)
 
-#####################################################################
+    return( render_template( "pages/admin_model_read/main.html" , tdata = tdata ) )
 
-@ROUTES.route( "/user_state" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-def user_state( ) :
 
-    messages = { }
+@ROUTES.route( "/admin_model_update" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_model_update( ) :
 
-    messages[ "model" ] = _database.user_state_model( api_id = _g.api[ "id" ] )
-    messages[ "group" ] = _database.user_state_group( api_id = _g.api[ "id" ] )
-    messages[ "pipeline" ] = _database.user_state_pipeline( api_id = _g.api[ "id" ] )
+    id = _common.request_arg_str( "id" )
 
-    return( _common.response_default( messages ) )
+    row = _database.db_query_select_row( "SELECT * from `rolemodel` WHERE id=%s LIMIT 1" , [id])
+    if row is None : raise Exception( f"row None" )
 
+    tdata = {
+        "k1" : time.time( ) ,
+        "row" : row 
+    }
 
-@ROUTES.route( "/user_pipeline" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline( ) :
+    #print(tdata)
 
-    name = _common.request_arg_str( "name" )
-    if name == "" : return( _common.response_error( e_msg = "name blank" ) )
+    return( render_template( "pages/admin_model_update/main.html" , tdata = tdata ) )
 
-    ####
 
-    pipeline_row = _database.user_pipeline( _g.api[ "id" ] , name )
+@ROUTES.route( "/hx_admin_model_update" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_model_update( ) :
+
+    id = _common.request_arg_int( "id" )
+
+    # FIXME TODO check if id is available and allowed
+    #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
+    #if row is None : raise Exception( f"row None" )
 
     ####
 
-    pipeline = _pipeline.Pipeline( name )
-    pipeline.current_role_name = _g.api[ "role_name" ]
-    pipeline.status = pipeline_row[ "status" ]
-    pipeline.done = pipeline_row[ "done" ]
-    
+    form = request.form.to_dict( flat = False )
+    print(form)
+
     ####
+    row_data = { }
+
+    for i , ( k , v ) in enumerate( form.items( ) ) :
+        if k.startswith("[") : continue
+        row_data[k]=v[0]
+
 
-    for model_name in _database.user_state_model( api_id = _g.api[ "id" ] ) :
-        pipeline.io_info[ model_name ] = _database.io_info( model_name )
+    if "enable" not in row_data : row_data["enable"]=0
+    if "updateable" not in row_data : row_data["updateable"]=0
 
+    print(row_data)
+
+    _database.update_fromdict( "rolemodel" , id , row_data )
     ####
 
-    if( pipeline_row[ "status" ] != "RESERVED" ) :
+    tdata = {
+        "k1" : time.time( ) 
+    }
+
+    #print(tdata)
 
-        pipeline.nodes = _database.pipeline_nodes( pipeline_row[ "id" ] )
+    response = make_response( render_template( "pages/admin_model_update/hx_form.html" , tdata = tdata ) )
 
-        for i , ( k , v ) in enumerate( pipeline.nodes.items( ) ) :
-            pipeline.io_data.update( _database.io_data_from_taskuid( v[ "task_uid" ] ) )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_model_read" , id=id)
 
     ####
 
-    messages = { }
+    return( response )
 
-    messages[ "pipeline" ] = _util.object_encode( pipeline )
 
-    return( _common.response_default( messages ) )
+@ROUTES.route( "/admin_apis" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_apis( ) :
 
+    api_rows = _database.db_query_select_rows( "SELECT * from `api`" )
 
-@ROUTES.route( "/user_pipeline_submit_reserve" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline_submit_reserve( ) :
+    for api_row in api_rows :
+        account_row = _database.db_query_select_row( "SELECT * from `account` WHERE id=%s LIMIT 1" , [api_row["account_id"]])
+        api_row["[account_email]"]=account_row["email"]
+        api_row["[account_name]"]=account_row["name"]
+        api_role_row = _database.db_query_select_row( "SELECT * from `api_role` WHERE api_id=%s LIMIT 1" , [api_row["id"]])
+        role_row = _database.db_query_select_row( "SELECT * from `role` WHERE id=%s LIMIT 1" , [api_role_row["role_id"]])
+        api_row["[role_name]"]=role_row["name"]
 
+    columns = [ "uid" , "[account_email]" ,"[account_name]", "[role_name]" , "name" , "token" , "enable" , "ip" , "ip_update" ]
 
-    name = _common.request_arg_str( "name" ).strip( )
-    if name == "" : return( _common.response_error( e_msg = "name blank" ) )
+    tdata = {
+        "k1" : time.time( ) ,
+        "rows" : api_rows ,
+        "columns" : columns
+    }
 
-    ####
+    #print(tdata)
 
-    roleuser = _database.db_query_select_row( "SELECT id from roleuser WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if roleuser == None : return( _common.response_error( e_msg = "roleuser" ) )
+    return( render_template( "pages/admin_apis/main.html" , tdata = tdata ) )
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE roleuser_id=%s AND name=%s AND status=%s AND archived=0 LIMIT 1" , [ roleuser[ "id" ] , name , "RESERVED" ] )
-    if pipeline_row == None : return( _common.response_error( e_msg = f"Pipeline [{name}] RESERVED not found. Already submitted?" ) )
 
-    ####
+@ROUTES.route( "/admin_groups" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_groups( ) :
 
-    nodes = request.json.get( "nodes" , None )
-    if nodes == None : return( _common.response_error( e_msg = f"No nodes" ) )
-    if not isinstance( nodes , dict ) : return( _common.response_error( e_msg = f"nodes not dict" ) )
-    nodes_keys = list( nodes.keys( ) )
-    if len( nodes_keys ) == 0 :
-        messages = {
-            "pipeline_uid" : pipeline_row[ "uid" ] ,
-            "task_uids" : [ ]
-        }
-        return( _common.response_default( messages ) )
+    rows = _database.db_query_select_rows( "SELECT * from `group`" )
+    columns = [ "id" , "name" , "enable" ]
 
-    ####
+    tdata = {
+        "k1" : time.time( ) ,
+        "rows" : rows ,
+        "columns" : columns
+    }
 
-    # FIXME TODO creating pipeline and tasks should be in a transaction!
+    #print(tdata)
 
-    task_ids = { }
+    return( render_template( "pages/admin_groups/main.html" , tdata = tdata ) )
 
-    for i , ( k , v ) in enumerate( nodes.items( ) ) :
-        model_name = v[ "name" ]
-        rolemodel_row = _database.db_query_select_row( "SELECT * from rolemodel WHERE name=%s LIMIT 1" , [ model_name ] )
-        if rolemodel_row == None : _common.response_error( e_msg = f"[{model_name}] not found" )
-        task_row = { "rolemodel_id" : rolemodel_row[ "id" ] , "rolemodel_name_alt" : k }
-        task_id = _database.insert_fromdict( "task" , task_row )
-        if task_id == None : return( _common.response_error( e_msg = "task insert" ) )
-        task_ids[ k ] = task_id 
+@ROUTES.route( "/admin_group_read" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_group_read( ) :
 
-    #_util.debug_json_print( task_ids , "task_ids" )
-    
-    ###
+    id = _common.request_arg_str( "id" )
 
-    edges = request.json.get( "edges" , None )
+    row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
+    if row is None : raise Exception( f"api_row None" )
 
-    pipeline_obj = _pipeline.Pipeline( edges_in = request.json[ "edges" ] )
+    tdata = {
+        "k1" : time.time( ) ,
+        "row" : row 
+    }
 
-    if not pipeline_obj.is_valid( ) : return( _common.response_error( e_msg = "bad dag" ) )
+    #print(tdata)
 
-    edge_order = copy.deepcopy( pipeline_obj.topological_sort_edges( ) )
+    return( render_template( "pages/admin_group_read/main.html" , tdata = tdata ) )
 
-    graph_nodes = pipeline_obj.get_node_graph_names( )
-    #print(graph_nodes)
-    for node in nodes_keys :
-        if not node in graph_nodes :
-            edge_order.append( [ node , None ] )
 
-    #_util.debug_json_print( edge_order , "edge_order" )
+@ROUTES.route( "/admin_api_read" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_api_read( ) :
 
-    ###
+    api_uid = _common.request_arg_str( "api_uid" )
 
-    for edges in edge_order :
-        pipeline_task_row = {
-            "pipeline_id" : pipeline_row[ "id" ] ,
-            "task_id" : task_ids.get( edges[ 0 ] , None ) ,
-            "next_task_id" : task_ids.get( edges[ 1 ] , None )
-        }
-        pipeline_task_id = _database.insert_fromdict( "pipeline_task" , pipeline_task_row )
-        if pipeline_task_id == None : return( _common.response_error( e_msg = "pipeline_task insert" ) )
+    api_row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [api_uid])
 
-    ####
+    if api_row is None : raise Exception( f"api_row None" )
 
-    task_uids = { }
 
-    for i , ( k , v ) in enumerate( task_ids.items( ) ) :
-        task_row = _database.db_query_select_row( "SELECT * from task WHERE id=%s LIMIT 1" , [ v ] )
-        if task_row == None : _common.response_error( e_msg = f"task_row [{v}] not found" )
-        task_uids[ k ] = task_row[ "uid" ]
 
-    ####
+    api_row["[group_names]"]=[]
+    api_group_rows = _database.db_query_select_rows( "SELECT * from `api_group` WHERE api_id=%s" , [api_row['id']])
+
+    print(f"{api_group_rows=}")
+
+    for api_group_row in api_group_rows :
+        group_row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [api_group_row['group_id']])
+        api_row["[group_names]"].append(group_row["name"])
+
 
-    messages = {
-        "pipeline_uid" : pipeline_row[ "uid" ] ,
-        "task_uids" : task_uids
+    tdata = {
+        "k1" : time.time( ) ,
+        "row" : api_row 
     }
 
-    return( _common.response_default( messages ) )
+    #print(tdata)
 
-@ROUTES.route( "/user_pipeline_submit_io" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline_submit_io( ) :
+    return( render_template( "pages/admin_api_read/main.html" , tdata = tdata ) )
 
-    task_uid = _common.request_arg_str( "task_uid" )
-    if task_uid == "" : return( _common.response_error( e_msg = "task_uid blank" ) )
 
+@ROUTES.route( "/admin_api_update" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_api_update( ) :
 
-    is_local = request.remote_addr == "127.0.0.1"
+    api_uid = _common.request_arg_str( "api_uid" )
+
+    api_row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [api_uid])
+
+    if api_row is None : raise Exception( f"api_row None" )
+
+    api_row["[group_names]"]=[]
+    api_group_rows = _database.db_query_select_rows( "SELECT * from `api_group` WHERE api_id=%s" , [api_row['id']])
+
+    for api_group_row in api_group_rows :
+        group_row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [api_group_row['group_id']])
+        api_row["[group_names]"].append(group_row["name"])
 
-    messages = {
-        "io_uid" : _database.io_insert( task_uid , request.json , is_local = is_local )
-    }
 
-    return( _common.response_default( messages ) )
+    group_rows = _database.db_query_select_rows( "SELECT * from `group`" )
 
+    tdata = {
+        "k1" : time.time( ) ,
+        "row" : api_row ,
+        "group_rows" : group_rows
+    }
 
-@ROUTES.route( "/user_ioblock_status" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-def user_ioblock_status( ) :
+    #print(tdata)
 
-    io_uid = _common.request_arg_str( "io_uid" )
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
+    return( render_template( "pages/admin_api_update/main.html" , tdata = tdata ) )
 
-    messages = _database.io_block_status( io_uid )
+@ROUTES.route( "/admin_group_update" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( "_admin" )
+def page_admin_group_update( ) :
 
-    return( _common.response_default( messages ) )
+    id = _common.request_arg_str( "id" )
 
+    row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
+    if row is None : raise Exception( f"api_row None" )
 
-@ROUTES.route( "/user_ioblock_upload_block" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-def user_ioblock_upload_block( ) :
+    tdata = {
+        "k1" : time.time( ) ,
+        "row" : row 
+    }
 
-    io_uid = _common.request_arg_str( "io_uid" )
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
+    #print(tdata)
 
-    io_row = _database.db_query_select_row( "SELECT * from io WHERE uid=%s LIMIT 1" , [ io_uid ] )
-    if io_row == None : return( _common.response_error( e_msg = "io_row none" ) )
+    return( render_template( "pages/admin_group_update/main.html" , tdata = tdata ) )
 
-    block = _common.request_arg_int( "block" )
 
-    if block >= io_row[ "blocks" ] : return( _common.response_error( e_msg = "block out of range" ) )
+@ROUTES.route( "/hx_admin_group_update" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_group_update( ) :
 
-    file_hash = _common.request_arg_str( "hash" )
-    if file_hash == "" : return( _common.response_error( e_msg = "file_hash blank" ) )
+    id = _common.request_arg_int( "id" )
 
-    file_compressor = _common.request_arg_str( "compressor" )
-    if file_compressor == "" : return( _common.response_error( e_msg = "file_compressor blank" ) )
+    # FIXME TODO check if id is available and allowed
+    #row = _database.db_query_select_row( "SELECT * from `group` WHERE id=%s LIMIT 1" , [id])
+    #if row is None : raise Exception( f"row None" )
 
-    request_data_hash = _util.filedata_hash( request.data )
-    if request_data_hash != file_hash: return( _common.response_error( e_msg = "hash mismatch" ) )
 
     ####
 
-    file_path = _util.get_io_hash_filepath( file_hash )
+    form = request.form.to_dict( flat = False )
+    print(form)
+
+    ####
+    row_data = { }
 
-    file_path_tmp = file_path + ".tmp"
+    for i , ( k , v ) in enumerate( form.items( ) ) :
+        if k.startswith("[") : continue
+        row_data[k]=v[0]
 
-    print(f"{file_path=}")
+    if "enable" not in row_data : row_data["enable"]=0
 
-    # FIXME TODO the tmp file should not exist...?
-    if not os.path.isfile( file_path_tmp ) : 
-        print(f"{file_path_tmp=}")
-        with open( file_path_tmp , "wb" ) as f : f.write( request.data )
-        os.rename( file_path_tmp , file_path )
+    print(row_data)
 
+    _database.update_fromdict( "group" , id , row_data )
     ####
 
-    ioblock_row = {
-        "io_id" : io_row[ "id" ] ,
-        "block" : block ,
-        "size" : len( request.data ) ,
-        "hash" : file_hash ,
-        "compressor" : file_compressor
+    tdata = {
+        "k1" : time.time( ) 
     }
 
-    _database.insert_fromdict( "ioblock" , ioblock_row )
-    if id == None : return( _common.response_error( e_msg = "id none"  ) )
+    #print(tdata)
+
+    response = make_response( render_template( "pages/admin_group_update/hx_form.html" , tdata = tdata ) )
 
-    return( _common.response_default( ) )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_group_read" , id=id)
 
-@ROUTES.route( "/user_pipeline_submit" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline_submit( ) :
+    ####
 
-    name = _common.request_arg_str( "name" ).strip( )
-    if name == "" : return( _common.response_error( e_msg = "name blank" ) )
+    return( response )
 
-    roleuser_row = _database.db_query_select_row( "SELECT id from roleuser WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if roleuser_row == None : return( _common.response_error( e_msg = "roleuser_row" ) )
+@ROUTES.route( "/hx_admin_api_update" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( "_admin" )
+def hx_admin_api_update( ) :
+
+    api_uid = _common.request_arg_str( "api_uid" )
+
+    api_row = _database.db_query_select_row( "SELECT * from `api` WHERE uid=%s LIMIT 1" , [api_uid])
+    if api_row is None : raise Exception( f"api_row None" )
+
+    api_id = api_row[ "id" ]
+
+    ####
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE roleuser_id=%s AND name=%s AND status=%s AND archived=0 LIMIT 1" , [ roleuser_row[ "id" ] , name , "RESERVED" ] )
-    if pipeline_row == None : return( _common.response_error( e_msg = f"Pipeline [{name}] not found" ) )
+    form = request.form.to_dict( flat = False )
+    print(form)
 
+    ####
+    row_data = { }
 
-    pipeline_task_rows = _database.db_query_select_rows( "SELECT * from pipeline_task WHERE pipeline_id=%s" , [ pipeline_row[ "id" ] ] )
-    if pipeline_task_rows == None : return( _common.response_error( e_msg = "pipeline_task_rows" ) )
+    for i , ( k , v ) in enumerate( form.items( ) ) :
+        if k.startswith("[") : continue
+        row_data[k]=v[0]
 
+    if "ip_update" not in row_data : row_data["ip_update"]=0
+    if "enable" not in row_data : row_data["enable"]=0
 
-    task_ids = set( )
-    for pipeline_task_row in pipeline_task_rows :
-        task_ids.update( [ pipeline_task_row[ "task_id" ] ] )
-        if pipeline_task_row[ "next_task_id" ] != None :
-            task_ids.update( [ pipeline_task_row[ "next_task_id" ] ] )
+    print(row_data)
 
+    _database.update_fromdict( "api" , api_uid , row_data , cid = "uid")
     ####
 
-    if len( task_ids ) == 0 :
-        _database.update_fromdict( "pipeline" , pipeline_row[ "id" ] , { "status" : "COMPLETED" } )
-        return( _common.response_default( ) )
+    incoming_group_ids = [ ]
+    if "[group_ids]" in form : incoming_group_ids = form["[group_ids]"]
+    incoming_group_ids = list(map(int, incoming_group_ids))
+
+    print(incoming_group_ids)
+    api_group_rows = _database.db_query_select_rows( "SELECT * from `api_group` WHERE api_id=%s" , [ api_id ] )
+
+    current_group_ids = [ ]
+    for api_group_row in api_group_rows : current_group_ids.append( api_group_row[ "group_id" ] )
+
+    print(current_group_ids)
+
+    for current_group_id in current_group_ids :
+        if current_group_id not in incoming_group_ids :
+            _database.db_query_delete( "DELETE FROM api_group WHERE `group_id`=%s AND api_id=%s LIMIT 1" , [ current_group_id , api_id ] )
+
+    for incoming_group_id in incoming_group_ids :
+        if incoming_group_id not in current_group_ids :
+            _database.insert_fromdict( "api_group" , { "api_id" : api_id , "group_id" : incoming_group_id } )
+
+
+
 
     ####
 
-    for task_id in task_ids :
+    tdata = {
+        "k1" : time.time( ) 
+    }
+
+    #print(tdata)
 
-        task_row = _database.db_query_select_row( "SELECT * from task WHERE id=%s AND status=%s LIMIT 1" , [ task_id , "RESERVED" ] )
-        if task_row == None : return( _common.response_error( e_msg = f"task_row not found" ) )
-        #print(task_row)
+    response = make_response( render_template( "pages/admin_api_update/hx_form.html" , tdata = tdata ) )
 
-        _database.update_fromdict( "task" , task_row[ "id" ] , { "status" : "SUBMITTED" } )
+    response.headers[ "HX-Redirect" ] = url_for( ".page_admin_api_read" , api_uid=api_uid)
 
     ####
 
-    _database.update_fromdict( "pipeline" , pipeline_row[ "id" ] , { "status" : "SUBMITTED" } )
+    return( response )
 
-    return( _common.response_default( ) )
 
-@ROUTES.route( "/user_pipeline_archive" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline_archive( ) :
 
-    name = _common.request_arg_str( "name" )
-    if name == "" : return( _common.response_error( e_msg = "name blank" ) )
+@ROUTES.route( "/member_api_create" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( )
+def page_member_api_create( ) :
+    return( render_template( "pages/member_api_create/main.html" ) )
 
-    roleuser_row = _database.db_query_select_row( "SELECT id from roleuser WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if roleuser_row == None : return( _common.response_error( e_msg = "roleuser_row" ) )
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE roleuser_id=%s AND name=%s AND archived=0 LIMIT 1" , [ roleuser_row[ "id" ] , name ] )
-    if pipeline_row == None : return( _common.response_error( e_msg = "pipeline_row" ) )
+@ROUTES.route( "/hx_member_api_create" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( )
+def hx_member_api_create( ) :
 
-    if pipeline_row[ "done" ] == 0 : return( _common.response_error( e_msg = "pipeline_row not done" ) )
-    if pipeline_row[ "archived" ] != 0 : return( _common.response_error( e_msg = "pipeline_row already archived" ) )
+    form = request.form.to_dict( flat = False )
+    print(form)
 
-    #print( pipeline_row )
+    error_msgs = [ ]
 
-    _database.update_fromdict( "pipeline" , pipeline_row[ "id" ] , { "archived" : 1 } )
+    try : api_name = _common.request_form_str( form , "api_name" , 1 )
+    except Exception as e : error_msgs.append( f"{e}" )
 
-    return( _common.response_default( ) )
+    try : role_name = _common.request_form_str( form , "role_name" , 1 )
+    except Exception as e : error_msgs.append( f"{e}" )
 
+    #print(f"{api_name=} {role_name=}")
 
-@ROUTES.route( "/user_pipeline_cancel" , methods = [ "POST" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-@_common.decorator_request_json
-def user_pipeline_cancel( ) :
+    if role_name not in ["user","model"] : error_msgs.append( f"role error" )
 
-    name = _common.request_arg_str( "name" )
-    if name == "" : return( _common.response_error( e_msg = "name blank" ) )
+    role_row = _database.db_query_select_row( "SELECT * from `role` where `name`=%s" , [role_name] )
+    if role_row is None : error_msgs.append( f"role_row None" )
 
-    roleuser_row = _database.db_query_select_row( "SELECT id from roleuser WHERE api_id=%s LIMIT 1" , [ _g.api[ "id" ] ] )
-    if roleuser_row == None : return( _common.response_error( e_msg = "roleuser_row" ) )
+    api_row = None
+    if len( error_msgs ) == 0 : 
 
-    pipeline_row = _database.db_query_select_row( "SELECT * from pipeline WHERE roleuser_id=%s AND name=%s AND archived=0 LIMIT 1" , [ roleuser_row[ "id" ] , name ] )
-    if pipeline_row == None : return( _common.response_error( e_msg = "pipeline_row" ) )
+        session_data = _common.session_get( )
 
-    if pipeline_row[ "archived" ] != 0 : return( _common.response_error( e_msg = "pipeline_row already archived" ) )
+        account_row = session_data.get("account_row")
+        if not account_row : raise Exception( f"account_row None" )
 
-    #print( pipeline_row )
+        api_id = _database.insert_fromdict( "api" , { "account_id" : account_row["id"] , "name" : api_name , "ip":_common.request_ip()} )
 
-    _database.update_fromdict( "pipeline" , pipeline_row[ "id" ] , { "status" : "CANCELLED" } )
+        api_role_id = _database.insert_fromdict( "api_role" , { "api_id" : api_id , "role_id":role_row["id"]} )
 
-    ####
-    pipeline_task_rows = _database.db_query_select_rows( "SELECT * from pipeline_task WHERE pipeline_id=%s" , [ pipeline_row[ "id" ] ] )
+        if role_name=="user" : 
+            roleuser_id = _database.insert_fromdict( "roleuser" , { "api_id" : api_id } )
 
-    task_ids = set( )
-    for pipeline_task_row in pipeline_task_rows :
-        task_ids.update( [ pipeline_task_row[ "task_id" ] ] )
-        if pipeline_task_row[ "next_task_id" ] != None :
-            task_ids.update( [ pipeline_task_row[ "next_task_id" ] ] )
-    for task_id in task_ids :
-        _database.update_fromdict( "task" , task_id , { "status" : "CANCELLED" } )
+        api_row = _database.db_query_select_row( "SELECT * from `api` where `id`=%s" , [api_id] )
 
-    ####
 
 
-    return( _common.response_default( ) )
+    tdata = {
+        "k1" : time.time( ) ,
+        "error_msgs" : error_msgs ,
+        "api_row" : api_row
+    }
 
+    #print(tdata)
 
-@ROUTES.route( "/user_ioblock" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "user" )
-def user_ioblock( ) :  
 
-    io_uid = _common.request_arg_str( "io_uid" ) 
-    if io_uid == "" : return( _common.response_error( e_msg = "io_uid blank" ) )
 
-    ioblock_block = _common.request_arg_int( "ioblock_block" )
-    if ioblock_block == None : return( _common.response_error( e_msg = "ioblock_block bad" ) )
+    return( render_template( "pages/member_api_create/hx_form.html" , tdata = tdata ) )
 
-    ####
 
-    io_row = _database.db_query_select_row( "SELECT * from io WHERE uid=%s LIMIT 1" , [ io_uid ] )
-    if io_row == None : _common.response_error( e_msg = f"io_row not found" )
-    io_id = io_row[ "id" ]
 
-    ioblock_row = _database.db_query_select_row( "SELECT * from ioblock WHERE io_id=%s AND block=%s LIMIT 1" , [ io_id , ioblock_block ] )
-    if ioblock_row == None : _common.response_error( e_msg = f"ioblock_row not found" )
+@ROUTES.route( "/admin_settings" , methods = [ "GET" ] )
+@_common.decorator_web_login_required( )
+def page_admin_settings( ) :
 
-    io_hash_filepath = _util.get_io_hash_filepath( ioblock_row[ "hash" ] )
- 
-    #print( io_hash_filepath )
+    error_msgs = [ ]
 
-    return( send_file( io_hash_filepath ) )
+    system_row = _database.db_query_select_row( "SELECT * from `system` where `key`=%s" , ["system/mailer/token"] )
+    if system_row is None : error_msgs.append( f"system_row None" )
 
-#####################################################################
+    tdata = {
+        "k1" : time.time( ) ,
+        "error_msgs" : error_msgs ,
+        "system/mailer/token" : system_row[ "val_str" ]
+    }
 
-@ROUTES.route( "/dashboard_state" , methods = [ "GET" ] )
-@_common.decorator_token_required
-@_common.decorator_role_required( "dashboard" )
-def dashboard_state( ) :
 
-    messages = { }
+    return( render_template( "pages/admin_settings/main.html" , tdata = tdata ) )
+
+@ROUTES.route( "/hx_admin_settings_form_system_mailer" , methods = [ "POST" ] )
+@_common.decorator_web_login_required( )
+def hx_admin_settings_form_system_mailer( ) :
+
+    form = request.form.to_dict( flat = False )
+    print( form )
+
+    try : val_str = _common.request_form_str( form , "val_str" , 1 )
+    except Exception as e : error_msgs.append( f"{e}" )
+
+    row_data = {
+        "val_str" : val_str
+    }
+    _database.update_fromdict( "system" , "system/mailer/token" , row_data , cid = "key" )
 
-    messages[ "psutils" ] = _util.psutil_status( )
+    return( render_template( "pages/admin_settings/hx_form_system_mailer.html" ) )
 
-    return( _common.response_default( messages ) )
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/common.py` & `esanom-0.7.9.3232/esanom/routes/v3/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,21 +215,14 @@
     if len( v ) < minlen : raise Exception( f"{k} to short" )
     if not _util.email_check( v ) : raise Exception( "Invalid email address" )
     return( v )
 
 def request_form_checkbox_single( form , k ) :
     return( k in form )
 
-def request_form_int( form , k , default = 0 ) :
-    if k not in form : raise Exception( f"{k} not found" )
-    if len( form[ k ] ) != 1 : raise Exception( f"len form {k} != 1" )
-    v = form[ k ][ 0 ].strip( )
-    if len( v ) == 0 : return( default )
-    return( int( v ) )
-
 def session_get( ) :
     session_data = { }
     session_key = request.cookies.get( "key" , "" ).strip( )
     if len( session_key ) == 64 :
         session_row = _database.db_query_select_row( "SELECT * from `session` WHERE `key`=%s LIMIT 1" , [ session_key ] )
         if session_row != None :
             session_data = json.loads( session_row[ "data" ] )
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/bootstrap.bundle.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/bootstrap.min.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/dashboard.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/datatables.min.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/datatables.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/datatables.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/htmx.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/nom-logo.png` & `esanom-0.7.9.3232/esanom/routes/v3/static/nom-logo.png`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/plotly.min.js` & `esanom-0.7.9.3232/esanom/routes/v3/static/plotly.min.js`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/static/theme.css` & `esanom-0.7.9.3232/esanom/routes/v3/static/theme.css`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/admin_db_pipeline_row.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/admin_db_pipeline_rows.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/admin_db_pipeline_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/base.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/base.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/db_rolemodel_row.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_row.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/db_rolemodel_rows.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/db_rolemodel_rows.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_model_io.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_model_io_port.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_model_io_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_models.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_models.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_content_pipelines.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_content_pipelines.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_debug.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_debug.html`

 * *Files 11% similar despite different names*

```diff
@@ -47,33 +47,19 @@
 <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
   <div class="offcanvas-header">
     <h5 class="offcanvas-title" id="offcanvasExampleLabel">DEBUG</h5>
     <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
   </div>
   <div class="offcanvas-body">
     <div>
-
-<div>
+<pre>
 benchmark={{_tdata["benchmark"]}}
-</div>
-
-
-
-{% if _tdata["is_fs_tmp"] %}
-{% set alert_name="danger" %}
-{% else %}
-{% set alert_name="success" %}
-{% endif %}
-<div class="alert alert-{{alert_name}}" role="alert">
 fs_storage_path={{_tdata["config_data"]["fs_storage_path"]}}
-</div>
-
-<div>
 _load_from_env={{_tdata["config_data"]["_load_from_env"]}}
-</div>
+</pre>
 
     </div>
 
 
   </div>
 </div>
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_loggedin_nav_admin.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_loggedin_nav_admin.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_head.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_head.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/inc_page_header.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/inc_page_header.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/page_dashboard_tasks.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/page_dashboard_tasks.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/page_model.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/page_model.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_account_create/inc_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,10 @@
 
         <button type="submit" class="btn btn-primary">Create</button>
 
     </form>
 
 </div>
 
-<div id="hx-results"></div>
+<div id="hx-results">FOO</div>
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_read/main.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_read/main.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_api_update/inc_form.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_group_update/inc_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 {% if tdata['row']['enable']==1 %}
 {% set enable_checked='checked' %}
 {% else %}
 {% set enable_checked='' %}
 {% endif %}
 
-<form hx-post="{{url_for('.hx_admin_group_update',uid=tdata['row']['uid'])}}" hx-target="#hx-results">
+<form hx-post="{{url_for('.hx_admin_group_update',id=tdata['row']['id'])}}" hx-target="#hx-results">
 
 
     <div class="mb-3">
         <label for="input_1" class="form-label">name</label>
         <input class="form-control" id="input_1" name="name" value="{{tdata['row']['name']}}">
     </div>
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/admin_model_update/inc_form.html`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 {% if tdata['row']['updateable']==1 %}
 {% set updateable_checked='checked' %}
 {% else %}
 {% set updateable_checked='' %}
 {% endif %}
 
-<form hx-post="{{url_for('.hx_admin_model_update',uid=tdata['row']['uid'])}}" hx-target="#hx-results">
+<form hx-post="{{url_for('.hx_admin_model_update',id=tdata['row']['id'])}}" hx-target="#hx-results">
 
 
     <div class="form-check">
         <input class="form-check-input" type="checkbox" value="1" id="input_2" name="enable" {{enable_checked}}>
         <label class="form-check-label" for="input_2">enable</label>
     </div>
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_account_create.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/legacy/admin/hx_admin_accounts.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/login/main.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/login/main.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 {% extends 'base.html' %}
 
 {% block main_title %}LOG IN{% endblock %}
 
 {% block main_content %}
 
+<div class="col-3 bg-light p-3 border">
+
 <form hx-post="{{url_for('.hx_login')}}" hx-target="#login-results">
-    <div class="mb-3 col-md-4">
-        <label for="form_email" class="form-label">Email</label>
-        <input type="email" class="form-control" id="form_email" name="account_email">
-    </div>
-    <div class="mb-3 col-md-4">
-        <label for="form_password" class="form-label">Password</label>
-        <input type="password" class="form-control" id="form_password" name="account_password">
-    </div>
-    <input type="hidden" id="_nom_form" name="[_nom_form]" value="0"> 
-    <button type="submit" class="btn btn-primary">Log In</button>
+  <div class="mb-3">
+    <label for="form_email" class="form-label">Email</label>
+    <input type="email" class="form-control" id="form_email" name="account_email">
+  </div>
+  <div class="mb-3">
+    <label for="form_password" class="form-label">Password</label>
+    <input type="password" class="form-control" id="form_password" name="account_password">
+  </div>
+  <button type="submit" class="btn btn-primary">Log In</button>
 </form>
 
+</div>
 
-<div id="login-results"></div>
+<div id="login-results">FOO</div>
 
 {% endblock %}
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/member_api_create/inc_form.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/member_api_create/inc_form.html`

 * *Files 15% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
         <button type="submit" class="btn btn-primary">Create</button>
 
     </form>
 
 </div>
 
-<div id="hx-results"></div>
+<div id="hx-results">FOO</div>
```

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_port.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_port.html-bak1`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/read_inc_ports.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/read_inc_ports.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html` & `esanom-0.7.9.3232/esanom/routes/v3/templates/pages/models/rows_inc_table_body.html`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/sample_gunicorn_config.py` & `esanom-0.7.9.3232/esanom/sample_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/sample_nom_config.json` & `esanom-0.7.9.3232/esanom/sample_nom_config.json`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/scheduler.py` & `esanom-0.7.9.3232/esanom/scheduler.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/esanom/util.py` & `esanom-0.7.9.3232/esanom/util.py`

 * *Files identical despite different names*

### Comparing `esanom-0.7.12.30/PKG-INFO` & `esanom-0.7.9.3232/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esanom
-Version: 0.7.12.30
+Version: 0.7.9.3232
 Summary: ESANOM
 Author: Zafar Iqbal
 Author-email: zaf@sparc.space
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

