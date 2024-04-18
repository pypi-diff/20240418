# Comparing `tmp/iqrfpy-0.2.4.tar.gz` & `tmp/iqrfpy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.2.4.tar", last modified: Tue Apr 16 13:35:45 2024, max compression
+gzip compressed data, was "iqrfpy-0.2.5.tar", last modified: Thu Apr 18 13:01:47 2024, max compression
```

## Comparing `iqrfpy-0.2.4.tar` & `iqrfpy-0.2.5.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.740980 iqrfpy-0.2.4/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11351 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/LICENSE
--rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-16 13:35:45.740980 iqrfpy-0.2.4/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3314 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.688978 iqrfpy-0.2.4/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      235 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4379 2024-04-14 14:45:29.000000 iqrfpy-0.2.4/iqrfpy/async_response.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4163 2024-04-14 14:44:54.000000 iqrfpy-0.2.4/iqrfpy/confirmation.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.692978 iqrfpy-0.2.4/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      284 2024-04-14 15:45:45.000000 iqrfpy-0.2.4/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8049 2024-04-12 14:09:30.000000 iqrfpy-0.2.4/iqrfpy/enums/commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5261 2024-04-12 14:09:30.000000 iqrfpy-0.2.4/iqrfpy/enums/message_types.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      615 2024-04-12 14:09:30.000000 iqrfpy-0.2.4/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/enums/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7981 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.692978 iqrfpy-0.2.4/iqrfpy/ext/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      395 2024-04-16 13:29:53.000000 iqrfpy-0.2.4/iqrfpy/ext/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/ext/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    14602 2024-04-14 14:47:29.000000 iqrfpy-0.2.4/iqrfpy/irequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6711 2024-04-14 14:45:57.000000 iqrfpy-0.2.4/iqrfpy/iresponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3391 2024-04-14 14:47:42.000000 iqrfpy-0.2.4/iqrfpy/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    12857 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/messages.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/objects/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1544 2024-04-15 11:50:25.000000 iqrfpy-0.2.4/iqrfpy/objects/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3119 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/binaryoutput_state.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2441 2024-04-14 14:42:17.000000 iqrfpy-0.2.4/iqrfpy/objects/coordinator_authorize_bond_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      253 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/coordinator_dpa_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1316 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/exploration_per_enum_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/exploration_per_info_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1279 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/frc_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      944 2024-04-15 13:36:31.000000 iqrfpy-0.2.4/iqrfpy/objects/init_phy_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3138 2024-04-14 14:42:36.000000 iqrfpy-0.2.4/iqrfpy/objects/io_triplet.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1249 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/node_read_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2329 2024-04-14 14:43:12.000000 iqrfpy-0.2.4/iqrfpy/objects/node_validate_bonds_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5713 2024-04-14 14:35:06.000000 iqrfpy-0.2.4/iqrfpy/objects/os_batch_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      224 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/os_indicate_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1295 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/os_load_code_flags.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1321 2024-04-12 16:24:06.000000 iqrfpy-0.2.4/iqrfpy/objects/os_read_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      200 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/os_security_type_param.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3720 2024-04-14 14:42:47.000000 iqrfpy-0.2.4/iqrfpy/objects/os_sleep_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4430 2024-04-14 14:53:00.000000 iqrfpy-0.2.4/iqrfpy/objects/os_tr_conf_byte.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    30892 2024-04-14 14:50:47.000000 iqrfpy-0.2.4/iqrfpy/objects/os_tr_conf_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1911 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/objects/sensor_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2537 2024-04-14 14:42:44.000000 iqrfpy-0.2.4/iqrfpy/objects/sensor_written_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1123 2024-04-15 11:49:24.000000 iqrfpy-0.2.4/iqrfpy/objects/tr_mcu_type_data.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/peripherals/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      418 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      414 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      236 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4543 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/set_output.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      197 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3516 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3616 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/set_output.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.696978 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1623 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.700979 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1338 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2612 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4523 2024-04-14 14:03:12.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3656 2024-04-14 14:01:16.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5438 2024-04-14 15:49:27.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2647 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2675 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5208 2024-04-14 14:48:14.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3854 2024-04-14 14:03:32.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4204 2024-04-14 14:02:47.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4037 2024-04-14 14:01:43.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5300 2024-04-14 14:02:41.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5118 2024-04-14 14:01:30.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     9433 2024-04-14 14:02:32.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.704979 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3679 2024-04-14 14:08:17.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3793 2024-04-14 14:08:30.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3434 2024-04-14 14:07:56.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3727 2024-04-14 14:04:30.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3565 2024-04-14 14:04:15.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2943 2024-04-14 14:04:43.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3649 2024-04-14 14:03:42.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3431 2024-04-14 14:08:50.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3443 2024-04-14 14:09:01.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2859 2024-04-14 14:04:24.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3590 2024-04-14 14:03:48.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2024-04-14 14:04:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2706 2024-04-14 14:08:07.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3778 2024-04-14 14:03:55.000000 iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.704979 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      299 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.704979 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      160 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4980 2024-04-14 14:24:23.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5137 2024-04-14 14:24:28.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      165 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3332 2024-04-14 14:24:36.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:24:45.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      298 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4936 2024-04-14 14:23:49.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5133 2024-04-14 14:23:52.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      164 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3353 2024-04-14 14:23:58.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2879 2024-04-14 14:24:11.000000 iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      733 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2934 2024-04-14 14:10:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3218 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/peripheral_information.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.708979 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      516 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4754 2024-04-14 14:10:57.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4882 2024-04-14 14:11:02.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4185 2024-04-14 14:10:52.000000 iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/peripheral_information.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      594 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      392 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/extra_result.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5102 2024-04-14 14:15:18.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/send.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6789 2024-04-14 14:19:27.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/send_selective.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4065 2024-04-14 14:15:24.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/set_frc_params.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      336 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3485 2024-04-14 14:17:50.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/extra_result.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3713 2024-04-14 14:16:40.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/send.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3835 2024-04-14 14:17:43.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/send_selective.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3557 2024-04-14 14:17:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/set_frc_params.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      370 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/generic/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      106 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/generic/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3268 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/generic/requests/generic.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/generic/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      109 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/generic/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3382 2024-04-14 14:16:16.000000 iqrfpy-0.2.4/iqrfpy/peripherals/generic/responses/generic.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      435 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.712979 iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      275 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4127 2024-04-14 14:20:30.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/direction.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2553 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/get.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4085 2024-04-14 14:28:05.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/set.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      217 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2875 2024-04-14 14:20:36.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/direction.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3300 2024-04-14 14:20:41.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/get.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2797 2024-04-14 14:20:51.000000 iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/set.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:24:51.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:25:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:24:56.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:25:03.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.716979 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.720979 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:23:12.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:23:34.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:23:16.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:23:23.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.720979 iqrfpy-0.2.4/iqrfpy/peripherals/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      719 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.720979 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      419 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3607 2024-04-14 14:13:30.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2557 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3939 2024-04-14 14:19:01.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4426 2024-04-14 14:13:26.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/validate_bonds.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.720979 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      448 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3432 2024-04-14 14:14:06.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3860 2024-04-14 14:13:54.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2758 2024-04-14 14:14:11.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2863 2024-04-14 14:13:46.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2946 2024-04-14 14:13:38.000000 iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/validate_bonds.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.720979 iqrfpy-0.2.4/iqrfpy/peripherals/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.724979 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1351 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3903 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2625 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/factory_settings.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3203 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/indicate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7835 2024-04-14 14:21:12.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/load_code.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2543 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2615 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/read_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/reset.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/restart.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/rfpgm.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5690 2024-04-14 14:20:58.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/selective_batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5439 2024-04-14 14:21:26.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/set_security.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3209 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/sleep.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5979 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/test_rf_signal.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4243 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/write_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4128 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.728979 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1149 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:16.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2848 2024-04-14 14:21:54.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/factory_settings.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2752 2024-04-14 14:21:31.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/indicate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4336 2024-04-14 14:21:44.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/load_code.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4967 2024-04-14 14:22:11.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4617 2024-04-14 14:22:28.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/read_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:04.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/reset.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2739 2024-04-14 14:22:33.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/restart.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:23.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/rfpgm.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2825 2024-04-14 14:21:37.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/selective_batch.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2790 2024-04-14 14:21:49.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/set_security.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:40.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/sleep.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/test_rf_signal.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2820 2024-04-14 14:22:56.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/write_tr_conf.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2872 2024-04-14 14:22:47.000000 iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/py.typed
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.728979 iqrfpy-0.2.4/iqrfpy/peripherals/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      396 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.728979 iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4915 2024-04-14 14:14:42.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4881 2024-04-14 14:14:26.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/read_any.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5109 2024-04-14 14:14:45.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      222 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3351 2024-04-14 14:19:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3275 2024-04-14 14:15:01.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/read_any.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:15:12.000000 iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/write.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      587 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      381 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2592 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5087 2024-04-14 14:19:53.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/read_sensors.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5629 2024-04-14 14:19:37.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      366 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3723 2024-04-14 14:20:02.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/enumerate.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3242 2024-04-14 14:20:21.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/read_sensors.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3882 2024-04-14 14:20:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      229 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      112 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2606 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/requests/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      115 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3695 2024-04-14 14:11:10.000000 iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/responses/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      515 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.732979 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      303 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5736 2024-04-14 14:11:33.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/clear_write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/close.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3779 2024-04-14 14:11:19.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/open.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5686 2024-04-14 14:11:45.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/write_read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.736980 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      312 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3462 2024-04-14 14:12:00.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/clear_write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2692 2024-04-14 14:12:15.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/close.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2680 2024-04-14 14:11:54.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/open.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-04-14 14:12:09.000000 iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/write_read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    42515 2024-04-14 14:45:20.000000 iqrfpy-0.2.4/iqrfpy/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.736980 iqrfpy-0.2.4/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      272 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    30552 2024-04-14 15:02:10.000000 iqrfpy-0.2.4/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11872 2024-04-15 13:39:51.000000 iqrfpy-0.2.4/iqrfpy/utils/dpa.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      755 2024-04-12 14:02:36.000000 iqrfpy-0.2.4/iqrfpy/utils/enums.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2175 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/utils/frc_parser.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/iqrfpy/utils/py.typed
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    14869 2024-04-14 14:27:42.000000 iqrfpy-0.2.4/iqrfpy/utils/quantity_data.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2661 2024-04-14 14:33:26.000000 iqrfpy-0.2.4/iqrfpy/utils/sensor_constants.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    26329 2024-04-14 14:32:11.000000 iqrfpy-0.2.4/iqrfpy/utils/sensor_parser.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-03-18 17:43:19.000000 iqrfpy-0.2.4/iqrfpy/utils/validators.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-16 13:35:45.736980 iqrfpy-0.2.4/iqrfpy.egg-info/
--rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-16 13:35:45.000000 iqrfpy-0.2.4/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    10645 2024-04-16 13:35:45.000000 iqrfpy-0.2.4/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-16 13:35:45.000000 iqrfpy-0.2.4/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      114 2024-04-16 13:35:45.000000 iqrfpy-0.2.4/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-16 13:35:45.000000 iqrfpy-0.2.4/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      116 2024-04-02 13:56:09.000000 iqrfpy-0.2.4/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1545 2024-04-16 13:35:45.740980 iqrfpy-0.2.4/setup.cfg
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.654533 iqrfpy-0.2.5/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11351 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/LICENSE
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-18 13:01:47.654533 iqrfpy-0.2.5/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3314 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.606533 iqrfpy-0.2.5/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      235 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4379 2024-04-14 14:45:29.000000 iqrfpy-0.2.5/iqrfpy/async_response.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4163 2024-04-14 14:44:54.000000 iqrfpy-0.2.5/iqrfpy/confirmation.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.606533 iqrfpy-0.2.5/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      284 2024-04-14 15:45:45.000000 iqrfpy-0.2.5/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8049 2024-04-12 14:09:30.000000 iqrfpy-0.2.5/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5261 2024-04-12 14:09:30.000000 iqrfpy-0.2.5/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      615 2024-04-12 14:09:30.000000 iqrfpy-0.2.5/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/enums/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7981 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.606533 iqrfpy-0.2.5/iqrfpy/ext/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      399 2024-04-18 12:59:14.000000 iqrfpy-0.2.5/iqrfpy/ext/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/ext/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14602 2024-04-14 14:47:29.000000 iqrfpy-0.2.5/iqrfpy/irequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6711 2024-04-14 14:45:57.000000 iqrfpy-0.2.5/iqrfpy/iresponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3391 2024-04-14 14:47:42.000000 iqrfpy-0.2.5/iqrfpy/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    12857 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/messages.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.610533 iqrfpy-0.2.5/iqrfpy/objects/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1544 2024-04-15 11:50:25.000000 iqrfpy-0.2.5/iqrfpy/objects/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3119 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/binaryoutput_state.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2441 2024-04-14 14:42:17.000000 iqrfpy-0.2.5/iqrfpy/objects/coordinator_authorize_bond_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      253 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/coordinator_dpa_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1316 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/exploration_per_enum_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/exploration_per_info_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1279 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/frc_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      944 2024-04-15 13:36:31.000000 iqrfpy-0.2.5/iqrfpy/objects/init_phy_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3138 2024-04-14 14:42:36.000000 iqrfpy-0.2.5/iqrfpy/objects/io_triplet.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1249 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/node_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2329 2024-04-14 14:43:12.000000 iqrfpy-0.2.5/iqrfpy/objects/node_validate_bonds_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5713 2024-04-14 14:35:06.000000 iqrfpy-0.2.5/iqrfpy/objects/os_batch_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      224 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/os_indicate_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1295 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/os_load_code_flags.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1321 2024-04-12 16:24:06.000000 iqrfpy-0.2.5/iqrfpy/objects/os_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      200 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/os_security_type_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3720 2024-04-14 14:42:47.000000 iqrfpy-0.2.5/iqrfpy/objects/os_sleep_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4430 2024-04-14 14:53:00.000000 iqrfpy-0.2.5/iqrfpy/objects/os_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    30892 2024-04-14 14:50:47.000000 iqrfpy-0.2.5/iqrfpy/objects/os_tr_conf_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1911 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/objects/sensor_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2537 2024-04-14 14:42:44.000000 iqrfpy-0.2.5/iqrfpy/objects/sensor_written_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1123 2024-04-15 11:49:24.000000 iqrfpy-0.2.5/iqrfpy/objects/tr_mcu_type_data.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.614533 iqrfpy-0.2.5/iqrfpy/peripherals/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      418 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.614533 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      414 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.614533 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      236 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4543 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.614533 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      197 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3516 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3616 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.614533 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1623 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.618533 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1338 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2612 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4523 2024-04-14 14:03:12.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3656 2024-04-14 14:01:16.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5438 2024-04-14 15:49:27.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2647 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2675 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5208 2024-04-14 14:48:14.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3854 2024-04-14 14:03:32.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4204 2024-04-14 14:02:47.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4037 2024-04-14 14:01:43.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5300 2024-04-14 14:02:41.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5118 2024-04-14 14:01:30.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     9433 2024-04-14 14:02:32.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3679 2024-04-14 14:08:17.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3793 2024-04-14 14:08:30.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3434 2024-04-14 14:07:56.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3727 2024-04-14 14:04:30.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3565 2024-04-14 14:04:15.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2943 2024-04-14 14:04:43.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3649 2024-04-14 14:03:42.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3431 2024-04-14 14:08:50.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3443 2024-04-14 14:09:01.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2859 2024-04-14 14:04:24.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3590 2024-04-14 14:03:48.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2024-04-14 14:04:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2706 2024-04-14 14:08:07.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3778 2024-04-14 14:03:55.000000 iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      299 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      160 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4980 2024-04-14 14:24:23.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5137 2024-04-14 14:24:28.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      165 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3332 2024-04-14 14:24:36.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:24:45.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      298 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4936 2024-04-14 14:23:49.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5133 2024-04-14 14:23:52.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      164 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3353 2024-04-14 14:23:58.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2879 2024-04-14 14:24:11.000000 iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      733 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.622533 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2934 2024-04-14 14:10:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3218 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.626533 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      516 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4754 2024-04-14 14:10:57.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4882 2024-04-14 14:11:02.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4185 2024-04-14 14:10:52.000000 iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.626533 iqrfpy-0.2.5/iqrfpy/peripherals/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      594 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.626533 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      392 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5102 2024-04-14 14:15:18.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6789 2024-04-14 14:19:27.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4065 2024-04-14 14:15:24.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.626533 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      336 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3485 2024-04-14 14:17:50.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3713 2024-04-14 14:16:40.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3835 2024-04-14 14:17:43.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3557 2024-04-14 14:17:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.626533 iqrfpy-0.2.5/iqrfpy/peripherals/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      370 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/generic/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      106 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/generic/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3268 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/generic/requests/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/generic/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      109 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/generic/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3382 2024-04-14 14:16:16.000000 iqrfpy-0.2.5/iqrfpy/peripherals/generic/responses/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      435 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      275 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4127 2024-04-14 14:20:30.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2553 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4085 2024-04-14 14:28:05.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      217 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2875 2024-04-14 14:20:36.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3300 2024-04-14 14:20:41.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2797 2024-04-14 14:20:51.000000 iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.630533 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.634533 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:24:51.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:25:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:24:56.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:25:03.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.634533 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.634533 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.634533 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2698 2024-04-14 14:23:12.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2662 2024-04-14 14:23:34.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2679 2024-04-14 14:23:16.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2667 2024-04-14 14:23:23.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.634533 iqrfpy-0.2.5/iqrfpy/peripherals/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      719 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.638533 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      419 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3607 2024-04-14 14:13:30.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2557 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3939 2024-04-14 14:19:01.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4426 2024-04-14 14:13:26.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.638533 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      448 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3432 2024-04-14 14:14:06.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3860 2024-04-14 14:13:54.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2758 2024-04-14 14:14:11.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2863 2024-04-14 14:13:46.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2946 2024-04-14 14:13:38.000000 iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.638533 iqrfpy-0.2.5/iqrfpy/peripherals/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.642533 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1351 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3903 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2625 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3203 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7835 2024-04-14 14:21:12.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2543 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2615 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5690 2024-04-14 14:20:58.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5439 2024-04-14 14:21:26.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3209 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5979 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4243 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4128 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1149 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:16.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2848 2024-04-14 14:21:54.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2752 2024-04-14 14:21:31.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4336 2024-04-14 14:21:44.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4967 2024-04-14 14:22:11.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4617 2024-04-14 14:22:28.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2713 2024-04-14 14:22:04.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2739 2024-04-14 14:22:33.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:23.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2825 2024-04-14 14:21:37.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2790 2024-04-14 14:21:49.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2707 2024-04-14 14:22:40.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2820 2024-04-14 14:22:56.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2872 2024-04-14 14:22:47.000000 iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/py.typed
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      396 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4915 2024-04-14 14:14:42.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4881 2024-04-14 14:14:26.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5109 2024-04-14 14:14:45.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      222 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3351 2024-04-14 14:19:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3275 2024-04-14 14:15:01.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2858 2024-04-14 14:15:12.000000 iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      587 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      381 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2592 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5087 2024-04-14 14:19:53.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5629 2024-04-14 14:19:37.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      366 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3723 2024-04-14 14:20:02.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3242 2024-04-14 14:20:21.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3882 2024-04-14 14:20:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.646533 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      229 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.650533 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      112 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2606 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/requests/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.650533 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      115 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3695 2024-04-14 14:11:10.000000 iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/responses/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.650533 iqrfpy-0.2.5/iqrfpy/peripherals/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      515 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.650533 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      303 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5736 2024-04-14 14:11:33.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3779 2024-04-14 14:11:19.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5686 2024-04-14 14:11:45.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/write_read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.650533 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      312 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3462 2024-04-14 14:12:00.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2692 2024-04-14 14:12:15.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2680 2024-04-14 14:11:54.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-04-14 14:12:09.000000 iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    42515 2024-04-14 14:45:20.000000 iqrfpy-0.2.5/iqrfpy/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.654533 iqrfpy-0.2.5/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      272 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    30552 2024-04-14 15:02:10.000000 iqrfpy-0.2.5/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11872 2024-04-15 13:39:51.000000 iqrfpy-0.2.5/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      755 2024-04-12 14:02:36.000000 iqrfpy-0.2.5/iqrfpy/utils/enums.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2175 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/utils/frc_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/iqrfpy/utils/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14869 2024-04-14 14:27:42.000000 iqrfpy-0.2.5/iqrfpy/utils/quantity_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2661 2024-04-14 14:33:26.000000 iqrfpy-0.2.5/iqrfpy/utils/sensor_constants.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    26329 2024-04-14 14:32:11.000000 iqrfpy-0.2.5/iqrfpy/utils/sensor_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-03-18 17:43:19.000000 iqrfpy-0.2.5/iqrfpy/utils/validators.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-18 13:01:47.654533 iqrfpy-0.2.5/iqrfpy.egg-info/
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-18 13:01:47.000000 iqrfpy-0.2.5/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    10645 2024-04-18 13:01:47.000000 iqrfpy-0.2.5/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-18 13:01:47.000000 iqrfpy-0.2.5/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      114 2024-04-18 13:01:47.000000 iqrfpy-0.2.5/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-18 13:01:47.000000 iqrfpy-0.2.5/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      116 2024-04-02 13:56:09.000000 iqrfpy-0.2.5/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1545 2024-04-18 13:01:47.654533 iqrfpy-0.2.5/setup.cfg
```

### Comparing `iqrfpy-0.2.4/LICENSE` & `iqrfpy-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/PKG-INFO` & `iqrfpy-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Changelog, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html#changelog
 Project-URL: Documentation, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html
```

### Comparing `iqrfpy-0.2.4/README.md` & `iqrfpy-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/async_response.py` & `iqrfpy-0.2.5/iqrfpy/async_response.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/confirmation.py` & `iqrfpy-0.2.5/iqrfpy/confirmation.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/enums/commands.py` & `iqrfpy-0.2.5/iqrfpy/enums/commands.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/enums/message_types.py` & `iqrfpy-0.2.5/iqrfpy/enums/message_types.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/enums/peripherals.py` & `iqrfpy-0.2.5/iqrfpy/enums/peripherals.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/exceptions.py` & `iqrfpy-0.2.5/iqrfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/irequest.py` & `iqrfpy-0.2.5/iqrfpy/irequest.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/iresponse.py` & `iqrfpy-0.2.5/iqrfpy/iresponse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/itransport.py` & `iqrfpy-0.2.5/iqrfpy/itransport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/messages.py` & `iqrfpy-0.2.5/iqrfpy/messages.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/__init__.py` & `iqrfpy-0.2.5/iqrfpy/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/binaryoutput_state.py` & `iqrfpy-0.2.5/iqrfpy/objects/binaryoutput_state.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/coordinator_authorize_bond_params.py` & `iqrfpy-0.2.5/iqrfpy/objects/coordinator_authorize_bond_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/exploration_per_enum_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/exploration_per_enum_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/exploration_per_info_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/exploration_per_info_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/frc_params.py` & `iqrfpy-0.2.5/iqrfpy/objects/frc_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/init_phy_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/init_phy_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/io_triplet.py` & `iqrfpy-0.2.5/iqrfpy/objects/io_triplet.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/node_read_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/node_read_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/node_validate_bonds_params.py` & `iqrfpy-0.2.5/iqrfpy/objects/node_validate_bonds_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_batch_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_batch_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_load_code_flags.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_load_code_flags.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_read_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_read_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_sleep_params.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_sleep_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_tr_conf_byte.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_tr_conf_byte.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/os_tr_conf_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/os_tr_conf_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/sensor_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/sensor_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/sensor_written_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/sensor_written_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/objects/tr_mcu_type_data.py` & `iqrfpy-0.2.5/iqrfpy/objects/tr_mcu_type_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/enumerate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/requests/set_output.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/requests/set_output.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/enumerate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/binaryoutput/responses/set_output.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/binaryoutput/responses/set_output.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/addr_info.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/addr_info.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/authorize_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/authorize_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/backup.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/bond_node.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/bond_node.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/bonded_devices.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/bonded_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/discovered_devices.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/discovered_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/discovery.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/discovery.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/remove_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/remove_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/restore.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_hops.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_hops.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/set_mid.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/set_mid.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/requests/smart_connect.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/requests/smart_connect.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/addr_info.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/addr_info.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/authorize_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/authorize_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/backup.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/bond_node.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/bond_node.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/bonded_devices.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/bonded_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/discovered_devices.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/discovered_devices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/discovery.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/discovery.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/remove_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/remove_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/restore.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_hops.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_hops.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/set_mid.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/set_mid.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/coordinator/responses/smart_connect.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/coordinator/responses/smart_connect.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/requests/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/requests/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeeprom/responses/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeeprom/responses/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/requests/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/requests/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/eeprom/responses/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/eeprom/responses/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/requests/peripheral_information.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/requests/peripheral_information.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/exploration/responses/peripheral_information.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/exploration/responses/peripheral_information.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/extra_result.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/extra_result.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/send.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/send.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/send_selective.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/send_selective.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/requests/set_frc_params.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/requests/set_frc_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/extra_result.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/extra_result.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/send.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/send.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/send_selective.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/send_selective.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/frc/responses/set_frc_params.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/frc/responses/set_frc_params.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/generic/requests/generic.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/generic/requests/generic.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/generic/responses/generic.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/generic/responses/generic.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/direction.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/direction.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/get.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/get.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/requests/set.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/requests/set.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/direction.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/direction.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/get.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/get.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/io/responses/set.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/io/responses/set.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/flashing.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/pulse.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/set_off.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/requests/set_on.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/requests/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/flashing.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/pulse.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/set_off.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledg/responses/set_on.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledg/responses/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/flashing.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/pulse.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/set_off.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/requests/set_on.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/requests/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/flashing.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/flashing.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/pulse.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/pulse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/set_off.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/set_off.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ledr/responses/set_on.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ledr/responses/set_on.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/backup.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/remove_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/remove_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/restore.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/requests/validate_bonds.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/requests/validate_bonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/backup.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/remove_bond.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/remove_bond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/restore.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/node/responses/validate_bonds.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/node/responses/validate_bonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/batch.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/batch.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/factory_settings.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/factory_settings.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/indicate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/indicate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/load_code.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/load_code.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/read_tr_conf.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/read_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/reset.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/reset.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/restart.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/restart.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/rfpgm.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/rfpgm.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/selective_batch.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/selective_batch.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/set_security.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/set_security.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/sleep.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/sleep.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/test_rf_signal.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/write_tr_conf.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/write_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/batch.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/batch.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/factory_settings.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/factory_settings.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/indicate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/indicate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/load_code.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/load_code.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/read_tr_conf.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/read_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/reset.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/reset.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/restart.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/restart.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/rfpgm.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/rfpgm.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/selective_batch.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/selective_batch.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/set_security.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/set_security.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/sleep.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/sleep.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/test_rf_signal.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/write_tr_conf.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/write_tr_conf.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/read_any.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/read_any.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/requests/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/requests/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/read_any.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/read_any.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/ram/responses/write.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/ram/responses/write.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/enumerate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/read_sensors.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/read_sensors.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/enumerate.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/enumerate.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/read_sensors.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/read_sensors.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/requests/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/requests/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/thermometer/responses/read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/thermometer/responses/read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/__init__.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/clear_write_read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/clear_write_read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/close.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/close.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/open.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/open.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/requests/write_read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/requests/write_read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/clear_write_read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/clear_write_read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/close.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/close.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/open.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/open.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/peripherals/uart/responses/write_read.py` & `iqrfpy-0.2.5/iqrfpy/peripherals/uart/responses/write_read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/response_factory.py` & `iqrfpy-0.2.5/iqrfpy/response_factory.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/common.py` & `iqrfpy-0.2.5/iqrfpy/utils/common.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/dpa.py` & `iqrfpy-0.2.5/iqrfpy/utils/dpa.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/enums.py` & `iqrfpy-0.2.5/iqrfpy/utils/enums.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/frc_parser.py` & `iqrfpy-0.2.5/iqrfpy/utils/frc_parser.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/quantity_data.py` & `iqrfpy-0.2.5/iqrfpy/utils/quantity_data.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/sensor_constants.py` & `iqrfpy-0.2.5/iqrfpy/utils/sensor_constants.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/sensor_parser.py` & `iqrfpy-0.2.5/iqrfpy/utils/sensor_parser.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy/utils/validators.py` & `iqrfpy-0.2.5/iqrfpy/utils/validators.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.2.5/iqrfpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Project-URL: Changelog, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html#changelog
 Project-URL: Documentation, https://apidocs.iqrf.org/iqrfpy/latest/iqrfpy.html
```

### Comparing `iqrfpy-0.2.4/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.2.5/iqrfpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.2.4/setup.cfg` & `iqrfpy-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iqrfpy
-version = 0.2.4
+version = 0.2.5
 url = https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy
 author = Karel Hanák
 author_email = karel.hanak@iqrf.org
 description = A python library for communication with IQRF Network
 changelog = https://gitlab.iqrf.org/open-source/iqrf-sdk/iqrfpy/iqrfpy/-/blob/master/changelog.md
 long_description = file: README.md
 long_description_content_type = text/markdown
```

