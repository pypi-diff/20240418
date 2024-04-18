# Comparing `tmp/labelu-1.0.2.tar.gz` & `tmp/labelu-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelu-1.0.2.tar", max compression
+gzip compressed data, was "labelu-1.0.3.tar", max compression
```

## Comparing `labelu-1.0.2.tar` & `labelu-1.0.3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0     6434 2024-03-22 07:42:22.470993 labelu-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/__init__.py
--rw-r--r--   0        0        0     3186 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/alembic.ini
--rw-r--r--   0        0        0     2908 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/alembic_labelu_tools.py
--rw-r--r--   0        0        0     2439 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/env.py
--rw-r--r--   0        0        0      871 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/run_migrate.py
--rw-r--r--   0        0        0      510 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/script.py.mako
--rw-r--r--   0        0        0     3950 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/0145db0fec34_change_result_format.py
--rw-r--r--   0        0        0     3125 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/1b174ca5159a_update_fields.py
--rw-r--r--   0        0        0    10896 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/363f9eea797e_change_tool_config_format.py
--rw-r--r--   0        0        0      339 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/54fee6a7ecd8_init_db.py
--rw-r--r--   0        0        0     2920 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/9d5da133bbe4_replace_key_with_value_in_sample_table.py
--rw-r--r--   0        0        0     5884 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/bc8fcb35b66b_add_media_and_pre_annotation.py
--rw-r--r--   0        0        0     2697 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/alembic_labelu/versions/e76c2ca5562e_add_inner_id.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/__init__.py
--rw-r--r--   0        0        0     1001 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/persistence/crud_attachment.py
--rw-r--r--   0        0        0     3324 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/persistence/crud_pre_annotation.py
--rw-r--r--   0        0        0     3880 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/persistence/crud_sample.py
--rw-r--r--   0        0        0     1896 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/persistence/crud_task.py
--rw-r--r--   0        0        0      547 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/persistence/crud_user.py
--rw-r--r--   0        0        0      713 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/__init__.py
--rw-r--r--   0        0        0     3826 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/attachment.py
--rw-r--r--   0        0        0     4695 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/pre_annotation.py
--rw-r--r--   0        0        0     5998 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/sample.py
--rw-r--r--   0        0        0     3874 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/task.py
--rw-r--r--   0        0        0     2077 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/adapter/routers/user.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/__init__.py
--rw-r--r--   0        0        0      411 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/attachment.py
--rw-r--r--   0        0        0      380 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/pre_annotation.py
--rw-r--r--   0        0        0     1320 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/sample.py
--rw-r--r--   0        0        0     1239 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/task.py
--rw-r--r--   0        0        0      271 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/command/user.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/__init__.py
--rw-r--r--   0        0        0      429 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/attachment.py
--rw-r--r--   0        0        0      609 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/base.py
--rw-r--r--   0        0        0     1206 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/pre_annotation.py
--rw-r--r--   0        0        0     1607 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/sample.py
--rw-r--r--   0        0        0     1819 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/task.py
--rw-r--r--   0        0        0      272 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/response/user.py
--rw-r--r--   0        0        0     6356 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/service/attachment.py
--rw-r--r--   0        0        0     8215 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/service/pre_annotation.py
--rw-r--r--   0        0        0     9618 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/service/sample.py
--rw-r--r--   0        0        0     6864 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/service/task.py
--rw-r--r--   0        0        0     2390 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/application/service/user.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/__init__.py
--rw-r--r--   0        0        0    48950 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/color.py
--rw-r--r--   0        0        0     1086 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/config.py
--rw-r--r--   0        0        0    13336 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/converter.py
--rw-r--r--   0        0        0      710 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/db.py
--rw-r--r--   0        0        0     5163 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/error_code.py
--rw-r--r--   0        0        0      206 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/io.py
--rw-r--r--   0        0        0     3445 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/logger.py
--rw-r--r--   0        0        0     1192 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/common/security.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/dependencies/__init__.py
--rw-r--r--   0        0        0     1554 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/dependencies/user.py
--rw-r--r--   0        0        0     1101 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/domain/models/attachment.py
--rw-r--r--   0        0        0     1393 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/domain/models/pre_annotation.py
--rw-r--r--   0        0        0     1923 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/domain/models/sample.py
--rw-r--r--   0        0        0     1935 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/domain/models/task.py
--rw-r--r--   0        0        0      568 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/domain/models/user.py
--rw-r--r--   0        0        0      288 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/middleware/__init__.py
--rw-r--r--   0        0        0      753 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/middleware/tracing.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/internal/statics/__init__.py
--rw-r--r--   0        0        0     6192 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/analyze-wiz.umd.js
--rw-r--r--   0        0        0     3674 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/LOGO-dc1e36cf.svg
--rw-r--r--   0        0        0     1883 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/add-category-a41eef77.svg
--rw-r--r--   0        0        0     1158 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/add-text-76764c37.svg
--rw-r--r--   0        0        0      320 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/check-7b9e8325.svg
--rw-r--r--   0        0        0     2354 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/create-task-2f9c2ca2.svg
--rw-r--r--   0        0        0     1452 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/delete-fe6e1878.svg
--rw-r--r--   0        0        0      630 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/email-dca8edaf.svg
--rw-r--r--   0        0        0     2647 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/file-84424c23.svg
--rw-r--r--   0        0        0    97210 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/index-39e27c01.js
--rw-r--r--   0        0        0  5318982 2024-03-21 03:13:09.000000 labelu-1.0.2/labelu/internal/statics/assets/index-48eb8e21.js
--rw-r--r--   0        0        0    55674 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/index-6457dedf.css
--rw-r--r--   0        0        0     1098 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/local-deploy-98715da3.svg
--rw-r--r--   0        0        0     3254 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/not-found-530d1fe5.svg
--rw-r--r--   0        0        0      878 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/outputData-a8eb3ce7.svg
--rw-r--r--   0        0        0      977 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/password-6f4e2921.svg
--rw-r--r--   0        0        0     1745 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/personal-10f326c6.svg
--rw-r--r--   0        0        0    28912 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-42f3099a.js
--rw-r--r--   0        0        0    28912 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-6ff076da-7084945b.js
--rw-r--r--   0        0        0      762 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/tree-switcher-68b25e90.svg
--rw-r--r--   0        0        0    14143 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/upload-bg-f071f390.svg
--rw-r--r--   0        0        0   650663 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/video.es-57367aa8-e794451e-455bdbff.js
--rw-r--r--   0        0        0   650663 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/assets/video.es-57367aa8-e9be4385.js
--rw-r--r--   0        0        0      259 2024-03-22 07:42:25.587001 labelu-1.0.2/labelu/internal/statics/backend_version.js
--rw-r--r--   0        0        0     1376 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/favicon.svg
--rw-r--r--   0        0        0      485 2024-03-21 03:13:27.000000 labelu-1.0.2/labelu/internal/statics/frontend_version.js
--rw-r--r--   0        0        0     2027 2024-03-21 03:13:08.000000 labelu-1.0.2/labelu/internal/statics/index.html
--rw-r--r--   0        0        0     5347 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/logo192.png
--rw-r--r--   0        0        0     9664 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/logo512.png
--rw-r--r--   0        0        0      488 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/manifest.json
--rw-r--r--   0        0        0       67 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/robots.txt
--rw-r--r--   0        0        0      221 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/check.png
--rw-r--r--   0        0        0     2354 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/createTask.svg
--rw-r--r--   0        0        0      262 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/dataOutput.png
--rw-r--r--   0        0        0      615 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/delete.svg
--rw-r--r--   0        0        0      597 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/deleteBlue.svg
--rw-r--r--   0        0        0      630 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/email.svg
--rw-r--r--   0        0        0     2647 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/file.svg
--rw-r--r--   0        0        0      362 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/finishCheck.svg
--rw-r--r--   0        0        0      417 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/finished.svg
--rw-r--r--   0        0        0      757 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/folder.png
--rw-r--r--   0        0        0      730 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/helpText.svg
--rw-r--r--   0        0        0      468 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/outputData.svg
--rw-r--r--   0        0        0      463 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/outputData1.svg
--rw-r--r--   0        0        0      425 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/outputDataBlue.svg
--rw-r--r--   0        0        0      977 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/password.svg
--rw-r--r--   0        0        0      690 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/pending.png
--rw-r--r--   0        0        0     1745 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/personal.svg
--rw-r--r--   0        0        0     1068 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/picture.png
--rw-r--r--   0        0        0      406 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/rightCorner.png
--rw-r--r--   0        0        0      363 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/setting.png
--rw-r--r--   0        0        0     6002 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/setting.svg
--rw-r--r--   0        0        0      302 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/uploadFile.svg
--rw-r--r--   0        0        0      767 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/uploadFolder.svg
--rw-r--r--   0        0        0      412 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/warning.png
--rw-r--r--   0        0        0    14690 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/上传.svg
--rw-r--r--   0        0        0    66315 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/icons/数据导入.svg
--rw-r--r--   0        0        0   116414 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear1.webp
--rw-r--r--   0        0        0   207762 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear2.webp
--rw-r--r--   0        0        0     8374 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear3.webp
--rw-r--r--   0        0        0    21964 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear4.webp
--rw-r--r--   0        0        0    18642 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear5.webp
--rw-r--r--   0        0        0    13752 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear6.webp
--rw-r--r--   0        0        0    23382 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/src/img/example/bear7.webp
--rw-r--r--   0        0        0    68678 2024-03-21 03:13:06.000000 labelu-1.0.2/labelu/internal/statics/yaml.js
--rw-r--r--   0        0        0     2576 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/main.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/__init__.py
--rw-r--r--   0        0        0     2796 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/conftest.py
--rw-r--r--   0        0        0     1126 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/data/test.jsonl
--rw-r--r--   0        0        0    17539 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/data/test.png
--rw-r--r--   0        0        0       17 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/data/test.txt
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/__init__.py
--rw-r--r--   0        0        0     1685 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/persistence/test_crud_user.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/__init__.py
--rw-r--r--   0        0        0     9067 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/test_attachment.py
--rw-r--r--   0        0        0    14390 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/test_pre_annotation.py
--rw-r--r--   0        0        0    23674 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/test_sample.py
--rw-r--r--   0        0        0    10223 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/test_task.py
--rw-r--r--   0        0        0     4351 2024-03-22 07:42:22.470993 labelu-1.0.2/labelu/tests/internal/adapter/routers/test_user.py
--rw-r--r--   0        0        0     8822 2024-03-22 07:42:22.474993 labelu-1.0.2/labelu/tests/internal/common/test_converter.py
--rw-r--r--   0        0        0     1279 2024-03-22 07:42:22.474993 labelu-1.0.2/labelu/tests/internal/common/test_security.py
--rw-r--r--   0        0        0        0 2024-03-22 07:42:22.474993 labelu-1.0.2/labelu/tests/utils/__init__.py
--rw-r--r--   0        0        0      251 2024-03-22 07:42:22.474993 labelu-1.0.2/labelu/tests/utils/utils.py
--rw-r--r--   0        0        0     1114 2024-03-22 07:43:52.951251 labelu-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8530 1970-01-01 00:00:00.000000 labelu-1.0.2/setup.py
--rw-r--r--   0        0        0     7738 1970-01-01 00:00:00.000000 labelu-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6434 2024-04-18 09:22:42.284530 labelu-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/alembic.ini
+-rw-r--r--   0        0        0     2908 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/alembic_labelu_tools.py
+-rw-r--r--   0        0        0     2439 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/env.py
+-rw-r--r--   0        0        0      871 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/run_migrate.py
+-rw-r--r--   0        0        0      510 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/script.py.mako
+-rw-r--r--   0        0        0     3950 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/0145db0fec34_change_result_format.py
+-rw-r--r--   0        0        0     3125 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/1b174ca5159a_update_fields.py
+-rw-r--r--   0        0        0    10896 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/363f9eea797e_change_tool_config_format.py
+-rw-r--r--   0        0        0      339 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/54fee6a7ecd8_init_db.py
+-rw-r--r--   0        0        0     2920 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/9d5da133bbe4_replace_key_with_value_in_sample_table.py
+-rw-r--r--   0        0        0     5884 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/bc8fcb35b66b_add_media_and_pre_annotation.py
+-rw-r--r--   0        0        0     2697 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/alembic_labelu/versions/e76c2ca5562e_add_inner_id.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/persistence/crud_attachment.py
+-rw-r--r--   0        0        0     3324 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/persistence/crud_pre_annotation.py
+-rw-r--r--   0        0        0     3880 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/persistence/crud_sample.py
+-rw-r--r--   0        0        0     1896 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/persistence/crud_task.py
+-rw-r--r--   0        0        0      547 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/persistence/crud_user.py
+-rw-r--r--   0        0        0      713 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/__init__.py
+-rw-r--r--   0        0        0     3826 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/attachment.py
+-rw-r--r--   0        0        0     4695 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/pre_annotation.py
+-rw-r--r--   0        0        0     5998 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/sample.py
+-rw-r--r--   0        0        0     3874 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/task.py
+-rw-r--r--   0        0        0     2077 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/adapter/routers/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/attachment.py
+-rw-r--r--   0        0        0      380 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/pre_annotation.py
+-rw-r--r--   0        0        0     1320 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/sample.py
+-rw-r--r--   0        0        0     1239 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/task.py
+-rw-r--r--   0        0        0      271 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/command/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/attachment.py
+-rw-r--r--   0        0        0      609 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/base.py
+-rw-r--r--   0        0        0     1206 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/pre_annotation.py
+-rw-r--r--   0        0        0     1607 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/sample.py
+-rw-r--r--   0        0        0     1819 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/task.py
+-rw-r--r--   0        0        0      272 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/response/user.py
+-rw-r--r--   0        0        0     6356 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/service/attachment.py
+-rw-r--r--   0        0        0     8215 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/service/pre_annotation.py
+-rw-r--r--   0        0        0     9618 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/service/sample.py
+-rw-r--r--   0        0        0     6864 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/service/task.py
+-rw-r--r--   0        0        0     2390 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/application/service/user.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/__init__.py
+-rw-r--r--   0        0        0    48950 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/color.py
+-rw-r--r--   0        0        0     1086 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/config.py
+-rw-r--r--   0        0        0    13356 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/converter.py
+-rw-r--r--   0        0        0      710 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/db.py
+-rw-r--r--   0        0        0     5163 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/error_code.py
+-rw-r--r--   0        0        0      206 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/io.py
+-rw-r--r--   0        0        0     3445 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/logger.py
+-rw-r--r--   0        0        0     1192 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/common/security.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/dependencies/__init__.py
+-rw-r--r--   0        0        0     1554 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/dependencies/user.py
+-rw-r--r--   0        0        0     1101 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/domain/models/attachment.py
+-rw-r--r--   0        0        0     1393 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/domain/models/pre_annotation.py
+-rw-r--r--   0        0        0     1923 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/domain/models/sample.py
+-rw-r--r--   0        0        0     1935 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/domain/models/task.py
+-rw-r--r--   0        0        0      568 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/domain/models/user.py
+-rw-r--r--   0        0        0      288 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/middleware/__init__.py
+-rw-r--r--   0        0        0      753 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/middleware/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/internal/statics/__init__.py
+-rw-r--r--   0        0        0     6192 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/analyze-wiz.umd.js
+-rw-r--r--   0        0        0     3674 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/LOGO-dc1e36cf.svg
+-rw-r--r--   0        0        0     1883 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/add-category-a41eef77.svg
+-rw-r--r--   0        0        0     1158 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/add-text-76764c37.svg
+-rw-r--r--   0        0        0      320 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/check-7b9e8325.svg
+-rw-r--r--   0        0        0     2354 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/create-task-2f9c2ca2.svg
+-rw-r--r--   0        0        0     1452 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/delete-fe6e1878.svg
+-rw-r--r--   0        0        0      630 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/email-dca8edaf.svg
+-rw-r--r--   0        0        0     2647 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/file-84424c23.svg
+-rw-r--r--   0        0        0    97210 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/index-39e27c01.js
+-rw-r--r--   0        0        0  5318982 2024-03-21 03:13:09.000000 labelu-1.0.3/labelu/internal/statics/assets/index-48eb8e21.js
+-rw-r--r--   0        0        0    55674 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/index-6457dedf.css
+-rw-r--r--   0        0        0     1098 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/local-deploy-98715da3.svg
+-rw-r--r--   0        0        0     3254 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/not-found-530d1fe5.svg
+-rw-r--r--   0        0        0      878 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/outputData-a8eb3ce7.svg
+-rw-r--r--   0        0        0      977 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/password-6f4e2921.svg
+-rw-r--r--   0        0        0     1745 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/personal-10f326c6.svg
+-rw-r--r--   0        0        0    28912 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-42f3099a.js
+-rw-r--r--   0        0        0    28912 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-6ff076da-7084945b.js
+-rw-r--r--   0        0        0      762 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/tree-switcher-68b25e90.svg
+-rw-r--r--   0        0        0    14143 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/upload-bg-f071f390.svg
+-rw-r--r--   0        0        0   650663 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/video.es-57367aa8-e794451e-455bdbff.js
+-rw-r--r--   0        0        0   650663 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/assets/video.es-57367aa8-e9be4385.js
+-rw-r--r--   0        0        0      259 2024-04-18 09:22:48.864508 labelu-1.0.3/labelu/internal/statics/backend_version.js
+-rw-r--r--   0        0        0     1376 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/favicon.svg
+-rw-r--r--   0        0        0      485 2024-03-21 03:13:27.000000 labelu-1.0.3/labelu/internal/statics/frontend_version.js
+-rw-r--r--   0        0        0     2027 2024-03-21 03:13:08.000000 labelu-1.0.3/labelu/internal/statics/index.html
+-rw-r--r--   0        0        0     5347 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/logo192.png
+-rw-r--r--   0        0        0     9664 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/logo512.png
+-rw-r--r--   0        0        0      488 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/manifest.json
+-rw-r--r--   0        0        0       67 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/robots.txt
+-rw-r--r--   0        0        0      221 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/check.png
+-rw-r--r--   0        0        0     2354 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/createTask.svg
+-rw-r--r--   0        0        0      262 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/dataOutput.png
+-rw-r--r--   0        0        0      615 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/delete.svg
+-rw-r--r--   0        0        0      597 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/deleteBlue.svg
+-rw-r--r--   0        0        0      630 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/email.svg
+-rw-r--r--   0        0        0     2647 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/file.svg
+-rw-r--r--   0        0        0      362 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/finishCheck.svg
+-rw-r--r--   0        0        0      417 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/finished.svg
+-rw-r--r--   0        0        0      757 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/folder.png
+-rw-r--r--   0        0        0      730 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/helpText.svg
+-rw-r--r--   0        0        0      468 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/outputData.svg
+-rw-r--r--   0        0        0      463 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/outputData1.svg
+-rw-r--r--   0        0        0      425 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/outputDataBlue.svg
+-rw-r--r--   0        0        0      977 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/password.svg
+-rw-r--r--   0        0        0      690 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/pending.png
+-rw-r--r--   0        0        0     1745 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/personal.svg
+-rw-r--r--   0        0        0     1068 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/picture.png
+-rw-r--r--   0        0        0      406 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/rightCorner.png
+-rw-r--r--   0        0        0      363 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/setting.png
+-rw-r--r--   0        0        0     6002 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/setting.svg
+-rw-r--r--   0        0        0      302 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/uploadFile.svg
+-rw-r--r--   0        0        0      767 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/uploadFolder.svg
+-rw-r--r--   0        0        0      412 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/warning.png
+-rw-r--r--   0        0        0    14690 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/上传.svg
+-rw-r--r--   0        0        0    66315 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/icons/数据导入.svg
+-rw-r--r--   0        0        0   116414 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear1.webp
+-rw-r--r--   0        0        0   207762 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear2.webp
+-rw-r--r--   0        0        0     8374 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear3.webp
+-rw-r--r--   0        0        0    21964 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear4.webp
+-rw-r--r--   0        0        0    18642 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear5.webp
+-rw-r--r--   0        0        0    13752 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear6.webp
+-rw-r--r--   0        0        0    23382 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/src/img/example/bear7.webp
+-rw-r--r--   0        0        0    68678 2024-03-21 03:13:06.000000 labelu-1.0.3/labelu/internal/statics/yaml.js
+-rw-r--r--   0        0        0     3216 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/main.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/__init__.py
+-rw-r--r--   0        0        0     2796 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/conftest.py
+-rw-r--r--   0        0        0     1126 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/data/test.jsonl
+-rw-r--r--   0        0        0    17539 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/data/test.png
+-rw-r--r--   0        0        0       17 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/data/test.txt
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/__init__.py
+-rw-r--r--   0        0        0     1685 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/persistence/test_crud_user.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/__init__.py
+-rw-r--r--   0        0        0     9067 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/test_attachment.py
+-rw-r--r--   0        0        0    14390 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/test_pre_annotation.py
+-rw-r--r--   0        0        0    23674 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/test_sample.py
+-rw-r--r--   0        0        0    10223 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/test_task.py
+-rw-r--r--   0        0        0     4351 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/adapter/routers/test_user.py
+-rw-r--r--   0        0        0     8822 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/common/test_converter.py
+-rw-r--r--   0        0        0     1279 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/internal/common/test_security.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/utils/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-18 09:22:42.284530 labelu-1.0.3/labelu/tests/utils/utils.py
+-rw-r--r--   0        0        0     1114 2024-04-18 09:24:10.428226 labelu-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8530 1970-01-01 00:00:00.000000 labelu-1.0.3/setup.py
+-rw-r--r--   0        0        0     7738 1970-01-01 00:00:00.000000 labelu-1.0.3/PKG-INFO
```

### Comparing `labelu-1.0.2/README.md` & `labelu-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/alembic.ini` & `labelu-1.0.3/labelu/alembic_labelu/alembic.ini`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/alembic_labelu_tools.py` & `labelu-1.0.3/labelu/alembic_labelu/alembic_labelu_tools.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/env.py` & `labelu-1.0.3/labelu/alembic_labelu/env.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/run_migrate.py` & `labelu-1.0.3/labelu/alembic_labelu/run_migrate.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/0145db0fec34_change_result_format.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/0145db0fec34_change_result_format.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/1b174ca5159a_update_fields.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/1b174ca5159a_update_fields.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/363f9eea797e_change_tool_config_format.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/363f9eea797e_change_tool_config_format.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/9d5da133bbe4_replace_key_with_value_in_sample_table.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/9d5da133bbe4_replace_key_with_value_in_sample_table.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/bc8fcb35b66b_add_media_and_pre_annotation.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/bc8fcb35b66b_add_media_and_pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/alembic_labelu/versions/e76c2ca5562e_add_inner_id.py` & `labelu-1.0.3/labelu/alembic_labelu/versions/e76c2ca5562e_add_inner_id.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/persistence/crud_attachment.py` & `labelu-1.0.3/labelu/internal/adapter/persistence/crud_attachment.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/persistence/crud_pre_annotation.py` & `labelu-1.0.3/labelu/internal/adapter/persistence/crud_pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/persistence/crud_sample.py` & `labelu-1.0.3/labelu/internal/adapter/persistence/crud_sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/persistence/crud_task.py` & `labelu-1.0.3/labelu/internal/adapter/persistence/crud_task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/persistence/crud_user.py` & `labelu-1.0.3/labelu/internal/adapter/persistence/crud_user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/__init__.py` & `labelu-1.0.3/labelu/internal/adapter/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/attachment.py` & `labelu-1.0.3/labelu/internal/adapter/routers/attachment.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/pre_annotation.py` & `labelu-1.0.3/labelu/internal/adapter/routers/pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/sample.py` & `labelu-1.0.3/labelu/internal/adapter/routers/sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/task.py` & `labelu-1.0.3/labelu/internal/adapter/routers/task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/adapter/routers/user.py` & `labelu-1.0.3/labelu/internal/adapter/routers/user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/command/sample.py` & `labelu-1.0.3/labelu/internal/application/command/sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/command/task.py` & `labelu-1.0.3/labelu/internal/application/command/task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/response/base.py` & `labelu-1.0.3/labelu/internal/application/response/base.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/response/pre_annotation.py` & `labelu-1.0.3/labelu/internal/application/response/pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/response/sample.py` & `labelu-1.0.3/labelu/internal/application/response/sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/response/task.py` & `labelu-1.0.3/labelu/internal/application/response/task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/service/attachment.py` & `labelu-1.0.3/labelu/internal/application/service/attachment.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/service/pre_annotation.py` & `labelu-1.0.3/labelu/internal/application/service/pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/service/sample.py` & `labelu-1.0.3/labelu/internal/application/service/sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/service/task.py` & `labelu-1.0.3/labelu/internal/application/service/task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/application/service/user.py` & `labelu-1.0.3/labelu/internal/application/service/user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/color.py` & `labelu-1.0.3/labelu/internal/common/color.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/config.py` & `labelu-1.0.3/labelu/internal/common/config.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/converter.py` & `labelu-1.0.3/labelu/internal/common/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
             annotated_result_str = json.dumps(annotated_result, ensure_ascii=False)
             results.append(
                 {
                     "id": sample.get("id"),
                     "result": annotated_result_str,
                     "url": file.get("url"),
-                    "fileName": file.get("filename"),
+                    "fileName": file.get("filename", "")[9:],
                 }
             )
 
         # Serializing json
         json_object = json.dumps(results, default=str)
         with file_full_path.open("w") as outfile:
             outfile.write(json_object)
@@ -162,15 +162,15 @@
 
             # annotation result
             annotation_result = json.loads(annotation_data.get("result", {}))
 
             # coco image
             image = {
                 "id": sample.get("id"),
-                "fileName": file.get("filename"),
+                "fileName": file.get("filename", "")[9:],
                 "width": annotation_result.get("width", 0),
                 "height": annotation_result.get("height", 0),
                 "valid": False
                 if sample.get("state", "") == "SKIPPED"
                 else annotation_result.get("valid", True),
                 "rotate": annotation_result.get("rotate", 0),
             }
@@ -262,15 +262,15 @@
             file = sample.get("file", {})
             if sample.get("state") != "DONE":
                 continue
             annotation_data = json.loads(sample.get("data"))
             logger.info("data is: {}", sample)
             filename = file.get("filename")
             if filename and filename.split("/")[-1]:
-                file_relative_path_base_name = filename.split("/")[-1].split(".")[0]
+                file_relative_path_base_name = filename.split("/")[-1].split(".")[0][9:]
             else:
                 file_relative_path_base_name = "result"
 
             # annotation result
             annotation_result = json.loads(annotation_data.get("result", {}))
             if not annotation_result or not annotation_result.get("polygonTool", {}):
                 continue
```

### Comparing `labelu-1.0.2/labelu/internal/common/db.py` & `labelu-1.0.3/labelu/internal/common/db.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/error_code.py` & `labelu-1.0.3/labelu/internal/common/error_code.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/logger.py` & `labelu-1.0.3/labelu/internal/common/logger.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/common/security.py` & `labelu-1.0.3/labelu/internal/common/security.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/dependencies/user.py` & `labelu-1.0.3/labelu/internal/dependencies/user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/domain/models/attachment.py` & `labelu-1.0.3/labelu/internal/domain/models/attachment.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/domain/models/pre_annotation.py` & `labelu-1.0.3/labelu/internal/domain/models/pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/domain/models/sample.py` & `labelu-1.0.3/labelu/internal/domain/models/sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/domain/models/task.py` & `labelu-1.0.3/labelu/internal/domain/models/task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/domain/models/user.py` & `labelu-1.0.3/labelu/internal/domain/models/user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/middleware/tracing.py` & `labelu-1.0.3/labelu/internal/middleware/tracing.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/analyze-wiz.umd.js` & `labelu-1.0.3/labelu/internal/statics/analyze-wiz.umd.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/LOGO-dc1e36cf.svg` & `labelu-1.0.3/labelu/internal/statics/assets/LOGO-dc1e36cf.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/add-category-a41eef77.svg` & `labelu-1.0.3/labelu/internal/statics/assets/add-category-a41eef77.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/add-text-76764c37.svg` & `labelu-1.0.3/labelu/internal/statics/assets/add-text-76764c37.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/create-task-2f9c2ca2.svg` & `labelu-1.0.3/labelu/internal/statics/assets/create-task-2f9c2ca2.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/delete-fe6e1878.svg` & `labelu-1.0.3/labelu/internal/statics/assets/delete-fe6e1878.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/email-dca8edaf.svg` & `labelu-1.0.3/labelu/internal/statics/assets/email-dca8edaf.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/file-84424c23.svg` & `labelu-1.0.3/labelu/internal/statics/assets/file-84424c23.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/index-39e27c01.js` & `labelu-1.0.3/labelu/internal/statics/assets/index-39e27c01.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/index-48eb8e21.js` & `labelu-1.0.3/labelu/internal/statics/assets/index-48eb8e21.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/index-6457dedf.css` & `labelu-1.0.3/labelu/internal/statics/assets/index-6457dedf.css`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/local-deploy-98715da3.svg` & `labelu-1.0.3/labelu/internal/statics/assets/local-deploy-98715da3.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/not-found-530d1fe5.svg` & `labelu-1.0.3/labelu/internal/statics/assets/not-found-530d1fe5.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/outputData-a8eb3ce7.svg` & `labelu-1.0.3/labelu/internal/statics/assets/outputData-a8eb3ce7.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/password-6f4e2921.svg` & `labelu-1.0.3/labelu/internal/statics/assets/password-6f4e2921.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/personal-10f326c6.svg` & `labelu-1.0.3/labelu/internal/statics/assets/personal-10f326c6.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-42f3099a.js` & `labelu-1.0.3/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-42f3099a.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-6ff076da-7084945b.js` & `labelu-1.0.3/labelu/internal/statics/assets/polygon-clipping.esm-baf20f41-6ff076da-7084945b.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/tree-switcher-68b25e90.svg` & `labelu-1.0.3/labelu/internal/statics/assets/tree-switcher-68b25e90.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/upload-bg-f071f390.svg` & `labelu-1.0.3/labelu/internal/statics/assets/upload-bg-f071f390.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/video.es-57367aa8-e794451e-455bdbff.js` & `labelu-1.0.3/labelu/internal/statics/assets/video.es-57367aa8-e794451e-455bdbff.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/assets/video.es-57367aa8-e9be4385.js` & `labelu-1.0.3/labelu/internal/statics/assets/video.es-57367aa8-e9be4385.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/favicon.svg` & `labelu-1.0.3/labelu/internal/statics/favicon.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/index.html` & `labelu-1.0.3/labelu/internal/statics/index.html`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/logo192.png` & `labelu-1.0.3/labelu/internal/statics/logo192.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/logo512.png` & `labelu-1.0.3/labelu/internal/statics/logo512.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/createTask.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/createTask.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/delete.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/deleteBlue.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/deleteBlue.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/email.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/email.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/file.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/file.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/folder.png` & `labelu-1.0.3/labelu/internal/statics/src/icons/folder.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/helpText.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/helpText.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/password.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/password.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/pending.png` & `labelu-1.0.3/labelu/internal/statics/src/icons/pending.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/personal.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/personal.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/picture.png` & `labelu-1.0.3/labelu/internal/statics/src/icons/picture.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/setting.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/setting.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/uploadFolder.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/uploadFolder.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/上传.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/上传.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/icons/数据导入.svg` & `labelu-1.0.3/labelu/internal/statics/src/icons/数据导入.svg`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear1.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear1.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear2.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear2.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear3.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear3.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear4.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear4.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear5.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear5.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear6.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear6.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/src/img/example/bear7.webp` & `labelu-1.0.3/labelu/internal/statics/src/img/example/bear7.webp`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/internal/statics/yaml.js` & `labelu-1.0.3/labelu/internal/statics/yaml.js`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/main.py` & `labelu-1.0.3/labelu/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from typing import Any
 import uvicorn
 from typer import Typer
-from fastapi import FastAPI, Request
+from fastapi import FastAPI, Request, Response
 from fastapi.staticfiles import StaticFiles
 
 from labelu.internal.adapter.routers import add_router
 from labelu.internal.middleware import add_middleware
 from labelu.internal.common.logger import init_logging
 from labelu.internal.common.db import init_tables
 from labelu.internal.common.config import settings
@@ -89,20 +90,35 @@
 init_logging()
 init_tables()
 run_sqlite_migrations()
 add_exception_handler(app=app)
 add_router(app=app)
 add_middleware(app=app)
 
-app.mount("", StaticFiles(packages=["labelu.internal"], html=True))
+class NoCacheStaticFiles(StaticFiles):
+    def __init__(self, *args: Any, **kwargs: Any):
+        self.cachecontrol = "max-age=0, no-cache, no-store, , must-revalidate"
+        self.pragma = "no-cache"
+        self.expires = "0"
+        super().__init__(*args, **kwargs)
+
+    def file_response(self, *args: Any, **kwargs: Any) -> Response:
+        resp = super().file_response(*args, **kwargs)
+        resp.headers.setdefault("Cache-Control", self.cachecontrol)
+        resp.headers.setdefault("Pragma", self.pragma)
+        resp.headers.setdefault("Expires", self.expires)
+        return resp
+
+app.mount("", NoCacheStaticFiles(packages=["labelu.internal"], html=True))
 
 
 @app.middleware("http")
 async def add_correct_content_type(request: Request, call_next):
     response = await call_next(request)
+    
     if request.url.path.endswith(".js"):
         response.headers["content-type"] = "application/javascript"
     return response
 
 
 cli = Typer()
```

### Comparing `labelu-1.0.2/labelu/tests/conftest.py` & `labelu-1.0.3/labelu/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/data/test.jsonl` & `labelu-1.0.3/labelu/tests/data/test.jsonl`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/data/test.png` & `labelu-1.0.3/labelu/tests/data/test.png`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/persistence/test_crud_user.py` & `labelu-1.0.3/labelu/tests/internal/adapter/persistence/test_crud_user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/routers/test_attachment.py` & `labelu-1.0.3/labelu/tests/internal/adapter/routers/test_attachment.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/routers/test_pre_annotation.py` & `labelu-1.0.3/labelu/tests/internal/adapter/routers/test_pre_annotation.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/routers/test_sample.py` & `labelu-1.0.3/labelu/tests/internal/adapter/routers/test_sample.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/routers/test_task.py` & `labelu-1.0.3/labelu/tests/internal/adapter/routers/test_task.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/adapter/routers/test_user.py` & `labelu-1.0.3/labelu/tests/internal/adapter/routers/test_user.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/common/test_converter.py` & `labelu-1.0.3/labelu/tests/internal/common/test_converter.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/labelu/tests/internal/common/test_security.py` & `labelu-1.0.3/labelu/tests/internal/common/test_security.py`

 * *Files identical despite different names*

### Comparing `labelu-1.0.2/pyproject.toml` & `labelu-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labelu"
-version = '1.0.2'
+version = '1.0.3'
 description = ""
 license = "Apache-2.0"
 authors = ["pengjinhu <pengjinhu@pjlab.org.cn>"]
 readme = "README.md"
 repository = "https://github.com/opendatalab/labelU"
 packages = [{include = "labelu"}]
```

### Comparing `labelu-1.0.2/setup.py` & `labelu-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
  'uvicorn>=0.19.0,<0.20.0']
 
 entry_points = \
 {'console_scripts': ['labelu = labelu.main:cli']}
 
 setup_kwargs = {
     'name': 'labelu',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': '',
     'long_description': '<div align="center">\n<article style="display: flex; flex-direction: column; align-items: center; justify-content: center;">\n    <p align="center"><img width="300" src="https://user-images.githubusercontent.com/25022954/209616423-9ab056be-5d62-4eeb-b91d-3b20f64cfcf8.svg" /></p>\n    <h1 style="width: 100%; text-align: center;"></h1>\n    <p align="center">\n        English | <a href="./README_zh-CN.md" >简体中文</a>\n    </p>\n</article>\n    \n   \n</div>\n\n## Introduction\n\nLabelU offers a variety of annotation tools and features, supporting image, video, and audio annotation.\n\n- Image: Multifunctional image processing tools encompassing 2D bounding box, cuboid, semantic segmentation, polylines, keypoints, and many other annotation tools, assist in completing image identification, annotation, and analysis.\n- Video: The video annotation has robust video processing capabilities, able to implement video segmentation, video classification, video information extraction, and other functions, providing high-quality annotated data for model training.\n- Audio: Highly efficient and accurate audio analysis tool can achieve audio segmentation, audio classification, audio information extraction, and other functions, making complex sound information visually intuitive.\n\n<p align="center">\n<img style="width: 600px" src="https://user-images.githubusercontent.com/25022954/209318236-79d3a5c3-2700-46c3-b59a-62d9c132a6c3.gif">\n</p>\n\n## Features\n\n- Simplicity: Provides a variety of image annotation tools that can be annotated through simple visual configuration.\n- Flexibility: A variety of tools can be freely combined to meet most image, video, and audio annotation needs.\n- Universality: Supports exporting to various data formats, including JSON, COCO, MASK.\n\n## Getting started\n\n- <a href="https://opendatalab.github.io/labelU-Kit/">\n    <button>Try LabelU annotation toolkit</button>\n</a>\n\n- <a href="https://labelu.shlab.tech/">\n    <button>Try LabelU online</button>\n</a>\n\n### Local deployment\n\n1. Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html), Choose the corresponding operating system type and download it for installation.\n\n> **Note：** If your system is MacOS with an Intel chip, please install [Miniconda of intel x86_64](https://repo.anaconda.com/miniconda/)。\n\n2. After the installation is complete, run the following command in the terminal (you can choose the default \'y\' for prompts during the process):\n\n```bash\nconda create -n labelu python=3.7\n```\n\n> **Note：** For Windows platform, you can run the above command in Anaconda Prompt.\n\n3. Activate the environment：\n\n```bash\nconda activate labelu\n```\n\n4. Install LabelU：\n\n```bash\npip install labelu\n```\n\n> To install the test version：`pip install --extra-index-url https://test.pypi.org/simple/ labelu==<test revision>`\n\n5. Run LabelU：\n\n```bash\nlabelu\n```\n\n6. Visit [http://localhost:8000/](http://localhost:8000/) and ready to go.\n\n### Local development\n\n```bash\n# Download and Install miniconda\n# https://docs.conda.io/en/latest/miniconda.html\n\n# Create virtual environment(python = 3.7)\nconda create -n labelu python=3.7\n\n# Activate virtual environment\nconda activate labelu\n\n# Install peotry\n# https://python-poetry.org/docs/#installing-with-the-official-installer\n\n# Install all package dependencies\npoetry install\n\n# Start labelu, server: http://localhost:8000\nuvicorn labelu.main:app --reload\n\n# Update submodule\ngit submodule update --remote --merge\n```\n\n## Supported Scenarios\n\n### Image\n\n- Label Classification: Can help users quickly classify objects in images and can be used for image retrieval, object detection tasks.\n- Text Description: Text transcription can help users quickly extract text information in images and can be used for text retrieval, machine translation tasks.\n- Bounding Box: Can help users quickly select objects in images and can be used for image recognition, object tracking tasks.\n- Point Annotation: Points can help users accurately label key information in the image and can be used for object recognition, scene analysis tasks.\n- Polygon: Can help users accurately label irregular shapes and can be used for object recognition, scene analysis tasks.\n- Line Annotation: Lines can help users accurately label edges and contours in the image and can be used for object recognition, scene analysis tasks.\n- Cuboid: Cuboid can help users accurately label the size, shape, and location of objects within images, and can be used for object recognition, scene analysis tasks.\n\n### Video\n\n- Label Classification: Classifying and labeling videos can be used for video retrieval, recommendation, and classification tasks.\n- Text Description: Converting speech content in videos into text can be used for voice recognition, transcription, and translation tasks.\n- Segment Segmentation: Extracting specific clips or scenes from the video for annotation is very useful for video object detection, action recognition, and video summary tasks.\n- Timestamps: Point to or mark specific parts of the video; users can click on timestamps to jump directly to that part of the video.\n\n### Audio\n\n- Label Classification: By listening to the audio and selecting the appropriate classification for annotation, it\'s applicable for audio retrieval, recommendations, and classification tasks.\n- Text Description: Converting speech content in audio into text makes it easier for users to analyze and process text. It\'s very useful for voice recognition, transcription tasks, and can help users better understand and process voice content.\n- Segment Segmentation: Extracting specific clips from audio for annotation is very useful for audio event detection, voice recognition, and audio editing tasks.\n- Timestamps: Used to point to or mark specific parts of the audio; users can click on timestamps to jump directly to that part of the audio.\n\n## Quick start\n\n- [Guidance](https://opendatalab.github.io/labelU)\n\n## Annotation format\n\n- [Documentation](https://opendatalab.github.io/labelU/#/schema)\n\n## Communication\n\nWelcome to the OpenDataLab official WeChat group！\n\n<p align="center">\n<img style="width: 400px" src="https://user-images.githubusercontent.com/25022954/208374419-2dffb701-321a-4091-944d-5d913de79a15.jpg">\n</p>\n\n## Links\n\n- [LabelU-kit](https://github.com/opendatalab/labelU-Kit) (LabelU is developed using LabelU-kit.)\n\n## License\n\nThis project is released under the [Apache 2.0 license](./LICENSE).\n',
     'author': 'pengjinhu',
     'author_email': 'pengjinhu@pjlab.org.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opendatalab/labelU',
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 'appdirs>=1.4.4,<2.0.0', 'email-validator>=1.3.0,<2.0.0',
 'fastapi>=0.86.0,<0.87.0', 'loguru>=0.6.0,<0.7.0', 'passlib
 [bcrypt]>=1.7.4,<2.0.0', 'pillow>=9.3.0,<10.0.0', 'python-
 dotenv>=0.21.0,<0.22.0', 'python-jose[cryptography]>=3.3.0,<4.0.0', 'python-
 multipart>=0.0.5,<0.0.6', 'sqlalchemy>=1.4.43,<2.0.0', 'typer
 [all]>=0.7.0,<0.8.0', 'uvicorn>=0.19.0,<0.20.0'] entry_points = \
 {'console_scripts': ['labelu = labelu.main:cli']} setup_kwargs = { 'name':
-'labelu', 'version': '1.0.2', 'description': '', 'long_description': '
+'labelu', 'version': '1.0.3', 'description': '', 'long_description': '
                                      \n\n
  [https://user-images.githubusercontent.com/25022954/209616423-9ab056be-5d62-
                           4eeb-b91d-3b20f64cfcf8.svg]
                                       \n
                                       \n
                           \n English | _ç_®__ä_½__ä_¸_­_æ__\n
                                   \n\n \n \n
```

### Comparing `labelu-1.0.2/PKG-INFO` & `labelu-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelu
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Home-page: https://github.com/opendatalab/labelU
 License: Apache-2.0
 Author: pengjinhu
 Author-email: pengjinhu@pjlab.org.cn
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labelu Version: 1.0.2 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: labelu Version: 1.0.3 Summary: Home-page: https://
 github.com/opendatalab/labelU License: Apache-2.0 Author: pengjinhu Author-
 email: pengjinhu@pjlab.org.cn Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: aiofiles
```

