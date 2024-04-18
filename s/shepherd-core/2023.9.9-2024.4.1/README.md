# Comparing `tmp/shepherd_core-2023.9.9.tar.gz` & `tmp/shepherd_core-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.9.9.tar", last modified: Sat Sep 30 12:20:13 2023, max compression
+gzip compressed data, was "shepherd_core-2024.4.1.tar", last modified: Thu Apr 18 13:25:03 2024, max compression
```

## Comparing `shepherd_core-2023.9.9.tar` & `shepherd_core-2024.4.1.tar`

### file list

```diff
@@ -1,142 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.642400 shepherd_core-2023.9.9/
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-09-30 12:20:13.642400 shepherd_core-2023.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-09-30 12:20:13.642400 shepherd_core-2023.9.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.626400 shepherd_core-2023.9.9/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.626400 shepherd_core-2023.9.9/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.626400 shepherd_core-2023.9.9/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.630400 shepherd_core-2023.9.9/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/_external_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/firmware_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.630400 shepherd_core-2023.9.9/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.630400 shepherd_core-2023.9.9/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.630400 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/data_models/testbed/testbed_fixture.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.630400 shepherd_core-2023.9.9/shepherd_core/decoder_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/decoder_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/decoder_waveform/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.634400 shepherd_core-2023.9.9/shepherd_core/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/fw_tools/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/fw_tools/converter_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/fw_tools/patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/fw_tools/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.634400 shepherd_core-2023.9.9/shepherd_core/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/inventory/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/inventory/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/inventory/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    23652 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.634400 shepherd_core-2023.9.9/shepherd_core/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/testbed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/testbed_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/testbed_client/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/testbed_client/user_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.634400 shepherd_core-2023.9.9/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.642400 shepherd_core-2023.9.9/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 12:20:13.000000 shepherd_core-2023.9.9/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.634400 shepherd_core-2023.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/data_models/test_testbed_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/decoder_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/decoder_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/decoder_waveform/test_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/fw_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/fw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/fw_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/fw_tools/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/fw_tools/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/fw_tools/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/inventory/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/testbed_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/testbed_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:13.638400 shepherd_core-2023.9.9/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/vsource/test_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-30 12:19:59.000000 shepherd_core-2023.9.9/tests/vsource/test_z.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.176937 shepherd_core-2024.4.1/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.180937 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/data_models/testbed/testbed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/decoder_waveform/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/converter_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/fw_tools/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/inventory/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26082 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/testbed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/cache_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/testbed_client/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.184937 shepherd_core-2024.4.1/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14355 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:25:03.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:02.000000 shepherd_core-2024.4.1/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:03.188937 shepherd_core-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-18 13:24:56.000000 shepherd_core-2024.4.1/tests/test_writer.py
```

### Comparing `shepherd_core-2023.9.9/PKG-INFO` & `shepherd_core-2024.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,140 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.9.9
+Version: 2024.4.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
-Home-page: https://pypi.org/project/shepherd-core/
-Author: Ingmar Splitt, Kai Geissdoerfer
-Author-email: ingmar.splitt@tu-dresden.de
-Maintainer-email: ingmar.splitt@tu-dresden.de
-License: MIT
-Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
-Project-URL: Source, https://github.com/orgua/shepherd-datalib
+Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
+Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
+Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
+Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
+Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Platform: win64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: pyYAML
 Requires-Dist: chromalog
 Requires-Dist: pydantic[email]>2.0.0
-Requires-Dist: tqdm
 Requires-Dist: scipy
+Requires-Dist: tqdm
 Requires-Dist: intelhex
 Requires-Dist: requests
 Requires-Dist: pyelftools
 Requires-Dist: zstandard
 Provides-Extra: elf
 Requires-Dist: pwntools-elf-only; extra == "elf"
 Provides-Extra: inventory
 Requires-Dist: psutil; extra == "inventory"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 
 # Core Library
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
-[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
-[![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![image](https://img.shields.io/pypi/pyversions/shepherd_core.svg)](https://pypi.python.org/pypi/shepherd-core)
+[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml)
+[![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-**Documentation**: <https://orgua.github.io/shepherd/external/shepherd_core.html>
+**Main Documentation**: <https://orgua.github.io/shepherd>
 
 **Source Code**: <https://github.com/orgua/shepherd-datalib>
 
 **Main Project**: <https://github.com/orgua/shepherd>
 
 ---
 
-This Python Module is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+`shepherd-core` is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
 
-For postprocessing shepherds .h5-files users want to use [shepherd_data](https://pypi.org/project/shepherd_data).
+For postprocessing shepherds .h5-files usage of [shepherd_data](https://pypi.org/project/shepherd_data) is recommended.
 
 ## Features
 
 - read and write shepherds hdf5-files
-- create, read, write and convert experiments for the testbed (all data-models included)
+- create, read, write and convert experiments for the testbed
+  - all required data-models are included
 - simulate the virtual source, including virtual harvesters (and virtual converter as a whole)
-- connect and query the testbed via a webclient (TestbedClient)
+- connect and query the testbed via a webclient (TestbedClient in alpha-stage)
   - offline usage defaults to static demo-fixtures loaded from yaml-files in the model-directories
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
 - decode waveforms (gpio-state & timestamp) to UART
-- create an inventory (used versions of software, hardware)
+- create an inventory (for deployed versions of software, hardware)
+
+See [official documentation](https://orgua.github.io/shepherd) or [example scripts](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased in both. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a [trafficbench](https://github.com/orgua/TrafficBench)-experiment that's used to derive the link-matrix of the testbed-nodes.
 
-See [examples](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased there. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a trafficbench-experiment that's used to derive the link-matrix.
+## Config-Models in Detail
 
-### Data-Models in Detail
+These pydantic data-models are used throughout all shepherd interfaces. Users can create an experiment, include their own content and feed it to the testbed.
 
-- new orchestration ``/data-models`` with focus on remote shepherd-testbed
+- orchestration ``/data-models`` with focus on remote shepherd-testbed
 - classes of sub-models
   - ``/base``: base-classes, configuration and -functionality for all models
   - ``/testbed``: meta-data representation of all testbed-components
-  - ``/content``: reusable meta-data for fw, h5 and vsrc-definitions
+  - ``/content``: reusable user-defined meta-data for fw, h5 and vsrc-definitions
   - ``/experiment``: configuration-models including sub-systems
   - ``/task``: digestible configs for shepherd-herd or -sheep
   - behavior controlled by ``ShpModel`` and ``content``-model
 - a basic database is available as fixtures through a ``tb_client``
   - fixtures selectable by name & ID
   - fixtures support inheritance
-- models support
+- the models support
   - auto-completion with neutral / sensible values
   - complex and custom datatypes (i.e. PositiveInt, lists-checks on length)
   - checking of inputs and type-casting
   - generate their own schema (for web-forms)
   - pre-validation
   - store to & load from yaml with typecheck through wrapper
   - documentation
 - experiment-definition is designed securely
   - types are limited in size (str)
   - exposes no internal paths
 - experiments can be transformed to task-sets (``TestbedTasks.from_xp()``)
 
+## Compatibility
+
+| OS      |   PyVersion  | Comment                                    |
+|---------|--------------|--------------------------------------------|
+| Ubuntu  | 3.8 - 3.12   |                                            |
+| Windows | 3.8 - 3.12   | no support for elf and hex-conversions yet |
+| MacOS   | 3.8 - 3.12   | hex-conversion missing                     |
+
+Notes:
+- hex-conversion needs a working and accessible objcopy
+- elf-supports needs
+  - ``shepherd-core[elf]`` installs ``pwntools-elf-only``
+  - most elf-features also still utilize hex-conversion
+
 ## Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core -U
 
@@ -148,7 +163,21 @@
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
 
 For creating an inventory of the host-system you should install
 
 ```shell
   pip install shepherd-core[inventory]
 ```
+
+## Unittests
+
+To run the testbench, follow these steps:
+
+1. Navigate your host-shell into the package-folder and
+2. install dependencies
+3. run the testbench (~ 320 tests):
+
+```Shell
+cd shepherd-datalib/shepherd_core
+pip3 install ./[tests]
+pytest
+```
```

### Comparing `shepherd_core-2023.9.9/README.md` & `shepherd_core-2024.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 # Core Library
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
-[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
-[![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![image](https://img.shields.io/pypi/pyversions/shepherd_core.svg)](https://pypi.python.org/pypi/shepherd-core)
+[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml)
+[![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-**Documentation**: <https://orgua.github.io/shepherd/external/shepherd_core.html>
+**Main Documentation**: <https://orgua.github.io/shepherd>
 
 **Source Code**: <https://github.com/orgua/shepherd-datalib>
 
 **Main Project**: <https://github.com/orgua/shepherd>
 
 ---
 
-This Python Module is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+`shepherd-core` is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
 
-For postprocessing shepherds .h5-files users want to use [shepherd_data](https://pypi.org/project/shepherd_data).
+For postprocessing shepherds .h5-files usage of [shepherd_data](https://pypi.org/project/shepherd_data) is recommended.
 
 ## Features
 
 - read and write shepherds hdf5-files
-- create, read, write and convert experiments for the testbed (all data-models included)
+- create, read, write and convert experiments for the testbed
+  - all required data-models are included
 - simulate the virtual source, including virtual harvesters (and virtual converter as a whole)
-- connect and query the testbed via a webclient (TestbedClient)
+- connect and query the testbed via a webclient (TestbedClient in alpha-stage)
   - offline usage defaults to static demo-fixtures loaded from yaml-files in the model-directories
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
 - decode waveforms (gpio-state & timestamp) to UART
-- create an inventory (used versions of software, hardware)
+- create an inventory (for deployed versions of software, hardware)
 
-See [examples](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased there. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a trafficbench-experiment that's used to derive the link-matrix.
+See [official documentation](https://orgua.github.io/shepherd) or [example scripts](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased in both. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a [trafficbench](https://github.com/orgua/TrafficBench)-experiment that's used to derive the link-matrix of the testbed-nodes.
 
-### Data-Models in Detail
+## Config-Models in Detail
 
-- new orchestration ``/data-models`` with focus on remote shepherd-testbed
+These pydantic data-models are used throughout all shepherd interfaces. Users can create an experiment, include their own content and feed it to the testbed.
+
+- orchestration ``/data-models`` with focus on remote shepherd-testbed
 - classes of sub-models
   - ``/base``: base-classes, configuration and -functionality for all models
   - ``/testbed``: meta-data representation of all testbed-components
-  - ``/content``: reusable meta-data for fw, h5 and vsrc-definitions
+  - ``/content``: reusable user-defined meta-data for fw, h5 and vsrc-definitions
   - ``/experiment``: configuration-models including sub-systems
   - ``/task``: digestible configs for shepherd-herd or -sheep
   - behavior controlled by ``ShpModel`` and ``content``-model
 - a basic database is available as fixtures through a ``tb_client``
   - fixtures selectable by name & ID
   - fixtures support inheritance
-- models support
+- the models support
   - auto-completion with neutral / sensible values
   - complex and custom datatypes (i.e. PositiveInt, lists-checks on length)
   - checking of inputs and type-casting
   - generate their own schema (for web-forms)
   - pre-validation
   - store to & load from yaml with typecheck through wrapper
   - documentation
 - experiment-definition is designed securely
   - types are limited in size (str)
   - exposes no internal paths
 - experiments can be transformed to task-sets (``TestbedTasks.from_xp()``)
 
+## Compatibility
+
+| OS      |   PyVersion  | Comment                                    |
+|---------|--------------|--------------------------------------------|
+| Ubuntu  | 3.8 - 3.12   |                                            |
+| Windows | 3.8 - 3.12   | no support for elf and hex-conversions yet |
+| MacOS   | 3.8 - 3.12   | hex-conversion missing                     |
+
+Notes:
+- hex-conversion needs a working and accessible objcopy
+- elf-supports needs
+  - ``shepherd-core[elf]`` installs ``pwntools-elf-only``
+  - most elf-features also still utilize hex-conversion
+
 ## Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core -U
 
@@ -89,7 +107,21 @@
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
 
 For creating an inventory of the host-system you should install
 
 ```shell
   pip install shepherd-core[inventory]
 ```
+
+## Unittests
+
+To run the testbench, follow these steps:
+
+1. Navigate your host-shell into the package-folder and
+2. install dependencies
+3. run the testbench (~ 320 tests):
+
+```Shell
+cd shepherd-datalib/shepherd_core
+pip3 install ./[tests]
+pytest
+```
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-"""
-shepherd.core
+"""shepherd.core
 ~~~~~
 Provides classes for storing and retrieving sampled IV data to/from
 HDF5 files.
 
 """
+
 from .data_models.base.calibration import Calc_t
 from .data_models.base.calibration import CalibrationCape
 from .data_models.base.calibration import CalibrationEmulator
 from .data_models.base.calibration import CalibrationHarvester
 from .data_models.base.calibration import CalibrationPair
 from .data_models.base.calibration import CalibrationSeries
-from .data_models.task import Compression
+from .data_models.base.timezone import local_now
+from .data_models.base.timezone import local_tz
+from .data_models.task.emulation import Compression
 from .inventory import Inventory
 from .logger import get_verbose_level
 from .logger import increase_verbose_level
 from .logger import logger
 from .reader import Reader
 from .testbed_client.client import TestbedClient
 from .testbed_client.client import tb_client
 from .writer import Writer
 
-__version__ = "2023.9.9"
+__version__ = "2024.04.1"
 
 __all__ = [
     "Reader",
     "Writer",
     "get_verbose_level",
     "increase_verbose_level",
     "logger",
     "CalibrationCape",
     "CalibrationSeries",
     "CalibrationEmulator",
     "CalibrationHarvester",
     "CalibrationPair",
+    "local_tz",
+    "local_now",
     "Calc_t",
     "Compression",
     "TestbedClient",
     "tb_client",  # using this (instead of the Class) is the cleaner, but less pythonic way
     "Inventory",
 ]
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/calibration_hw_def.py` & `shepherd_core-2024.4.1/shepherd_core/calibration_hw_def.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-
-Contains some info about the hardware configuration on the shepherd
+"""Contains some info about the hardware configuration on the shepherd
 cape. Based on these values, one can derive the expected adc readings given
 an input voltage/current or, for emulation, the expected voltage and current
 given the digital code in the DAC.
 
 currently configured for cape v2.4c
 
 """
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/base/cal_measurement.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,29 +52,29 @@
     dac_V_Sim: CalMeasPairs
     adc_V_Sense: CalMeasPairs
     adc_C_Hrv: CalMeasPairs
 
     def to_cal(self) -> CalibrationHarvester:
         dv = self.model_dump()
         dcal = CalibrationHarvester().model_dump()
-        for key in dv.keys():
+        for key in dv:
             dcal[key] = meas_to_cal(self[key], f"hrv_{key}")
         return CalibrationHarvester(**dcal)
 
 
 class CalMeasurementEmulator(ShpModel):
     dac_V_A: CalMeasPairs  # TODO: why not V_dac_A or V_dac_a
     dac_V_B: CalMeasPairs
     adc_C_A: CalMeasPairs
     adc_C_B: CalMeasPairs
 
     def to_cal(self) -> CalibrationEmulator:
         dv = self.model_dump()
         dcal = CalibrationEmulator().model_dump()
-        for key in dv.keys():
+        for key in dv:
             dcal[key] = meas_to_cal(self[key], f"emu_{key}")
         return CalibrationEmulator(**dcal)
 
 
 class CalMeasurementCape(ShpModel):
     cape: Optional[CapeData] = None
     host: Optional[str] = None
@@ -83,14 +83,14 @@
     emulator: Optional[CalMeasurementEmulator] = None
 
     def to_cal(self) -> CalibrationCape:
         dv = self.model_dump()
         dcal = CalibrationCape().model_dump()
         # TODO: is it helpful to default wrong / missing values?
         for key, value in dv.items():
-            if key in ["harvester", "emulator"]:
+            if key in {"harvester", "emulator"}:
                 if value is not None:
                     dcal[key] = self[key].to_cal()
             else:
                 dcal[key] = self[key]
 
         return CalibrationCape(**dcal)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/base/calibration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 import struct
-from datetime import date
 from typing import Callable
 from typing import Generator
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 
 import numpy as np
 from numpy.typing import NDArray
 from pydantic import Field
 from pydantic import PositiveFloat
 from pydantic import conbytes
 from pydantic import constr
 from pydantic import validate_call
+from typing_extensions import Self
 
 from ...calibration_hw_def import adc_current_to_raw
 from ...calibration_hw_def import adc_voltage_to_raw
 from ...calibration_hw_def import dac_voltage_to_raw
 from .shepherd import ShpModel
+from .timezone import local_iso_date
 
 Calc_t = TypeVar("Calc_t", NDArray[np.float64], float)
 
 
-def dict_generator(indict, pre=None) -> Generator[list, None, None]:
+def dict_generator(
+    in_dict: Union[dict, list], pre: Optional[list] = None
+) -> Generator[list, None, None]:
     pre = pre[:] if pre else []
-    if isinstance(indict, dict):
-        for key, value in indict.items():
+    if isinstance(in_dict, dict):
+        for key, value in in_dict.items():
             if isinstance(value, dict):
-                yield from dict_generator(value, pre + [key])
+                yield from dict_generator(value, [*pre, key])
             elif isinstance(value, (list, tuple)):
                 for v in value:
-                    yield from dict_generator(v, pre + [key])
+                    yield from dict_generator(v, [*pre, key])
             else:
-                yield pre + [key, value]
+                yield [*pre, key, value]
     else:
-        yield pre + [indict]
+        yield [*pre, in_dict]
 
 
 class CalibrationPair(ShpModel):
     """SI-value [SI-Unit] = raw-value * gain + offset"""
 
     gain: PositiveFloat
     offset: float = 0
 
-    def raw_to_si(self, values_raw: Calc_t, allow_negative: bool = True) -> Calc_t:
+    def raw_to_si(self, values_raw: Calc_t, *, allow_negative: bool = True) -> Calc_t:
         """Convert between physical units and raw unsigned integers"""
         values_si = values_raw * self.gain + self.offset
         if not allow_negative:
             if isinstance(values_si, np.ndarray):
                 values_si[values_si < 0.0] = 0.0
                 # if pyright still complains, cast with .astype(float)
             else:
@@ -63,15 +66,15 @@
             values_raw[values_raw < 0.0] = 0.0
             values_raw = np.around(values_raw)
         else:
             values_raw = round(max(values_raw, 0.0))
         return values_raw
 
     @classmethod
-    def from_fn(cls, fn: Callable):
+    def from_fn(cls, fn: Callable) -> Self:
         offset = fn(0)
         gain_inv = fn(1.0) - offset
         return cls(
             gain=1.0 / float(gain_inv),
             offset=-float(offset) / gain_inv,
         )
 
@@ -87,16 +90,15 @@
 class CalibrationHarvester(ShpModel):
     dac_V_Hrv: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     dac_V_Sim: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     adc_V_Sense: CalibrationPair = CalibrationPair.from_fn(adc_voltage_to_raw)
     adc_C_Hrv: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
 
     def export_for_sysfs(self) -> dict:
-        """
-        [scaling according to commons.h]
+        """[scaling according to commons.h]
         # ADC-C is handled in nA (nano-ampere), gain is shifted by 8 bit
         # ADC-V is handled in uV (micro-volt), gain is shifted by 8 bit
         # DAC-V is handled in uV (micro-volt), gain is shifted by 20 bit
         """
         cal_set = {
             "adc_current_gain": round(1e9 * (2**8) * self.adc_C_Hrv.gain),
             "adc_current_offset": round(1e9 * (2**0) * self.adc_C_Hrv.offset),
@@ -126,16 +128,15 @@
 
     dac_V_A: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     dac_V_B: CalibrationPair = CalibrationPair.from_fn(dac_voltage_to_raw)
     adc_C_A: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
     adc_C_B: CalibrationPair = CalibrationPair.from_fn(adc_current_to_raw)
 
     def export_for_sysfs(self) -> dict:
-        """
-        [scaling according to commons.h]
+        """[scaling according to commons.h]
         # ADC-C is handled in nA (nano-ampere), gain is shifted by 8 bit
         # ADC-V -> unused by vsrc / emu
         # DAC-V is handled in uV (micro-volt), gain is shifted by 20 bit
         TODO: current impl does not distinguish target_ports for DAC
         """
         cal_set = {
             "adc_current_gain": round(1e9 * (2**8) * self.adc_C_A.gain),
@@ -160,26 +161,27 @@
     According to BeagleBone specifications, each cape should host an EEPROM
     that contains some standardized information about the type of cape,
     manufacturer, version etc.
 
     `See<https://github.com/beagleboard/beaglebone-black/wiki/System-Reference-Manual#824_EEPROM_Data_Format>`_
     """
 
-    header: conbytes(max_length=4) = b"\xAA\x55\x33\xEE"
+    header: conbytes(max_length=4) = b"\xaa\x55\x33\xee"
     eeprom_revision: constr(max_length=2) = "A2"
     board_name: constr(max_length=32) = "BeagleBone SHEPHERD2 Cape"
     version: constr(max_length=4) = "24B0"
     manufacturer: constr(max_length=16) = "NES TU DRESDEN"
     part_number: constr(max_length=16) = "BB-SHPRD"
 
     serial_number: constr(max_length=12)
 
-    cal_date: constr(max_length=12) = Field(default_factory=date.today().isoformat)
+    cal_date: constr(max_length=12) = Field(default_factory=local_iso_date)
+    # ⤷ produces something like '2023-01-01'
 
-    def __repr__(self) -> str:
+    def __repr__(self) -> str:  # TODO: override useful?
         """string-representation allows print(model)"""
         return str(self.model_dump())
 
 
 class CalibrationCape(ShpModel):
     """Represents calibration data of shepherd cape.
     Defines the format of calibration data and provides convenient functions
@@ -191,23 +193,25 @@
     cape: Optional[CapeData] = None
     host: Optional[str] = None
 
     harvester: CalibrationHarvester = CalibrationHarvester()
     emulator: CalibrationEmulator = CalibrationEmulator()
 
     @classmethod
-    def from_bytestr(cls, data: bytes, cape: Optional[CapeData] = None):
+    def from_bytestr(cls, data: bytes, cape: Optional[CapeData] = None) -> Self:
         """Instantiates calibration data based on byte string.
         This is mainly used to deserialize data read from an EEPROM memory.
 
         Args:
+        ----
             data: Byte string containing calibration data.
             cape: data can be supplied
         Returns:
             CalibrationCape object with extracted calibration data.
+
         """
         dv = cls().model_dump(include={"harvester", "emulator"})
         lw = list(dict_generator(dv))
         values = struct.unpack(">" + len(lw) * "d", data)
         # ⤷ X => double float, big endian
         for _i, walk in enumerate(lw):
             # hardcoded fixed depth ... bad but easy
@@ -215,16 +219,18 @@
         dv["cape"] = cape
         return cls(**dv)
 
     def to_bytestr(self) -> bytes:
         """Serializes calibration data to byte string.
         Used to prepare data for writing it to EEPROM.
 
-        Returns:
+        Returns
+        -------
             Byte string representation of calibration values.
+
         """
         lw = list(dict_generator(self.model_dump(include={"harvester", "emulator"})))
         values = [walk[-1] for walk in lw]
         return struct.pack(">" + len(lw) * "d", *values)
 
 
 class CalibrationSeries(ShpModel):
@@ -232,18 +238,19 @@
     # ⤷ default allows 0 - 12 V in 3 nV-Steps
     current: CalibrationPair = CalibrationPair(gain=250 * 1e-12)
     # ⤷ default allows 0 - 1 A in 250 pA - Steps
     time: CalibrationPair = CalibrationPair(gain=1e-9)
     # ⤷ default = nanoseconds
 
     @classmethod
-    @validate_call
+    @validate_call(validate_return=False)
     def from_cal(
         cls,
         cal: Union[CalibrationHarvester, CalibrationEmulator],
+        *,
         emu_port_a: bool = True,
-    ):
+    ) -> Self:
         if isinstance(cal, CalibrationHarvester):
             return cls(voltage=cal.adc_V_Sense, current=cal.dac_V_Hrv)
         if emu_port_a:
             return cls(voltage=cal.dac_V_A, current=cal.adc_C_A)
         return cls(voltage=cal.dac_V_B, current=cal.adc_C_B)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/base/content.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/base/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import hashlib
 from datetime import datetime
 from typing import Optional
+from typing import Union
+from uuid import uuid4
 
+from pydantic import UUID4
 from pydantic import Field
 from pydantic import StringConstraints
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from .shepherd import ShpModel
+from .timezone import local_now
 
 # constr -> to_lower=True, max_length=16, regex=r"^[\w]+$"
 # ⤷ Regex = AlphaNum
 IdInt = Annotated[int, Field(ge=0, lt=2**128)]
-NameStr = Annotated[
-    str, StringConstraints(max_length=32, pattern=r'^[^<>:;,?"*|\/\\]+$')
-]
+NameStr = Annotated[str, StringConstraints(max_length=32, pattern=r"^[^<>:;,?\"\*|\/\\]+$")]
 # ⤷ Regex = FileSystem-Compatible ASCII
 SafeStr = Annotated[str, StringConstraints(pattern=r"^[ -~]+$")]
 # ⤷ Regex = All Printable ASCII-Characters with Space
 
 
 def id_default() -> int:
-    time_stamp = str(datetime.now()).encode("utf-8")
-    time_hash = hashlib.sha3_224(time_stamp).hexdigest()[-16:]
+    # note: IdInt has space for 128 bit, so 128/4 = 32 hex-chars
+    time_stamp = str(local_now()).encode("utf-8")
+    time_hash = hashlib.sha3_224(time_stamp).hexdigest()[-32:]
     return int(time_hash, 16)
 
 
 class ContentModel(ShpModel):
     # General Properties
-    id: IdInt = Field(  # noqa: A003
+    # id: UUID4 = Field(  # TODO: db-migration - temp fix for documentation
+    id: Union[UUID4, int] = Field(
         description="Unique ID",
-        default_factory=id_default,
+        default_factory=uuid4,
     )
     name: NameStr
-    description: Annotated[
-        Optional[SafeStr], Field(description="Required when public")
-    ] = None
+    description: Annotated[Optional[SafeStr], Field(description="Required when public")] = None
     comment: Optional[SafeStr] = None
     created: datetime = Field(default_factory=datetime.now)
+    updated_last: datetime = Field(default_factory=datetime.now)
 
     # Ownership & Access
+    # TODO: remove owner & group, only needed for DB
     owner: NameStr
     group: Annotated[NameStr, Field(description="University or Subgroup")]
     visible2group: bool = False
     visible2all: bool = False
 
     # TODO: we probably need to remember the lib-version for content &| experiment
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="after")
-    def content_validation(self):
+    def content_validation(self) -> Self:
         is_visible = self.visible2group or self.visible2all
         if is_visible and self.description is None:
             raise ValueError(
-                "Public instances require a description "
-                "(check visible2*- and description-field)"
+                "Public instances require a description (check visible2*- and description-field)"
             )
         return self
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/base/shepherd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import hashlib
-import os
 import pathlib
-from datetime import datetime
 from datetime import timedelta
 from ipaddress import IPv4Address
 from pathlib import Path
+from typing import Any
+from typing import Generator
 from typing import Optional
 from typing import Union
+from uuid import UUID
 
 import yaml
 from pydantic import BaseModel
 from pydantic import ConfigDict
+from typing_extensions import Self
+from yaml import Dumper
 from yaml import SafeDumper
+from yaml import ScalarNode
 
+from .timezone import local_now
 from .wrapper import Wrapper
 
 
-def path2str(dumper, data):
+def path2str(
+    dumper: Dumper, data: Union[pathlib.Path, pathlib.WindowsPath, pathlib.PosixPath]
+) -> ScalarNode:
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
-def time2int(dumper, data):
-    return dumper.represent_scalar(
-        "tag:yaml.org,2002:int", str(int(data.total_seconds()))
-    )
+def time2int(dumper: Dumper, data: timedelta) -> ScalarNode:
+    return dumper.represent_scalar("tag:yaml.org,2002:int", str(int(data.total_seconds())))
 
 
-def generic2str(dumper, data):
+def generic2str(dumper: Dumper, data: Any) -> ScalarNode:
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data))
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
 yaml.add_representer(IPv4Address, generic2str, SafeDumper)
+yaml.add_representer(UUID, generic2str, SafeDumper)
 
 
 class ShpModel(BaseModel):
     """Pre-configured Pydantic Base-Model (specifically for shepherd)
 
     Inheritable Features:
     - constant / frozen, hashable .get_hash()
@@ -77,72 +83,76 @@
         content = yaml.safe_dump(
             self.model_dump(exclude_unset=True, exclude_defaults=True),
             default_flow_style=False,
             sort_keys=False,
         )
         return str(content)
 
-    def __getitem__(self, key):
-        """allows dict access -> model["key"], in addition to model.key"""
+    def __getitem__(self, key: str) -> Any:
+        """Allows dict access -> model["key"], in addition to model.key"""
         return self.__getattribute__(key)
 
-    def keys(self):
+    def __contains__(self, item: str) -> bool:
+        """Allows checks like 'x in YClass'"""
+        return item in self.model_dump().keys()  # noqa: SIM118
+        # more correct, but probably slower than hasattr
+
+    def keys(self):  # noqa: ANN201
         """Fn of dict"""
         return self.model_dump().keys()
 
-    def items(self):
+    def items(self) -> Generator[tuple, None, None]:
         """Fn of dict"""
         for key in self.keys():
             yield key, self[key]
 
     @classmethod
     def schema_to_file(cls, path: Union[str, Path]) -> None:
-        """store schema to yaml (for frontend-generators)"""
+        """Store schema to yaml (for frontend-generators)"""
         model_dict = cls.model_json_schema()
-        model_yaml = yaml.safe_dump(
-            model_dict, default_flow_style=False, sort_keys=False
-        )
-        with open(Path(path).resolve().with_suffix(".yaml"), "w") as f:
+        model_yaml = yaml.safe_dump(model_dict, default_flow_style=False, sort_keys=False)
+        with Path(path).resolve().with_suffix(".yaml").open("w") as f:
             f.write(model_yaml)
 
     def to_file(
         self,
         path: Union[str, Path],
-        minimal: bool = True,
         comment: Optional[str] = None,
+        *,
+        minimal: bool = True,
     ) -> Path:
-        """store data to yaml in a wrapper
+        """Store data to yaml in a wrapper
         minimal: stores minimal set (filters out unset & default parameters)
         comment: documentation
         """
         model_dict = self.model_dump(exclude_unset=minimal)
         model_wrap = Wrapper(
             datatype=type(self).__name__,
             comment=comment,
-            created=datetime.now(),
+            created=local_now(),
             parameters=model_dict,
         )
         model_yaml = yaml.safe_dump(
             model_wrap.model_dump(exclude_unset=minimal, exclude_defaults=minimal),
             default_flow_style=False,
             sort_keys=False,
         )
         # TODO: handle directory
         model_path = Path(path).resolve().with_suffix(".yaml")
         if not model_path.parent.exists():
-            os.makedirs(model_path.parent)
-        with open(model_path, "w") as f:
+            model_path.parent.mkdir(parents=True)
+        with model_path.open("w") as f:
             f.write(model_yaml)
         return model_path
 
     @classmethod
-    def from_file(cls, path: Union[str, Path]):
-        """load from yaml"""
-        with open(Path(path).resolve()) as shp_file:
+    def from_file(cls, path: Union[str, Path]) -> Self:
+        """Load from yaml"""
+        with Path(path).open() as shp_file:
             shp_dict = yaml.safe_load(shp_file)
         shp_wrap = Wrapper(**shp_dict)
         if shp_wrap.datatype != cls.__name__:
             raise ValueError("Model in file does not match the requirement")
         return cls(**shp_wrap.parameters)
 
-    def get_hash(self):
+    def get_hash(self) -> str:
         return hashlib.sha3_224(str(self.model_dump()).encode("utf-8")).hexdigest()
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/base/wrapper.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/base/wrapper.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/content/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/content/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/content/energy_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..base.content import ContentModel
 
 
 class EnergyDType(str, Enum):
     ivsample = "ivsample"
     ivsamples = "ivsample"
     ivcurve = "ivcurve"
-    ivcurves = "ivcurve"
+    ivcurves = "ivcurve"  # a stream could also be called iv-surface
     isc_voc = "isc_voc"
 
 
 class EnergyEnvironment(ContentModel):
     """Recording of meta-data representation of a testbed-component"""
 
     # General Metadata & Ownership -> ContentModel
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/content/firmware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pathlib import Path
 from typing import Optional
+from typing import TypedDict
 from typing import Union
 
 from pydantic import StringConstraints
 from pydantic import model_validator
 from pydantic import validate_call
 from typing_extensions import Annotated
+from typing_extensions import Self
+from typing_extensions import Unpack
 
 from ... import fw_tools
 from ...logger import logger
 from ...testbed_client import tb_client
 from ..base.content import ContentModel
 from ..testbed.mcu import MCU
 from .firmware_datatype import FirmwareDType
@@ -56,37 +59,43 @@
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         # crosscheck type with actual data
         _type = values.get("data_type")
-        if _type in [
+        if _type in {
             FirmwareDType.base64_hex,
             FirmwareDType.base64_elf,
-        ]:
+        }:
             try:
                 _hash = fw_tools.base64_to_hash(values.get("data"))
             except ValueError:
-                raise ValueError("Embedded Firmware seems to be faulty")
+                raise ValueError("Embedded Firmware seems to be faulty") from None
             if values.get("data_hash") is not None and _hash != values.get("data_hash"):
                 raise ValueError("Embedded Firmware and Hash do not match!")
-        elif _type in [
+        elif _type in {
             FirmwareDType.path_hex,
             FirmwareDType.path_elf,
-        ]:
+        }:
             try:
                 _ = Path(values.get("data"))
             except (SyntaxError, NameError):
-                raise ValueError("Firmware-Path is invalid")
+                raise ValueError("Firmware-Path is invalid") from None
         return tb_client.fill_in_user_data(values)
 
     @classmethod
-    def from_firmware(cls, file: Path, embed: bool = True, **kwargs):
-        """embeds firmware and tries to fill parameters
+    def from_firmware(
+        cls,
+        file: Path,
+        *,
+        embed: bool = True,
+        **kwargs: Unpack[TypedDict],
+    ) -> Self:
+        """Embeds firmware and tries to fill parameters
         ELF -> mcu und data_type are deducted
         HEX -> must supply mcu manually
         """
         # TODO: use new determine_type() & determine_arch() and also allow to not embed
         kwargs["data_hash"] = fw_tools.file_to_hash(file)
         if embed:
             kwargs["data"] = fw_tools.file_to_base64(file)
@@ -137,15 +146,15 @@
 
         if not match:
             logger.warning("FW-Hash does not match with stored value!")
         return match
 
     @validate_call
     def extract_firmware(self, file: Path) -> Path:
-        """stores embedded data in file
+        """Stores embedded data in file
         - file-suffix is derived from data-type and adapted
         - if provided path is a directory, the firmware-name is used
         """
         if file.is_dir():
             file = file / self.name
         file_new = fw_tools.extract_firmware(self.data, self.data_type, file)
         self.compare_hash(file_new)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Optional
 from typing import Tuple
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
 from ...testbed_client import tb_client
 from ..base.calibration import CalibrationHarvester
 from ..base.content import ContentModel
 from ..base.shepherd import ShpModel
@@ -71,15 +72,15 @@
         values = tb_client.fill_in_user_data(values)
         if values["name"] == "neutral":
             # TODO: same test is later done in calc_algorithm_num() again
             raise ValueError("Resulting Harvester can't be neutral")
         logger.debug("VHrv-Inheritances: %s", chain)
 
         # post corrections -> should be in separate validator
-        cal = CalibrationHarvester()  # todo: as argument?
+        cal = CalibrationHarvester()  # TODO: as argument?
         c_limit = values.get("current_limit_uA", 50_000)  # cls.current_limit_uA)
         values["current_limit_uA"] = max(10**6 * cal.adc_C_Hrv.raw_to_si(4), c_limit)
 
         if values.get("voltage_step_mV") is None:
             # algo includes min & max!
             v_max = values.get("voltage_max_mV", 5_000)  # cls.voltage_max_mV)
             v_min = values.get("voltage_min_mV", 0)  # cls.voltage_min_mV)
@@ -89,42 +90,42 @@
         values["voltage_step_mV"] = max(
             10**3 * cal.dac_V_Hrv.raw_to_si(4), values["voltage_step_mV"]
         )
 
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         if self.voltage_min_mV > self.voltage_max_mV:
             raise ValueError("Voltage min > max")
         if self.voltage_mV < self.voltage_min_mV:
             raise ValueError("Voltage below min")
         if self.voltage_mV > self.voltage_max_mV:
             raise ValueError("Voltage above max")
 
         return self
 
-    def calc_hrv_mode(self, for_emu: bool) -> int:
+    def calc_hrv_mode(self, *, for_emu: bool) -> int:
         return 1 * int(for_emu) + 2 * self.rising
 
-    def calc_algorithm_num(self, for_emu: bool) -> int:
+    def calc_algorithm_num(self, *, for_emu: bool) -> int:
         num = algo_to_num.get(self.algorithm)
         if for_emu and self.get_datatype() != EnergyDType.ivsample:
             raise ValueError(
                 f"[{self.name}] Select valid harvest-algorithm for emulator, "
                 f"current usage = {self.algorithm}",
             )
         if num < algo_to_num["isc_voc"]:
             raise ValueError(
                 f"[{self.name}] Select valid harvest-algorithm for harvester, "
                 f"current usage = {self.algorithm}",
             )
         return num
 
-    def calc_timings_ms(self, for_emu: bool) -> Tuple[float, float]:
+    def calc_timings_ms(self, *, for_emu: bool) -> Tuple[float, float]:
         """factor-in model-internal timing-constraints"""
         window_length = self.samples_n * (1 + self.wait_cycles)
         time_min_ms = (1 + self.wait_cycles) * 1_000 / samplerate_sps_default
         if for_emu:
             window_ms = window_length * 1_000 / samplerate_sps_default
             time_min_ms = max(time_min_ms, window_ms)
 
@@ -139,15 +140,18 @@
             )
         return interval_ms, duration_ms
 
     def get_datatype(self) -> EnergyDType:
         return algo_to_dtype[self.algorithm]
 
     def calc_window_size(
-        self, for_emu: bool, dtype_in: Optional[EnergyDType] = EnergyDType.ivsample
+        self,
+        dtype_in: Optional[EnergyDType] = EnergyDType.ivsample,
+        *,
+        for_emu: bool,
     ) -> int:
         if for_emu:
             if dtype_in == EnergyDType.ivcurve:
                 return self.samples_n * (1 + self.wait_cycles)
             if dtype_in == EnergyDType.ivsample:
                 return 0
             # isc_voc: 2 * (1 + wait_cycles), noqa
@@ -166,15 +170,15 @@
 # - emulation with "ivcurve" or lower is also resulting in Error
 # - "_opt" has its own algo for emulation, but is only a fast mppt_po for harvesting
 algo_to_num = {
     "neutral": 2**0,
     "isc_voc": 2**3,
     "ivcurve": 2**4,
     "cv": 2**8,
-    # "ci": 2**9, # is this desired?
+    # is "ci" desired?
     "mppt_voc": 2**12,
     "mppt_po": 2**13,
     "mppt_opt": 2**14,
 }
 
 algo_to_dtype = {
     "isc_voc": EnergyDType.isc_voc,
@@ -183,16 +187,15 @@
     "mppt_voc": EnergyDType.ivsample,
     "mppt_po": EnergyDType.ivsample,
     "mppt_opt": EnergyDType.ivsample,
 }
 
 
 class HarvesterPRUConfig(ShpModel):
-    """
-    Map settings-list to internal state-vars struct HarvesterConfig
+    """Map settings-list to internal state-vars struct HarvesterConfig
     NOTE:
       - yaml is based on si-units like nA, mV, ms, uF
       - c-code and py-copy is using nA, uV, ns, nF, fW, raw
       - ordering is intentional and in sync with shepherd/commons.h
     """
 
     algorithm: u32
@@ -213,30 +216,31 @@
     wait_cycles_n: u32
     # ⤷ for DAC to settle
 
     @classmethod
     def from_vhrv(
         cls,
         data: VirtualHarvesterConfig,
-        for_emu: bool = False,
         dtype_in: Optional[EnergyDType] = EnergyDType.ivsample,
         window_size: Optional[u32] = None,
-    ):
+        *,
+        for_emu: bool = False,
+    ) -> Self:
         if isinstance(dtype_in, str):
             dtype_in = EnergyDType[dtype_in]
-        if for_emu and dtype_in not in [EnergyDType.ivsample, EnergyDType.ivcurve]:
+        if for_emu and dtype_in not in {EnergyDType.ivsample, EnergyDType.ivcurve}:
             raise ValueError("Not Implemented")
         # TODO: use dtype properly in shepherd
-        interval_ms, duration_ms = data.calc_timings_ms(for_emu)
+        interval_ms, duration_ms = data.calc_timings_ms(for_emu=for_emu)
         return cls(
-            algorithm=data.calc_algorithm_num(for_emu),
-            hrv_mode=data.calc_hrv_mode(for_emu),
+            algorithm=data.calc_algorithm_num(for_emu=for_emu),
+            hrv_mode=data.calc_hrv_mode(for_emu=for_emu),
             window_size=window_size
             if window_size is not None
-            else data.calc_window_size(for_emu, dtype_in),
+            else data.calc_window_size(dtype_in, for_emu=for_emu),
             voltage_uV=round(data.voltage_mV * 10**3),
             voltage_min_uV=round(data.voltage_min_mV * 10**3),
             voltage_max_uV=round(data.voltage_max_mV * 10**3),
             voltage_step_uV=round(data.voltage_step_mV * 10**3),
             current_limit_nA=round(data.current_limit_uA * 10**3),
             setpoint_n8=round(min(255, data.setpoint_n * 2**8)),
             interval_n=round(interval_ms * samplerate_sps_default * 1e-3),
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/content/virtual_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ...commons import samplerate_sps_default
 from ...logger import logger
 from ...testbed_client import tb_client
 from .. import ShpModel
 from ..base.content import ContentModel
 from .virtual_harvester import HarvesterPRUConfig
@@ -20,20 +21,21 @@
 
 
 class VirtualSourceConfig(ContentModel, title="Config for the virtual Source"):
     """The virtual Source uses the energy environment (file)
     for supplying the Target Node during the experiment.
     If not already done, the energy will be harvested and then converted.
     The converter-stage is software defined and offers:
-      buck-boost-combinations,
-      a simple diode + resistor and
-      an intermediate buffer capacitor.
-      TODO: I,V,R should be in regular unit (V, A, Ohm)
+    - buck-boost-combinations,
+    - a simple diode + resistor and
+    - an intermediate buffer capacitor.
     """
 
+    # TODO: I,V,R should be in regular unit (V, A, Ohm)
+
     # General Metadata & Ownership -> ContentModel
 
     enable_boost: bool = False
     # ⤷ if false -> v_intermediate = v_input, output-switch-hysteresis is still usable
     enable_buck: bool = False
     # ⤷ if false -> v_output = v_intermediate
 
@@ -105,36 +107,38 @@
     def query_database(cls, values: dict) -> dict:
         values, chain = tb_client.try_completing_model(cls.__name__, values)
         values = tb_client.fill_in_user_data(values)
         logger.debug("VSrc-Inheritances: %s", chain)
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         # trigger stricter test of harv-parameters
         HarvesterPRUConfig.from_vhrv(self.harvester, for_emu=True)
         return self
 
     def calc_internal_states(self) -> dict:
-        """
-        compensate for (hard to detect) current-surge of real capacitors
+        """Compensate for (hard to detect) current-surge of real capacitors
         when converter gets turned on -> this can be const value, because
         the converter always turns on with "V_storage_enable_threshold_uV"
         TODO: currently neglecting delay after disabling converter, boost
         only has simpler formula, second enabling when V_Cap >= V_out
 
         Math behind this calculation:
-        Energy-Change Storage Cap   ->  E_new = E_old - E_output
-        with Energy of a Cap 	    -> 	E_x = C_x * V_x^2 / 2
-        combine formulas 		    ->
-                    C_store * V_store_new^2 / 2 = C_store * V_store_old^2 / 2 - C_out * V_out^2 / 2
-        convert formula to V_new 	->	V_store_new^2 = V_store_old^2 - (C_out / C_store) * V_out^2
-        convert into dV	 	        ->	dV = V_store_new - V_store_old
-        in case of V_cap = V_out 	-> 	dV = V_store_old * (sqrt(1 - C_out / C_store) - 1)
-        -> dV values will be reversed (negated), because dV is always negative (Voltage drop)
+
+        - Energy-Change Storage Cap ->  E_new = E_old - E_output
+        - with Energy of a Cap 	    -> 	E_x = C_x * V_x^2 / 2
+        - combine formulas 		    ->  C_store * V_store_new^2 / 2 =
+          C_store * V_store_old^2 / 2 - C_out * V_out^2 / 2
+        - convert formula to V_new 	->	V_store_new^2 =
+          V_store_old^2 - (C_out / C_store) * V_out^2
+        - convert into dV	 	        ->	dV = V_store_new - V_store_old
+        - in case of V_cap = V_out 	-> 	dV = V_store_old * (sqrt(1 - C_out / C_store) - 1)
+
+        Note: dV values will be reversed (negated), because dV is always negative (Voltage drop)
         """
         values = {}
         if self.C_intermediate_uF > 0 and self.C_output_uF > 0:
             # first case: storage cap outside of en/dis-thresholds
             v_old = self.V_intermediate_enable_threshold_mV
             v_out = self.V_output_mV
             c_store = self.C_intermediate_uF
@@ -149,75 +153,62 @@
             # v_enable is either bucks v_out or same dV-Value is calculated a second time
             dV_output_imed_low_mV = v_out * (1 - pow(1 - c_out / c_store, 0.5))
         else:
             dV_output_en_thrs_mV = 0
             dV_output_imed_low_mV = 0
 
         # protect from complex solutions (non valid input combinations)
-        if not (
-            isinstance(dV_output_en_thrs_mV, (int, float))
-            and (dV_output_en_thrs_mV >= 0)
-        ):
+        if not (isinstance(dV_output_en_thrs_mV, (int, float)) and (dV_output_en_thrs_mV >= 0)):
             dV_output_en_thrs_mV = 0
-        if not (
-            isinstance(dV_output_imed_low_mV, (int, float))
-            and (dV_output_imed_low_mV >= 0)
-        ):
+        if not (isinstance(dV_output_imed_low_mV, (int, float)) and (dV_output_imed_low_mV >= 0)):
             logger.warning("VSrc: C_output shouldn't be larger than C_intermediate")
             dV_output_imed_low_mV = 0
 
         # decide which hysteresis-thresholds to use for buck-converter
         if self.enable_buck > 0:
             V_pre_output_mV = self.V_output_mV + self.V_buck_drop_mV
 
             if self.V_intermediate_enable_threshold_mV > V_pre_output_mV:
                 values["dV_enable_output_mV"] = dV_output_en_thrs_mV
-                values[
-                    "V_enable_output_threshold_mV"
-                ] = self.V_intermediate_enable_threshold_mV
+                values["V_enable_output_threshold_mV"] = self.V_intermediate_enable_threshold_mV
 
             else:
                 values["dV_enable_output_mV"] = dV_output_imed_low_mV
                 values["V_enable_output_threshold_mV"] = (
                     V_pre_output_mV + values["dV_enable_output_mV"]
                 )
 
             if self.V_intermediate_disable_threshold_mV > V_pre_output_mV:
-                values[
-                    "V_disable_output_threshold_mV"
-                ] = self.V_intermediate_disable_threshold_mV
+                values["V_disable_output_threshold_mV"] = self.V_intermediate_disable_threshold_mV
             else:
                 values["V_disable_output_threshold_mV"] = V_pre_output_mV
 
         else:
             values["dV_enable_output_mV"] = dV_output_en_thrs_mV
-            values[
-                "V_enable_output_threshold_mV"
-            ] = self.V_intermediate_enable_threshold_mV
-            values[
-                "V_disable_output_threshold_mV"
-            ] = self.V_intermediate_disable_threshold_mV
+            values["V_enable_output_threshold_mV"] = self.V_intermediate_enable_threshold_mV
+            values["V_disable_output_threshold_mV"] = self.V_intermediate_disable_threshold_mV
         return values
 
-    def calc_converter_mode(self, log_intermediate_node: bool) -> int:
-        """assembles bitmask from discrete values
+    def calc_converter_mode(self, *, log_intermediate_node: bool) -> int:
+        """Assembles bitmask from discrete values
+
         log_intermediate_node: record / log virtual intermediate (cap-)voltage and
-                            -current (out) instead of output-voltage and -current
+        -current (out) instead of output-voltage and -current
         """
         enable_storage = self.C_intermediate_uF > 0
         enable_boost = self.enable_boost and enable_storage
         return (
             1 * int(enable_storage)
             + 2 * int(enable_boost)
             + 4 * int(self.enable_buck)
             + 8 * int(log_intermediate_node)
         )
 
     def calc_cap_constant_us_per_nF_n28(self) -> int:
-        """calc constant to convert capacitor-current to Voltage-delta
+        """Calc constant to convert capacitor-current to Voltage-delta
         dV[uV] = constant[us/nF] * current[nA] = constant[us*V/nAs] * current[nA]
         """
         C_cap_uF = max(self.C_intermediate_uF, 0.001)
         return int((10**3 * (2**28)) // (C_cap_uF * samplerate_sps_default))
 
 
 u32 = Annotated[int, Field(ge=0, lt=2**32)]
@@ -229,16 +220,15 @@
         max_length=LUT_SIZE,
     ),
 ]
 lut_o = Annotated[List[u32], Field(min_length=LUT_SIZE, max_length=LUT_SIZE)]
 
 
 class ConverterPRUConfig(ShpModel):
-    """
-    Map settings-list to internal state-vars struct ConverterConfig
+    """Map settings-list to internal state-vars struct ConverterConfig
     NOTE:
       - yaml is based on si-units like nA, mV, ms, uF
       - c-code and py-copy is using nA, uV, ns, nF, fW, raw
       - ordering is intentional and in sync with shepherd/commons.h
     """
 
     converter_mode: u32
@@ -274,61 +264,55 @@
     LUT_input_V_min_log2_uV: u32
     LUT_input_I_min_log2_nA: u32
     LUT_output_I_min_log2_nA: u32
     LUT_inp_efficiency_n8: lut_i
     LUT_out_inv_efficiency_n4: lut_o
 
     @classmethod
-    def from_vsrc(cls, data: VirtualSourceConfig, log_intermediate_node: bool = False):
+    def from_vsrc(
+        cls,
+        data: VirtualSourceConfig,
+        *,
+        log_intermediate_node: bool = False,
+    ) -> Self:
         states = data.calc_internal_states()
         return cls(
             # General
-            converter_mode=data.calc_converter_mode(log_intermediate_node),
+            converter_mode=data.calc_converter_mode(log_intermediate_node=log_intermediate_node),
             interval_startup_delay_drain_n=round(
                 data.interval_startup_delay_drain_ms * samplerate_sps_default * 1e-3
             ),
             V_input_max_uV=round(data.V_input_max_mV * 1e3),
             I_input_max_nA=round(data.I_input_max_mA * 1e6),
             V_input_drop_uV=round(data.V_input_drop_mV * 1e3),
             R_input_kOhm_n22=round(data.R_input_mOhm * (1e-6 * 2**22)),
             Constant_us_per_nF_n28=data.calc_cap_constant_us_per_nF_n28(),
             V_intermediate_init_uV=round(data.V_intermediate_init_mV * 1e3),
             I_intermediate_leak_nA=round(data.I_intermediate_leak_nA),
-            V_enable_output_threshold_uV=round(
-                states["V_enable_output_threshold_mV"] * 1e3
-            ),
-            V_disable_output_threshold_uV=round(
-                states["V_disable_output_threshold_mV"] * 1e3
-            ),
+            V_enable_output_threshold_uV=round(states["V_enable_output_threshold_mV"] * 1e3),
+            V_disable_output_threshold_uV=round(states["V_disable_output_threshold_mV"] * 1e3),
             dV_enable_output_uV=round(states["dV_enable_output_mV"] * 1e3),
             interval_check_thresholds_n=round(
                 data.interval_check_thresholds_ms * samplerate_sps_default * 1e-3
             ),
-            V_pwr_good_enable_threshold_uV=round(
-                data.V_pwr_good_enable_threshold_mV * 1e3
-            ),
-            V_pwr_good_disable_threshold_uV=round(
-                data.V_pwr_good_disable_threshold_mV * 1e3
-            ),
+            V_pwr_good_enable_threshold_uV=round(data.V_pwr_good_enable_threshold_mV * 1e3),
+            V_pwr_good_disable_threshold_uV=round(data.V_pwr_good_disable_threshold_mV * 1e3),
             immediate_pwr_good_signal=data.immediate_pwr_good_signal,
-            V_output_log_gpio_threshold_uV=round(
-                data.V_output_log_gpio_threshold_mV * 1e3
-            ),
+            V_output_log_gpio_threshold_uV=round(data.V_output_log_gpio_threshold_mV * 1e3),
             # Boost-Converter
             V_input_boost_threshold_uV=round(data.V_input_boost_threshold_mV * 1e3),
             V_intermediate_max_uV=round(data.V_intermediate_max_mV * 1e3),
             # Buck-Converter
             V_output_uV=round(data.V_output_mV * 1e3),
             V_buck_drop_uV=round(data.V_buck_drop_mV * 1e3),
             # LUTs
             LUT_input_V_min_log2_uV=data.LUT_input_V_min_log2_uV,
             LUT_input_I_min_log2_nA=data.LUT_input_I_min_log2_nA,
             LUT_output_I_min_log2_nA=data.LUT_output_I_min_log2_nA,
             LUT_inp_efficiency_n8=[
-                [min(255, round(256 * ival)) for ival in il]
-                for il in data.LUT_input_efficiency
+                [min(255, round(256 * ival)) for ival in il] for il in data.LUT_input_efficiency
             ],
             LUT_out_inv_efficiency_n4=[
                 min((2**14), round((2**4) / value)) if (value > 0) else int(2**14)
                 for value in data.LUT_output_efficiency
             ],
         )
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/doc_virtual_source.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,14 @@
-from pathlib import Path
-
 from pydantic import Field
-from pydantic import model_validator
 
-from .. import logger
-from ..data_models import Fixture
 from ..data_models import ShpModel
 from .content import VirtualHarvesterConfig
 from .content.virtual_source import LUT1D
 from .content.virtual_source import LUT2D
 
-fixture_path = Path(__file__).resolve().with_name("content/virtual_source_fixture.yaml")
-fixtures = Fixture(fixture_path, "content.VirtualSource")
-
 
 @DeprecationWarning
 class VirtualSourceDoc(ShpModel, title="Virtual Source (Documented, Testversion)"):
     # General Config
     name: str = Field(
         title="Name of Virtual Source",
         description="Slug to use this Name as later reference",
@@ -209,15 +201,7 @@
     LUT_output_I_min_log2_nA: int = Field(
         description="Example: n=8, 2^n = 256 nA -> array[0] is for inputs < 256 nA, "
         "see notes on LUT_input for explanation",
         default=0,
         ge=0,
         le=20,
     )
-
-    @model_validator(mode="before")
-    @classmethod
-    def query_database(cls, values: dict) -> dict:
-        values = fixtures.try_completing_model(values)
-        values, chain = fixtures.try_inheritance(values)
-        logger.debug("VSrc-Inheritances: %s", chain)
-        return values
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/experiment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from datetime import datetime
 from datetime import timedelta
 from typing import List
 from typing import Optional
+from typing import Union
+from uuid import uuid4
 
-from pydantic import EmailStr
+from pydantic import UUID4
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
-from ..base.content import id_default
 from ..base.shepherd import ShpModel
 from ..testbed.target import Target
 from ..testbed.testbed import Testbed
 from .observer_features import SystemLogging
 from .target_config import TargetConfig
 
 
 class Experiment(ShpModel, title="Config of an Experiment"):
     """Configuration for Experiments on the Shepherd-Testbed
-    emulating Energy Environments for Target Nodes"""
+    emulating Energy Environments for Target Nodes
+    """
 
     # General Properties
-    id: IdInt = Field(  # noqa: A003
-        description="Unique ID",
-        default_factory=id_default,
-    )
+    # id: UUID4 ... # TODO db-migration - temp fix for documentation
+    id: Union[UUID4, int] = Field(default_factory=uuid4)
     # ⤷ TODO: automatic ID is problematic for identification by hash
+
     name: NameStr
     description: Annotated[
         Optional[SafeStr], Field(description="Required for public instances")
     ] = None
     comment: Optional[SafeStr] = None
     created: datetime = Field(default_factory=datetime.now)
 
-    # Ownership & Access, TODO
-    owner_id: Optional[IdInt] = 5472  # UUID?
+    # Ownership & Access
+    owner_id: Optional[IdInt] = None
 
     # feedback
-    email_results: Optional[EmailStr] = None
-    # ⤷ TODO: can be bool, as its linked to account
+    email_results: bool = False
+
     sys_logging: SystemLogging = SystemLogging(dmesg=True, ptp=True, shepherd=True)
 
     # schedule
     time_start: Optional[datetime] = None  # = ASAP
     duration: Optional[timedelta] = None  # = till EOF
     abort_on_error: bool = False
 
     # targets
-    target_configs: Annotated[List[TargetConfig], Field(min_length=1, max_length=64)]
+    target_configs: Annotated[List[TargetConfig], Field(min_length=1, max_length=128)]
 
     # TODO: we probably need to remember the lib-version for content &| experiment
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         self.validate_targets(self.target_configs)
         self.validate_observers(self.target_configs)
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Duration of experiment can't be negative.")
         return self
 
     @staticmethod
@@ -74,43 +76,29 @@
             if _config.custom_IDs is not None:
                 custom_ids = custom_ids + _config.custom_IDs[: len(_config.target_IDs)]
             else:
                 custom_ids = custom_ids + _config.target_IDs
         if len(target_ids) > len(set(target_ids)):
             raise ValueError("Target-ID used more than once in Experiment!")
         if len(target_ids) > len(set(custom_ids)):
-            raise ValueError(
-                "Custom Target-ID are faulty (some form of id-collisions)!"
-            )
+            raise ValueError("Custom Target-ID are faulty (some form of id-collisions)!")
 
     @staticmethod
     def validate_observers(configs: List[TargetConfig]) -> None:
-        target_ids = []
-        for _config in configs:
-            for _id in _config.target_IDs:
-                target_ids.append(_id)
+        target_ids = [_id for _config in configs for _id in _config.target_IDs]
 
         testbed = Testbed(name="shepherd_tud_nes")
-        obs_ids = []
-        for _id in target_ids:
-            obs_ids.append(testbed.get_observer(_id).id)
+        obs_ids = [testbed.get_observer(_id).id for _id in target_ids]
         if len(target_ids) > len(set(obs_ids)):
             raise ValueError(
-                "Observer used more than once in Experiment "
-                "-> only 1 target per observer!"
+                "Observer used more than once in Experiment -> only 1 target per observer!"
             )
 
     def get_target_ids(self) -> list:
-        target_ids = []
-        for _config in self.target_configs:
-            for _id in _config.target_IDs:
-                target_ids.append(_id)
-        return target_ids
+        return [_id for _config in self.target_configs for _id in _config.target_IDs]
 
     def get_target_config(self, target_id: int) -> TargetConfig:
         for _config in self.target_configs:
             if target_id in _config.target_IDs:
                 return _config
-        # .. gets already caught in target_config .. but keep:
-        raise ValueError(
-            f"Target-ID {target_id} was not found in Experiment '{self.name}'"
-        )
+        # gets already caught in target_config - but keep:
+        raise ValueError(f"Target-ID {target_id} was not found in Experiment '{self.name}'")
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 
 import numpy as np
 from pydantic import Field
 from pydantic import PositiveFloat
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.shepherd import ShpModel
 from ..testbed.gpio import GPIO
 
 
 class PowerTracing(ShpModel, title="Config for Power-Tracing"):
     """Configuration for recording the Power-Consumption of the Target Nodes
@@ -30,55 +31,53 @@
     calculate_power: bool = False
     samplerate: Annotated[int, Field(ge=10, le=100_000)] = 100_000  # down-sample
     discard_current: bool = False
     discard_voltage: bool = False
     # ⤷ reduce file-size by omitting current / voltage
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         if self.delay and self.delay.total_seconds() < 0:
             raise ValueError("Delay can't be negative.")
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Duration can't be negative.")
 
         discard_all = self.discard_current and self.discard_voltage
         if not self.calculate_power and discard_all:
-            raise ValueError(
-                "Error in config -> tracing enabled, but output gets discarded"
-            )
+            raise ValueError("Error in config -> tracing enabled, but output gets discarded")
         if self.calculate_power:
             raise ValueError("postprocessing not implemented ATM")
         return self
 
 
 class GpioTracing(ShpModel, title="Config for GPIO-Tracing"):
     """Configuration for recording the GPIO-Output of the Target Nodes
     TODO: postprocessing not implemented ATM
     """
 
     # initial recording
     mask: Annotated[int, Field(ge=0, lt=2**10)] = 0b11_1111_1111  # all
     # ⤷ TODO: custom mask not implemented in PRU, ATM
-    gpios: Optional[
-        Annotated[List[GPIO], Field(min_length=1, max_length=10)]
-    ] = None  # = all
+    gpios: Optional[Annotated[List[GPIO], Field(min_length=1, max_length=10)]] = None  # = all
     # ⤷ TODO: list of GPIO to build mask, one of both should be internal / computed field
 
     # time
     delay: timedelta = 0  # seconds
     duration: Optional[timedelta] = None  # till EOF
 
     # post-processing,
-    uart_decode: bool = False  # todo: is currently done online in userspace
+    uart_decode: bool = False
+    # TODO: quickfix - uart-log currently done online in userspace
+    # NOTE: gpio-tracing currently shows rather big - but rare - "blind" windows (~1-4us)
     uart_pin: GPIO = GPIO(name="GPIO8")
     uart_baudrate: Annotated[int, Field(ge=2_400, le=921_600)] = 115_200
     # TODO: add a "discard_gpio" (if only uart is wanted)
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         if self.mask == 0:
             raise ValueError("Error in config -> tracing enabled but mask is 0")
         if self.delay and self.delay.total_seconds() < 0:
             raise ValueError("Delay can't be negative.")
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Duration can't be negative.")
         return self
@@ -99,43 +98,42 @@
     gpio: GPIO
     level: GpioLevel
     period: Annotated[float, Field(ge=10e-6)] = 1
     # ⤷ time base of periodicity in s
     count: Annotated[int, Field(ge=1, le=4096)] = 1
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         if not self.gpio.user_controllable():
-            raise ValueError(
-                f"GPIO '{self.gpio.name}' in actuation-event not controllable by user"
-            )
+            raise ValueError(f"GPIO '{self.gpio.name}' in actuation-event not controllable by user")
         return self
 
     def get_events(self) -> np.ndarray:
         stop = self.delay + self.count * self.period
         return np.arange(self.delay, stop, self.period)
 
 
 class GpioActuation(ShpModel, title="Config for GPIO-Actuation"):
-    """Configuration for a GPIO-Actuation-Sequence
-    TODO: not implemented ATM:
-        - decide if pru control sys-gpio or
-        - reverses pru-gpio (preferred if possible)
-    """
+    """Configuration for a GPIO-Actuation-Sequence"""
+
+    # TODO: not implemented ATM - decide if pru control sys-gpio or
+    # TODO: not implemented ATM - reverses pru-gpio (preferred if possible)
 
     events: Annotated[List[GpioEvent], Field(min_length=1, max_length=1024)]
 
     def get_gpios(self) -> set:
         return {_ev.gpio for _ev in self.events}
 
 
 class SystemLogging(ShpModel, title="Config for System-Logging"):
     """Configuration for recording Debug-Output of the Observers System-Services"""
 
     dmesg: bool = True
     ptp: bool = True
     shepherd: bool = True
+    # TODO: rename to kernel, timesync, sheep
+    # TODO: add utilization as option
 
 
 # TODO: some more interaction would be good
 #     - execute limited python-scripts
 #     - send uart-frames
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/experiment/target_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.energy_environment import EnergyEnvironment
 from ..content.firmware import Firmware
 from ..content.virtual_source import VirtualSourceConfig
 from ..testbed.target import IdInt16
@@ -16,42 +17,38 @@
 from .observer_features import GpioTracing
 from .observer_features import PowerTracing
 
 
 class TargetConfig(ShpModel, title="Target Config"):
     """Configuration for Target Nodes (DuT)"""
 
-    target_IDs: Annotated[List[IdInt], Field(min_length=1, max_length=64)]
-    custom_IDs: Optional[
-        Annotated[List[IdInt16], Field(min_length=1, max_length=64)]
-    ] = None
+    target_IDs: Annotated[List[IdInt], Field(min_length=1, max_length=128)]
+    custom_IDs: Optional[Annotated[List[IdInt16], Field(min_length=1, max_length=128)]] = None
     # ⤷ will replace 'const uint16_t SHEPHERD_NODE_ID' in firmware
     #   if no custom ID is provided, the original ID of target is used
 
     energy_env: EnergyEnvironment  # alias: input
     virtual_source: VirtualSourceConfig = VirtualSourceConfig(name="neutral")
     target_delays: Optional[
-        Annotated[List[Annotated[int, Field(ge=0)]], Field(min_length=1, max_length=64)]
+        Annotated[List[Annotated[int, Field(ge=0)]], Field(min_length=1, max_length=128)]
     ] = None
     # ⤷ individual starting times -> allows to use the same environment
     # TODO: delays not used ATM
 
     firmware1: Firmware
     firmware2: Optional[Firmware] = None
 
     power_tracing: Optional[PowerTracing] = None
     gpio_tracing: Optional[GpioTracing] = None
     gpio_actuation: Optional[GpioActuation] = None
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         if not self.energy_env.valid:
-            raise ValueError(
-                f"EnergyEnv '{self.energy_env.name}' for target must be valid"
-            )
+            raise ValueError(f"EnergyEnv '{self.energy_env.name}' for target must be valid")
         for _id in self.target_IDs:
             target = Target(id=_id)
             for mcu_num in [1, 2]:
                 val_fw = getattr(self, f"firmware{mcu_num}")
                 has_fw = val_fw is not None
                 tgt_mcu = target[f"mcu{mcu_num}"]
                 has_mcu = tgt_mcu is not None
@@ -71,16 +68,15 @@
                         f"is incompatible (={tgt_mcu.name})"
                     )
 
         c_ids = self.custom_IDs
         t_ids = self.target_IDs
         if c_ids is not None and (len(set(c_ids)) < len(set(t_ids))):
             raise ValueError(
-                f"Provided custom IDs {c_ids} not enough "
-                f"to cover target range {t_ids}"
+                f"Provided custom IDs {c_ids} not enough to cover target range {t_ids}"
             )
         # TODO: if custom ids present, firmware must be ELF
         return self
 
     def get_custom_id(self, target_id: int) -> Optional[int]:
         if self.custom_IDs is not None and target_id in self.target_IDs:
             return self.custom_IDs[self.target_IDs.index(target_id)]
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,24 @@
     "Compression",
     # helper functions
     "prepare_task",
     "extract_tasks",
 ]
 
 
-def prepare_task(
-    config: Union[ShpModel, Path, str], observer: Optional[str] = None
-) -> Wrapper:
-    """
-    - Opens file (from Path or str of Path)
+def prepare_task(config: Union[ShpModel, Path, str], observer: Optional[str] = None) -> Wrapper:
+    """- Opens file (from Path or str of Path)
     - wraps task-model
     - and if it's an TestbedTasks it will extract the correct ObserverTask
     """
     if isinstance(config, str):
         config = Path(config)
 
     if isinstance(config, Path):
-        with open(config.resolve()) as shp_file:
+        with config.resolve().open() as shp_file:
             shp_dict = yaml.safe_load(shp_file)
         shp_wrap = Wrapper(**shp_dict)
     elif isinstance(config, ShpModel):
         shp_wrap = Wrapper(
             datatype=type(config).__name__,
             parameters=config.model_dump(),
         )
@@ -70,30 +67,28 @@
         shp_wrap = Wrapper(
             datatype=type(obt).__name__,
             parameters=obt.model_dump(),
         )
     return shp_wrap
 
 
-def extract_tasks(shp_wrap: Wrapper, no_task_sets: bool = True) -> List[ShpModel]:
+def extract_tasks(shp_wrap: Wrapper, *, no_task_sets: bool = True) -> List[ShpModel]:
     """ """
     if shp_wrap.datatype == ObserverTasks.__name__:
         obt = ObserverTasks(**shp_wrap.parameters)
         content = obt.get_tasks()
     elif shp_wrap.datatype == EmulationTask.__name__:
         content = [EmulationTask(**shp_wrap.parameters)]
     elif shp_wrap.datatype == HarvestTask.__name__:
         content = [HarvestTask(**shp_wrap.parameters)]
     elif shp_wrap.datatype == FirmwareModTask.__name__:
         content = [FirmwareModTask(**shp_wrap.parameters)]
     elif shp_wrap.datatype == ProgrammingTask.__name__:
         content = [ProgrammingTask(**shp_wrap.parameters)]
     elif shp_wrap.datatype == TestbedTasks.__name__:
         if no_task_sets:
-            raise ValueError(
-                "Model in Wrapper was TestbedTasks -> Task-Sets not allowed!"
-            )
+            raise ValueError("Model in Wrapper was TestbedTasks -> Task-Sets not allowed!")
         content = [TestbedTasks(**shp_wrap.parameters)]
     else:
         raise ValueError("Extractor had unknown task: %s", shp_wrap.datatype)
 
     return content
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/emulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 from typing import Optional
 from typing import Union
 
 from pydantic import Field
 from pydantic import model_validator
 from pydantic import validate_call
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
+from ..base.timezone import local_tz
 from ..content.virtual_source import VirtualSourceConfig
 from ..experiment.experiment import Experiment
 from ..experiment.observer_features import GpioActuation
 from ..experiment.observer_features import GpioTracing
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from ..testbed import Testbed
 from ..testbed.cape import TargetPort
 
 
 class Compression(str, Enum):
     lzf = "lzf"  # not native hdf5
     gzip1 = 1  # higher compr & load
     gzip = 1
-    default = 1
+    default = "lzf"
     null = None
+    # NOTE: changed to lzf as BBB needs every straw it can get
 
 
 compressions_allowed: list = [None, "lzf", 1]
 c_translate = {"lzf": "lzf", "1": 1, "None": None, None: None}
 
 
 class EmulationTask(ShpModel):
@@ -46,28 +49,27 @@
     #   - providing a directory -> file is named emu_timestamp.h5
     #   - for a complete path the filename is not changed except it exists and
     #     overwrite is disabled -> emu#num.h5
     # TODO: should the output-path be mandatory?
     force_overwrite: bool = False
     # ⤷ Overwrite existing file
     output_compression: Optional[Compression] = Compression.default
-    # ⤷ should be 1 (level 1 gzip), lzf, or None (order of recommendation)
-
+    # ⤷ should be lzf, 1 (gzip level 1) or None (order of recommendation)
     time_start: Optional[datetime] = None
     # timestamp or unix epoch time, None = ASAP
     duration: Optional[timedelta] = None
     # ⤷ Duration of recording in seconds, None = till EOF
     abort_on_error: bool = False
 
     # emulation-specific
     use_cal_default: bool = False
     # ⤷ Use default calibration values, skip loading from EEPROM
 
     enable_io: bool = False
-    # TODO: direction of pins! also it seems error-prone when only setting _tracing
+    # TODO: add direction of pins! also it seems error-prone when only setting _tracing
     # ⤷ Switch the GPIO level converter to targets on/off
     #   pre-req for sampling gpio,
     io_port: TargetPort = TargetPort.A
     # ⤷ Either Port A or B that gets connected to IO
     pwr_port: TargetPort = TargetPort.A
     # ⤷ chosen port will be current-monitored (main, connected to virtual Source),
     #   the other port is aux
@@ -84,66 +86,63 @@
 
     power_tracing: Optional[PowerTracing] = PowerTracing()
     gpio_tracing: Optional[GpioTracing] = GpioTracing()
     gpio_actuation: Optional[GpioActuation] = None
     sys_logging: Optional[SystemLogging] = SystemLogging()
 
     verbose: Annotated[int, Field(ge=0, le=4)] = 2
-    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
+    # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug, TODO: just bool now, systemwide
 
     @model_validator(mode="before")
     @classmethod
     def pre_correction(cls, values: dict) -> dict:
         # convert & add local timezone-data
         has_time = values.get("time_start") is not None
         if has_time and isinstance(values["time_start"], (int, float)):
-            values["time_start"] = datetime.fromtimestamp(values["time_start"])
+            values["time_start"] = datetime.fromtimestamp(values["time_start"], tz=local_tz())
         if has_time and isinstance(values["time_start"], str):
             values["time_start"] = datetime.fromisoformat(values["time_start"])
         if has_time and values["time_start"].tzinfo is None:
             values["time_start"] = values["time_start"].astimezone()
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         # TODO: limit paths
         has_time = self.time_start is not None
         time_now = datetime.now().astimezone()
         if has_time and self.time_start < time_now:
             raise ValueError(
                 "Start-Time for Emulation can't be in the past "
                 f"('{self.time_start}' vs '{time_now}'."
             )
         if self.duration and self.duration.total_seconds() < 0:
             raise ValueError("Task-Duration can't be negative.")
-        if isinstance(self.voltage_aux, str) and self.voltage_aux not in [
+        if isinstance(self.voltage_aux, str) and self.voltage_aux not in {
             "main",
             "buffer",
-        ]:
-            raise ValueError(
-                "Voltage Aux must be in float (0 - 4.5) or string 'main' / 'mid'."
-            )
+        }:
+            raise ValueError("Voltage Aux must be in float (0 - 4.5) or string 'main' / 'mid'.")
         if self.gpio_actuation is not None:
             raise ValueError("GPIO Actuation not yet implemented!")
         return self
 
     @classmethod
     @validate_call
-    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt, root_path: Path):
+    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt, root_path: Path) -> Self:
         obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
         return cls(
             input_path=tgt_cfg.energy_env.data_path,
             output_path=root_path / f"emu_{obs.name}.h5",
             time_start=copy.copy(xp.time_start),
             duration=xp.duration,
             abort_on_error=xp.abort_on_error,
-            enable_io=(tgt_cfg.gpio_tracing is not None)
-            or (tgt_cfg.gpio_actuation is not None),
+            enable_io=(tgt_cfg.gpio_tracing is not None) or (tgt_cfg.gpio_actuation is not None),
             io_port=obs.get_target_port(tgt_id),
             pwr_port=obs.get_target_port(tgt_id),
             virtual_source=tgt_cfg.virtual_source,
             power_tracing=tgt_cfg.power_tracing,
             gpio_tracing=tgt_cfg.gpio_tracing,
             gpio_actuation=tgt_cfg.gpio_actuation,
             sys_logging=xp.sys_logging,
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/firmware_mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import copy
 from pathlib import Path
 from typing import Optional
+from typing import TypedDict
 from typing import Union
 
 from pydantic import Field
 from pydantic import model_validator
 from pydantic import validate_call
 from typing_extensions import Annotated
+from typing_extensions import Self
+from typing_extensions import Unpack
 
 from ...logger import logger
 from ..base.content import IdInt
 from ..base.shepherd import ShpModel
 from ..content.firmware import Firmware
 from ..content.firmware import FirmwareDType
 from ..content.firmware import FirmwareStr
@@ -28,38 +31,37 @@
     custom_id: Optional[IdInt16] = None
     firmware_file: Path
 
     verbose: Annotated[int, Field(ge=0, le=4)] = 2
     # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
 
     @model_validator(mode="after")
-    def post_validation(self):
-        if self.data_type in [
+    def post_validation(self) -> Self:
+        if self.data_type in {
             FirmwareDType.base64_hex,
             FirmwareDType.path_hex,
-        ]:
-            logger.warning(
-                "Firmware is scheduled to get custom-ID but is not in elf-format"
-            )
+        }:
+            logger.warning("Firmware is scheduled to get custom-ID but is not in elf-format")
         return self
 
     @classmethod
     @validate_call
     def from_xp(
         cls,
         xp: Experiment,
         tb: Testbed,
         tgt_id: IdInt,
         mcu_port: MCUPort,
         fw_path: Path,
-    ):
+    ) -> Self:
         tgt_cfg = xp.get_target_config(tgt_id)
 
         fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
         if fw is None:
+            # TODO: if target has default fw -> use that! otherwise no sleep is flashed
             return None
 
         fw_id = tgt_cfg.get_custom_id(tgt_id)
         if fw_id is None:
             obs = tb.get_observer(tgt_id)
             fw_id = obs.get_target(tgt_id).testbed_id
 
@@ -67,16 +69,21 @@
             data=fw.data,
             data_type=fw.data_type,
             custom_id=fw_id,
             firmware_file=copy.copy(fw_path),
         )
 
     @classmethod
-    @validate_call
-    def from_firmware(cls, fw: Firmware, **kwargs):
+    def from_firmware(
+        cls,
+        fw: Firmware,
+        **kwargs: Unpack[TypedDict],
+    ) -> Self:
+        if not isinstance(fw, Firmware):
+            raise ValueError("fw-argument must be of type Firmware")
         kwargs["data"] = fw.data
         kwargs["data_type"] = fw.data_type
         fw.compare_hash()
         path = kwargs.get("firmware_file")
         if path is not None and path.is_dir():
             path_new: Path = path / fw.name
             kwargs["firmware_file"] = path_new.with_suffix(".hex")
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/harvest.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.shepherd import ShpModel
+from ..base.timezone import local_tz
 from ..content.virtual_harvester import VirtualHarvesterConfig
 from ..experiment.observer_features import PowerTracing
 from ..experiment.observer_features import SystemLogging
 from .emulation import Compression
 
 
 class HarvestTask(ShpModel):
@@ -54,23 +56,23 @@
 
     @model_validator(mode="before")
     @classmethod
     def pre_correction(cls, values: dict) -> dict:
         # convert & add local timezone-data, TODO: used twice, refactor
         has_time = values.get("time_start") is not None
         if has_time and isinstance(values["time_start"], (int, float)):
-            values["time_start"] = datetime.fromtimestamp(values["time_start"])
+            values["time_start"] = datetime.fromtimestamp(values["time_start"], tz=local_tz())
         if has_time and isinstance(values["time_start"], str):
             values["time_start"] = datetime.fromisoformat(values["time_start"])
         if has_time and values["time_start"].tzinfo is None:
             values["time_start"] = values["time_start"].astimezone()
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         # TODO: limit paths
         has_time = self.time_start is not None
         time_now = datetime.now().astimezone()
         if has_time and self.time_start < time_now:
             raise ValueError(
                 "Start-Time for Emulation can't be in the past "
                 f"('{self.time_start}' vs '{time_now}'."
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/observer_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from pydantic import validate_call
+from typing_extensions import Self
 
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.testbed import Testbed
 from .emulation import EmulationTask
@@ -16,15 +17,15 @@
 from .programming import ProgrammingTask
 
 
 class ObserverTasks(ShpModel):
     """Collection of tasks for selected observer included in experiment"""
 
     observer: NameStr
-    owner_id: IdInt
+    owner_id: Optional[IdInt]  # TODO: set to optional for now, shouldn't be
 
     # PRE PROCESS
     time_prep: datetime  # TODO: should be optional
     root_path: Path
     abort_on_error: bool
 
     # fw mod, store as hex-file and program
@@ -40,15 +41,15 @@
     #  - delete firmwares
     #  - decode uart
     #  - downsample
     #  - zip it
 
     @classmethod
     @validate_call
-    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt):
+    def from_xp(cls, xp: Experiment, tb: Testbed, tgt_id: IdInt) -> Self:
         if not tb.shared_storage:
             raise ValueError("Implementation currently relies on shared storage!")
 
         t_start = (
             xp.time_start
             if isinstance(xp.time_start, datetime)
             else datetime.now().astimezone() + timedelta(minutes=3)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/programming.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/programming.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 from pathlib import Path
+from typing import Optional
 
 from pydantic import Field
 from pydantic import model_validator
 from pydantic import validate_call
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ..base.content import IdInt
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 from ..content.firmware import suffix_to_DType
 from ..content.firmware_datatype import FirmwareDType
 from ..experiment.experiment import Experiment
@@ -32,30 +34,30 @@
 
     simulate: bool = False
 
     verbose: Annotated[int, Field(ge=0, le=4)] = 2
     # ⤷ 0=Errors, 1=Warnings, 2=Info, 3=Debug
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         d_type = suffix_to_DType.get(self.firmware_file.suffix.lower())
         if d_type != FirmwareDType.base64_hex:
             ValueError(f"Firmware is not intel-.hex ('{self.firmware_file}')")
         return self
 
     @classmethod
     @validate_call
     def from_xp(
         cls,
         xp: Experiment,
         tb: Testbed,
         tgt_id: IdInt,
         mcu_port: MCUPort,
         fw_path: Path,
-    ):
+    ) -> Optional[Self]:
         obs = tb.get_observer(tgt_id)
         tgt_cfg = xp.get_target_config(tgt_id)
 
         fw = tgt_cfg.firmware1 if mcu_port == 1 else tgt_cfg.firmware2
         if fw is None:
             return None
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from typing import List
 from typing import Optional
 
-from pydantic import EmailStr
 from pydantic import Field
 from pydantic import validate_call
 from typing_extensions import Annotated
+from typing_extensions import Self
 
+from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.shepherd import ShpModel
 from ..experiment.experiment import Experiment
 from ..testbed.testbed import Testbed
 from .observer_tasks import ObserverTasks
 
 
 class TestbedTasks(ShpModel):
     """Collection of tasks for all observers included in experiment"""
 
     name: NameStr
-    observer_tasks: Annotated[List[ObserverTasks], Field(min_length=1, max_length=64)]
+    observer_tasks: Annotated[List[ObserverTasks], Field(min_length=1, max_length=128)]
 
     # POST PROCESS
-    email: Optional[EmailStr] = None
+    email_results: bool = False
+    owner_id: Optional[IdInt]
+    # TODO: had real email previously, does it really need these at all?
+    #  DB stores experiment and knows when to email
 
     @classmethod
     @validate_call
-    def from_xp(cls, xp: Experiment, tb: Optional[Testbed] = None):
+    def from_xp(cls, xp: Experiment, tb: Optional[Testbed] = None) -> Self:
         if tb is None:
             # TODO: just for testing OK
             tb = Testbed(name="shepherd_tud_nes")
         tgt_ids = xp.get_target_ids()
         obs_tasks = [ObserverTasks.from_xp(xp, tb, _id) for _id in tgt_ids]
         return cls(
             name=xp.name,
             observer_tasks=obs_tasks,
-            email=xp.email_results,
+            email_results=xp.email_results,
+            owner_id=xp.owner_id,
         )
 
-    def get_observer_tasks(self, observer) -> Optional[ObserverTasks]:
+    def get_observer_tasks(self, observer: str) -> Optional[ObserverTasks]:
         for tasks in self.observer_tasks:
             if observer == tasks.observer:
                 return tasks
         return None
 
     def get_output_paths(self) -> dict:
         # TODO: computed field preferred, but they don't work here, as
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/cape.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     a = "A"
     b = "B"
 
 
 class Cape(ShpModel, title="Shepherd-Cape"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     version: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
     # TODO: wake_interval, calibration
 
     active: bool = True
     created: Union[date, datetime] = Field(default_factory=datetime.now)
     calibrated: Union[date, datetime, None] = None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/gpio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Optional
 
 from pydantic import Field
 from pydantic import StringConstraints
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 
@@ -21,43 +22,43 @@
     Bidirectional = "IO"
     IO = "IO"
 
 
 class GPIO(ShpModel, title="GPIO of Observer Node"):
     """meta-data representation of a testbed-component"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     description: Optional[SafeStr] = None
     comment: Optional[SafeStr] = None
 
     direction: Direction = Direction.Input
     dir_switch: Optional[Annotated[str, StringConstraints(max_length=32)]] = None
 
     reg_pru: Optional[Annotated[str, StringConstraints(max_length=10)]] = None
     pin_pru: Optional[Annotated[str, StringConstraints(max_length=10)]] = None
     reg_sys: Optional[Annotated[int, Field(ge=0)]] = None
     pin_sys: Optional[Annotated[str, StringConstraints(max_length=10)]] = None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         # ensure that either pru or sys is used, otherwise instance is considered faulty
         no_pru = (self.reg_pru is None) or (self.pin_pru is None)
         no_sys = (self.reg_sys is None) or (self.pin_sys is None)
         if no_pru and no_sys:
             raise ValueError(
                 "GPIO-Instance is faulty -> "
                 f"it needs to use pru or sys, content: {self.model_dump()}"
             )
         return self
 
     def user_controllable(self) -> bool:
-        return ("gpio" in self.name.lower()) and (self.direction in ["IO", "OUT"])
+        return ("gpio" in self.name.lower()) and (self.direction in {"IO", "OUT"})
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/mcu.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,29 @@
     UART = "UART"
     uart = "UART"
 
 
 class MCU(ShpModel, title="Microcontroller of the Target Node"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     platform: NameStr
     core: NameStr
     prog_protocol: ProgrammerProtocol
     prog_voltage: Annotated[float, Field(ge=1, le=5)] = 3
     prog_datarate: Annotated[int, Field(gt=0, le=1_000_000)] = 500_000
 
     fw_name_default: str
     # ⤷ can't be FW-Object (circular import)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/observer.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 from typing import Optional
 
 from pydantic import Field
 from pydantic import IPvAnyAddress
 from pydantic import StringConstraints
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 from .cape import Cape
 from .cape import TargetPort
 from .target import Target
 
 MACStr = Annotated[
     str,
-    StringConstraints(
-        max_length=17, pattern=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$"
-    ),
+    StringConstraints(max_length=17, pattern=r"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$"),
 ]
 
 
 class Observer(ShpModel, title="Shepherd-Sheep"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     ip: IPvAnyAddress
     mac: MACStr
 
@@ -46,60 +45,46 @@
     cape: Optional[Cape] = None
     target_a: Optional[Target] = None
     target_b: Optional[Target] = None
 
     created: datetime = Field(default_factory=datetime.now)
     alive_last: Optional[datetime] = None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         has_cape = self.cape is not None
         has_target = (self.target_a is not None) or (self.target_b is not None)
         if not has_cape and has_target:
-            raise ValueError(
-                f"Observer '{self.name}' is faulty " f"-> has targets but no cape"
-            )
+            raise ValueError(f"Observer '{self.name}' is faulty -> has targets but no cape")
         return self
 
     def has_target(self, target_id: int) -> bool:
-        if (
-            self.target_a is not None
-            and target_id == self.target_a.id
-            and self.target_a.active
-        ):
+        if self.target_a is not None and target_id == self.target_a.id and self.target_a.active:
             return True
-        if (
-            self.target_b is not None
-            and target_id == self.target_b.id
-            and self.target_b.active
-        ):
+        if self.target_b is not None and target_id == self.target_b.id and self.target_b.active:
             return True
         return False
 
     def get_target_port(self, target_id: int) -> TargetPort:
         if self.has_target(target_id):
             if self.target_a is not None and target_id == self.target_a.id:
                 return TargetPort.A
             if self.target_b is not None and target_id == self.target_b.id:
                 return TargetPort.B
-        raise ValueError(
-            f"Target-ID {target_id} was not found in Observer '{self.name}'"
-        )
+        raise ValueError(f"Target-ID {target_id} was not found in Observer '{self.name}'")
 
     def get_target(self, target_id: int) -> Target:
         if self.has_target(target_id):
             if self.target_a is not None and target_id == self.target_a.id:
                 return self.target_a
             if self.target_b is not None and target_id == self.target_b.id:
                 return self.target_b
-        raise ValueError(
-            f"Target-ID {target_id} was not found in Observer '{self.name}'"
-        )
+        raise ValueError(f"Target-ID {target_id} was not found in Observer '{self.name}'")
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 MCUPort = Annotated[int, Field(ge=1, le=2)]
 
 
 class Target(ShpModel, title="Target Node (DuT)"):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     version: NameStr
     description: SafeStr
 
     comment: Optional[SafeStr] = None
 
     active: bool = True
@@ -34,15 +34,15 @@
     testbed_id: Optional[IdInt16] = None
     # ⤷ is derived from ID (targets are still selected by id!)
     mcu1: Union[MCU, NameStr]
     mcu2: Union[MCU, NameStr, None] = None
 
     # TODO programming pins per mcu should be here (or better in Cape)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2024.4.1/shepherd_core/data_models/testbed/testbed.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 from typing import List
 from typing import Optional
 
 from pydantic import Field
 from pydantic import HttpUrl
 from pydantic import model_validator
 from typing_extensions import Annotated
+from typing_extensions import Self
 
 from ...testbed_client import tb_client
 from ..base.content import IdInt
 from ..base.content import NameStr
 from ..base.content import SafeStr
 from ..base.shepherd import ShpModel
 from .observer import Observer
 
 
 class Testbed(ShpModel):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt  # noqa: A003
+    id: IdInt
     name: NameStr
     description: SafeStr
     comment: Optional[SafeStr] = None
 
     url: Optional[HttpUrl] = None
 
-    observers: Annotated[List[Observer], Field(min_length=1, max_length=64)]
+    observers: Annotated[List[Observer], Field(min_length=1, max_length=128)]
 
     shared_storage: bool = True
     data_on_server: Path
     data_on_observer: Path
     # ⤷ storage layout: root_path/content_type/group/owner/[object]
 
     prep_duration: timedelta = timedelta(minutes=5)
@@ -39,15 +40,15 @@
     @model_validator(mode="before")
     @classmethod
     def query_database(cls, values: dict) -> dict:
         values, _ = tb_client.try_completing_model(cls.__name__, values)
         return values
 
     @model_validator(mode="after")
-    def post_validation(self):
+    def post_validation(self) -> Self:
         observers = []
         ips = []
         macs = []
         capes = []
         targets = []
         eth_ports = []
         for _obs in self.observers:
@@ -82,10 +83,8 @@
     def get_observer(self, target_id: int) -> Observer:
         for _observer in self.observers:
             if not _observer.active or not _observer.cape.active:
                 # skip decommissioned setups
                 continue
             if _observer.has_target(target_id):
                 return _observer
-        raise ValueError(
-            f"Target-ID {target_id} was not found in Testbed '{self.name}'"
-        )
+        raise ValueError(f"Target-ID {target_id} was not found in Testbed '{self.name}'")
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/decoder_waveform/uart.py` & `shepherd_core-2024.4.1/shepherd_core/decoder_waveform/uart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""
-UART - Decoder - Features:
+"""UART - Decoder - Features:
 - 1 bit Start (LOW)
 - 1 .. **8** .. 64 bit data-frame
 - **1**, 1.5, 2 bit stop (HIGH) - don't care?
 - **no**, even, odd parity bit (there are more, see sigrok-link) - TODO
 - **LSB** / MSB first - detectable with dict-compare - TODO
 - **no** inversion
 
-TODO:
+Todo:
+----
   - detect bitOrder
   - detect dataframe length
   - detect parity
 
 More Info:
 https://en.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter
 https://sigrok.org/wiki/Protocol_decoder:Uart
+
 """
+
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 import numpy as np
 
@@ -44,63 +46,52 @@
         self,
         content: Union[Path, np.ndarray],
         baud_rate: Optional[int] = None,
         frame_length: Optional[int] = 8,
         inversion: Optional[bool] = None,
         parity: Optional[Parity] = Parity.no,
         bit_order: Optional[BitOrder] = BitOrder.lsb_first,
-    ):
+    ) -> None:
         """Provide a file with two columns:
         - timestamp (seconds with fraction) and signal (can be analog).
         - class-parameters that are None (above) get auto-detected
           (some detectors still missing)
         """
-
         if isinstance(content, Path):
-            self.events_sig: np.ndarray = np.loadtxt(
-                content.as_posix(), delimiter=",", skiprows=1
-            )
+            self.events_sig: np.ndarray = np.loadtxt(content.as_posix(), delimiter=",", skiprows=1)
             # TODO: if float fails load as str -
             #  cast first col as np.datetime64 with ns-resolution, convert to delta
         else:
             self.events_sig = content
 
         # verify table
         if self.events_sig.shape[1] != 2:
-            raise TypeError(
-                "Input file should have 2 rows -> (comma-separated) timestamp & value"
-            )
+            raise TypeError("Input file should have 2 rows -> (comma-separated) timestamp & value")
         if self.events_sig.shape[0] < 8:
             raise TypeError("Input file is too short (< state-changes)")
         # verify timestamps
         time_steps = self.events_sig[1:, 0] - self.events_sig[:-1, 0]
         if any(time_steps < 0):
             raise TypeError("Timestamps are not continuous")
 
         # prepare samples & process params (order is important)
         self._convert_analog2digital()
         self._filter_redundant_states()
 
-        self.baud_rate: int = (
-            baud_rate if baud_rate is not None else self.detect_baud_rate()
-        )
+        self.baud_rate: int = baud_rate if baud_rate is not None else self.detect_baud_rate()
         self.dur_tick: float = 1.0 / self.baud_rate
 
         self._add_duration()
 
-        self.inversion: bool = (
-            inversion if inversion is not None else self.detect_inversion()
-        )
+        self.inversion: bool = inversion if inversion is not None else self.detect_inversion()
         self.half_stop: bool = self.detect_half_stop()  # not needed ATM
 
         # TODO: add detectors
         self.parity: Parity = parity if parity is not None else Parity.no
-        self.bit_order: BitOrder = (
-            bit_order if bit_order is not None else BitOrder.lsb_first
-        )
+        self.bit_order: BitOrder = bit_order if bit_order is not None else BitOrder.lsb_first
         self.frame_length: int = frame_length if frame_length is not None else 8
 
         if not (0 < self.frame_length <= 64):
             raise ValueError("Dataframe length is out of bound (0, 64]")
         if self.parity != Parity.no:
             raise ValueError("Parities beside 'no' are not supported ATM")
         if self.bit_order != BitOrder.lsb_first:
@@ -113,101 +104,91 @@
             logger.error("Signal still inverted?!? Check parameters and input")
 
         # results
         self.events_symbols: Optional[np.ndarray] = None
         self.events_lines: Optional[np.ndarray] = None
         self.text: Optional[str] = None
 
-    def _convert_analog2digital(self, invert: bool = False) -> None:
-        """divide dimension in two, divided by mean-value"""
+    def _convert_analog2digital(self, *, invert: bool = False) -> None:
+        """Divide dimension in two, divided by mean-value"""
         data = self.events_sig[:, 1]
         mean = np.mean(data)
         if invert:
             self.events_sig[:, 1] = data <= mean
         else:
             self.events_sig[:, 1] = data >= mean
 
     def _filter_redundant_states(self) -> None:
-        """sum of two sequential states is always 1 (True + False) if alternating"""
+        """Sum of two sequential states is always 1 (True + False) if alternating"""
         data_0 = self.events_sig[:, 1]
         data_1 = np.concatenate([[not data_0[0]], data_0[:-1]])
         data_f = data_0 + data_1
         self.events_sig = self.events_sig[data_f == 1]
 
         if len(data_0) > len(self.events_sig):
             logger.debug(
                 "filtered out %d/%d events (redundant)",
                 len(data_0) - len(self.events_sig),
                 len(data_0),
             )
 
     def _add_duration(self) -> None:
-        """calculate third column -> duration of state in [baud-ticks]"""
+        """Calculate third column -> duration of state in [baud-ticks]"""
         if self.events_sig.shape[1] > 2:
             logger.warning("Tried to add state-duration, but it seems already present")
             return
         if not hasattr(self, "dur_tick"):
-            raise ValueError(
-                "Make sure that baud-rate was calculated before running add_dur()"
-            )
+            raise ValueError("Make sure that baud-rate was calculated before running add_dur()")
         dur_steps = self.events_sig[1:, 0] - self.events_sig[:-1, 0]
         dur_steps = np.reshape(dur_steps, (dur_steps.size, 1))
-        self.events_sig = np.append(
-            self.events_sig[:-1, :], dur_steps / self.dur_tick, axis=1
-        )
+        self.events_sig = np.append(self.events_sig[:-1, :], dur_steps / self.dur_tick, axis=1)
 
     def detect_inversion(self) -> bool:
-        """analyze bit-state during long pauses (unchanged states)
+        """Analyze bit-state during long pauses (unchanged states)
         - pause should be HIGH for non-inverted mode (default)
         - assumes max frame size of 64 bit + x for safety
         """
         events = self.events_sig[:1000, :]  # speedup for large datasets
         pauses = events[:, 2] > 80
         states_1 = events[:, 1]
         pause_states = states_1[pauses]
         mean_state = pause_states.mean()
         if 0.1 < mean_state < 0.9:
             raise ValueError("Inversion in pauses could not be detected")
         return mean_state < 0.5
 
     def detect_baud_rate(self) -> int:
-        """analyze the smallest step"""
+        """Analyze the smallest step"""
         events = self.events_sig[:1000, :]  # speedup for large datasets
         dur_steps = events[1:, 0] - events[:-1, 0]
         def_step = np.percentile(dur_steps[dur_steps > 0], 10)
         mean_tick = dur_steps[
             (dur_steps >= 0.66 * def_step) & (dur_steps <= 1.33 * def_step)
         ].mean()
         return round(1 / mean_tick)
 
     def detect_half_stop(self) -> bool:
-        """looks into the spacing between time-steps"""
+        """Looks into the spacing between time-steps"""
         events = self.events_sig[:1000, :]  # speedup for large datasets
-        return (
-            np.sum((events > 1.333 * self.dur_tick) & (events < 1.667 * self.dur_tick))
-            > 0
-        )
+        return np.sum((events > 1.333 * self.dur_tick) & (events < 1.667 * self.dur_tick)) > 0
 
     def detect_dataframe_length(self) -> int:
-        """look after longest pauses
+        """Look after longest pauses
         - accumulate steps until a state with uneven step-size is found
         """
-        pass
 
-    def get_symbols(self, force_redo: bool = False) -> np.ndarray:
-        """
-        ways to detect EOF:
+    def get_symbols(self, *, force_redo: bool = False) -> np.ndarray:
+        """Ways to detect EOF:
         - long pause on HIGH
         - off_tick pause on high
         - bit_pos > max
         # TODO:
             - slowest FN -> speedup with numba or parallelization?
             - dset could be divided (long pauses) and threaded for speedup
         """
-
         if force_redo:
             self.events_symbols = None
         if self.events_symbols is not None:
             return self.events_symbols
 
         pos_df = None
         symbol = 0
@@ -225,15 +206,15 @@
                     pos_df = None
                 else:
                     logger.debug("Error - Long pause - but SigLow (@%d)", time)
                 continue
             if pos_df is None and value == 0:
                 # Start of frame (first low after pause / EOF)
                 pos_df = 0
-                steps -= 1
+                steps -= 1  # noqa: PLW2901
                 t_start = time
             if pos_df is not None:
                 if round(steps) >= 1 and value:
                     chunk = min(steps, self.frame_length - pos_df - 1)
                     lshift = min(pos_df, self.frame_length - 1)
                     symbol += (2 ** round(chunk) - 1) << lshift
                 pos_df += round(steps)
@@ -245,19 +226,20 @@
                         t_start = None
                         symbol = 0
                     pos_df = None
                     if off_tick and value == 0:
                         logger.debug("Error - Off-sized step - but SigLow (@%d)", time)
         self.events_symbols = np.concatenate(content).reshape((len(content), 2))
         # TODO: numpy is converting timestamp to string -> must be added as tuple (ts, symbol)
-        # symbol_events[:, 0] = symbol_events[:, 0].astype(float)  # does not work, noqa: 800
+        # symbol_events[:, 0] = symbol_events[:, 0].astype(float)  # noqa: ERA001
+        # ⤷ does not work
         return self.events_symbols
 
-    def get_lines(self, force_redo: bool = False) -> np.ndarray:
-        """timestamped symbols to line, cut at \r, \r\n or \n"""
+    def get_lines(self, *, force_redo: bool = False) -> np.ndarray:
+        """Timestamped symbols to line, cut at \r, \r\n or \n"""
         if force_redo:
             self.events_lines = None
         if self.events_lines is not None:
             return self.events_lines
         if self.events_symbols is None:
             self.get_symbols()
 
@@ -280,16 +262,16 @@
 
             if t_start is None:
                 t_start = time
             line += symbol
         self.events_lines = np.concatenate(content).reshape((len(content), 2))
         return self.events_lines
 
-    def get_text(self, force_redo: bool = False) -> str:
-        """remove timestamps and just return the whole string"""
+    def get_text(self, *, force_redo: bool = False) -> str:
+        """Remove timestamps and just return the whole string"""
         if force_redo:
             self.text = None
         if self.text is not None:
             return self.text
         if self.events_lines is None:
             self.get_lines()
         self.text = "".join(self.events_lines[:, 1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/fw_tools/__init__.py` & `shepherd_core-2024.4.1/shepherd_core/fw_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+from typing import Any
+
 try:
-    from pwnlib.elf import ELF  # noqa: F401
+    from importlib.util import find_spec
+
+    find_spec("pwnlib.elf.ELF")
 except ImportError:
     # replace missing dependencies from elf-only pwntools
     import sys
     from importlib.util import find_spec
     from unittest.mock import MagicMock
 
     class Mock(MagicMock):
         @classmethod
-        def __getattr__(cls, name):
+        def __getattr__(cls, name: str) -> Any:
             return MagicMock()
 
     MOCK_MODULES = [
         "socks",  # general lib-init / context-init
         "serial",
         # troublemaker on bbone and/or windows
         "capstone",
         "paramiko",
         "unicorn",
         "cffi",
     ]
     # only update when module is not avail
-    MOCK_MODULES = [
-        mod_name for mod_name in MOCK_MODULES if find_spec(mod_name) is None
-    ]
+    MOCK_MODULES = [mod_name for mod_name in MOCK_MODULES if find_spec(mod_name) is None]
     sys.modules.update((mod_name, Mock()) for mod_name in MOCK_MODULES)
 
 from .converter import base64_to_file
 from .converter import base64_to_hash
 from .converter import extract_firmware
 from .converter import file_to_base64
 from .converter import file_to_hash
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/fw_tools/converter.py` & `shepherd_core-2024.4.1/shepherd_core/fw_tools/converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import base64
 import hashlib
-import os
 import shutil
 from pathlib import Path
 from typing import Union
 
 import zstandard as zstd
 from pydantic import validate_call
 
@@ -17,90 +16,80 @@
 @validate_call
 def firmware_to_hex(file_path: Path) -> Path:
     """Generic converter that handles ELF & HEX"""
     if not file_path.is_file():
         raise ValueError("Fn needs an existing file as input")
     if is_elf(file_path):
         return elf_to_hex(file_path)
-    elif is_hex(file_path):
+    if is_hex(file_path):
         return file_path
-    else:
-        raise ValueError(
-            "FW2Hex: unknown file '%s', it should be ELF or HEX", file_path.name
-        )
+    raise ValueError("FW2Hex: unknown file '%s', it should be ELF or HEX", file_path.name)
 
 
 @validate_call
 def file_to_base64(file_path: Path) -> str:
     """Compress and encode content of file
     - base64 adds ~33 % overhead
     - zstd compression ~ 1:3
     """
     if not file_path.is_file():
         raise ValueError("Fn needs an existing file as input")
-    with open(file_path.resolve(), "rb") as file:
+    with file_path.resolve().open("rb") as file:
         file_content = file.read()
     file_cmpress = zstd.ZstdCompressor(level=20).compress(file_content)
     return base64.b64encode(file_cmpress).decode("ascii")
 
 
 @validate_call
 def base64_to_file(content: str, file_path: Path) -> None:
     """DeCompress and decode Content of file
     - base64 adds ~33 % overhead
     - zstd compression ~ 1:3
     """
     file_cmpress = base64.b64decode(content)
     file_content = zstd.ZstdDecompressor().decompress(file_cmpress)
     if not file_path.parent.exists():
-        os.makedirs(file_path.parent)
-    with open(file_path.resolve(), "wb") as file:
+        file_path.parent.mkdir(parents=True)
+    with file_path.resolve().open("wb") as file:
         file.write(file_content)
 
 
 @validate_call
 def file_to_hash(file_path: Path) -> str:
     if not file_path.is_file():
         raise ValueError("Fn needs an existing file as input")
-    with open(file_path.resolve(), "rb") as file:
+    with file_path.resolve().open("rb") as file:
         file_content = file.read()
     return hashlib.sha3_224(file_content).hexdigest()
 
 
 @validate_call
 def base64_to_hash(content: str) -> str:
     file_cmpress = base64.b64decode(content)
     file_content = zstd.ZstdDecompressor().decompress(file_cmpress)
     return hashlib.sha3_224(file_content).hexdigest()
 
 
 @validate_call
-def extract_firmware(
-    data: Union[str, Path], data_type: FirmwareDType, file_path: Path
-) -> Path:
-    """
-    - base64-string will be transformed into file
+def extract_firmware(data: Union[str, Path], data_type: FirmwareDType, file_path: Path) -> Path:
+    """- base64-string will be transformed into file
     - if data is a path the file will be copied to the destination
     """
     if data_type == FirmwareDType.base64_elf:
         file = file_path.with_suffix(".elf")
         base64_to_file(data, file)
     elif data_type == FirmwareDType.base64_hex:
         file = file_path.with_suffix(".hex")
         base64_to_file(data, file)
     elif isinstance(data, (Path, str)):
         if data_type == FirmwareDType.path_elf:
             file = file_path.with_suffix(".elf")
         elif data_type == FirmwareDType.path_hex:
             file = file_path.with_suffix(".hex")
         else:
-            raise ValueError(
-                "FW-Extraction failed due to unknown datatype '%s'", data_type
-            )
+            raise ValueError("FW-Extraction failed due to unknown datatype '%s'", data_type)
         if not file.parent.exists():
-            os.makedirs(file.parent)
+            file.parent.mkdir(parents=True)
         shutil.copy(data, file)
     else:
-        raise ValueError(
-            "FW-Extraction failed due to unknown data-type '%s'", type(data)
-        )
+        raise ValueError("FW-Extraction failed due to unknown data-type '%s'", type(data))
     return file
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/fw_tools/converter_elf.py` & `shepherd_core-2024.4.1/shepherd_core/fw_tools/converter_elf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess  # noqa: S404
+import subprocess
 from pathlib import Path
 from typing import Optional
 
 from pydantic import validate_call
 
 # extra src-file necessary to prevent circular import
 
@@ -13,15 +13,15 @@
         raise ValueError("Fn needs an existing file as input")
     if not file_hex:
         file_hex = file_elf.resolve().with_suffix(".hex")
     cmd = ["objcopy", "-O", "ihex", file_elf.resolve().as_posix(), file_hex.as_posix()]
     # TODO: observe - maybe $ARCH-Versions of objcopy are needed
     #  (hex of nRF / msp identical between the 3 $arch-versions)
     try:
-        ret = subprocess.run(cmd)  # noqa: S603
+        subprocess.run(cmd, check=True)  # noqa: S603
     except FileNotFoundError as err:
         raise RuntimeError(
             "Objcopy not found -> are binutils or build-essential installed?"
         ) from err
-    if ret.returncode != 0:
-        raise RuntimeError("Objcopy failed to convert ELF to iHEX")
+    except subprocess.CalledProcessError:
+        raise RuntimeError("Objcopy failed to convert ELF to iHEX") from None
     return file_hex
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/fw_tools/patcher.py` & `shepherd_core-2024.4.1/shepherd_core/fw_tools/patcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,27 @@
 from ..commons import uid_len_default
 from ..commons import uid_str_default
 from ..logger import logger
 from .validation import is_elf
 
 try:
     from pwnlib.elf import ELF
-
-    elf_support = True
 except ImportError as e:
-    elf_support = False
+    ELF = None
     elf_error_text = (
         "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
 def find_symbol(file_elf: Path, symbol: str) -> bool:
     if symbol is None or not is_elf(file_elf):
         return False
-    if not elf_support:
+    if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     try:
         addr = elf.symbols[symbol]
     except KeyError:
         addr = None
     if addr is None:
@@ -44,21 +42,19 @@
         elf.endian,
     )
     elf.close()
     return True
 
 
 @validate_call
-def read_symbol(
-    file_elf: Path, symbol: str, length: int = uid_len_default
-) -> Optional[int]:
-    """interpreted as int"""
+def read_symbol(file_elf: Path, symbol: str, length: int = uid_len_default) -> Optional[int]:
+    """Interpreted as int"""
     if not find_symbol(file_elf, symbol):
         return None
-    if not elf_support:
+    if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     addr = elf.symbols[symbol]
     value_raw = elf.read(address=addr, count=length)[-length:]
     elf.close()
     return int.from_bytes(bytes=value_raw, byteorder=elf.endian, signed=False)
 
@@ -66,68 +62,63 @@
 def read_uid(file_elf: Path) -> Optional[int]:
     return read_symbol(file_elf, symbol=uid_str_default, length=uid_len_default)
 
 
 def read_arch(file_elf: Path) -> Optional[str]:
     if not is_elf(file_elf):
         return None
-    if not elf_support:
+    if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     if "exec" in elf.elftype.lower():
         return elf.arch.lower()
     logger.error("ELF is not Executable")
     return None
 
 
 @validate_call
 def modify_symbol_value(
     file_elf: Path,
     symbol: str,
     value: Annotated[int, Field(ge=0, lt=2 ** (8 * uid_len_default))],
+    *,
     overwrite: bool = False,
 ) -> Optional[Path]:
-    """replaces value of symbol in ELF-File, hardcoded for uint16_t (2 byte)
+    """Replaces value of symbol in ELF-File, hardcoded for uint16_t (2 byte)
     testbed uses FN to patch firmware with custom target-ID
     NOTE: can overwrite provided file
 
     """
     if not find_symbol(file_elf, symbol):
         return None
-    if not elf_support:
+    if ELF is None:
         raise RuntimeError(elf_error_text)
     elf = ELF(path=file_elf)
     addr = elf.symbols[symbol]
     value_raw = elf.read(address=addr, count=uid_len_default)[-uid_len_default:]
     # ⤷ cutting needed -> msp produces 4b instead of 2
     value_old = int.from_bytes(bytes=value_raw, byteorder=elf.endian, signed=False)
-    value_raw = value.to_bytes(
-        length=uid_len_default, byteorder=elf.endian, signed=False
-    )
+    value_raw = value.to_bytes(length=uid_len_default, byteorder=elf.endian, signed=False)
     try:
         elf.write(address=addr, data=value_raw)
     except AttributeError:
         logger.warning("ELF-Modifier failed @%s for symbol '%s'", f"0x{addr:X}", symbol)
         return None
     if overwrite:
         file_new = file_elf
     else:
-        file_new = file_elf.with_name(
-            file_elf.stem + "_" + str(value) + file_elf.suffix
-        )
+        file_new = file_elf.with_name(file_elf.stem + "_" + str(value) + file_elf.suffix)
         # could be simplified, but py3.8-- doesn't know .with_stem()
     elf.save(path=file_new)
     elf.close()
     logger.debug(
         "Value of Symbol '%s' modified: %s -> %s @%s",
         symbol,
         hex(value_old),
         hex(value),
         hex(addr),
     )
     return file_new
 
 
 def modify_uid(file_elf: Path, value: int) -> Optional[Path]:
-    return modify_symbol_value(
-        file_elf, symbol=uid_str_default, value=value, overwrite=True
-    )
+    return modify_symbol_value(file_elf, symbol=uid_str_default, value=value, overwrite=True)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/fw_tools/validation.py` & `shepherd_core-2024.4.1/shepherd_core/fw_tools/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-""" TODO: Work in Progress
+"""TODO: Work in Progress"""
 
-"""
-import os
 import tempfile
 from pathlib import Path
 
 from intelhex import IntelHex
 from intelhex import IntelHexError
 from pydantic import validate_call
 
 from ..data_models.content.firmware_datatype import FirmwareDType
 from ..logger import logger
 from .converter_elf import elf_to_hex
 
 try:
     from elftools.common.exceptions import ELFError
     from pwnlib.elf import ELF
-
-    elf_support = True
 except ImportError as e:
-    elf_support = False
+    ELF = None
+    ELFError = None
     elf_error_text = (
         "Please install functionality with 'pip install shepherd_core[elf] -U' first, "
         f"underlying exception: {e.msg}"
     )
 
 
 @validate_call
-def is_hex(file: Path):
+def is_hex(file: Path) -> bool:
     try:
         _ = IntelHex(file.as_posix())
     except ValueError:  # parsing
         return False
     except IntelHexError:  # structural errors
         return False
     return True
 
 
-def is_hex_msp430(file: Path):
+def is_hex_msp430(file: Path) -> bool:
     """Observations:
     - addresses begin at 0x4000
     - value @0xFFFE (IVT) is start_address (of pgm-code)
     """
     if is_hex(file):
         ih = IntelHex(file.as_posix())
         if ih.minaddr() != 0x4000:
@@ -78,38 +75,38 @@
 #  - remove conversion to hex
 #  - use elftools to verify magic-bytes and similar things done for the hex
 #  https://github.com/eliben/pyelftools/wiki/User's-guide
 
 
 @validate_call
 def is_elf(file: Path) -> bool:
-    if not elf_support:
+    if ELF is None:
         raise RuntimeError(elf_error_text)
-    if not os.path.isfile(file):
+    if not file.is_file():
         return False
     try:
         _ = ELF(path=file)
     except ELFError:
         logger.debug("File %s is not ELF - Magic number does not match", file.name)
         return False
     return True
 
 
-def is_elf_msp430(file: Path) -> bool:
+def is_elf_msp430(file: Path) -> bool:  # TODO: allow detection without conversion
     if is_elf(file):
         with tempfile.TemporaryDirectory() as path:
             file_hex = Path(path) / "file.hex"
             file_hex = elf_to_hex(file, file_hex)
             if is_hex_msp430(file_hex):
                 return True
         return False
     return False
 
 
-def is_elf_nrf52(file: Path) -> bool:
+def is_elf_nrf52(file: Path) -> bool:  # TODO: allow detection without conversion
     if is_elf(file):
         with tempfile.TemporaryDirectory() as path:
             file_hex = Path(path) / "file.hex"
             file_hex = elf_to_hex(file, file_hex)
             if is_hex_nrf52(file_hex):
                 return True
         return False
@@ -117,27 +114,27 @@
 
 
 def determine_type(file: Path) -> FirmwareDType:
     if not file.is_file():
         raise ValueError("Fn needs an existing file as input")
     if is_hex(file):
         return FirmwareDType.path_hex
-    elif is_elf(file):
+    if is_elf(file):
         return FirmwareDType.path_elf
     raise ValueError("Type of file '%s' could not be determined", file.name)
 
 
 def determine_arch(file: Path) -> str:
     file_t = determine_type(file)
     if file_t == FirmwareDType.path_elf:
         if is_elf_nrf52(file):
             return "nrf52"
-        elif is_elf_msp430(file):
+        if is_elf_msp430(file):
             return "msp430"
         raise ValueError("Arch of ELF '%s' could not be determined", file.name)
-    elif file_t == FirmwareDType.path_hex:
+    if file_t == FirmwareDType.path_hex:
         if is_hex_nrf52(file):
             return "nrf52"
-        elif is_hex_msp430(file):
+        if is_hex_msp430(file):
             return "msp430"
         raise ValueError("Arch of HEX '%s' could not be determined", file.name)
     raise ValueError("Arch of file '%s' could not be determined", file.name)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/inventory/python.py` & `shepherd_core-2024.4.1/shepherd_core/inventory/python.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import platform
 from contextlib import suppress
 from importlib import import_module
 from typing import Optional
 
 from pydantic import ConfigDict
+from typing_extensions import Self
 
 from ..data_models import ShpModel
 
 
 class PythonInventory(ShpModel):
     # program versions
-    python: Optional[str] = None
-    numpy: Optional[str] = None
     h5py: Optional[str] = None
+    numpy: Optional[str] = None
     pydantic: Optional[str] = None
-    yaml: Optional[str] = None
+    python: Optional[str] = None
     shepherd_core: Optional[str] = None
     shepherd_sheep: Optional[str] = None
+    yaml: Optional[str] = None
+    zstandard: Optional[str] = None
 
     model_config = ConfigDict(str_min_length=0)
 
     @classmethod
-    def collect(cls):
+    def collect(cls) -> Self:
         model_dict = {"python": platform.python_version()}
         module_names = [
-            "numpy",
             "h5py",
+            "numpy",
             "pydantic",
-            "yaml",
             "shepherd_core",
             "shepherd_sheep",
+            "yaml",
+            "zstandard",
         ]
 
         for module_name in module_names:
             with suppress(ImportError):
                 module = import_module(module_name)
                 model_dict[module_name] = module.__version__
                 globals()
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/inventory/system.py` & `shepherd_core-2024.4.1/shepherd_core/inventory/system.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 import platform
-import subprocess  # noqa: S404
+import subprocess
 import time
 from contextlib import suppress
+from datetime import datetime
 from typing import Optional
 
+from typing_extensions import Self
+
+from .. import local_now
 from .. import logger
 
 try:
     import psutil
-
-    psutil_support = True
 except ImportError:
-    psutil_support = False
+    psutil = None
 
 from pydantic import ConfigDict
 from pydantic.types import PositiveInt
 
 from ..data_models import ShpModel
 
 
 class SystemInventory(ShpModel):
     uptime: PositiveInt
     # ⤷ seconds
+    timestamp: datetime
+    # time_delta: timedelta = timedelta(0)  # noqa: ERA001
+    # ⤷ lag behind earliest observer, TODO: wrong place
 
     system: str
     release: str
     version: str
 
     machine: str
     processor: str
 
     ptp: Optional[str] = None
 
     hostname: str
 
-    interfaces: dict = {}
+    interfaces: dict = {}  # noqa: RUF012
     # ⤷ tuple with
     #   ip IPvAnyAddress
     #   mac MACStr
 
     model_config = ConfigDict(str_min_length=0)
 
     @classmethod
-    def collect(cls):
-        if psutil_support:
-            ifs1 = psutil.net_if_addrs().items()
-            ifs2 = {
-                name: (_if[1].address, _if[0].address)
-                for name, _if in ifs1
-                if len(_if) > 1
-            }
-            uptime = time.time() - psutil.boot_time()
-        else:
+    def collect(cls) -> Self:
+        ts = local_now()
+
+        if psutil is None:
             ifs2 = {}
             uptime = 0
             logger.warning(
                 "Inventory-Parameters will be missing. "
                 "Please install functionality with "
                 "'pip install shepherd_core[inventory] -U' first"
             )
+        else:
+            ifs1 = psutil.net_if_addrs().items()
+            ifs2 = {name: (_if[1].address, _if[0].address) for name, _if in ifs1 if len(_if) > 1}
+            uptime = time.time() - psutil.boot_time()
 
         model_dict = {
             "uptime": round(uptime),
+            "timestamp": ts,
             "system": platform.system(),
             "release": platform.release(),
             "version": platform.version(),
             "machine": platform.machine(),
             "processor": platform.processor(),
             "hostname": platform.node(),
             "interfaces": ifs2,
+            # TODO: add free space on /
         }
 
         with suppress(FileNotFoundError):
-            ret = subprocess.run(["/usr/sbin/ptp4l", "-v"])  # noqa: S603
+            ret = subprocess.run(["/usr/sbin/ptp4l", "-v"], check=False)  # noqa: S603
             model_dict["ptp"] = ret.stdout
             # alternative: check_output - seems to be lighter
 
         return cls(**model_dict)
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/logger.py` & `shepherd_core-2024.4.1/shepherd_core/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,41 +11,39 @@
 verbose_level: int = 2
 
 
 def get_verbose_level() -> int:
     return verbose_level
 
 
-def set_log_verbose_level(
-    log_: Union[logging.Logger, logging.Handler], verbose: int
-) -> None:
+def set_log_verbose_level(log_: Union[logging.Logger, logging.Handler], verbose: int) -> None:
     if verbose == 0:
         log_.setLevel(logging.ERROR)
         logging.basicConfig(level=logging.ERROR)
     elif verbose == 1:
         log_.setLevel(logging.WARNING)
     elif verbose == 2:
         log_.setLevel(logging.INFO)
     elif verbose > 2:
         log_.setLevel(logging.DEBUG)
 
     if verbose < 3:
         # reduce log-overhead when not debugging, also more user-friendly exceptions
-        logging._srcfile = None
+        logging._srcfile = None  # noqa: SLF001
         logging.logThreads = 0
         logging.logProcesses = 0
 
     if verbose > 2:
         chromalog.basicConfig(format="%(name)s %(levelname)s: %(message)s")
     else:
         chromalog.basicConfig(format="%(message)s")  # reduce internals
 
 
 def increase_verbose_level(verbose: int) -> None:
-    global verbose_level
+    global verbose_level  # noqa: PLW0603
     if verbose >= verbose_level:
         verbose_level = min(max(verbose, 0), 3)
         set_log_verbose_level(logger, verbose_level)
 
 
 increase_verbose_level(2)
 
@@ -56,7 +54,9 @@
 # %o    decimal as octal
 # %x    decimal as hex
 #
 # %05d  pad right (aligned with 5chars)
 # %-05d pad left (left aligned)
 # %06.2f    6chars float, including dec point, with 2 chars after
 # %.5s  truncate to 5 chars
+#
+# %% for a percent character
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/reader.py` & `shepherd_core-2024.4.1/shepherd_core/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,68 @@
-"""
-Reader-Baseclass
-"""
+"""Reader-Baseclass"""
+
 import contextlib
 import errno
 import logging
 import math
 import os
 from itertools import product
 from pathlib import Path
+from types import TracebackType
+from typing import Any
+from typing import ClassVar
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
+from typing import Type
 from typing import Union
 
 import h5py
 import numpy as np
 import yaml
 from pydantic import validate_call
 from tqdm import trange
+from typing_extensions import Self
 
 from .commons import samplerate_sps_default
 from .data_models.base.calibration import CalibrationPair
 from .data_models.base.calibration import CalibrationSeries
 from .data_models.content.energy_environment import EnergyDType
 from .decoder_waveform import Uart
 
 
 class Reader:
     """Sequentially Reads shepherd-data from HDF5 file.
 
     Args:
+    ----
         file_path: Path of hdf5 file containing shepherd data with iv-samples, iv-curves or isc&voc
         verbose: more debug-info during usage, 'None' skips the setter
+
     """
 
     samples_per_buffer: int = 10_000
 
-    mode_dtype_dict = {
+    mode_dtype_dict: ClassVar[dict] = {
         "harvester": [
             EnergyDType.ivsample,
             EnergyDType.ivcurve,
             EnergyDType.isc_voc,
         ],
         "emulator": [EnergyDType.ivsample],
     }
 
     @validate_call
-    def __init__(self, file_path: Optional[Path], verbose: Optional[bool] = True):
+    def __init__(
+        self,
+        file_path: Optional[Path],
+        *,
+        verbose: Optional[bool] = True,
+    ) -> None:
         if not hasattr(self, "file_path"):
             self.file_path: Optional[Path] = None
             if isinstance(file_path, (Path, str)):
                 self.file_path = Path(file_path).resolve()
 
         if not hasattr(self, "_logger"):
             self._logger: logging.Logger = logging.getLogger("SHPCore.Reader")
@@ -77,121 +88,135 @@
             if not isinstance(self.file_path, Path):
                 raise TypeError("Provide a valid Path-Object to Reader!")
             if not (self.file_path.exists() and self.file_path.is_file()):
                 raise FileNotFoundError(
                     errno.ENOENT, os.strerror(errno.ENOENT), self.file_path.name
                 )
 
-            self.h5file = h5py.File(self.file_path, "r")  # = readonly
-            self._reader_opened = True
+            try:
+                self.h5file = h5py.File(self.file_path, "r")  # = readonly
+                self._reader_opened = True
+            except OSError as _xcp:
+                raise TypeError(f"Unable to open HDF5-File '{self.file_path.name}'") from _xcp
 
             if self.is_valid():
-                self._logger.info("File is available now")
+                self._logger.debug("File is available now")
             else:
                 self._logger.error(
-                    "File is faulty! Will try to open but there might be dragons",
+                    "[FileValidation] File is faulty! "
+                    "Will try to open but there might be dragons, for '%s'",
+                    self.file_path.name,
                 )
 
         if not isinstance(self.h5file, h5py.File):
-            raise TypeError("Type of opened file is not h5py.File")
+            raise TypeError("Type of opened file is not h5py.File, for %s", self.file_path.name)
 
         self.ds_time: h5py.Dataset = self.h5file["data"]["time"]
         self.ds_voltage: h5py.Dataset = self.h5file["data"]["voltage"]
         self.ds_current: h5py.Dataset = self.h5file["data"]["current"]
 
         # retrieve cal-data
         if not hasattr(self, "_cal"):
             cal_dict = CalibrationSeries().model_dump()
-            for ds, param in product(
-                ["current", "voltage", "time"], ["gain", "offset"]
-            ):
+            for ds, param in product(["current", "voltage", "time"], ["gain", "offset"]):
                 cal_dict[ds][param] = self.h5file["data"][ds].attrs[param]
             self._cal = CalibrationSeries(**cal_dict)
 
         self._refresh_file_stats()
 
         if file_path is not None:
             # file opened by this reader
-            self._logger.info(
+            self._logger.debug(
                 "Reading data from '%s'\n"
                 "\t- runtime %.1f s\n"
                 "\t- mode = %s\n"
                 "\t- window_size = %d\n"
                 "\t- size = %.3f MiB\n"
                 "\t- rate = %.0f KiB/s",
-                self.file_path,
+                self.file_path.name,
                 self.runtime_s,
                 self.get_mode(),
                 self.get_window_samples(),
                 self.file_size / 2**20,
                 self.data_rate / 2**10,
             )
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         return self
 
-    def __exit__(self, *exc):  # type: ignore
+    def __exit__(
+        self,
+        typ: Optional[Type[BaseException]] = None,
+        exc: Optional[BaseException] = None,
+        tb: Optional[TracebackType] = None,
+        extra_arg: int = 0,
+    ) -> None:
         if self._reader_opened:
             self.h5file.close()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return yaml.safe_dump(
             self.get_metadata(minimal=True), default_flow_style=False, sort_keys=False
         )
 
     def _refresh_file_stats(self) -> None:
-        """update internal states, helpful after resampling or other changes in data-group"""
+        """Update internal states, helpful after resampling or other changes in data-group"""
         self.h5file.flush()
         if (self.ds_time.shape[0] > 1) and (self.ds_time[1] != self.ds_time[0]):
-            self.sample_interval_s = self._cal.time.raw_to_si(
-                self.ds_time[1] - self.ds_time[0]
-            )
+            # this assumes isochronal sampling
+            self.sample_interval_s = self._cal.time.raw_to_si(self.ds_time[1] - self.ds_time[0])
             self.sample_interval_ns = int(10**9 * self.sample_interval_s)
             self.samplerate_sps = max(int(10**9 // self.sample_interval_ns), 1)
-        self.runtime_s = round(self.ds_time.shape[0] / self.samplerate_sps, 1)
+        self.runtime_s = round(self.ds_voltage.shape[0] / self.samplerate_sps, 1)
         if isinstance(self.file_path, Path):
             self.file_size = self.file_path.stat().st_size
         else:
             self.file_size = 0
         self.data_rate = self.file_size / self.runtime_s if self.runtime_s > 0 else 0
 
     def read_buffers(
-        self, start_n: int = 0, end_n: Optional[int] = None, is_raw: bool = False
+        self,
+        start_n: int = 0,
+        end_n: Optional[int] = None,
+        *,
+        is_raw: bool = False,
+        omit_ts: bool = False,
     ) -> Generator[tuple, None, None]:
         """Generator that reads the specified range of buffers from the hdf5 file.
         can be configured on first call
-        TODO: reconstruct - start/end mark samples and
-              each call can request a certain number of samples
+        TODO: reconstruct - start/end mark samples &
+         each call can request a certain number of samples
 
         Args:
+        ----
             :param start_n: (int) Index of first buffer to be read
             :param end_n: (int) Index of last buffer to be read
             :param is_raw: (bool) output original data, not transformed to SI-Units
-        Yields:
-            Buffers between start and end (tuple with time, voltage, current)
+            :param omit_ts: (bool) optimize reading if timestamp is never used
+        Yields: Buffers between start and end (tuple with time, voltage, current)
+
         """
         if end_n is None:
-            end_n = int(self.ds_time.shape[0] // self.samples_per_buffer)
-        self._logger.debug(
-            "Reading blocks from %d to %d from source-file", start_n, end_n
-        )
+            end_n = int(self.ds_voltage.shape[0] // self.samples_per_buffer)
+        self._logger.debug("Reading blocks %d to %d from source-file", start_n, end_n)
         _raw = is_raw
+        _wts = not omit_ts
 
         for i in range(start_n, end_n):
             idx_start = i * self.samples_per_buffer
             idx_end = idx_start + self.samples_per_buffer
             if _raw:
                 yield (
-                    self.ds_time[idx_start:idx_end],
+                    self.ds_time[idx_start:idx_end] if _wts else None,
                     self.ds_voltage[idx_start:idx_end],
                     self.ds_current[idx_start:idx_end],
                 )
             else:
                 yield (
-                    self._cal.time.raw_to_si(self.ds_time[idx_start:idx_end]),
+                    self._cal.time.raw_to_si(self.ds_time[idx_start:idx_end]) if _wts else None,
                     self._cal.voltage.raw_to_si(self.ds_voltage[idx_start:idx_end]),
                     self._cal.current.raw_to_si(self.ds_current[idx_start:idx_end]),
                 )
 
     def get_calibration_data(self) -> CalibrationSeries:
         """Reads calibration-data from hdf5 file.
 
@@ -224,167 +249,200 @@
             if "datatype" in self.h5file["data"].attrs:
                 return EnergyDType[self.h5file["data"].attrs["datatype"]]
             return None
         except KeyError:
             return None
 
     def get_hrv_config(self) -> dict:
-        """essential info for harvester
+        """Essential info for harvester
         :return: config-dict directly for vHarvester to be used during emulation
         """
         return {
             "datatype": self.get_datatype(),
             "window_samples": self.get_window_samples(),
         }
 
     def is_valid(self) -> bool:
-        """checks file for plausibility
+        """Checks file for plausibility
 
         :return: state of validity
         """
         # hard criteria
-        if "data" not in self.h5file.keys():
-            self._logger.error("root data-group not found (@Validator)")
+        if "data" not in self.h5file:
+            self._logger.error(
+                "[FileValidation] root data-group not found in '%s'",
+                self.file_path.name,
+            )
             return False
         for attr in ["mode"]:
-            if attr not in self.h5file.attrs.keys():
+            if attr not in self.h5file.attrs:
                 self._logger.error(
-                    "attribute '%s' not found in file (@Validator)", attr
+                    "[FileValidation] attribute '%s' not found in '%s'",
+                    attr,
+                    self.file_path.name,
                 )
                 return False
             if self.h5file.attrs["mode"] not in self.mode_dtype_dict:
-                self._logger.error("unsupported mode '%s' (@Validator)", attr)
+                self._logger.error(
+                    "[FileValidation] unsupported mode '%s' in '%s'",
+                    attr,
+                    self.file_path.name,
+                )
                 return False
         for attr in ["window_samples", "datatype"]:
-            if attr not in self.h5file["data"].attrs.keys():
+            if attr not in self.h5file["data"].attrs:
                 self._logger.error(
-                    "attribute '%s' not found in data-group (@Validator)", attr
+                    "[FileValidationError] attribute '%s' not found in data-group in '%s'",
+                    attr,
+                    self.file_path.name,
                 )
                 return False
         for dset in ["time", "current", "voltage"]:
-            if dset not in self.h5file["data"].keys():
-                self._logger.error("dataset '%s' not found (@Validator)", dset)
+            if dset not in self.h5file["data"]:
+                self._logger.error(
+                    "[FileValidation] dataset '%s' not found in '%s'",
+                    dset,
+                    self.file_path.name,
+                )
                 return False
             for attr in ["gain", "offset"]:
-                if attr not in self.h5file["data"][dset].attrs.keys():
+                if attr not in self.h5file["data"][dset].attrs:
                     self._logger.error(
-                        "attribute '%s' not found in dataset '%s' (@Validator)",
+                        "[FileValidation] attribute '%s' not found in dataset '%s' in '%s'",
                         attr,
                         dset,
+                        self.file_path.name,
                     )
                     return False
         if self.get_datatype() not in self.mode_dtype_dict[self.get_mode()]:
             self._logger.error(
-                "unsupported type '%s' for mode '%s' (@Validator)",
+                "[FileValidation] unsupported type '%s' for mode '%s'  in '%s'",
                 self.get_datatype(),
                 self.get_mode(),
+                self.file_path.name,
             )
             return False
 
         if self.get_datatype() == EnergyDType.ivcurve and self.get_window_samples() < 1:
             self._logger.error(
-                "window size / samples is < 1 "
-                "-> invalid for ivcurve-datatype (@Validator)"
+                "[FileValidation] window size / samples is < 1 "
+                "-> invalid for ivcurve-datatype, in '%s'",
+                self.file_path.name,
             )
             return False
 
         # soft-criteria:
         if self.get_datatype() != EnergyDType.ivcurve and self.get_window_samples() > 0:
             self._logger.warning(
-                "window size / samples is > 0 despite "
-                "not using the ivcurve-datatype (@Validator)"
+                "[FileValidation] window size / samples is > 0 despite "
+                "not using the ivcurve-datatype, in '%s'",
+                self.file_path.name,
             )
         # same length of datasets:
-        ds_time_size = self.h5file["data"]["time"].shape[0]
-        for dset in ["current", "voltage"]:
+        ds_volt_size = self.h5file["data"]["voltage"].shape[0]
+        for dset in ["current", "time"]:
             ds_size = self.h5file["data"][dset].shape[0]
-            if ds_time_size != ds_size:
+            if ds_volt_size != ds_size:
                 self._logger.warning(
-                    "dataset '%s' has different size (=%d), "
-                    "compared to time-ds (=%d) (@Validator)",
+                    "[FileValidation] dataset '%s' has different size (=%d), "
+                    "compared to time-ds (=%d), in '%s'",
                     dset,
                     ds_size,
-                    ds_time_size,
+                    ds_volt_size,
+                    self.file_path.name,
                 )
         # dataset-length should be multiple of buffersize
-        remaining_size = ds_time_size % self.samples_per_buffer
+        remaining_size = ds_volt_size % self.samples_per_buffer
         if remaining_size != 0:
             self._logger.warning(
-                "datasets are not aligned with buffer-size (@Validator)"
+                "[FileValidation] datasets are not aligned with buffer-size in '%s'",
+                self.file_path.name,
             )
         # check compression
         for dset in ["time", "current", "voltage"]:
             comp = self.h5file["data"][dset].compression
             opts = self.h5file["data"][dset].compression_opts
-            if comp not in [None, "gzip", "lzf"]:
+            if comp not in {None, "gzip", "lzf"}:
                 self._logger.warning(
-                    "unsupported compression found (%s != None, lzf, gzip) (@Validator)",
+                    "[FileValidation] unsupported compression found "
+                    "(%s != None, lzf, gzip) in '%s'",
                     comp,
+                    self.file_path.name,
                 )
             if (comp == "gzip") and (opts is not None) and (int(opts) > 1):
                 self._logger.warning(
-                    "gzip compression is too high (%d > 1) for BBone (@Validator)", opts
+                    "[FileValidation] gzip compression is too high (%d > 1) for BBone in '%s'",
+                    opts,
+                    self.file_path.name,
                 )
         # host-name
         if self.get_hostname() == "unknown":
-            self._logger.warning("Hostname was not set (@Validator)")
+            self._logger.warning(
+                "[FileValidation] Hostname was not set in '%s'", self.file_path.name
+            )
+        # errors during execution
+        _err = self.count_errors_in_log()
+        if _err > 0:
+            self._logger.warning(
+                "[FileValidation] Sheep reported %d errors during execution -> check logs in '%s'",
+                _err,
+                self.file_path.name,
+            )
         return True
 
-    def __getitem__(self, key: str):
-        """returns attribute or (if none found) a handle for a group or dataset (if found)
+    def __getitem__(self, key: str) -> Any:
+        """Returns attribute or (if none found) a handle for a group or dataset (if found)
 
         :param key: attribute, group, dataset
         :return: value of that key, or handle of object
         """
         if key in self.h5file.attrs:
             return self.h5file.attrs.__getitem__(key)
         if key in self.h5file:
             return self.h5file.__getitem__(key)
         raise KeyError
 
     def energy(self) -> float:
-        """determine the recorded energy of the trace
+        """Determine the recorded energy of the trace
         # multiprocessing: https://stackoverflow.com/a/71898911
         # -> failed with multiprocessing.pool and pathos.multiprocessing.ProcessPool
 
         :return: sampled energy in Ws (watt-seconds)
         """
-        iterations = math.ceil(self.ds_time.shape[0] / self.max_elements)
+        iterations = math.ceil(self.ds_voltage.shape[0] / self.max_elements)
         job_iter = trange(
             0,
-            self.ds_time.shape[0],
+            self.ds_voltage.shape[0],
             self.max_elements,
             desc="energy",
             leave=False,
             disable=iterations < 8,
         )
 
         def _calc_energy(idx_start: int) -> float:
-            idx_stop = min(idx_start + self.max_elements, self.ds_time.shape[0])
+            idx_stop = min(idx_start + self.max_elements, self.ds_voltage.shape[0])
             vol_v = self._cal.voltage.raw_to_si(self.ds_voltage[idx_start:idx_stop])
             cur_a = self._cal.current.raw_to_si(self.ds_current[idx_start:idx_stop])
             return (vol_v[:] * cur_a[:]).sum() * self.sample_interval_s
 
         energy_ws = [_calc_energy(i) for i in job_iter]
         return float(sum(energy_ws))
 
     def _dset_statistics(
         self, dset: h5py.Dataset, cal: Optional[CalibrationPair] = None
     ) -> Dict[str, float]:
-        """some basic stats for a provided dataset
+        """Some basic stats for a provided dataset
         :param dset: dataset to evaluate
         :param cal: calibration (if wanted)
         :return: dict with entries for mean, min, max, std
         """
         si_converted = True
         if not isinstance(cal, CalibrationPair):
             if "gain" in dset.attrs and "offset" in dset.attrs:
-                cal = CalibrationPair(
-                    gain=dset.attrs["gain"], offset=dset.attrs["offset"]
-                )
+                cal = CalibrationPair(gain=dset.attrs["gain"], offset=dset.attrs["offset"])
             else:
                 cal = CalibrationPair(gain=1)
                 si_converted = False
         iterations = math.ceil(dset.shape[0] / self.max_elements)
         job_iter = trange(
             0,
             dset.shape[0],
@@ -394,32 +452,31 @@
             disable=iterations < 8,
         )
 
         def _calc_statistics(data: np.ndarray) -> list:
             return [np.mean(data), np.min(data), np.max(data), np.std(data)]
 
         stats_list = [
-            _calc_statistics(cal.raw_to_si(dset[i : i + self.max_elements]))
-            for i in job_iter
+            _calc_statistics(cal.raw_to_si(dset[i : i + self.max_elements])) for i in job_iter
         ]
         if len(stats_list) < 1:
             return {}
         stats_nd = np.stack(stats_list)
         stats: Dict[str, float] = {
             # TODO: wrong calculation for ndim-datasets with n>1
             "mean": float(stats_nd[:, 0].mean()),
             "min": float(stats_nd[:, 1].min()),
             "max": float(stats_nd[:, 2].max()),
             "std": float(stats_nd[:, 3].mean()),  # TODO: sooo wrong :)
             "si_converted": si_converted,
         }
         return stats
 
-    def data_timediffs(self) -> List[float]:
-        """calculate list of (unique) time-deltas between buffers [s]
+    def _data_timediffs(self) -> List[float]:
+        """Calculate list of (unique) time-deltas between buffers [s]
             -> optimized version that only looks at the start of each buffer
 
         :return: list of (unique) time-deltas between buffers [s]
         """
         iterations = math.ceil(self.ds_time.shape[0] / self.max_elements)
         job_iter = trange(
             0,
@@ -442,30 +499,44 @@
             round(self._cal.time.raw_to_si(j) / self.samples_per_buffer, 6)
             for i in diffs_ll
             for j in i
         }
         return list(diffs)
 
     def check_timediffs(self) -> bool:
-        """validate equal time-deltas
+        """Validate equal time-deltas
         -> unexpected time-jumps hint at a corrupted file or faulty measurement
 
         :return: True if OK
         """
-        diffs = self.data_timediffs()
+        diffs = self._data_timediffs()
         if len(diffs) > 1:
             self._logger.warning(
                 "Time-jumps detected -> expected equal steps, but got: %s s", diffs
             )
         return (len(diffs) <= 1) and diffs[0] == round(0.1 / self.samples_per_buffer, 6)
 
+    def count_errors_in_log(self, group_name: str = "sheep", min_level: int = 40) -> int:
+        if group_name not in self.h5file:
+            return 0
+        if "level" not in self.h5file["sheep"]:
+            return 0
+        _lvl = self.h5file["sheep"]["level"]
+        if _lvl.shape[0] < 1:
+            return 0
+        _items = [1 for _x in _lvl[:] if _x >= min_level]
+        return len(_items)
+
     def get_metadata(
-        self, node: Union[h5py.Dataset, h5py.Group, None] = None, minimal: bool = False
+        self,
+        node: Union[h5py.Dataset, h5py.Group, None] = None,
+        *,
+        minimal: bool = False,
     ) -> Dict[str, dict]:
-        """recursive FN to capture the structure of the file
+        """Recursive FN to capture the structure of the file
         :param node: starting node, leave free to go through whole file
         :param minimal: just provide a bare tree (much faster)
         :return: structure of that node with everything inside it
         """
         if node is None:
             self._refresh_file_stats()
             return self.get_metadata(self.h5file, minimal=minimal)
@@ -476,21 +547,21 @@
                 "datatype": str(node.dtype),
                 "shape": str(node.shape),
                 "chunks": str(node.chunks),
                 "compression": str(node.compression),
                 "compression_opts": str(node.compression_opts),
             }
             if node.name == "/data/time":
-                metadata["_dataset_info"]["time_diffs_s"] = self.data_timediffs()
+                metadata["_dataset_info"]["time_diffs_s"] = self._data_timediffs()
                 # TODO: already convert to str to calm the typechecker?
                 #  or construct a pydantic-class
             elif "int" in str(node.dtype):
                 metadata["_dataset_info"]["statistics"] = self._dset_statistics(node)
                 # TODO: put this into metadata["_dataset_statistics"] ??
-        for attr in node.attrs.keys():
+        for attr in node.attrs:
             attr_value = node.attrs[attr]
             if isinstance(attr_value, str):
                 with contextlib.suppress(yaml.YAMLError):
                     attr_value = yaml.safe_load(attr_value)
             elif "int" in str(type(attr_value)):
                 # TODO: why not isinstance? can it be List[int] other complex type?
                 attr_value = int(attr_value)
@@ -502,34 +573,32 @@
                 metadata["_group_info"] = {
                     "energy_Ws": self.energy(),
                     "runtime_s": round(self.runtime_s, 1),
                     "data_rate_KiB_s": round(self.data_rate / 2**10),
                     "file_size_MiB": round(self.file_size / 2**20, 3),
                     "valid": self.is_valid(),
                 }
-            for item in node.keys():
+            for item in node:
                 metadata[item] = self.get_metadata(node[item], minimal=minimal)
 
         return metadata
 
     def save_metadata(self, node: Union[h5py.Dataset, h5py.Group, None] = None) -> dict:
-        """get structure of file and dump content to yaml-file with same name as original
+        """Get structure of file and dump content to yaml-file with same name as original
 
         :param node: starting node, leave free to go through whole file
         :return: structure of that node with everything inside it
         """
         if isinstance(self.file_path, Path):
             yaml_path = Path(self.file_path).resolve().with_suffix(".yaml")
             if yaml_path.exists():
-                self._logger.info("%s already exists, will skip", yaml_path)
+                self._logger.info("File already exists, will skip '%s'", yaml_path.name)
                 return {}
-            metadata = self.get_metadata(
-                node
-            )  # {"h5root": self.get_metadata(self.h5file)}
-            with open(yaml_path, "w", encoding="utf-8-sig") as yfd:
+            metadata = self.get_metadata(node)  # {"h5root": self.get_metadata(self.h5file)}
+            with yaml_path.open("w", encoding="utf-8-sig") as yfd:
                 yaml.safe_dump(metadata, yfd, default_flow_style=False, sort_keys=False)
         else:
             metadata = {}
         return metadata
 
     def get_gpio_pin_num(self, name: str) -> Optional[int]:
         # reverse lookup in a 2D-dict: key1 are pin_num, key2 are descriptor-names
@@ -539,15 +608,15 @@
         for desc_name, desc in descriptions.items():
             if name in desc["name"]:
                 return int(desc_name)
         return None
 
     @staticmethod
     def get_filter_for_redundant_states(data: np.ndarray) -> np.ndarray:
-        """input is 1D state-vector, kep only first from identical & sequential states
+        """Input is 1D state-vector, kep only first from identical & sequential states
         algo: create an offset-by-one vector and compare against original
         """
         if len(data.shape) > 1:
             ValueError("Array must be 1D")
         data_1 = np.concatenate(([not data[0]], data[:-1]))
         return data != data_1
 
@@ -556,17 +625,15 @@
         if "gpio" not in self.h5file:
             return waveforms
 
         gpio_ts = self.h5file["gpio"]["time"]
         gpio_vs = self.h5file["gpio"]["value"]
 
         if name is None:
-            descriptions = yaml.safe_load(
-                self.h5file["gpio"]["value"].attrs["description"]
-            )
+            descriptions = yaml.safe_load(self.h5file["gpio"]["value"].attrs["description"])
             pin_dict = {value["name"]: key for key, value in descriptions.items()}
         else:
             pin_dict = {name: self.get_gpio_pin_num(name)}
 
         for pin_name, pin_num in pin_dict.items():
             gpio_ps = (gpio_vs[:] & (0b1 << pin_num)) > 0
             gpio_f = self.get_filter_for_redundant_states(gpio_ps)
@@ -574,22 +641,20 @@
             self._logger.debug(
                 "GPIO '%s' has %d state-changes (includes initial state)",
                 pin_name,
                 sum(gpio_f),
             )
         return waveforms
 
-    def waveform_to_csv(
-        self, pin_name: str, pin_wf: np.ndarray, separator: str = ","
-    ) -> None:
+    def waveform_to_csv(self, pin_name: str, pin_wf: np.ndarray, separator: str = ",") -> None:
         path_csv = self.file_path.with_suffix(f".waveform.{pin_name}.csv")
         if path_csv.exists():
-            self._logger.warning("%s already exists, will skip", path_csv)
+            self._logger.info("File already exists, will skip '%s'", path_csv.name)
             return
-        with open(path_csv, "w") as csv:
+        with path_csv.open("w") as csv:
             csv.write(f"timestamp [s],{pin_name}\n")
             for row in pin_wf:
                 csv.write(f"{row[0] / 1e9}{separator}{int(row[1])}\n")
 
     def gpio_to_uart(self) -> Optional[np.ndarray]:
         wfs = self.gpio_to_waveforms("uart")
         if len(wfs) < 1:
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/testbed_client/client.py` & `shepherd_core-2024.4.1/shepherd_core/testbed_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from importlib import import_module
 from pathlib import Path
 from typing import Optional
+from typing import TypedDict
 from typing import Union
 
 from pydantic import validate_call
+from typing_extensions import Self
+from typing_extensions import Unpack
 
 from ..commons import testbed_server_default
 from ..data_models.base.shepherd import ShpModel
 from ..data_models.base.wrapper import Wrapper
 from .fixtures import Fixtures
 from .user_model import User
 
 
 class TestbedClient:
-    _instance = None
+    _instance: Optional[Self] = None
 
-    def __init__(self, **kwargs):
+    def __init__(self, server: Optional[str] = None, token: Union[str, Path, None] = None) -> None:
         if not hasattr(self, "_token"):
             self._token: str = "null"
             self._server: Optional[str] = testbed_server_default
             self._user: Optional[User] = None
             self._key: Optional[str] = None
             self._fixtures: Optional[Fixtures] = Fixtures()
             self._connected: bool = False
             self._req = None
-        if "server" in kwargs or "token" in kwargs:
-            self.connect(**kwargs)
+        if server is not None:
+            self.connect(server=server, token=token)
 
-    def __new__(cls):
+    @classmethod
+    def __new__(cls, *_args: tuple, **_kwargs: Unpack[TypedDict]) -> Self:
         if cls._instance is None:
-            cls._instance = super().__new__(cls)
+            cls._instance = object.__new__(cls)
         return cls._instance
 
-    def __del__(self):
+    def __del__(self) -> None:
         TestbedClient._instance = None
 
     @validate_call
-    def connect(
-        self, server: Optional[str] = None, token: Union[str, Path, None] = None
-    ) -> bool:
-        """
-        server: either "local" to use demo-fixtures or something like "https://HOST:PORT"
+    def connect(self, server: Optional[str] = None, token: Union[str, Path, None] = None) -> bool:
+        """server: either "local" to use demo-fixtures or something like "https://HOST:PORT"
         token: your account validation
         """
         if isinstance(token, Path):
-            with open(token.resolve()) as file:
+            with token.resolve().open() as file:
                 self._token = file.read()
         elif isinstance(token, str):
             self._token = token
 
         if server:
             self._server = server.lower()
 
@@ -64,17 +65,15 @@
 
     def insert(self, data: ShpModel) -> bool:
         wrap = Wrapper(
             datatype=type(data).__name__,
             parameters=data.model_dump(),
         )
         if self._connected:
-            r = self._req.post(
-                self._server + "/add", data=wrap.model_dump_json(), timeout=2
-            )
+            r = self._req.post(self._server + "/add", data=wrap.model_dump_json(), timeout=2)
             r.raise_for_status()
         else:
             self._fixtures.insert_model(wrap)
         return True
 
     def query_ids(self, model_type: str) -> list:
         if self._connected:
@@ -116,32 +115,27 @@
 
     def try_inheritance(self, model_type: str, values: dict) -> (dict, list):
         if self._connected:
             raise RuntimeError("Not Implemented, TODO")
         return self._fixtures[model_type].inheritance(values)
 
     def try_completing_model(self, model_type: str, values: dict) -> (dict, list):
-        """init by name/id, for none existing instances raise Exception"""
-        if len(values) == 1 and list(values.keys())[0] in ["id", "name"]:
-            value = list(values.values())[0]
+        """Init by name/id, for none existing instances raise Exception"""
+        if len(values) == 1 and next(iter(values.keys())) in {"id", "name"}:
+            value = next(iter(values.values()))
             if (
                 isinstance(value, str)
                 and value.lower() in self._fixtures[model_type].elements_by_name
             ):
                 values = self.query_item(model_type, name=value)
-            elif (
-                isinstance(value, int)
-                and value in self._fixtures[model_type].elements_by_id
-            ):
+            elif isinstance(value, int) and value in self._fixtures[model_type].elements_by_id:
                 # TODO: still depending on _fixture
                 values = self.query_item(model_type, uid=value)
             else:
-                raise ValueError(
-                    f"Query {model_type} by name / ID failed - " f"{values} is unknown!"
-                )
+                raise ValueError(f"Query {model_type} by name / ID failed - {values} is unknown!")
         return self.try_inheritance(model_type, values)
 
     def fill_in_user_data(self, values: dict) -> dict:
         if self._user:
             # TODO: this looks wrong, should have "is None", why not always overwrite?
             if values.get("owner"):
                 values["owner"] = self._user.name
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/testbed_client/fixtures.py` & `shepherd_core-2024.4.1/shepherd_core/testbed_client/fixtures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import copy
 import os
-import pickle  # noqa: S403
+import pickle
 from datetime import datetime
 from datetime import timedelta
 from pathlib import Path
+from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Union
 
 import yaml
+from pydantic import validate_call
+from typing_extensions import Self
 
+from ..data_models.base.timezone import local_now
+from ..data_models.base.timezone import local_tz
 from ..data_models.base.wrapper import Wrapper
 from ..logger import logger
+from .cache_path import cache_user_path
 
 # Proposed field-name:
 # - inheritance
 # - inherit_from  <-- current choice
 # - inheritor
 # - hereditary
 # - based_on
 
 
 class Fixture:
     """Current implementation of a file-based database"""
 
-    def __init__(self, model_type: str):
+    def __init__(self, model_type: str) -> None:
         self.model_type: str = model_type.lower()
         self.elements_by_name: Dict[str, dict] = {}
         self.elements_by_id: Dict[int, dict] = {}
         # Iterator reset
         self._iter_index: int = 0
         self._iter_list: list = list(self.elements_by_name.values())
 
@@ -44,35 +51,37 @@
         _id = data.parameters["id"]
         data = data.parameters
         self.elements_by_name[name] = data
         self.elements_by_id[_id] = data
         # update iterator
         self._iter_list: list = list(self.elements_by_name.values())
 
-    def __getitem__(self, key) -> dict:
-        key = key.lower()
-        if key in self.elements_by_name:
-            return self.elements_by_name[key]
+    def __getitem__(self, key: Union[str, int]) -> dict:
+        if isinstance(key, str):
+            key = key.lower()
+            if key in self.elements_by_name:
+                return self.elements_by_name[key]
+            key = int(key) if key.isdigit() else None
         if key in self.elements_by_id:
-            return self.elements_by_id[key]
+            return self.elements_by_id[int(key)]
         raise ValueError(f"{self.model_type} '{key}' not found!")
 
-    def __iter__(self):
+    def __iter__(self) -> Self:
         self._iter_index = 0
         self._iter_list = list(self.elements_by_name.values())
         return self
 
-    def __next__(self):
+    def __next__(self) -> Any:
         if self._iter_index < len(self._iter_list):
             member = self._iter_list[self._iter_index]
             self._iter_index += 1
             return member
         raise StopIteration
 
-    def keys(self):  # -> _dict_keys[Any, Any]:
+    def keys(self):  # noqa: ANN201
         return self.elements_by_name.keys()
 
     def refs(self) -> dict:
         return {_i["id"]: _i["name"] for _i in self.elements_by_id.values()}
 
     def inheritance(self, values: dict, chain: Optional[list] = None) -> (dict, list):
         if chain is None:
@@ -136,89 +145,90 @@
             # keep previous entries
             base[key] = value
         return base
 
     def query_id(self, _id: int) -> dict:
         if isinstance(_id, int) and _id in self.elements_by_id:
             return self.elements_by_id[_id]
-        raise ValueError(
-            f"Initialization of {self.model_type} by ID failed - {_id} is unknown!"
-        )
+        raise ValueError(f"Initialization of {self.model_type} by ID failed - {_id} is unknown!")
 
-    def query_name(self, name: str):
+    def query_name(self, name: str) -> dict:
         if isinstance(name, str) and name.lower() in self.elements_by_name:
             return self.elements_by_name[name.lower()]
-        raise ValueError(
-            f"Initialization of {self.model_type} by name failed - {name} is unknown!"
-        )
+        raise ValueError(f"Initialization of {self.model_type} by name failed - {name} is unknown!")
 
 
-def file_older_than(file: Path, delta: timedelta):
-    cutoff = datetime.utcnow() - delta
-    mtime = datetime.utcfromtimestamp(os.path.getmtime(file))
+def file_older_than(file: Path, delta: timedelta) -> bool:
+    cutoff = local_now() - delta
+    mtime = datetime.fromtimestamp(file.stat().st_mtime, tz=local_tz())
     if mtime < cutoff:
         return True
     return False
 
 
 class Fixtures:
     suffix = ".yaml"
 
-    def __init__(self, file_path: Optional[Path] = None):
+    @validate_call
+    def __init__(self, file_path: Optional[Path] = None, *, reset: bool = False) -> None:
         if file_path is None:
             self.file_path = Path(__file__).parent.parent.resolve() / "data_models"
         else:
             self.file_path = file_path
         self.components: Dict[str, Fixture] = {}
-        save_path = self.file_path / "fixtures.pickle"
+        save_path = cache_user_path / "fixtures.pickle"
 
-        if save_path.exists() and not file_older_than(save_path, timedelta(hours=24)):
+        if save_path.exists() and not file_older_than(save_path, timedelta(hours=24)) and not reset:
             # speedup
-            with open(save_path, "rb", -1) as fd:
+            # TODO: also add version as criterion
+            with save_path.open("rb", buffering=-1) as fd:
                 self.components = pickle.load(fd)  # noqa: S301
             logger.debug(" -> found & used pickled fixtures")
         else:
             if self.file_path.is_file():
                 files = [self.file_path]
             elif self.file_path.is_dir():
                 files = get_files(self.file_path, self.suffix)
             else:
                 raise ValueError("Path must either be file or directory (or empty)")
 
             for file in files:
                 self.insert_file(file)
 
-            with open(save_path, "wb", -1) as fd:
+            save_path.parent.mkdir(parents=True, exist_ok=True)
+            with save_path.open("wb", buffering=-1) as fd:
                 pickle.dump(self.components, fd)
 
-    def insert_file(self, file: Path):
-        with open(file) as fd:
+    @validate_call
+    def insert_file(self, file: Path) -> None:
+        with file.open() as fd:
             fixtures = yaml.safe_load(fd)
             for fixture in fixtures:
                 if not isinstance(fixture, dict):
                     continue
                 fix_wrap = Wrapper(**fixture)
                 self.insert_model(fix_wrap)
 
-    def insert_model(self, data: Wrapper):
+    def insert_model(self, data: Wrapper) -> None:
         fix_type = data.datatype.lower()
         if self.components.get(fix_type) is None:
             self.components[fix_type] = Fixture(model_type=fix_type)
         self.components[fix_type].insert(data)
 
-    def __getitem__(self, key) -> Fixture:
+    def __getitem__(self, key: str) -> Fixture:
         key = key.lower()
         if key in self.components:
             return self.components[key]
         raise ValueError(f"Component '{key}' not found!")
 
-    def keys(self):  # -> _dict_keys[Any, Any]:
+    def keys(self):  # noqa: ANN201
         return self.components.keys()
 
-    def to_file(self, file: Path):
+    @staticmethod
+    def to_file(file: Path) -> None:
         raise RuntimeError(f"Not Implemented, TODO (val={file})")
 
 
 def get_files(start_path: Path, suffix: str, recursion_depth: int = 0) -> List[Path]:
     if recursion_depth == 0:
         suffix = suffix.lower().split(".")[-1]
     dir_items = os.scandir(start_path)
@@ -230,13 +240,13 @@
             files += get_files(Path(item.path), suffix, recursion_depth)
             continue
 
         item_name = str(item.name).lower()
         item_ext = item_name.split(".")[-1]
         if item_ext == suffix and item_ext != item_name:
             files.append(Path(item.path))
-        if suffix == "" and item_ext == item_name:
+        if not suffix and item_ext == item_name:
             files.append(Path(item.path))
 
     if recursion_depth == 1 and len(files) > 0:
         logger.debug(" -> got %s files with the suffix '%s'", len(files), suffix)
     return files
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/testbed_client/user_model.py` & `shepherd_core-2024.4.1/shepherd_core/testbed_client/user_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import secrets
 from hashlib import pbkdf2_hmac
 from typing import Optional
+from typing import Union
+from uuid import uuid4
 
+from pydantic import UUID4
 from pydantic import EmailStr
 from pydantic import Field
 from pydantic import SecretBytes
 from pydantic import SecretStr
 from pydantic import StringConstraints
 from pydantic import model_validator
 from pydantic import validate_call
 from typing_extensions import Annotated
 
-from ..data_models.base.content import IdInt
 from ..data_models.base.content import NameStr
 from ..data_models.base.content import SafeStr
-from ..data_models.base.content import id_default
 from ..data_models.base.shepherd import ShpModel
 
 
 @validate_call
-def hash_password(
-    pw: Annotated[str, StringConstraints(min_length=20, max_length=100)]
-) -> bytes:
+def hash_password(pw: Annotated[str, StringConstraints(min_length=20, max_length=100)]) -> bytes:
     # TODO: add salt of testbed -> this fn should be part of Testbed-Object
     # NOTE: 1M Iterations need 25s on beaglebone
     return pbkdf2_hmac(
         "sha512",
         password=pw.encode("utf-8"),
         salt=b"testbed_salt_TODO",
         iterations=1_000_000,
         dklen=128,
     )
 
 
 class User(ShpModel):
     """meta-data representation of a testbed-component (physical object)"""
 
-    id: IdInt = Field(  # noqa: A003
+    # id: UUID4 = Field(  # TODO db-migration - temp fix for documentation
+    id: Union[UUID4, int] = Field(
         description="Unique ID",
-        default_factory=id_default,
+        default_factory=uuid4,
     )
     name: NameStr
     description: Optional[SafeStr] = None
     comment: Optional[SafeStr] = None
 
     name_full: Optional[NameStr] = None
     group: NameStr
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_converter_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-"""
-
-this is ported py-version of the pru-code, goals:
+"""this is ported py-version of the pru-code, goals:
 - stay close to original code-base
 - offer a comparison for the tests
 - step 1 to a virtualization of emulation
 
 NOTE: DO NOT OPTIMIZE -> stay close to original code-base
 
 Compromises:
-- bitshifted values (ie. _n28) are converted to float without shift
+- bitshifted values (i.e. _n28) are converted to float without shift
 
 """
 
 import math
 from typing import Optional
 
 from ..data_models import CalibrationEmulator
 from ..data_models.content.virtual_source import LUT_SIZE
 from ..data_models.content.virtual_source import ConverterPRUConfig
 
 
 class PruCalibration:
     """part of calibration.h"""
 
-    def __init__(self, cal_emu: Optional[CalibrationEmulator] = None):
+    def __init__(self, cal_emu: Optional[CalibrationEmulator] = None) -> None:
         self.cal = cal_emu if cal_emu else CalibrationEmulator()
 
     def conv_adc_raw_to_nA(self, current_raw: int) -> float:
         return self.cal.adc_C_A.raw_to_si(current_raw) * (10**9)
         # TODO: add feature "negative residue compensation" to here
 
-    def conv_adc_raw_to_uV(self, voltage_raw: int) -> float:
+    @staticmethod
+    def conv_adc_raw_to_uV(voltage_raw: int) -> float:
         raise RuntimeError(f"This Fn should not been used (val={voltage_raw})")
 
     def conv_uV_to_dac_raw(self, voltage_uV: float) -> int:
         dac_raw = self.cal.dac_V_A.si_to_raw(float(voltage_uV) / (10**6))
         if dac_raw > (2**16) - 1:
             dac_raw = (2**16) - 1
         return dac_raw
 
 
 class VirtualConverterModel:
-    def __init__(self, cfg: ConverterPRUConfig, cal: PruCalibration):
+    def __init__(self, cfg: ConverterPRUConfig, cal: PruCalibration) -> None:
         self._cal: PruCalibration = cal
         self._cfg: ConverterPRUConfig = cfg
 
         # simplifications for python
         self.R_input_kOhm = float(self._cfg.R_input_kOhm_n22) / 2**22
         self.Constant_us_per_nF = float(self._cfg.Constant_us_per_nF_n28) / 2**28
 
         # boost internal state
         self.V_input_uV: float = 0.0
         self.P_inp_fW: float = 0.0
         self.P_out_fW: float = 0.0
-        self.interval_startup_disabled_drain_n: int = (
-            self._cfg.interval_startup_delay_drain_n
-        )
+        self.interval_startup_disabled_drain_n: int = self._cfg.interval_startup_delay_drain_n
 
         # container for the stored energy
         self.V_mid_uV: float = self._cfg.V_intermediate_init_uV
 
         # buck internal state
         self.enable_storage: bool = (int(self._cfg.converter_mode) & 0b0001) > 0
         self.enable_boost: bool = (int(self._cfg.converter_mode) & 0b0010) > 0
@@ -68,20 +65,16 @@
 
         self.V_out_dac_uV: float = self._cfg.V_output_uV
         self.V_out_dac_raw: int = self._cal.conv_uV_to_dac_raw(self._cfg.V_output_uV)
         self.power_good: bool = True
 
         # prepare hysteresis-thresholds
         self.dV_enable_output_uV: float = self._cfg.dV_enable_output_uV
-        self.V_enable_output_threshold_uV: float = (
-            self._cfg.V_enable_output_threshold_uV
-        )
-        self.V_disable_output_threshold_uV: float = (
-            self._cfg.V_disable_output_threshold_uV
-        )
+        self.V_enable_output_threshold_uV: float = self._cfg.V_enable_output_threshold_uV
+        self.V_disable_output_threshold_uV: float = self._cfg.V_disable_output_threshold_uV
 
         if self.dV_enable_output_uV > self.V_enable_output_threshold_uV:
             self.V_enable_output_threshold_uV = self.dV_enable_output_uV
 
         # pulled from update_states_and_output() due to easier static init
         self.sample_count: int = 0xFFFFFFF0
         self.is_outputting: bool = True
@@ -136,15 +129,15 @@
     def calc_out_power(self, current_adc_raw: int) -> int:
         # Next 2 lines are Python-specific
         current_adc_raw = max(0, current_adc_raw)
         current_adc_raw = min((2**18) - 1, current_adc_raw)
 
         P_leak_fW = self.V_mid_uV * self._cfg.I_intermediate_leak_nA
         I_out_nA = self._cal.conv_adc_raw_to_nA(current_adc_raw)
-        if self.enable_buck:
+        if self.enable_buck:  # noqa: SIM108
             eta_inv_out = self.get_output_inv_efficiency(I_out_nA)
         else:
             eta_inv_out = 1.0
 
         self.P_out_fW = eta_inv_out * self.V_out_dac_uV * I_out_nA + P_leak_fW
 
         if self.interval_startup_disabled_drain_n > 0:
@@ -160,19 +153,15 @@
             P_sum_fW = self.P_inp_fW - self.P_out_fW
             I_mid_nA = P_sum_fW / V_mid_prot_uV
             dV_mid_uV = I_mid_nA * self.Constant_us_per_nF
             self.V_mid_uV += dV_mid_uV
 
         if self.V_mid_uV > self._cfg.V_intermediate_max_uV:
             self.V_mid_uV = self._cfg.V_intermediate_max_uV
-        if (
-            (not self.enable_boost)
-            and (self.P_inp_fW > 0.0)
-            and (self.V_mid_uV > self.V_input_uV)
-        ):
+        if (not self.enable_boost) and (self.P_inp_fW > 0.0) and (self.V_mid_uV > self.V_input_uV):
             # TODO: obfuscated - no "direct connection"?
             self.V_mid_uV = self.V_input_uV
         elif self.V_mid_uV < 1:
             self.V_mid_uV = 1
         return round(self.V_mid_uV)  # Python-specific, added for easier testing
 
     def update_states_and_output(self) -> int:
@@ -249,18 +238,18 @@
 
     def get_P_output_fW(self) -> int:
         return round(self.P_out_fW)
 
     def get_V_intermediate_uV(self) -> int:
         return round(self.V_mid_uV)
 
-    def get_V_intermediate_raw(self):
+    def get_V_intermediate_raw(self) -> int:
         return round(self._cal.conv_uV_to_dac_raw(self.V_mid_uV))
 
-    def get_power_good(self):
+    def get_power_good(self) -> bool:
         return self.power_good
 
     def get_I_mod_out_nA(self) -> float:
         return self.P_out_fW / self.V_mid_uV
 
     def get_state_log_intermediate(self) -> bool:
         return self.enable_log_mid
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-"""
-this is ported py-version of the pru-code, goals:
+"""this is ported py-version of the pru-code, goals:
 - stay close to original code-base
 - offer a comparison for the tests
 - step 1 to a virtualization of emulation
 
 NOTE1: DO NOT OPTIMIZE -> stay close to original c-code-base
 NOTE2: adc-harvest-routines are not part of this model (virtual_harvester lines 66:289)
 
 Compromises:
 - Py has to map the settings-list to internal vars -> is kernel-task
 - Python has no static vars -> FName_reset is handling the class-vars
 
 """
+
 from typing import Tuple
 
 from ..data_models.content.virtual_harvester import HarvesterPRUConfig
 
 
 class VirtualHarvesterModel:
     HRV_IVCURVE: int = 2**4
     HRV_CV: int = 2**8
     HRV_MPPT_VOC: int = 2**12
     HRV_MPPT_PO: int = 2**13
     HRV_MPPT_OPT: int = 2**14
 
-    def __init__(self, cfg: HarvesterPRUConfig):
+    def __init__(self, cfg: HarvesterPRUConfig) -> None:
         self._cfg: HarvesterPRUConfig = cfg
 
         # INIT global vars: shared states
         self.voltage_set_uV: int = self._cfg.voltage_uV + 1
-        # self.settle_steps: int = 0  # adc_ivcurve, noqa: E800, ERA001
         self.interval_step: int = 2**30
-
         self.is_rising: bool = (self._cfg.hrv_mode & (2**1)) != 0
 
         # PO-Relevant, iv & adc
         self.volt_step_uV: int = self._cfg.voltage_step_uV
 
-        # self.power_last_raw: int = 0  # adc_mppt_po, noqa: E800, ERA001
+        # adc_ivcurve
+        # self.settle_steps: int = 0  # noqa: ERA001
+
+        # adc_mppt_po
+        # self.power_last_raw: int = 0 # noqa: ERA001
 
         # globals for iv_cv
         self.voltage_hold: int = 0
         self.current_hold: int = 0
         self.voltage_step_x4_uV: int = self._cfg.voltage_step_uV * 4
 
         # INIT static vars: CV
@@ -88,17 +90,15 @@
         distance_now = abs(_voltage_uV - self.voltage_set_uV)
         distance_last = abs(self.voltage_last - self.voltage_set_uV)
 
         if compare_now != self.compare_last and step_size_now < self.voltage_step_x4_uV:
             if distance_now < distance_last and distance_now < self.voltage_step_x4_uV:
                 self.voltage_hold = _voltage_uV
                 self.current_hold = _current_nA
-            elif (
-                distance_last < distance_now and distance_last < self.voltage_step_x4_uV
-            ):
+            elif distance_last < distance_now and distance_last < self.voltage_step_x4_uV:
                 self.voltage_hold = self.voltage_last
                 self.current_hold = self.current_last
 
         self.voltage_last = _voltage_uV
         self.current_last = _current_nA
         self.compare_last = compare_now
         return self.voltage_hold, self.current_hold
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2024.4.1/shepherd_core/vsource/virtual_source_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""
-
-this is ported py-version of the pru-code, goals:
+"""this is ported py-version of the pru-code, goals:
 - stay close to original code-base
 - offer a comparison for the tests
 - step 1 to a virtualization of emulation
 
 NOTE: DO NOT OPTIMIZE -> stay close to original code-base
 
 """
+
 from typing import Optional
 
 from ..data_models import CalibrationEmulator
 from ..data_models import EnergyDType
 from ..data_models import VirtualSourceConfig
 from ..data_models.content.virtual_harvester import HarvesterPRUConfig
 from ..data_models.content.virtual_source import ConverterPRUConfig
@@ -23,44 +22,42 @@
 class VirtualSourceModel:
     """part of sampling.c"""
 
     def __init__(
         self,
         vsrc: Optional[VirtualSourceConfig],
         cal_emu: CalibrationEmulator,
-        log_intermediate: bool = False,
         dtype_in: EnergyDType = EnergyDType.ivsample,
         window_size: Optional[int] = None,
-    ):
+        *,
+        log_intermediate: bool = False,
+    ) -> None:
         self._cal_emu: CalibrationEmulator = cal_emu
         self._cal_pru: PruCalibration = PruCalibration(cal_emu)
 
         self.cfg_src = VirtualSourceConfig() if vsrc is None else vsrc
         cnv_config = ConverterPRUConfig.from_vsrc(
             self.cfg_src, log_intermediate_node=log_intermediate
         )
-        self.cnv: VirtualConverterModel = VirtualConverterModel(
-            cnv_config, self._cal_pru
-        )
+        self.cnv: VirtualConverterModel = VirtualConverterModel(cnv_config, self._cal_pru)
 
         hrv_config = HarvesterPRUConfig.from_vhrv(
             self.cfg_src.harvester,
             for_emu=True,
             dtype_in=dtype_in,
             window_size=window_size,
         )
 
         self.hrv: VirtualHarvesterModel = VirtualHarvesterModel(hrv_config)
 
         self.W_inp_fWs: float = 0.0
         self.W_out_fWs: float = 0.0
 
-    def iterate_sampling(self, V_inp_uV: int = 0, I_inp_nA: int = 0, I_out_nA: int = 0):
-        """
-        TEST-SIMPLIFICATION - code below is not part of pru-code,
+    def iterate_sampling(self, V_inp_uV: int = 0, I_inp_nA: int = 0, I_out_nA: int = 0) -> int:
+        """TEST-SIMPLIFICATION - code below is not part of pru-code,
         but in part sample_emulator() in sampling.c
 
         :param V_inp_uV:
         :param I_inp_nA:
         :param I_out_nA:
         :return:
         """
```

### Comparing `shepherd_core-2023.9.9/shepherd_core/writer.py` & `shepherd_core-2024.4.1/shepherd_core/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-"""
-Writer that inherits from Reader-Baseclass
-"""
+"""Writer that inherits from Reader-Baseclass"""
+
 import logging
 import math
-import os
 import pathlib
 from datetime import timedelta
 from itertools import product
 from pathlib import Path
+from types import TracebackType
 from typing import Any
 from typing import Optional
+from typing import Type
 from typing import Union
 
 import h5py
 import numpy as np
 import yaml
 from pydantic import validate_call
+from typing_extensions import Self
+from yaml import Dumper
 from yaml import SafeDumper
+from yaml import ScalarNode
 
 from .commons import samplerate_sps_default
 from .data_models.base.calibration import CalibrationEmulator as CalEmu
 from .data_models.base.calibration import CalibrationHarvester as CalHrv
 from .data_models.base.calibration import CalibrationSeries as CalSeries
 from .data_models.content.energy_environment import EnergyDType
 from .data_models.task import Compression
 from .data_models.task.emulation import c_translate
 from .reader import Reader
 
 
 # copy of core/models/base/shepherd - needed also here
-def path2str(dumper, data):
+def path2str(
+    dumper: Dumper, data: Union[pathlib.Path, pathlib.WindowsPath, pathlib.PosixPath]
+) -> ScalarNode:
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
-def time2int(dumper, data):
-    return dumper.represent_scalar(
-        "tag:yaml.org,2002:int", str(int(data.total_seconds()))
-    )
+def time2int(dumper: Dumper, data: timedelta) -> ScalarNode:
+    return dumper.represent_scalar("tag:yaml.org,2002:int", str(int(data.total_seconds())))
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
 
 
 def unique_path(base_path: Union[str, Path], suffix: str) -> Path:
-    """finds an unused filename in case it already exists
+    """Finds an unused filename in case it already exists
 
     :param base_path: file-path to test
     :param suffix: file-suffix
     :return: new non-existing path
     """
     counter = 0
     while True:
@@ -68,25 +71,27 @@
              -> 20 % cpu overhead for half the filesize
      - gzip: good compression, moderate speed, select level from 1-9, default is 4
              -> lower levels seem fine
              -> _algo=number instead of "gzip" is read as compression level for gzip
      -> comparison / benchmarks https://www.h5py.org/lzf/
 
     Args:
+    ----
         file_path: (Path) Name of the HDF5 file that data will be written to
         mode: (str) Indicates if this is data from harvester or emulator
         datatype: (str) choose type: ivsample (most common), ivcurve or isc_voc
         window_samples: (int) windows size for the datatype ivcurve
         cal_data: (CalibrationData) Data is written as raw ADC
             values. We need calibration data in order to convert to physical
             units later.
         modify_existing: (bool) explicitly enable modifying existing file
             otherwise a unique name will be found
         compression: (str) use either None, lzf or "1" (gzips compression level)
         verbose: (bool) provides more debug-info
+
     """
 
     comp_default: int = 1
     mode_default: str = "harvester"
     datatype_default: str = EnergyDType.ivsample
 
     _chunk_shape: tuple = (Reader.samples_per_buffer,)
@@ -96,18 +101,19 @@
         self,
         file_path: Path,
         mode: Optional[str] = None,
         datatype: Union[str, EnergyDType, None] = None,
         window_samples: Optional[int] = None,
         cal_data: Union[CalSeries, CalEmu, CalHrv, None] = None,
         compression: Optional[Compression] = Compression.default,
+        *,
         modify_existing: bool = False,
         force_overwrite: bool = False,
         verbose: Optional[bool] = True,
-    ):
+    ) -> None:
         self._modify = modify_existing
         if compression is not None:
             self._compression = c_translate[compression.value]
         else:
             self._compression = None
 
         if not hasattr(self, "_logger"):
@@ -119,68 +125,61 @@
             self._logger.info("Storing data to   '%s'", self.file_path)
         elif file_path.exists() and not file_path.is_file():
             raise TypeError(f"Path is not a file ({file_path})")
         else:
             base_dir = file_path.resolve().parents[0]
             self.file_path = unique_path(base_dir / file_path.stem, file_path.suffix)
             self._logger.warning(
-                "File '%s' already exists -> " "storing under '%s' instead",
+                "File '%s' already exists -> storing under '%s' instead",
                 file_path,
                 self.file_path.name,
             )
 
         if isinstance(mode, str) and mode not in self.mode_dtype_dict:
-            raise ValueError(
-                f"Can't handle mode '{mode}' " f"(choose one of {self.mode_dtype_dict})"
-            )
+            raise ValueError(f"Can't handle mode '{mode}' (choose one of {self.mode_dtype_dict})")
 
         _dtypes = self.mode_dtype_dict[mode if mode else self.mode_default]
         if isinstance(datatype, str):
             datatype = EnergyDType[datatype]
         if isinstance(datatype, EnergyDType) and datatype not in _dtypes:
             raise ValueError(
-                f"Can't handle value '{datatype}' of datatype "
-                f"(choose one of {_dtypes})"
+                f"Can't handle value '{datatype}' of datatype (choose one of {_dtypes})"
             )
 
         if self._modify:
             self._mode = mode
             self._datatype = datatype
             self._window_samples = window_samples
         else:
             self._mode = mode if isinstance(mode, str) else self.mode_default
             self._datatype = (
                 datatype if isinstance(datatype, EnergyDType) else self.datatype_default
             )
-            self._window_samples = (
-                window_samples if isinstance(window_samples, int) else 0
-            )
+            self._window_samples = window_samples if isinstance(window_samples, int) else 0
 
         if isinstance(cal_data, (CalEmu, CalHrv)):
             self._cal = CalSeries.from_cal(cal_data)
         elif isinstance(cal_data, CalSeries):
             self._cal = cal_data
         else:
             self._cal = CalSeries()
 
         # open file
         if self._modify:
             self.h5file = h5py.File(self.file_path, "r+")  # = rw
         else:
             if not self.file_path.parent.exists():
-                os.makedirs(self.file_path.parent)
+                self.file_path.parent.mkdir(parents=True)
             self.h5file = h5py.File(self.file_path, "w")
             # ⤷ write, truncate if exist
             self._create_skeleton()
 
         # show key parameters for h5-performance
         settings = list(self.h5file.id.get_access_plist().get_cache())
-        self._logger.debug(
-            "H5Py Cache_setting=%s (_mdc, _nslots, _nbytes, _w0)", settings
-        )
+        self._logger.debug("H5Py Cache_setting=%s (_mdc, _nslots, _nbytes, _w0)", settings)
 
         # Store the mode in order to allow user to differentiate harvesting vs emulation data
         if isinstance(self._mode, str) and self._mode in self.mode_dtype_dict:
             self.h5file.attrs["mode"] = self._mode
 
         if (
             isinstance(self._datatype, EnergyDType)
@@ -188,28 +187,34 @@
         ):
             self.h5file["data"].attrs["datatype"] = self._datatype.name
         elif not self._modify:
             self._logger.error("datatype invalid? '%s' not written", self._datatype)
 
         if isinstance(self._window_samples, int):
             self.h5file["data"].attrs["window_samples"] = self._window_samples
-        if datatype == EnergyDType.ivcurve and (self._window_samples in [None, 0]):
+        if datatype == EnergyDType.ivcurve and (self._window_samples in {None, 0}):
             raise ValueError("Window Size argument needed for ivcurve-Datatype")
 
         # include cal-data
         for ds, param in product(["current", "voltage", "time"], ["gain", "offset"]):
             self.h5file["data"][ds].attrs[param] = self._cal[ds][param]
 
         super().__init__(file_path=None, verbose=verbose)
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         super().__enter__()
         return self
 
-    def __exit__(self, *exc):  # type: ignore
+    def __exit__(
+        self,
+        typ: Optional[Type[BaseException]] = None,
+        exc: Optional[BaseException] = None,
+        tb: Optional[TracebackType] = None,
+        extra_arg: int = 0,
+    ) -> None:
         self._align()
         self._refresh_file_stats()
         self._logger.info(
             "closing hdf5 file, %.1f s iv-data, size = %.3f MiB, rate = %.0f KiB/s",
             self.runtime_s,
             self.file_size / 2**20,
             self.data_rate / 2**10,
@@ -240,17 +245,15 @@
             (0,),
             dtype="u8",
             maxshape=(None,),
             chunks=self._chunk_shape,
             compression=self._compression,
         )
         grp_data["time"].attrs["unit"] = "s"
-        grp_data["time"].attrs[
-            "description"
-        ] = "system time [s] = value * gain + (offset)"
+        grp_data["time"].attrs["description"] = "system time [s] = value * gain + (offset)"
 
         grp_data.create_dataset(
             "current",
             (0,),
             dtype="u4",
             maxshape=(None,),
             chunks=self._chunk_shape,
@@ -268,38 +271,40 @@
             compression=self._compression,
         )
         grp_data["voltage"].attrs["unit"] = "V"
         grp_data["voltage"].attrs["description"] = "voltage [V] = value * gain + offset"
 
     def append_iv_data_raw(
         self,
-        timestamp: Union[np.ndarray, float, int],
+        timestamp: Union[np.ndarray, float, int],  # noqa: PYI041
         voltage: np.ndarray,
         current: np.ndarray,
     ) -> None:
         """Writes raw data to database
 
         Args:
+        ----
             timestamp: just start of buffer or whole ndarray
             voltage: ndarray as raw unsigned integers
             current: ndarray as raw unsigned integers
+
         """
         len_new = min(voltage.size, current.size)
 
         if isinstance(timestamp, float):
             timestamp = int(timestamp)
         if isinstance(timestamp, int):
             time_series_ns = self.sample_interval_ns * np.arange(len_new).astype("u8")
             timestamp = timestamp + time_series_ns
         if isinstance(timestamp, np.ndarray):
             len_new = min(len_new, timestamp.size)
         else:
             raise ValueError("timestamp-data was not usable")
 
-        len_old = self.ds_time.shape[0]
+        len_old = self.ds_voltage.shape[0]
 
         # resize dataset
         self.ds_time.resize((len_old + len_new,))
         self.ds_voltage.resize((len_old + len_new,))
         self.ds_current.resize((len_old + len_new,))
 
         # append new data
@@ -314,54 +319,56 @@
         current: np.ndarray,
     ) -> None:
         """Writes data (in SI / physical unit) to file, but converts it to raw-data first
 
            SI-value [SI-Unit] = raw-value * gain + offset,
 
         Args:
+        ----
             timestamp: python timestamp (time.time()) in seconds (si-unit)
                        -> provide start of buffer or whole ndarray
             voltage: ndarray in physical-unit V
             current: ndarray in physical-unit A
+
         """
         timestamp = self._cal.time.si_to_raw(timestamp)
         voltage = self._cal.voltage.si_to_raw(voltage)
         current = self._cal.current.si_to_raw(current)
         self.append_iv_data_raw(timestamp, voltage, current)
 
     def _align(self) -> None:
         """Align datasets with buffer-size of shepherd"""
         self._refresh_file_stats()
-        n_buff = self.ds_time.size / self.samples_per_buffer
+        n_buff = self.ds_voltage.size / self.samples_per_buffer
         size_new = int(math.floor(n_buff) * self.samples_per_buffer)
-        if size_new < self.ds_time.size:
+        if size_new < self.ds_voltage.size:
             if self.samplerate_sps != samplerate_sps_default:
                 self._logger.debug("skipped alignment due to altered samplerate")
                 return
             self._logger.info(
                 "aligning with buffer-size, discarding last %d entries",
-                self.ds_time.size - size_new,
+                self.ds_voltage.size - size_new,
             )
             self.ds_time.resize((size_new,))
             self.ds_voltage.resize((size_new,))
             self.ds_current.resize((size_new,))
 
-    def __setitem__(self, key: str, item: Any):
+    def __setitem__(self, key: str, item: Any) -> None:
         """A convenient interface to store relevant key-value data (attribute) if H5-structure"""
-        return self.h5file.attrs.__setitem__(key, item)
+        self.h5file.attrs.__setitem__(key, item)
 
     def store_config(self, data: dict) -> None:
         """Important Step to get a self-describing Output-File
         TODO: use data-model?
         :param data: from virtual harvester or converter / source
         """
         self.h5file["data"].attrs["config"] = yaml.safe_dump(
             data, default_flow_style=False, sort_keys=False
         )
 
     def store_hostname(self, name: str) -> None:
-        """option to distinguish the host, target or data-source in the testbed
+        """Option to distinguish the host, target or data-source in the testbed
             -> perfect for plotting later
 
         :param name: something unique, or "artificial" in case of generated content
         """
         self.h5file.attrs["hostname"] = name
```

### Comparing `shepherd_core-2023.9.9/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2024.4.1/shepherd_core.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,140 @@
 Metadata-Version: 2.1
-Name: shepherd-core
-Version: 2023.9.9
+Name: shepherd_core
+Version: 2024.4.1
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
-Home-page: https://pypi.org/project/shepherd-core/
-Author: Ingmar Splitt, Kai Geissdoerfer
-Author-email: ingmar.splitt@tu-dresden.de
-Maintainer-email: ingmar.splitt@tu-dresden.de
-License: MIT
-Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
-Project-URL: Source, https://github.com/orgua/shepherd-datalib
+Author-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
+Maintainer-email: Ingmar Splitt <ingmar.splitt@tu-dresden.de>
+Project-URL: Documentation, https://github.com/orgua/shepherd-datalib/blob/main/README.md
+Project-URL: Issues, https://github.com/orgua/shepherd-datalib/issues
+Project-URL: Source, https://pypi.org/project/shepherd-core/
 Keywords: testbed,beaglebone,pru,batteryless,energyharvesting,solar
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Platform: win64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: pyYAML
 Requires-Dist: chromalog
 Requires-Dist: pydantic[email]>2.0.0
-Requires-Dist: tqdm
 Requires-Dist: scipy
+Requires-Dist: tqdm
 Requires-Dist: intelhex
 Requires-Dist: requests
 Requires-Dist: pyelftools
 Requires-Dist: zstandard
 Provides-Extra: elf
 Requires-Dist: pwntools-elf-only; extra == "elf"
 Provides-Extra: inventory
 Requires-Dist: psutil; extra == "inventory"
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 
 # Core Library
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
-[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
-[![CodeStyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![image](https://img.shields.io/pypi/pyversions/shepherd_core.svg)](https://pypi.python.org/pypi/shepherd-core)
+[![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/py_unittest.yml)
+[![CodeStyle](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-**Documentation**: <https://orgua.github.io/shepherd/external/shepherd_core.html>
+**Main Documentation**: <https://orgua.github.io/shepherd>
 
 **Source Code**: <https://github.com/orgua/shepherd-datalib>
 
 **Main Project**: <https://github.com/orgua/shepherd>
 
 ---
 
-This Python Module is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
+`shepherd-core` is designed as a library and bundles data-models and file-access-routines for the shepherd-testbed, that are used by several codebases.
 
-For postprocessing shepherds .h5-files users want to use [shepherd_data](https://pypi.org/project/shepherd_data).
+For postprocessing shepherds .h5-files usage of [shepherd_data](https://pypi.org/project/shepherd_data) is recommended.
 
 ## Features
 
 - read and write shepherds hdf5-files
-- create, read, write and convert experiments for the testbed (all data-models included)
+- create, read, write and convert experiments for the testbed
+  - all required data-models are included
 - simulate the virtual source, including virtual harvesters (and virtual converter as a whole)
-- connect and query the testbed via a webclient (TestbedClient)
+- connect and query the testbed via a webclient (TestbedClient in alpha-stage)
   - offline usage defaults to static demo-fixtures loaded from yaml-files in the model-directories
 - work with target-firmwares
   - embed, modify, verify, convert
   - **Note**: working with ELF-files requires external dependencies, see ``Installation``-Chapter
 - decode waveforms (gpio-state & timestamp) to UART
-- create an inventory (used versions of software, hardware)
+- create an inventory (for deployed versions of software, hardware)
+
+See [official documentation](https://orgua.github.io/shepherd) or [example scripts](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased in both. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a [trafficbench](https://github.com/orgua/TrafficBench)-experiment that's used to derive the link-matrix of the testbed-nodes.
 
-See [examples](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/examples) for more details and usage. Most functionality is showcased there. The [extra](https://github.com/orgua/shepherd-datalib/tree/main/shepherd_core/extra)-directory holds data-generators relevant for the testbed. Notably is a trafficbench-experiment that's used to derive the link-matrix.
+## Config-Models in Detail
 
-### Data-Models in Detail
+These pydantic data-models are used throughout all shepherd interfaces. Users can create an experiment, include their own content and feed it to the testbed.
 
-- new orchestration ``/data-models`` with focus on remote shepherd-testbed
+- orchestration ``/data-models`` with focus on remote shepherd-testbed
 - classes of sub-models
   - ``/base``: base-classes, configuration and -functionality for all models
   - ``/testbed``: meta-data representation of all testbed-components
-  - ``/content``: reusable meta-data for fw, h5 and vsrc-definitions
+  - ``/content``: reusable user-defined meta-data for fw, h5 and vsrc-definitions
   - ``/experiment``: configuration-models including sub-systems
   - ``/task``: digestible configs for shepherd-herd or -sheep
   - behavior controlled by ``ShpModel`` and ``content``-model
 - a basic database is available as fixtures through a ``tb_client``
   - fixtures selectable by name & ID
   - fixtures support inheritance
-- models support
+- the models support
   - auto-completion with neutral / sensible values
   - complex and custom datatypes (i.e. PositiveInt, lists-checks on length)
   - checking of inputs and type-casting
   - generate their own schema (for web-forms)
   - pre-validation
   - store to & load from yaml with typecheck through wrapper
   - documentation
 - experiment-definition is designed securely
   - types are limited in size (str)
   - exposes no internal paths
 - experiments can be transformed to task-sets (``TestbedTasks.from_xp()``)
 
+## Compatibility
+
+| OS      |   PyVersion  | Comment                                    |
+|---------|--------------|--------------------------------------------|
+| Ubuntu  | 3.8 - 3.12   |                                            |
+| Windows | 3.8 - 3.12   | no support for elf and hex-conversions yet |
+| MacOS   | 3.8 - 3.12   | hex-conversion missing                     |
+
+Notes:
+- hex-conversion needs a working and accessible objcopy
+- elf-supports needs
+  - ``shepherd-core[elf]`` installs ``pwntools-elf-only``
+  - most elf-features also still utilize hex-conversion
+
 ## Installation
 
 The Library is available via PyPI and can be installed with
 
 ```shell
   pip install shepherd-core -U
 
@@ -148,7 +163,21 @@
 and also make sure the prereqs for the [pwntools](https://docs.pwntools.com/en/stable/install.html) are met.
 
 For creating an inventory of the host-system you should install
 
 ```shell
   pip install shepherd-core[inventory]
 ```
+
+## Unittests
+
+To run the testbench, follow these steps:
+
+1. Navigate your host-shell into the package-folder and
+2. install dependencies
+3. run the testbench (~ 320 tests):
+
+```Shell
+cd shepherd-datalib/shepherd_core
+pip3 install ./[tests]
+pytest
+```
```

### Comparing `shepherd_core-2023.9.9/tests/test_cal_hw.py` & `shepherd_core-2024.4.1/tests/test_cal_hw.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,33 +6,29 @@
 from shepherd_core.calibration_hw_def import adc_raw_to_current
 from shepherd_core.calibration_hw_def import adc_raw_to_voltage
 from shepherd_core.calibration_hw_def import adc_voltage_to_raw
 from shepherd_core.calibration_hw_def import dac_raw_to_voltage
 from shepherd_core.calibration_hw_def import dac_voltage_to_raw
 
 
-@pytest.mark.parametrize(
-    "fn", [adc_current_to_raw, adc_voltage_to_raw, dac_voltage_to_raw]
-)
+@pytest.mark.parametrize("fn", [adc_current_to_raw, adc_voltage_to_raw, dac_voltage_to_raw])
 def test_convert_to_raw(fn: Callable) -> None:
     values = [-1, -1e-6, 1e-6, 1e-5, 1e-4, 1e-3, 1e-2, 1e-1, 1e-0]
     value_prev = -1
     for value in values:
         value_raw = fn(value)
-        assert 0 <= value_raw
+        assert value_raw >= 0
         assert value_raw < 2**18
         assert value_raw >= value_prev
         value_prev = value_raw
 
 
-@pytest.mark.parametrize(
-    "fn", [adc_raw_to_current, adc_raw_to_voltage, dac_raw_to_voltage]
-)
+@pytest.mark.parametrize("fn", [adc_raw_to_current, adc_raw_to_voltage, dac_raw_to_voltage])
 def test_convert_to_si(fn: Callable) -> None:
     values = [-100, -1, 0, 1, 2**6, 2**12, 2**18, 2**24]
     value_prev = -1
     for value in values:
         value_si = fn(value)
-        assert 0 <= value_si
+        assert value_si >= 0
         assert value_si <= 6
         assert value_si >= value_prev
         value_prev = value_si
```

### Comparing `shepherd_core-2023.9.9/tests/test_reader.py` & `shepherd_core-2024.4.1/tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 from pathlib import Path
 
 import h5py
 import pytest
 import yaml
 
-from shepherd_core import Reader as Reader
-from shepherd_core import Writer as Writer
+from shepherd_core import Reader
+from shepherd_core import Writer
 
 
 def test_reader_metadata(data_h5: Path) -> None:
     with Reader(data_h5, verbose=True) as sfr:
         assert sfr.energy() > 0
         assert sfr.is_valid()
 
         meta_data_a = sfr.save_metadata()
         meta_path = data_h5.resolve().with_suffix(".yaml")
         assert meta_path.exists()
-        with open(meta_path) as meta_file:
+        with meta_path.open() as meta_file:
             meta_data_b = yaml.safe_load(meta_file)
             assert len(meta_data_b) == len(meta_data_a)
             assert sys.getsizeof(meta_data_b) == sys.getsizeof(meta_data_a)
 
 
 def test_reader_items(data_h5: Path) -> None:
     """Access internal"""
@@ -37,17 +37,17 @@
         Reader(file_path=None)
 
     tmp_file = (tmp_path / "data.h5").resolve()
 
     with pytest.raises(FileNotFoundError):
         Reader(file_path=tmp_file)
 
-    with open(tmp_file, "w") as tf:
+    with tmp_file.open("w") as tf:
         tf.write("abc def ghi")
-    with pytest.raises(OSError):  # should be TypeError
+    with pytest.raises(TypeError):
         Reader(file_path=tmp_file)
 
 
 def test_reader_meta_repr(data_h5: Path) -> None:
     with Reader(data_h5, verbose=True) as sfr:
         print(sfr)
         print(sfr.get_calibration_data())
```

### Comparing `shepherd_core-2023.9.9/tests/test_writer.py` & `shepherd_core-2024.4.1/tests/test_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     mode: Optional[str] = None,
     datatype: Optional[str] = None,
     window_samples: Optional[int] = None,
     cal_data: Union[CalSeries, CalEmu, CalHrv, None] = None,
     config: Optional[dict] = None,
     compression: Optional[Compression] = Compression.default,
     hostname: str = "unknown",
-):
+) -> Path:
     if config is None:
         config = {}
     with Writer(
         store_path,
         mode=mode,
         datatype=datatype,
         window_samples=window_samples,
@@ -37,22 +37,23 @@
         file.store_hostname(hostname)
         file.store_config(config)
         duration_s = 2
         timestamps = np.arange(0.0, duration_s, file.sample_interval_ns / 1e9)
         voltages = np.linspace(3.60, 1.90, int(file.samplerate_sps * duration_s))
         currents = np.linspace(100e-6, 2000e-6, int(file.samplerate_sps * duration_s))
         file.append_iv_data_si(timestamps, voltages, currents)
+    return store_path
 
 
-@pytest.fixture
+@pytest.fixture()
 def h5_path(tmp_path: Path) -> Path:
     return tmp_path / "hrv_test.h5"
 
 
-@pytest.fixture
+@pytest.fixture()
 def h5_file(h5_path: Path) -> Path:
     generate_shp_file(h5_path)
     return h5_path
 
 
 def test_writer_basics(h5_path: Path) -> None:
     generate_shp_file(h5_path)
@@ -108,15 +109,18 @@
 
 
 def test_writer_faulty_window(h5_path: Path) -> None:
     with pytest.raises(ValueError):
         generate_shp_file(h5_path, mode="harvester", datatype="ivcurve")
     with pytest.raises(ValueError):
         generate_shp_file(
-            h5_path, mode="harvester", datatype="ivcurve", window_samples=0
+            h5_path,
+            mode="harvester",
+            datatype="ivcurve",
+            window_samples=0,
         )
 
 
 def test_writer_append_raw(h5_path: Path) -> None:
     with Writer(h5_path) as sfw:
         data_nd = np.zeros((sfw.samples_per_buffer,))
         time_float = 5.5
@@ -132,26 +136,26 @@
 def test_writer_align(h5_path: Path) -> None:
     with Writer(h5_path) as sfw:
         length = int(5.5 * sfw.samples_per_buffer)
         time_nd = np.arange(0, length * sfw.sample_interval_ns, sfw.sample_interval_ns)
         data_nd = np.zeros((int(length),))
         sfw.append_iv_data_raw(time_nd, data_nd, data_nd)
     with Reader(h5_path) as sfr:
-        assert sfr.ds_time.size < length
+        assert sfr.ds_voltage.size < length
 
 
 def test_writer_not_align(h5_path: Path) -> None:
     with Writer(h5_path) as sfw:
         length = int(5.5 * sfw.samples_per_buffer)
         sample_interval = 10 * sfw.sample_interval_ns
         time_nd = np.arange(0, length * sample_interval, sample_interval)
         data_nd = np.zeros((int(length),))
         sfw.append_iv_data_raw(time_nd, data_nd, data_nd)
     with Reader(h5_path) as sfr:
-        assert sfr.ds_time.size == length
+        assert sfr.ds_voltage.size == length
 
 
 def test_writer_setter(h5_path: Path) -> None:
     name = "pingu"
     with Writer(h5_path) as sfw:
         sfw["hostname"] = name
     with Reader(h5_path) as sfr:
```

