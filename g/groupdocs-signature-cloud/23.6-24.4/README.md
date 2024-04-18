# Comparing `tmp/groupdocs-signature-cloud-23.6.tar.gz` & `tmp/groupdocs_signature_cloud-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\groupdocs-signature-cloud-23.6.tar", last modified: Fri Jun 23 08:36:10 2023, max compression
+gzip compressed data, was "groupdocs_signature_cloud-24.4.tar", last modified: Thu Apr 18 06:58:59 2024, max compression
```

## Comparing `groupdocs-signature-cloud-23.6.tar` & `groupdocs_signature_cloud-24.4.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/
--rw-rw-rw-   0        0        0     1107 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/LICENSE
--rw-rw-rw-   0        0        0     2879 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/
--rw-rw-rw-   0        0        0     8368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/__init__.py
--rw-rw-rw-   0        0        0    27395 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_client.py
--rw-rw-rw-   0        0        0     2674 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_exception.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/
--rw-rw-rw-   0        0        0      524 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0    38653 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/file_api.py
--rw-rw-rw-   0        0        0    36263 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/folder_api.py
--rw-rw-rw-   0        0        0    18368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/info_api.py
--rw-rw-rw-   0        0        0     6591 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/license_api.py
--rw-rw-rw-   0        0        0     8868 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/preview_api.py
--rw-rw-rw-   0        0        0    30932 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/sign_api.py
--rw-rw-rw-   0        0        0    26576 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/storage_api.py
--rw-rw-rw-   0        0        0     3306 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/auth.py
--rw-rw-rw-   0        0        0     7680 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/
--rw-rw-rw-   0        0        0     6915 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/__init__.py
--rw-rw-rw-   0        0        0     5895 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_signature.py
--rw-rw-rw-   0        0        0     4063 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_type.py
--rw-rw-rw-   0        0        0     4329 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcodes_result.py
--rw-rw-rw-   0        0        0     4174 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/base_settings.py
--rw-rw-rw-   0        0        0     8339 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/border_line.py
--rw-rw-rw-   0        0        0     4249 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/brush.py
--rw-rw-rw-   0        0        0     4704 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py
--rw-rw-rw-   0        0        0     4043 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/color.py
--rw-rw-rw-   0        0        0     5228 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py
--rw-rw-rw-   0        0        0     5129 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/consumption_result.py
--rw-rw-rw-   0        0        0     6315 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_options.py
--rw-rw-rw-   0        0        0     6513 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_result.py
--rw-rw-rw-   0        0        0     4520 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_settings.py
--rw-rw-rw-   0        0        0     4739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_form_field_signature.py
--rw-rw-rw-   0        0        0     7413 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature.py
--rw-rw-rw-   0        0        0     6147 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature_appearance.py
--rw-rw-rw-   0        0        0     5187 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     6291 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error.py
--rw-rw-rw-   0        0        0     4905 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error_details.py
--rw-rw-rw-   0        0        0     6354 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_info.py
--rw-rw-rw-   0        0        0     5412 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_version.py
--rw-rw-rw-   0        0        0     4151 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4171 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_list.py
--rw-rw-rw-   0        0        0     4884 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     5612 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/form_field_signature.py
--rw-rw-rw-   0        0        0     4900 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/format.py
--rw-rw-rw-   0        0        0     4186 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/formats_result.py
--rw-rw-rw-   0        0        0     7876 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_appearance.py
--rw-rw-rw-   0        0        0     5172 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_signature.py
--rw-rw-rw-   0        0        0    12903 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_result.py
--rw-rw-rw-   0        0        0     5112 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_settings.py
--rw-rw-rw-   0        0        0     6082 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/linear_gradient_brush.py
--rw-rw-rw-   0        0        0    11168 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/metadata_signature.py
--rw-rw-rw-   0        0        0     5178 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/object_exist.py
--rw-rw-rw-   0        0        0     7705 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/options_base.py
--rw-rw-rw-   0        0        0     7507 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/padding.py
--rw-rw-rw-   0        0        0     7879 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/page_info.py
--rw-rw-rw-   0        0        0     7966 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pages_setup.py
--rw-rw-rw-   0        0        0     9110 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature.py
--rw-rw-rw-   0        0        0    11924 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py
--rw-rw-rw-   0        0        0    11570 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py
--rw-rw-rw-   0        0        0     8108 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py
--rw-rw-rw-   0        0        0     6566 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_page.py
--rw-rw-rw-   0        0        0     6502 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_result.py
--rw-rw-rw-   0        0        0     9611 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_settings.py
--rw-rw-rw-   0        0        0     5884 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_signature.py
--rw-rw-rw-   0        0        0     4059 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_type.py
--rw-rw-rw-   0        0        0     4319 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_codes_result.py
--rw-rw-rw-   0        0        0     5331 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radial_gradient_brush.py
--rw-rw-rw-   0        0        0     5238 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py
--rw-rw-rw-   0        0        0     6286 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/save_options.py
--rw-rw-rw-   0        0        0     6984 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_barcode_options.py
--rw-rw-rw-   0        0        0     3779 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_digital_options.py
--rw-rw-rw-   0        0        0     3733 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_options.py
--rw-rw-rw-   0        0        0     6972 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_qr_code_options.py
--rw-rw-rw-   0        0        0     5780 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_result.py
--rw-rw-rw-   0        0        0     4553 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_settings.py
--rw-rw-rw-   0        0        0     8267 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_barcode_options.py
--rw-rw-rw-   0        0        0    10300 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_digital_options.py
--rw-rw-rw-   0        0        0    21424 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_image_options.py
--rw-rw-rw-   0        0        0     4621 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_options.py
--rw-rw-rw-   0        0        0     9592 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_qr_code_options.py
--rw-rw-rw-   0        0        0     7283 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_result.py
--rw-rw-rw-   0        0        0     5389 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_settings.py
--rw-rw-rw-   0        0        0    11298 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_stamp_options.py
--rw-rw-rw-   0        0        0    31381 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_text_options.py
--rw-rw-rw-   0        0        0    13462 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature.py
--rw-rw-rw-   0        0        0     5115 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_appearance.py
--rw-rw-rw-   0        0        0     7507 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_font.py
--rw-rw-rw-   0        0        0     4409 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/solid_brush.py
--rw-rw-rw-   0        0        0    12435 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/stamp_line.py
--rw-rw-rw-   0        0        0     4276 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7173 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_file.py
--rw-rw-rw-   0        0        0     4481 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_form_field_signature.py
--rw-rw-rw-   0        0        0     5394 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_signature.py
--rw-rw-rw-   0        0        0     4575 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/texture_brush.py
--rw-rw-rw-   0        0        0     5369 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/time_stamp.py
--rw-rw-rw-   0        0        0    11389 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_options.py
--rw-rw-rw-   0        0        0     6517 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_result.py
--rw-rw-rw-   0        0        0     4520 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_settings.py
--rw-rw-rw-   0        0        0     4619 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_barcode_options.py
--rw-rw-rw-   0        0        0    11057 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_digital_options.py
--rw-rw-rw-   0        0        0     3718 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_options.py
--rw-rw-rw-   0        0        0     4603 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_qr_code_options.py
--rw-rw-rw-   0        0        0     5980 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_result.py
--rw-rw-rw-   0        0        0     4522 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_settings.py
--rw-rw-rw-   0        0        0     5926 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_text_options.py
--rw-rw-rw-   0        0        0    13739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/rest.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/
--rw-rw-rw-   0        0        0     2879 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6441 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/setup.cfg
--rw-rw-rw-   0        0        0     1665 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/
--rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Search/
--rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/__init__.py
--rw-rw-rw-   0        0        0     5189 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_barcode.py
--rw-rw-rw-   0        0        0     6450 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_collection.py
--rw-rw-rw-   0        0        0     4035 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_digital.py
--rw-rw-rw-   0        0        0     5171 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Search/test_search_qr_code.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/
--rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/__init__.py
--rw-rw-rw-   0        0        0     5969 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_barcode.py
--rw-rw-rw-   0        0        0    16368 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_collection.py
--rw-rw-rw-   0        0        0     5009 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_digital.py
--rw-rw-rw-   0        0        0     5395 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_image.py
--rw-rw-rw-   0        0        0     5921 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_qr_code.py
--rw-rw-rw-   0        0        0     8163 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_stamp.py
--rw-rw-rw-   0        0        0     5929 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_text.py
-drwxrwxrwx   0        0        0        0 2023-06-23 08:36:10.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/
--rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/__init__.py
--rw-rw-rw-   0        0        0     4121 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_barcode.py
--rw-rw-rw-   0        0        0     6232 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_collection.py
--rw-rw-rw-   0        0        0     3655 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_digital.py
--rw-rw-rw-   0        0        0     4107 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_qr_code.py
--rw-rw-rw-   0        0        0     3873 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_text.py
--rw-rw-rw-   0        0        0        0 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_auth_api.py
--rw-rw-rw-   0        0        0     3796 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_file_api.py
--rw-rw-rw-   0        0        0     3141 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_folder_api.py
--rw-rw-rw-   0        0        0     3658 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_info_api.py
--rw-rw-rw-   0        0        0     2732 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/apis/test_storage_api.py
--rw-rw-rw-   0        0        0     4739 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_context.py
--rw-rw-rw-   0        0        0     4965 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_file.py
--rw-rw-rw-   0        0        0     1703 2023-06-23 08:35:47.000000 groupdocs-signature-cloud-23.6/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.590199 groupdocs_signature_cloud-24.4/
+-rw-rw-rw-   0        0        0     1107 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/LICENSE
+-rw-rw-rw-   0        0        0     2991 2024-04-18 06:58:59.587204 groupdocs_signature_cloud-24.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.334291 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/
+-rw-rw-rw-   0        0        0     8368 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/__init__.py
+-rw-rw-rw-   0        0        0    27413 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/api_client.py
+-rw-rw-rw-   0        0        0     2674 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/api_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.362218 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/
+-rw-rw-rw-   0        0        0      524 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0    38653 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/file_api.py
+-rw-rw-rw-   0        0        0    36263 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/folder_api.py
+-rw-rw-rw-   0        0        0    18368 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/info_api.py
+-rw-rw-rw-   0        0        0     6591 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/license_api.py
+-rw-rw-rw-   0        0        0     8868 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/preview_api.py
+-rw-rw-rw-   0        0        0    30932 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/sign_api.py
+-rw-rw-rw-   0        0        0    26576 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/storage_api.py
+-rw-rw-rw-   0        0        0     3306 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/auth.py
+-rw-rw-rw-   0        0        0     7680 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.535198 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/
+-rw-rw-rw-   0        0        0     6984 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/__init__.py
+-rw-rw-rw-   0        0        0     5895 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcode_signature.py
+-rw-rw-rw-   0        0        0     4063 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcode_type.py
+-rw-rw-rw-   0        0        0     4329 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcodes_result.py
+-rw-rw-rw-   0        0        0     4174 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/base_settings.py
+-rw-rw-rw-   0        0        0     8339 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/border_line.py
+-rw-rw-rw-   0        0        0     4249 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/brush.py
+-rw-rw-rw-   0        0        0     4704 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/checkbox_form_field_signature.py
+-rw-rw-rw-   0        0        0     4043 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/color.py
+-rw-rw-rw-   0        0        0     5228 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/combobox_form_field_signature.py
+-rw-rw-rw-   0        0        0     5129 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/consumption_result.py
+-rw-rw-rw-   0        0        0     6315 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_options.py
+-rw-rw-rw-   0        0        0     6513 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_result.py
+-rw-rw-rw-   0        0        0     4520 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_settings.py
+-rw-rw-rw-   0        0        0     4739 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_form_field_signature.py
+-rw-rw-rw-   0        0        0     7413 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_signature.py
+-rw-rw-rw-   0        0        0     6147 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_signature_appearance.py
+-rw-rw-rw-   0        0        0     7338 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_vba.py
+-rw-rw-rw-   0        0        0     5187 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     6291 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/error.py
+-rw-rw-rw-   0        0        0     4905 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/error_details.py
+-rw-rw-rw-   0        0        0     6354 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5412 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4151 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4171 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4884 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     5612 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/form_field_signature.py
+-rw-rw-rw-   0        0        0     4900 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/format.py
+-rw-rw-rw-   0        0        0     4186 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/formats_result.py
+-rw-rw-rw-   0        0        0     7876 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/image_appearance.py
+-rw-rw-rw-   0        0        0     5172 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/image_signature.py
+-rw-rw-rw-   0        0        0    12903 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/info_result.py
+-rw-rw-rw-   0        0        0     5112 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/info_settings.py
+-rw-rw-rw-   0        0        0     6082 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/linear_gradient_brush.py
+-rw-rw-rw-   0        0        0    11168 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/metadata_signature.py
+-rw-rw-rw-   0        0        0     5178 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     7705 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/options_base.py
+-rw-rw-rw-   0        0        0     7507 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/padding.py
+-rw-rw-rw-   0        0        0     7879 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/page_info.py
+-rw-rw-rw-   0        0        0     7966 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pages_setup.py
+-rw-rw-rw-   0        0        0     9110 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_digital_signature.py
+-rw-rw-rw-   0        0        0    11924 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py
+-rw-rw-rw-   0        0        0    11570 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py
+-rw-rw-rw-   0        0        0     8108 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py
+-rw-rw-rw-   0        0        0     6566 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_page.py
+-rw-rw-rw-   0        0        0     6502 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_result.py
+-rw-rw-rw-   0        0        0     9611 2024-04-18 06:58:20.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_settings.py
+-rw-rw-rw-   0        0        0     5884 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_code_signature.py
+-rw-rw-rw-   0        0        0     4059 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_code_type.py
+-rw-rw-rw-   0        0        0     4319 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_codes_result.py
+-rw-rw-rw-   0        0        0     5331 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/radial_gradient_brush.py
+-rw-rw-rw-   0        0        0     5238 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/radio_button_form_field_signature.py
+-rw-rw-rw-   0        0        0     6286 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/save_options.py
+-rw-rw-rw-   0        0        0     6984 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_barcode_options.py
+-rw-rw-rw-   0        0        0     3779 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_digital_options.py
+-rw-rw-rw-   0        0        0     3733 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_options.py
+-rw-rw-rw-   0        0        0     6972 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_qr_code_options.py
+-rw-rw-rw-   0        0        0     5780 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_result.py
+-rw-rw-rw-   0        0        0     4553 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_settings.py
+-rw-rw-rw-   0        0        0     8267 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_barcode_options.py
+-rw-rw-rw-   0        0        0    12605 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_digital_options.py
+-rw-rw-rw-   0        0        0    21424 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_image_options.py
+-rw-rw-rw-   0        0        0     4621 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_options.py
+-rw-rw-rw-   0        0        0     9592 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_qr_code_options.py
+-rw-rw-rw-   0        0        0     7283 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_result.py
+-rw-rw-rw-   0        0        0     5389 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_settings.py
+-rw-rw-rw-   0        0        0    11298 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_stamp_options.py
+-rw-rw-rw-   0        0        0    31381 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_text_options.py
+-rw-rw-rw-   0        0        0    13462 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature.py
+-rw-rw-rw-   0        0        0     5115 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature_appearance.py
+-rw-rw-rw-   0        0        0     7507 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature_font.py
+-rw-rw-rw-   0        0        0     4409 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/solid_brush.py
+-rw-rw-rw-   0        0        0    12435 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/stamp_line.py
+-rw-rw-rw-   0        0        0     4276 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7173 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/storage_file.py
+-rw-rw-rw-   0        0        0     4481 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/text_form_field_signature.py
+-rw-rw-rw-   0        0        0     5394 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/text_signature.py
+-rw-rw-rw-   0        0        0     4575 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/texture_brush.py
+-rw-rw-rw-   0        0        0     5369 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/time_stamp.py
+-rw-rw-rw-   0        0        0    11389 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_options.py
+-rw-rw-rw-   0        0        0     6517 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_result.py
+-rw-rw-rw-   0        0        0     4520 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_settings.py
+-rw-rw-rw-   0        0        0     4619 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_barcode_options.py
+-rw-rw-rw-   0        0        0    11057 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_digital_options.py
+-rw-rw-rw-   0        0        0     3718 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_options.py
+-rw-rw-rw-   0        0        0     4603 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_qr_code_options.py
+-rw-rw-rw-   0        0        0     5980 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_result.py
+-rw-rw-rw-   0        0        0     4522 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_settings.py
+-rw-rw-rw-   0        0        0     5926 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_text_options.py
+-rw-rw-rw-   0        0        0    13739 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.585198 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/
+-rw-rw-rw-   0        0        0     2991 2024-04-18 06:58:58.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6489 2024-04-18 06:58:58.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:58:58.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-18 06:58:58.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-18 06:58:58.000000 groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:58:59.590199 groupdocs_signature_cloud-24.4/setup.cfg
+-rw-rw-rw-   0        0        0     1665 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.540207 groupdocs_signature_cloud-24.4/test/
+-rw-rw-rw-   0        0        0        0 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.551201 groupdocs_signature_cloud-24.4/test/apis/
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.559204 groupdocs_signature_cloud-24.4/test/apis/Search/
+-rw-rw-rw-   0        0        0        0 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Search/__init__.py
+-rw-rw-rw-   0        0        0     5189 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Search/test_search_barcode.py
+-rw-rw-rw-   0        0        0     6450 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Search/test_search_collection.py
+-rw-rw-rw-   0        0        0     4035 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Search/test_search_digital.py
+-rw-rw-rw-   0        0        0     5171 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Search/test_search_qr_code.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.569207 groupdocs_signature_cloud-24.4/test/apis/Sign/
+-rw-rw-rw-   0        0        0        0 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/__init__.py
+-rw-rw-rw-   0        0        0     5969 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_barcode.py
+-rw-rw-rw-   0        0        0    16368 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_collection.py
+-rw-rw-rw-   0        0        0     5009 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_digital.py
+-rw-rw-rw-   0        0        0     5395 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_image.py
+-rw-rw-rw-   0        0        0     5921 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_qr_code.py
+-rw-rw-rw-   0        0        0     8163 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_stamp.py
+-rw-rw-rw-   0        0        0     5929 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_text.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:58:59.583196 groupdocs_signature_cloud-24.4/test/apis/Verify/
+-rw-rw-rw-   0        0        0        0 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/__init__.py
+-rw-rw-rw-   0        0        0     4121 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_barcode.py
+-rw-rw-rw-   0        0        0     6232 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_collection.py
+-rw-rw-rw-   0        0        0     3655 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_digital.py
+-rw-rw-rw-   0        0        0     4107 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_qr_code.py
+-rw-rw-rw-   0        0        0     3873 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_text.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/__init__.py
+-rw-rw-rw-   0        0        0     3022 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/test_auth_api.py
+-rw-rw-rw-   0        0        0     3796 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/test_file_api.py
+-rw-rw-rw-   0        0        0     3141 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/test_folder_api.py
+-rw-rw-rw-   0        0        0     3658 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/test_info_api.py
+-rw-rw-rw-   0        0        0     2732 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/apis/test_storage_api.py
+-rw-rw-rw-   0        0        0     4739 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/test_context.py
+-rw-rw-rw-   0        0        0     4965 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/test_file.py
+-rw-rw-rw-   0        0        0     1703 2024-04-18 06:58:21.000000 groupdocs_signature_cloud-24.4/test/test_settings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `groupdocs-signature-cloud-23.6/LICENSE` & `groupdocs_signature_cloud-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/PKG-INFO` & `groupdocs_signature_cloud-24.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-signature-cloud
-Version: 23.6
+Version: 24.4
 Summary: GroupDocs.Signature Cloud Python SDK
 Home-page: http://github.com/groupdocs-signature-cloud/groupdocs-signature-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,signature,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3>=1.15
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
 
 # GroupDocs.Signature Cloud Python SDK
 Python package for communicating with the GroupDocs.Signature Cloud API
 
 ## Requirements
 
 Python 2.7 or 3.4+
```

### Comparing `groupdocs-signature-cloud-23.6/README.md` & `groupdocs_signature_cloud-24.4/README.md`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/__init__.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_client.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     }
 
     def __init__(self, configuration, header_name=None, header_value=None,
                  cookie=None):
         self.configuration = configuration
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '23.6'}
+        self.default_headers = {'x-groupdocs-client': 'python sdk', 'x-groupdocs-version': '24.4'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 23.6'
+        self.user_agent = 'python sdk 24.4'
 
     def __del__(self):
         if self.pool is not None:
             self.pool.close()
             self.pool.join()
 
     @property
@@ -531,15 +531,15 @@
         os.remove(path)
 
         content_disposition = response.getheader("Content-Disposition")
         if content_disposition:
             filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
                                  content_disposition).group(1)
             filename = filename.replace('/', '_')
-            path = os.path.join(os.path.dirname(path), filename)
+            path = os.path.join(os.path.dirname(path), os.path.basename(filename))
 
         with open(path, "wb") as f:
             f.write(response.data)
 
         return path
 
     def __deserialize_primitive(self, data, klass):
```

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/api_exception.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/api_exception.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/__init__.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/file_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/folder_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/info_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/license_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/license_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/preview_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/preview_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/sign_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/sign_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/apis/storage_api.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/apis/storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/auth.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/auth.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/configuration.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,10 +198,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.6\n"\
-               "SDK Package Version: 23.6".\
+               "Version of the API: 24.4\n"\
+               "SDK Package Version: 24.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/__init__.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from groupdocs_signature_cloud.models.base_settings import BaseSettings
 from groupdocs_signature_cloud.models.border_line import BorderLine
 from groupdocs_signature_cloud.models.brush import Brush
 from groupdocs_signature_cloud.models.color import Color
 from groupdocs_signature_cloud.models.consumption_result import ConsumptionResult
 from groupdocs_signature_cloud.models.delete_options import DeleteOptions
 from groupdocs_signature_cloud.models.delete_result import DeleteResult
+from groupdocs_signature_cloud.models.digital_vba import DigitalVBA
 from groupdocs_signature_cloud.models.disc_usage import DiscUsage
 from groupdocs_signature_cloud.models.error import Error
 from groupdocs_signature_cloud.models.error_details import ErrorDetails
 from groupdocs_signature_cloud.models.file_info import FileInfo
 from groupdocs_signature_cloud.models.file_versions import FileVersions
 from groupdocs_signature_cloud.models.files_list import FilesList
 from groupdocs_signature_cloud.models.files_upload_result import FilesUploadResult
```

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcode_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcode_type.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcode_type.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/barcodes_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/barcodes_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/base_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/base_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/border_line.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/border_line.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/brush.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/brush.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/checkbox_form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/checkbox_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/color.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/color.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/combobox_form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/combobox_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/consumption_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/consumption_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/delete_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/delete_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/digital_signature_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/digital_signature_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/disc_usage.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/error.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/error_details.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_info.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_version.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/file_versions.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_list.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/files_upload_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/format.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/format.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/formats_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/formats_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/image_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/image_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/image_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/info_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/info_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/info_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/linear_gradient_brush.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/linear_gradient_brush.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/metadata_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/metadata_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/object_exist.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/options_base.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/options_base.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/padding.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/padding.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/page_info.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/page_info.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pages_setup.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pages_setup.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_digital_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_digital_signature_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_text_annotation_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/pdf_text_sticker_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_page.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_page.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/preview_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/preview_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_code_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_code_type.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_code_type.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/qr_codes_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/qr_codes_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radial_gradient_brush.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/radial_gradient_brush.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/radio_button_form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/radio_button_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/save_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/save_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_barcode_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_barcode_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_digital_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_digital_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_qr_code_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_qr_code_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/search_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/search_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_barcode_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_barcode_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_digital_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_qr_code_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 # -----------------------------------------------------------------------------------
-# <copyright company="Aspose Pty Ltd" file="SignDigitalOptions.py">
+# <copyright company="Aspose Pty Ltd" file="SignQRCodeOptions.py">
 #   Copyright (c) 2003-2023 Aspose Pty Ltd
 # </copyright>
 # <summary>
 #   Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -26,259 +26,201 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from groupdocs_signature_cloud.models import SignImageOptions
+from groupdocs_signature_cloud.models import SignTextOptions
 
-class SignDigitalOptions(SignImageOptions):
+class SignQRCodeOptions(SignTextOptions):
     """
-    Represents the Digital sign options
+    Represents the QR-code signature options
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'reason': 'str',
-        'contact': 'str',
-        'location': 'str',
-        'visible': 'bool',
-        'password': 'str',
-        'certificate_file_path': 'str',
-        'x_ad_es_type': 'str'
+        'qr_code_type': 'str',
+        'transparency': 'float',
+        'code_text_alignment': 'str',
+        'inner_margins': 'Padding',
+        'logo_file_path': 'str'
     }
 
     attribute_map = {
-        'reason': 'Reason',
-        'contact': 'Contact',
-        'location': 'Location',
-        'visible': 'Visible',
-        'password': 'Password',
-        'certificate_file_path': 'CertificateFilePath',
-        'x_ad_es_type': 'XAdESType'
+        'qr_code_type': 'QRCodeType',
+        'transparency': 'Transparency',
+        'code_text_alignment': 'CodeTextAlignment',
+        'inner_margins': 'InnerMargins',
+        'logo_file_path': 'LogoFilePath'
     }
 
-    def __init__(self, reason=None, contact=None, location=None, visible=None, password=None, certificate_file_path=None, x_ad_es_type=None, **kwargs):  # noqa: E501
-        """Initializes new instance of SignDigitalOptions"""  # noqa: E501
+    def __init__(self, qr_code_type=None, transparency=None, code_text_alignment=None, inner_margins=None, logo_file_path=None, **kwargs):  # noqa: E501
+        """Initializes new instance of SignQRCodeOptions"""  # noqa: E501
 
-        self._reason = None
-        self._contact = None
-        self._location = None
-        self._visible = None
-        self._password = None
-        self._certificate_file_path = None
-        self._x_ad_es_type = None
-
-        if reason is not None:
-            self.reason = reason
-        if contact is not None:
-            self.contact = contact
-        if location is not None:
-            self.location = location
-        if visible is not None:
-            self.visible = visible
-        if password is not None:
-            self.password = password
-        if certificate_file_path is not None:
-            self.certificate_file_path = certificate_file_path
-        if x_ad_es_type is not None:
-            self.x_ad_es_type = x_ad_es_type
+        self._qr_code_type = None
+        self._transparency = None
+        self._code_text_alignment = None
+        self._inner_margins = None
+        self._logo_file_path = None
+
+        if qr_code_type is not None:
+            self.qr_code_type = qr_code_type
+        if transparency is not None:
+            self.transparency = transparency
+        if code_text_alignment is not None:
+            self.code_text_alignment = code_text_alignment
+        if inner_margins is not None:
+            self.inner_margins = inner_margins
+        if logo_file_path is not None:
+            self.logo_file_path = logo_file_path
 
-        base = super(SignDigitalOptions, self)
+        base = super(SignQRCodeOptions, self)
         base.__init__(**kwargs)
 
         self.swagger_types.update(base.swagger_types)
         self.attribute_map.update(base.attribute_map)
     
     @property
-    def reason(self):
+    def qr_code_type(self):
         """
-        Gets the reason.  # noqa: E501
+        Gets the qr_code_type.  # noqa: E501
 
-        Gets or sets the reason of signature.  # noqa: E501
+        Get or set QRCode type. Value should be one from supported QRCode types list  # noqa: E501
 
-        :return: The reason.  # noqa: E501
+        :return: The qr_code_type.  # noqa: E501
         :rtype: str
         """
-        return self._reason
+        return self._qr_code_type
 
-    @reason.setter
-    def reason(self, reason):
+    @qr_code_type.setter
+    def qr_code_type(self, qr_code_type):
         """
-        Sets the reason.
+        Sets the qr_code_type.
 
-        Gets or sets the reason of signature.  # noqa: E501
+        Get or set QRCode type. Value should be one from supported QRCode types list  # noqa: E501
 
-        :param reason: The reason.  # noqa: E501
+        :param qr_code_type: The qr_code_type.  # noqa: E501
         :type: str
         """
-        self._reason = reason
+        self._qr_code_type = qr_code_type
     
     @property
-    def contact(self):
+    def transparency(self):
         """
-        Gets the contact.  # noqa: E501
+        Gets the transparency.  # noqa: E501
 
-        Gets or sets the signature contact.  # noqa: E501
+        Gets or sets the signature transparency (value from 0.0 (opaque) through 1.0 (clear)). Default value is 0 (opaque).               # noqa: E501
 
-        :return: The contact.  # noqa: E501
-        :rtype: str
-        """
-        return self._contact
-
-    @contact.setter
-    def contact(self, contact):
-        """
-        Sets the contact.
-
-        Gets or sets the signature contact.  # noqa: E501
-
-        :param contact: The contact.  # noqa: E501
-        :type: str
-        """
-        self._contact = contact
-    
-    @property
-    def location(self):
-        """
-        Gets the location.  # noqa: E501
-
-        Gets or sets the signature location.  # noqa: E501
-
-        :return: The location.  # noqa: E501
-        :rtype: str
-        """
-        return self._location
-
-    @location.setter
-    def location(self, location):
+        :return: The transparency.  # noqa: E501
+        :rtype: float
         """
-        Sets the location.
+        return self._transparency
 
-        Gets or sets the signature location.  # noqa: E501
-
-        :param location: The location.  # noqa: E501
-        :type: str
-        """
-        self._location = location
-    
-    @property
-    def visible(self):
-        """
-        Gets the visible.  # noqa: E501
-
-        Gets or sets the visibility of signature.  # noqa: E501
-
-        :return: The visible.  # noqa: E501
-        :rtype: bool
+    @transparency.setter
+    def transparency(self, transparency):
         """
-        return self._visible
+        Sets the transparency.
 
-    @visible.setter
-    def visible(self, visible):
-        """
-        Sets the visible.
-
-        Gets or sets the visibility of signature.  # noqa: E501
+        Gets or sets the signature transparency (value from 0.0 (opaque) through 1.0 (clear)). Default value is 0 (opaque).               # noqa: E501
 
-        :param visible: The visible.  # noqa: E501
-        :type: bool
+        :param transparency: The transparency.  # noqa: E501
+        :type: float
         """
-        if visible is None:
-            raise ValueError("Invalid value for `visible`, must not be `None`")  # noqa: E501
-        self._visible = visible
+        if transparency is None:
+            raise ValueError("Invalid value for `transparency`, must not be `None`")  # noqa: E501
+        self._transparency = transparency
     
     @property
-    def password(self):
+    def code_text_alignment(self):
         """
-        Gets the password.  # noqa: E501
+        Gets the code_text_alignment.  # noqa: E501
 
-        Gets or sets the password of digital certificate  # noqa: E501
+        Gets or sets the alignment of text in the result QR-code Default value is None  # noqa: E501
 
-        :return: The password.  # noqa: E501
+        :return: The code_text_alignment.  # noqa: E501
         :rtype: str
         """
-        return self._password
+        return self._code_text_alignment
 
-    @password.setter
-    def password(self, password):
+    @code_text_alignment.setter
+    def code_text_alignment(self, code_text_alignment):
         """
-        Sets the password.
+        Sets the code_text_alignment.
 
-        Gets or sets the password of digital certificate  # noqa: E501
+        Gets or sets the alignment of text in the result QR-code Default value is None  # noqa: E501
 
-        :param password: The password.  # noqa: E501
+        :param code_text_alignment: The code_text_alignment.  # noqa: E501
         :type: str
         """
-        self._password = password
+        if code_text_alignment is None:
+            raise ValueError("Invalid value for `code_text_alignment`, must not be `None`")  # noqa: E501
+        allowed_values = ["None", "Above", "Below", "Right"]  # noqa: E501
+        if not code_text_alignment.isdigit():	
+            if code_text_alignment not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `code_text_alignment` ({0}), must be one of {1}"  # noqa: E501
+                    .format(code_text_alignment, allowed_values))
+            self._code_text_alignment = code_text_alignment
+        else:
+            self._code_text_alignment = allowed_values[int(code_text_alignment) if six.PY3 else long(code_text_alignment)]
     
     @property
-    def certificate_file_path(self):
+    def inner_margins(self):
         """
-        Gets the certificate_file_path.  # noqa: E501
+        Gets the inner_margins.  # noqa: E501
 
-        Gets or sets the digital certificate file GUID  # noqa: E501
+        Gets or sets the space between QRCode elements and result image borders  # noqa: E501
 
-        :return: The certificate_file_path.  # noqa: E501
-        :rtype: str
+        :return: The inner_margins.  # noqa: E501
+        :rtype: Padding
         """
-        return self._certificate_file_path
+        return self._inner_margins
 
-    @certificate_file_path.setter
-    def certificate_file_path(self, certificate_file_path):
+    @inner_margins.setter
+    def inner_margins(self, inner_margins):
         """
-        Sets the certificate_file_path.
+        Sets the inner_margins.
 
-        Gets or sets the digital certificate file GUID  # noqa: E501
+        Gets or sets the space between QRCode elements and result image borders  # noqa: E501
 
-        :param certificate_file_path: The certificate_file_path.  # noqa: E501
-        :type: str
+        :param inner_margins: The inner_margins.  # noqa: E501
+        :type: Padding
         """
-        self._certificate_file_path = certificate_file_path
+        self._inner_margins = inner_margins
     
     @property
-    def x_ad_es_type(self):
+    def logo_file_path(self):
         """
-        Gets the x_ad_es_type.  # noqa: E501
+        Gets the logo_file_path.  # noqa: E501
 
-        XAdES type GroupDocs.Signature.Options.DigitalSignOptions.XAdESType. Default value is None (XAdES is off). At this moment XAdES signature type is supported only for Spreadsheet documents.               # noqa: E501
+        Gets or sets the QR-code logo image file name. This property in use only if LogoStream is not specified. Using of this property could cause problems with verification. Use it carefully  # noqa: E501
 
-        :return: The x_ad_es_type.  # noqa: E501
+        :return: The logo_file_path.  # noqa: E501
         :rtype: str
         """
-        return self._x_ad_es_type
+        return self._logo_file_path
 
-    @x_ad_es_type.setter
-    def x_ad_es_type(self, x_ad_es_type):
+    @logo_file_path.setter
+    def logo_file_path(self, logo_file_path):
         """
-        Sets the x_ad_es_type.
+        Sets the logo_file_path.
 
-        XAdES type GroupDocs.Signature.Options.DigitalSignOptions.XAdESType. Default value is None (XAdES is off). At this moment XAdES signature type is supported only for Spreadsheet documents.               # noqa: E501
+        Gets or sets the QR-code logo image file name. This property in use only if LogoStream is not specified. Using of this property could cause problems with verification. Use it carefully  # noqa: E501
 
-        :param x_ad_es_type: The x_ad_es_type.  # noqa: E501
+        :param logo_file_path: The logo_file_path.  # noqa: E501
         :type: str
         """
-        if x_ad_es_type is None:
-            raise ValueError("Invalid value for `x_ad_es_type`, must not be `None`")  # noqa: E501
-        allowed_values = ["None", "XAdES"]  # noqa: E501
-        if not x_ad_es_type.isdigit():	
-            if x_ad_es_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `x_ad_es_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(x_ad_es_type, allowed_values))
-            self._x_ad_es_type = x_ad_es_type
-        else:
-            self._x_ad_es_type = allowed_values[int(x_ad_es_type) if six.PY3 else long(x_ad_es_type)]
+        self._logo_file_path = logo_file_path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -306,15 +248,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SignDigitalOptions):
+        if not isinstance(other, SignQRCodeOptions):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_image_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_image_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_stamp_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_stamp_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/sign_text_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/sign_text_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_appearance.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature_appearance.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/signature_font.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/signature_font.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/solid_brush.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/solid_brush.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/stamp_line.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/stamp_line.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_exist.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/storage_file.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_form_field_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/text_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/text_signature.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/text_signature.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/texture_brush.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/texture_brush.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/time_stamp.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/time_stamp.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/update_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/update_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_barcode_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_barcode_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_digital_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_digital_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_qr_code_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_qr_code_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_result.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_result.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_settings.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_settings.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/models/verify_text_options.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/models/verify_text_options.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud/rest.py` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/PKG-INFO` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupdocs-signature-cloud
-Version: 23.6
+Version: 24.4
 Summary: GroupDocs.Signature Cloud Python SDK
 Home-page: http://github.com/groupdocs-signature-cloud/groupdocs-signature-cloud-python
 Author: GroupDocs
 Author-email: support@groupdocs.cloud
 Keywords: groupdocs,signature,cloud,python,sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: urllib3>=1.15
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
 
 # GroupDocs.Signature Cloud Python SDK
 Python package for communicating with the GroupDocs.Signature Cloud API
 
 ## Requirements
 
 Python 2.7 or 3.4+
```

### Comparing `groupdocs-signature-cloud-23.6/groupdocs_signature_cloud.egg-info/SOURCES.txt` & `groupdocs_signature_cloud-24.4/groupdocs_signature_cloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 groupdocs_signature_cloud/models/consumption_result.py
 groupdocs_signature_cloud/models/delete_options.py
 groupdocs_signature_cloud/models/delete_result.py
 groupdocs_signature_cloud/models/delete_settings.py
 groupdocs_signature_cloud/models/digital_form_field_signature.py
 groupdocs_signature_cloud/models/digital_signature.py
 groupdocs_signature_cloud/models/digital_signature_appearance.py
+groupdocs_signature_cloud/models/digital_vba.py
 groupdocs_signature_cloud/models/disc_usage.py
 groupdocs_signature_cloud/models/error.py
 groupdocs_signature_cloud/models/error_details.py
 groupdocs_signature_cloud/models/file_info.py
 groupdocs_signature_cloud/models/file_version.py
 groupdocs_signature_cloud/models/file_versions.py
 groupdocs_signature_cloud/models/files_list.py
```

### Comparing `groupdocs-signature-cloud-23.6/setup.py` & `groupdocs_signature_cloud-24.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import datetime
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "groupdocs-signature-cloud"
-VERSION = "23.6"
+VERSION = "24.4"
 
 # Append current time to the version when publishing to test environment
 if "--test" in sys.argv:
     VERSION += "." + datetime.datetime.now().strftime("%Y%m%d%H%M")
     sys.argv.remove("--test")
 
 # To install the library, run the following
```

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_barcode.py` & `groupdocs_signature_cloud-24.4/test/apis/Search/test_search_barcode.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_collection.py` & `groupdocs_signature_cloud-24.4/test/apis/Search/test_search_collection.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_digital.py` & `groupdocs_signature_cloud-24.4/test/apis/Search/test_search_digital.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Search/test_search_qr_code.py` & `groupdocs_signature_cloud-24.4/test/apis/Search/test_search_qr_code.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_barcode.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_barcode.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_collection.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_collection.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_digital.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_digital.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_image.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_image.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_qr_code.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_qr_code.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_stamp.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_stamp.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Sign/test_sign_text.py` & `groupdocs_signature_cloud-24.4/test/apis/Sign/test_sign_text.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_barcode.py` & `groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_barcode.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_collection.py` & `groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_collection.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_digital.py` & `groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_digital.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_qr_code.py` & `groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_qr_code.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/Verify/test_verify_text.py` & `groupdocs_signature_cloud-24.4/test/apis/Verify/test_verify_text.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/test_auth_api.py` & `groupdocs_signature_cloud-24.4/test/apis/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/test_file_api.py` & `groupdocs_signature_cloud-24.4/test/apis/test_file_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/test_folder_api.py` & `groupdocs_signature_cloud-24.4/test/apis/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/test_info_api.py` & `groupdocs_signature_cloud-24.4/test/apis/test_info_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/apis/test_storage_api.py` & `groupdocs_signature_cloud-24.4/test/apis/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/test_context.py` & `groupdocs_signature_cloud-24.4/test/test_context.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/test_file.py` & `groupdocs_signature_cloud-24.4/test/test_file.py`

 * *Files identical despite different names*

### Comparing `groupdocs-signature-cloud-23.6/test/test_settings.py` & `groupdocs_signature_cloud-24.4/test/test_settings.py`

 * *Files identical despite different names*

