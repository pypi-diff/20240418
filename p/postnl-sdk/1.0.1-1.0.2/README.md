# Comparing `tmp/postnl-sdk-1.0.1.tar.gz` & `tmp/postnl_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnl-sdk-1.0.1.tar", last modified: Thu Apr 11 13:40:03 2024, max compression
+gzip compressed data, was "postnl_sdk-1.0.2.tar", last modified: Thu Apr 18 09:31:14 2024, max compression
```

## Comparing `postnl-sdk-1.0.1.tar` & `postnl_sdk-1.0.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.599769 postnl-sdk-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1213 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4493 2024-04-11 13:40:03.599769 postnl-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3991 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.457764 postnl-sdk-1.0.1/postnl/
--rw-r--r--   0 root         (0) root         (0)      144 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      560 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     5986 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.476765 postnl-sdk-1.0.1/postnl/controllers/
--rw-r--r--   0 root         (0) root         (0)      338 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5149 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/barcode_controller.py
--rw-r--r--   0 root         (0) root         (0)     1713 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     3253 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/checkout_controller.py
--rw-r--r--   0 root         (0) root         (0)     3308 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/confirming_controller.py
--rw-r--r--   0 root         (0) root         (0)    17156 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/deliverydate_controller.py
--rw-r--r--   0 root         (0) root         (0)     3844 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/labelling_controller.py
--rw-r--r--   0 root         (0) root         (0)    18720 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/locations_controller.py
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/postalcode_check_controller.py
--rw-r--r--   0 root         (0) root         (0)     3816 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/shipment_controller.py
--rw-r--r--   0 root         (0) root         (0)     6428 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/timeframes_controller.py
--rw-r--r--   0 root         (0) root         (0)    14360 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/controllers/track_trace_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.484765 postnl-sdk-1.0.1/postnl/exceptions/
--rw-r--r--   0 root         (0) root         (0)      481 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1466 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/barcode_method_not_allowed_exception.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/barcode_response_error_exception.py
--rw-r--r--   0 root         (0) root         (0)     1510 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/barcode_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1460 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/barcode_too_many_request_exception.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/checkout_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1608 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/confirming_response_error_1_exception.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/deliverydate_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1520 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/labelling_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/locations_response_invalid_exception.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/exceptions/timeframe_response_invalid_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.488766 postnl-sdk-1.0.1/postnl/http/
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.490766 postnl-sdk-1.0.1/postnl/http/auth/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/auth/custom_header_authentication.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      486 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1489 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.593769 postnl-sdk-1.0.1/postnl/models/
--rw-r--r--   0 root         (0) root         (0)     2632 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3594 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address.py
--rw-r--r--   0 root         (0) root         (0)     3485 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_1.py
--rw-r--r--   0 root         (0) root         (0)     8732 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_11.py
--rw-r--r--   0 root         (0) root         (0)     8649 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_2.py
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_3.py
--rw-r--r--   0 root         (0) root         (0)     6680 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_4.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/address_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     4567 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/amount.py
--rw-r--r--   0 root         (0) root         (0)     2135 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/amount_1.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/barcode_response.py
--rw-r--r--   0 root         (0) root         (0)     4642 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/checkout_request.py
--rw-r--r--   0 root         (0) root         (0)     3094 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/checkout_response.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/code_enum.py
--rw-r--r--   0 root         (0) root         (0)     1807 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/complete_status.py
--rw-r--r--   0 root         (0) root         (0)     2330 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/confirming_request.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/confirming_response.py
--rw-r--r--   0 root         (0) root         (0)     3278 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/contact.py
--rw-r--r--   0 root         (0) root         (0)     3554 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/content.py
--rw-r--r--   0 root         (0) root         (0)     3489 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/content_1.py
--rw-r--r--   0 root         (0) root         (0)      429 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/countrycode_enum.py
--rw-r--r--   0 root         (0) root         (0)     3845 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/cpc_response.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/currency_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      567 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/currency_enum.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/current_status.py
--rw-r--r--   0 root         (0) root         (0)     9522 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/custom.py
--rw-r--r--   0 root         (0) root         (0)     3959 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     3913 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/customer_1.py
--rw-r--r--   0 root         (0) root         (0)     2403 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/customer_2.py
--rw-r--r--   0 root         (0) root         (0)     2754 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/cut_off_time.py
--rw-r--r--   0 root         (0) root         (0)      965 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/day_enum.py
--rw-r--r--   0 root         (0) root         (0)     2210 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/delivery_option.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/delivery_options.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/delivery_options_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1593 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/detail.py
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/dimension.py
--rw-r--r--   0 root         (0) root         (0)     2894 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/dimension_1.py
--rw-r--r--   0 root         (0) root         (0)     1968 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/error.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/error_1.py
--rw-r--r--   0 root         (0) root         (0)     1909 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/error_2.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/error_3.py
--rw-r--r--   0 root         (0) root         (0)     2219 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/error_4.py
--rw-r--r--   0 root         (0) root         (0)     4022 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/event.py
--rw-r--r--   0 root         (0) root         (0)     1918 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/expectation.py
--rw-r--r--   0 root         (0) root         (0)     1858 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/extra_field.py
--rw-r--r--   0 root         (0) root         (0)     2024 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/fault.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/friday.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/friday_1.py
--rw-r--r--   0 root         (0) root         (0)     1925 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/get_locations_result.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/get_locations_result_1.py
--rw-r--r--   0 root         (0) root         (0)     3060 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/group.py
--rw-r--r--   0 root         (0) root         (0)     6337 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/hazardous_material.py
--rw-r--r--   0 root         (0) root         (0)     2414 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/label.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/label_1.py
--rw-r--r--   0 root         (0) root         (0)     3367 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/labelling_request.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/labelling_response.py
--rw-r--r--   0 root         (0) root         (0)     2760 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/labelling_response_1.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/language_enum.py
--rw-r--r--   0 root         (0) root         (0)     4557 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/location.py
--rw-r--r--   0 root         (0) root         (0)     6563 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/location_1.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/location_response.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/locations_response.py
--rw-r--r--   0 root         (0) root         (0)     2103 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/merged_label.py
--rw-r--r--   0 root         (0) root         (0)     1843 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2326 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/message_1.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/monday.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/monday_1.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/old_status.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/opening_hours.py
--rw-r--r--   0 root         (0) root         (0)      927 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/option_1_enum.py
--rw-r--r--   0 root         (0) root         (0)     1088 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/option_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      802 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/option_3_enum.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/option_enum.py
--rw-r--r--   0 root         (0) root         (0)     1717 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/options.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/options_2_enum.py
--rw-r--r--   0 root         (0) root         (0)     3128 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/pickup_option.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/product_option.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/product_option_1.py
--rw-r--r--   0 root         (0) root         (0)     1773 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/product_options.py
--rw-r--r--   0 root         (0) root         (0)     3352 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/reason_no_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/reason_no_timeframes.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/response_shipment.py
--rw-r--r--   0 root         (0) root         (0)     3245 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/response_shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     3240 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/response_shipment_2.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/saturday.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/saturday_1.py
--rw-r--r--   0 root         (0) root         (0)    18186 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment.py
--rw-r--r--   0 root         (0) root         (0)    18767 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_1.py
--rw-r--r--   0 root         (0) root         (0)     7218 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_11.py
--rw-r--r--   0 root         (0) root         (0)     9395 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_2.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2989 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_v_22_calculate_date_delivery_response.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shipment_v_22_calculate_date_shipping_response.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shippingstatus_response.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shippingstatus_response_signature.py
--rw-r--r--   0 root         (0) root         (0)     3424 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/shippingstatus_response_updated_shipment.py
--rw-r--r--   0 root         (0) root         (0)     2529 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/signature.py
--rw-r--r--   0 root         (0) root         (0)     3362 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/status.py
--rw-r--r--   0 root         (0) root         (0)     3342 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/status_2.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/string_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/string_enum.py
--rw-r--r--   0 root         (0) root         (0)     1831 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/sunday.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/sunday_1.py
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/sustainability.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/thursday.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/thursday_1.py
--rw-r--r--   0 root         (0) root         (0)     3547 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframe.py
--rw-r--r--   0 root         (0) root         (0)     2025 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframe_1.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframe_response.py
--rw-r--r--   0 root         (0) root         (0)     2986 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframe_timeframe.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframes.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/timeframes_1.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/tuesday.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/tuesday_1.py
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/type_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2871 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/warning.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/warning_1.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/warning_11.py
--rw-r--r--   0 root         (0) root         (0)     1867 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/warning_2.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/warnings.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/wednesday.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/models/wednesday_1.py
--rw-r--r--   0 root         (0) root         (0)     3989 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/postnl_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.595769 postnl-sdk-1.0.1/postnl/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/postnl/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 13:40:03.598769 postnl-sdk-1.0.1/postnl_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4493 2024-04-11 13:40:03.000000 postnl-sdk-1.0.1/postnl_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5513 2024-04-11 13:40:03.000000 postnl-sdk-1.0.1/postnl_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 13:40:03.000000 postnl-sdk-1.0.1/postnl_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-11 13:40:03.000000 postnl-sdk-1.0.1/postnl_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 13:40:03.000000 postnl-sdk-1.0.1/postnl_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      717 2024-04-11 13:39:35.000000 postnl-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-11 13:40:03.600769 postnl-sdk-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.490490 postnl_sdk-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4494 2024-04-18 09:31:14.490490 postnl_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.336488 postnl_sdk-1.0.2/postnl/
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      560 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5986 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.346488 postnl_sdk-1.0.2/postnl/controllers/
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/barcode_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/checkout_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/confirming_controller.py
+-rw-r--r--   0 root         (0) root         (0)    17156 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/deliverydate_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/labelling_controller.py
+-rw-r--r--   0 root         (0) root         (0)    18720 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/locations_controller.py
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/postalcode_check_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/shipment_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/timeframes_controller.py
+-rw-r--r--   0 root         (0) root         (0)    14360 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/controllers/track_trace_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.360488 postnl_sdk-1.0.2/postnl/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      481 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/barcode_method_not_allowed_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/barcode_response_error_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/barcode_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/barcode_too_many_request_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/checkout_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/confirming_response_error_1_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/deliverydate_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/labelling_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/locations_response_invalid_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/exceptions/timeframe_response_invalid_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.366488 postnl_sdk-1.0.2/postnl/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.368488 postnl_sdk-1.0.2/postnl/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/auth/custom_header_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      486 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.479490 postnl_sdk-1.0.2/postnl/models/
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_1.py
+-rw-r--r--   0 root         (0) root         (0)     8732 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_11.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_2.py
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_3.py
+-rw-r--r--   0 root         (0) root         (0)     6680 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_4.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/address_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/amount.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/amount_1.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/barcode_response.py
+-rw-r--r--   0 root         (0) root         (0)     4642 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/checkout_request.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/checkout_response.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/code_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/complete_status.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/confirming_request.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/confirming_response.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/contact.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/content.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/content_1.py
+-rw-r--r--   0 root         (0) root         (0)      429 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/countrycode_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3845 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/cpc_response.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/currency_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/currency_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/current_status.py
+-rw-r--r--   0 root         (0) root         (0)     9522 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/custom.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/customer_1.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/customer_2.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/cut_off_time.py
+-rw-r--r--   0 root         (0) root         (0)      965 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/day_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/delivery_option.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/delivery_options.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/delivery_options_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/dimension.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/dimension_1.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/error_1.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/error_2.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/error_3.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/error_4.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/event.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/expectation.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/extra_field.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/fault.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/friday.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/friday_1.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/get_locations_result.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/get_locations_result_1.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/hazardous_material.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/label.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/label_1.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/labelling_request.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/labelling_response.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/labelling_response_1.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/language_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4557 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     6563 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/location_1.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/locations_response.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/merged_label.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/message_1.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/monday.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/monday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/old_status.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/opening_hours.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/option_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/option_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      802 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/option_3_enum.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/option_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/options.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/options_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/pickup_option.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/product_option.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/product_option_1.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/product_options.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/reason_no_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/reason_no_timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/response_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/response_shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/response_shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/saturday.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/saturday_1.py
+-rw-r--r--   0 root         (0) root         (0)    18186 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment.py
+-rw-r--r--   0 root         (0) root         (0)    18767 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_1.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_11.py
+-rw-r--r--   0 root         (0) root         (0)     9395 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_2.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_v_22_calculate_date_delivery_response.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shipment_v_22_calculate_date_shipping_response.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shippingstatus_response.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shippingstatus_response_signature.py
+-rw-r--r--   0 root         (0) root         (0)     3424 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/shippingstatus_response_updated_shipment.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/signature.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/status.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/status_2.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/string_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/string_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/sunday.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/sunday_1.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/sustainability.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/thursday.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/thursday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframe_1.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframe_response.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframe_timeframe.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframes.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/timeframes_1.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/tuesday.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/tuesday_1.py
+-rw-r--r--   0 root         (0) root         (0)      523 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/type_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/warning.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/warning_1.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/warning_11.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/warning_2.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/wednesday.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/models/wednesday_1.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/postnl_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.481490 postnl_sdk-1.0.2/postnl/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/postnl/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:31:14.487490 postnl_sdk-1.0.2/postnl_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4494 2024-04-18 09:31:14.000000 postnl_sdk-1.0.2/postnl_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5513 2024-04-18 09:31:14.000000 postnl_sdk-1.0.2/postnl_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 09:31:14.000000 postnl_sdk-1.0.2/postnl_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-18 09:31:14.000000 postnl_sdk-1.0.2/postnl_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-18 09:31:14.000000 postnl_sdk-1.0.2/postnl_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-18 09:30:43.000000 postnl_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-18 09:31:14.493490 postnl_sdk-1.0.2/setup.cfg
```

### Comparing `postnl-sdk-1.0.1/LICENSE` & `postnl_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/PKG-INFO` & `postnl_sdk-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: postnl-sdk
-Version: 1.0.1
-Summary: Collection of PostNL API's for ecommerce processes
+Version: 1.0.2
+Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/
-Keywords: PostNK,ecommerce,SDK,API
+Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0
 Requires-Dist: apimatic-requests-client-adapter~=0.1.0
 Requires-Dist: enum34>=1.1.10,~=1.1
@@ -24,19 +24,19 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-sdk==1.0.1
+pip install postnl-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
```

### Comparing `postnl-sdk-1.0.1/README.md` & `postnl_sdk-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-sdk==1.0.1
+pip install postnl-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
```

### Comparing `postnl-sdk-1.0.1/postnl/api_helper.py` & `postnl_sdk-1.0.2/postnl/api_helper.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/configuration.py` & `postnl_sdk-1.0.2/postnl/configuration.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/barcode_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/barcode_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/base_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/checkout_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/checkout_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/confirming_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/confirming_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/deliverydate_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/deliverydate_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/labelling_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/labelling_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/locations_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/locations_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/postalcode_check_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/postalcode_check_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/shipment_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/shipment_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/timeframes_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/timeframes_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/controllers/track_trace_controller.py` & `postnl_sdk-1.0.2/postnl/controllers/track_trace_controller.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/api_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/barcode_method_not_allowed_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/barcode_method_not_allowed_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/barcode_response_error_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/barcode_response_error_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/barcode_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/barcode_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/barcode_too_many_request_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/barcode_too_many_request_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/checkout_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/checkout_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/confirming_response_error_1_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/confirming_response_error_1_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/deliverydate_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/deliverydate_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/labelling_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/labelling_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/locations_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/locations_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/exceptions/timeframe_response_invalid_exception.py` & `postnl_sdk-1.0.2/postnl/exceptions/timeframe_response_invalid_exception.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/http/api_response.py` & `postnl_sdk-1.0.2/postnl/http/api_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/http/auth/custom_header_authentication.py` & `postnl_sdk-1.0.2/postnl/http/auth/custom_header_authentication.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/http/http_request.py` & `postnl_sdk-1.0.2/postnl/http/http_request.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/http/http_response.py` & `postnl_sdk-1.0.2/postnl/http/http_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/__init__.py` & `postnl_sdk-1.0.2/postnl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address.py` & `postnl_sdk-1.0.2/postnl/models/address.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address_1.py` & `postnl_sdk-1.0.2/postnl/models/address_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address_11.py` & `postnl_sdk-1.0.2/postnl/models/address_11.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address_2.py` & `postnl_sdk-1.0.2/postnl/models/address_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address_3.py` & `postnl_sdk-1.0.2/postnl/models/address_3.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/address_4.py` & `postnl_sdk-1.0.2/postnl/models/address_4.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/amount.py` & `postnl_sdk-1.0.2/postnl/models/amount.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/amount_1.py` & `postnl_sdk-1.0.2/postnl/models/amount_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/barcode_response.py` & `postnl_sdk-1.0.2/postnl/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/checkout_request.py` & `postnl_sdk-1.0.2/postnl/models/checkout_request.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/checkout_response.py` & `postnl_sdk-1.0.2/postnl/models/checkout_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/code_enum.py` & `postnl_sdk-1.0.2/postnl/models/code_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/complete_status.py` & `postnl_sdk-1.0.2/postnl/models/complete_status.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/confirming_request.py` & `postnl_sdk-1.0.2/postnl/models/confirming_request.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/confirming_response.py` & `postnl_sdk-1.0.2/postnl/models/confirming_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/contact.py` & `postnl_sdk-1.0.2/postnl/models/contact.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/content.py` & `postnl_sdk-1.0.2/postnl/models/content.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/content_1.py` & `postnl_sdk-1.0.2/postnl/models/content_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/cpc_response.py` & `postnl_sdk-1.0.2/postnl/models/cpc_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/currency_enum.py` & `postnl_sdk-1.0.2/postnl/models/currency_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/current_status.py` & `postnl_sdk-1.0.2/postnl/models/current_status.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/custom.py` & `postnl_sdk-1.0.2/postnl/models/custom.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/customer.py` & `postnl_sdk-1.0.2/postnl/models/customer.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/customer_1.py` & `postnl_sdk-1.0.2/postnl/models/customer_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/customer_2.py` & `postnl_sdk-1.0.2/postnl/models/customer_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/cut_off_time.py` & `postnl_sdk-1.0.2/postnl/models/cut_off_time.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/day_enum.py` & `postnl_sdk-1.0.2/postnl/models/day_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/delivery_option.py` & `postnl_sdk-1.0.2/postnl/models/delivery_option.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/delivery_options.py` & `postnl_sdk-1.0.2/postnl/models/delivery_options.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/detail.py` & `postnl_sdk-1.0.2/postnl/models/detail.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/dimension.py` & `postnl_sdk-1.0.2/postnl/models/dimension.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/dimension_1.py` & `postnl_sdk-1.0.2/postnl/models/dimension_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/error.py` & `postnl_sdk-1.0.2/postnl/models/error.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/error_1.py` & `postnl_sdk-1.0.2/postnl/models/error_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/error_2.py` & `postnl_sdk-1.0.2/postnl/models/error_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/error_3.py` & `postnl_sdk-1.0.2/postnl/models/error_3.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/error_4.py` & `postnl_sdk-1.0.2/postnl/models/error_4.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/event.py` & `postnl_sdk-1.0.2/postnl/models/event.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/expectation.py` & `postnl_sdk-1.0.2/postnl/models/expectation.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/extra_field.py` & `postnl_sdk-1.0.2/postnl/models/extra_field.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/fault.py` & `postnl_sdk-1.0.2/postnl/models/fault.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/friday.py` & `postnl_sdk-1.0.2/postnl/models/friday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/friday_1.py` & `postnl_sdk-1.0.2/postnl/models/friday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/get_locations_result.py` & `postnl_sdk-1.0.2/postnl/models/get_locations_result.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/get_locations_result_1.py` & `postnl_sdk-1.0.2/postnl/models/get_locations_result_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/group.py` & `postnl_sdk-1.0.2/postnl/models/group.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/hazardous_material.py` & `postnl_sdk-1.0.2/postnl/models/hazardous_material.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/label.py` & `postnl_sdk-1.0.2/postnl/models/label.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/label_1.py` & `postnl_sdk-1.0.2/postnl/models/label_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/labelling_request.py` & `postnl_sdk-1.0.2/postnl/models/labelling_request.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/labelling_response.py` & `postnl_sdk-1.0.2/postnl/models/labelling_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/labelling_response_1.py` & `postnl_sdk-1.0.2/postnl/models/labelling_response_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/language_enum.py` & `postnl_sdk-1.0.2/postnl/models/language_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/location.py` & `postnl_sdk-1.0.2/postnl/models/location.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/location_1.py` & `postnl_sdk-1.0.2/postnl/models/location_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/location_response.py` & `postnl_sdk-1.0.2/postnl/models/location_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/locations_response.py` & `postnl_sdk-1.0.2/postnl/models/locations_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/merged_label.py` & `postnl_sdk-1.0.2/postnl/models/merged_label.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/message.py` & `postnl_sdk-1.0.2/postnl/models/message.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/message_1.py` & `postnl_sdk-1.0.2/postnl/models/message_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/monday.py` & `postnl_sdk-1.0.2/postnl/models/monday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/monday_1.py` & `postnl_sdk-1.0.2/postnl/models/monday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/old_status.py` & `postnl_sdk-1.0.2/postnl/models/old_status.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/opening_hours.py` & `postnl_sdk-1.0.2/postnl/models/opening_hours.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/option_1_enum.py` & `postnl_sdk-1.0.2/postnl/models/option_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/option_2_enum.py` & `postnl_sdk-1.0.2/postnl/models/option_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/option_3_enum.py` & `postnl_sdk-1.0.2/postnl/models/option_3_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/option_enum.py` & `postnl_sdk-1.0.2/postnl/models/option_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/options.py` & `postnl_sdk-1.0.2/postnl/models/options.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/options_2_enum.py` & `postnl_sdk-1.0.2/postnl/models/options_2_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/pickup_option.py` & `postnl_sdk-1.0.2/postnl/models/pickup_option.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/product_option.py` & `postnl_sdk-1.0.2/postnl/models/product_option.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/product_option_1.py` & `postnl_sdk-1.0.2/postnl/models/product_option_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/product_options.py` & `postnl_sdk-1.0.2/postnl/models/product_options.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/reason_no_timeframe.py` & `postnl_sdk-1.0.2/postnl/models/reason_no_timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/reason_no_timeframes.py` & `postnl_sdk-1.0.2/postnl/models/reason_no_timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/response_shipment.py` & `postnl_sdk-1.0.2/postnl/models/response_shipment.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/response_shipment_1.py` & `postnl_sdk-1.0.2/postnl/models/response_shipment_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/response_shipment_2.py` & `postnl_sdk-1.0.2/postnl/models/response_shipment_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/saturday.py` & `postnl_sdk-1.0.2/postnl/models/saturday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/saturday_1.py` & `postnl_sdk-1.0.2/postnl/models/saturday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment.py` & `postnl_sdk-1.0.2/postnl/models/shipment.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_1.py` & `postnl_sdk-1.0.2/postnl/models/shipment_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_11.py` & `postnl_sdk-1.0.2/postnl/models/shipment_11.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_2.py` & `postnl_sdk-1.0.2/postnl/models/shipment_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_type_enum.py` & `postnl_sdk-1.0.2/postnl/models/shipment_type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_v_22_calculate_date_delivery_response.py` & `postnl_sdk-1.0.2/postnl/models/shipment_v_22_calculate_date_delivery_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shipment_v_22_calculate_date_shipping_response.py` & `postnl_sdk-1.0.2/postnl/models/shipment_v_22_calculate_date_shipping_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shippingstatus_response.py` & `postnl_sdk-1.0.2/postnl/models/shippingstatus_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shippingstatus_response_signature.py` & `postnl_sdk-1.0.2/postnl/models/shippingstatus_response_signature.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/shippingstatus_response_updated_shipment.py` & `postnl_sdk-1.0.2/postnl/models/shippingstatus_response_updated_shipment.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/signature.py` & `postnl_sdk-1.0.2/postnl/models/signature.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/status.py` & `postnl_sdk-1.0.2/postnl/models/status.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/status_2.py` & `postnl_sdk-1.0.2/postnl/models/status_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/string_1_enum.py` & `postnl_sdk-1.0.2/postnl/models/string_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/string_enum.py` & `postnl_sdk-1.0.2/postnl/models/string_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/sunday.py` & `postnl_sdk-1.0.2/postnl/models/sunday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/sunday_1.py` & `postnl_sdk-1.0.2/postnl/models/sunday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/sustainability.py` & `postnl_sdk-1.0.2/postnl/models/sustainability.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/thursday.py` & `postnl_sdk-1.0.2/postnl/models/thursday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/thursday_1.py` & `postnl_sdk-1.0.2/postnl/models/thursday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframe.py` & `postnl_sdk-1.0.2/postnl/models/timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframe_1.py` & `postnl_sdk-1.0.2/postnl/models/timeframe_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframe_response.py` & `postnl_sdk-1.0.2/postnl/models/timeframe_response.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframe_timeframe.py` & `postnl_sdk-1.0.2/postnl/models/timeframe_timeframe.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframes.py` & `postnl_sdk-1.0.2/postnl/models/timeframes.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/timeframes_1.py` & `postnl_sdk-1.0.2/postnl/models/timeframes_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/tuesday.py` & `postnl_sdk-1.0.2/postnl/models/tuesday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/tuesday_1.py` & `postnl_sdk-1.0.2/postnl/models/tuesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/type_1_enum.py` & `postnl_sdk-1.0.2/postnl/models/type_1_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/type_enum.py` & `postnl_sdk-1.0.2/postnl/models/type_enum.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/warning.py` & `postnl_sdk-1.0.2/postnl/models/warning.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/warning_1.py` & `postnl_sdk-1.0.2/postnl/models/warning_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/warning_11.py` & `postnl_sdk-1.0.2/postnl/models/warning_11.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/warning_2.py` & `postnl_sdk-1.0.2/postnl/models/warning_2.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/warnings.py` & `postnl_sdk-1.0.2/postnl/models/warnings.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/wednesday.py` & `postnl_sdk-1.0.2/postnl/models/wednesday.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/models/wednesday_1.py` & `postnl_sdk-1.0.2/postnl/models/wednesday_1.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl/postnl_client.py` & `postnl_sdk-1.0.2/postnl/postnl_client.py`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/postnl_sdk.egg-info/PKG-INFO` & `postnl_sdk-1.0.2/postnl_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: postnl-sdk
-Version: 1.0.1
-Summary: Collection of PostNL API's for ecommerce processes
+Version: 1.0.2
+Summary: Collection of PostNL API's for ecommerce processes.
 Author-email: PostNL <apimatic@postnl.nl>
 Project-URL: Documentation, https://developer.postnl.nl/
-Keywords: PostNK,ecommerce,SDK,API
+Keywords: PostNL,SDK,API,ecommerce
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apimatic-core~=0.2.0
 Requires-Dist: apimatic-core-interfaces~=0.1.0
 Requires-Dist: apimatic-requests-client-adapter~=0.1.0
 Requires-Dist: enum34>=1.1.10,~=1.1
@@ -24,19 +24,19 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install postnl-sdk==1.0.1
+pip install postnl-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/postnl-sdk/1.0.1
+https://pypi.python.org/pypi/postnl-sdk/1.0.2
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
```

### Comparing `postnl-sdk-1.0.1/postnl_sdk.egg-info/SOURCES.txt` & `postnl_sdk-1.0.2/postnl_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postnl-sdk-1.0.1/pyproject.toml` & `postnl_sdk-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "postnl-sdk"
-description = "Collection of PostNL API's for ecommerce processes"
-version = "1.0.1"
+description = "Collection of PostNL API's for ecommerce processes."
+version = "1.0.2"
 readme = "README.md"
 requires-python = ">=3.7"
-keywords = ["PostNK", "ecommerce", "SDK", "API"]
+keywords = ["PostNL", "SDK", "API", "ecommerce"]
 authors = [{name = "PostNL", email = "apimatic@postnl.nl"}]
 urls = {Documentation = "https://developer.postnl.nl/"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
 testutils = ["pytest>=7.2.2"]
 [tool.setuptools.packages.find]
```

