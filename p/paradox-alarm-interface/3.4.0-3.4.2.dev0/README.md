# Comparing `tmp/paradox-alarm-interface-3.4.0.tar.gz` & `tmp/paradox_alarm_interface-3.4.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradox-alarm-interface-3.4.0.tar", last modified: Tue Nov 28 16:08:06 2023, max compression
+gzip compressed data, was "paradox_alarm_interface-3.4.2.dev0.tar", last modified: Thu Apr 18 18:56:30 2024, max compression
```

## Comparing `paradox-alarm-interface-3.4.0.tar` & `paradox_alarm_interface-3.4.2.dev0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.889182 paradox-alarm-interface-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22533 2023-11-28 16:08:06.889182 paradox-alarm-interface-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.865182 paradox-alarm-interface-3.4.0/paradox/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19549 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.869182 paradox-alarm-interface-3.4.0/paradox/connections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.869182 paradox-alarm-interface-3.4.0/paradox/connections/ip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/ip/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/ip/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/ip/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/ip/stun_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/connections/serial_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.869182 paradox-alarm-interface-3.4.0/paradox/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/console_scripts/ip150_connection_decrypt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/console_scripts/pai_dump_memory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      987 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/console_scripts/pai_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.869182 paradox-alarm-interface-3.4.0/paradox/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/data/element_type_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/data/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/data/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/data/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.873182 paradox-alarm-interface-3.4.0/paradox/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.873182 paradox-alarm-interface-3.4.0/paradox/hardware/evo/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.873182 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo192.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo48.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo96.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evohd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    32973 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/evo/property.py
--rw-r--r--   0 runner    (1001) docker     (127)    13369 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.873182 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    25423 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16710 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.877182 paradox-alarm-interface-3.4.0/paradox/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/interface_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.877182 paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/client_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.877182 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18724 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.877182 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/abstract_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/alarm_control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/binary_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/homeassistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.881182 paradox-alarm-interface-3.4.0/paradox/interfaces/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/gsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/homeassistant_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/pushover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/interfaces/text/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.881182 paradox-alarm-interface-3.4.0/paradox/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/async_message_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22187 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.881182 paradox-alarm-interface-3.4.0/paradox/lib/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.885182 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/de.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/el.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/en.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/he.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/hu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/pl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/pt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ru.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/ps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/stun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/lib/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4231 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    30302 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/paradox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.885182 paradox-alarm-interface-3.4.0/paradox/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/paradox/parsers/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.885182 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22533 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 16:08:06.000000 paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-11-28 16:08:06.889182 paradox-alarm-interface-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 16:08:06.885182 paradox-alarm-interface-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/tests/test_async_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2023-11-28 16:07:56.000000 paradox-alarm-interface-3.4.0/tests/test_paradox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.368051 paradox_alarm_interface-3.4.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22563 2024-04-18 18:56:30.368051 paradox_alarm_interface-3.4.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.348051 paradox_alarm_interface-3.4.2.dev0/paradox/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19605 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/stun_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/connections/serial_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/ip150_connection_decrypt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/pai_dump_memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      987 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/pai_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/data/element_type_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/data/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/data/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/data/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.352051 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.356051 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo192.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo48.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evohd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32973 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.356051 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25423 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.356051 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/interface_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.356051 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/client_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.356051 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.360051 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/abstract_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/alarm_control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/binary_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/homeassistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.360051 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/gsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/homeassistant_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.360051 paradox_alarm_interface-3.4.2.dev0/paradox/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/async_message_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.360051 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.364051 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/el.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/he.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/hu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/stun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/lib/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4231 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30068 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/paradox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.364051 paradox_alarm_interface-3.4.2.dev0/paradox/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/paradox/parsers/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.364051 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22563 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:56:30.000000 paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-18 18:56:30.368051 paradox_alarm_interface-3.4.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:56:30.364051 paradox_alarm_interface-3.4.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/tests/test_async_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 18:56:26.000000 paradox_alarm_interface-3.4.2.dev0/tests/test_paradox.py
```

### Comparing `paradox-alarm-interface-3.4.0/LICENSE` & `paradox_alarm_interface-3.4.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/PKG-INFO` & `paradox_alarm_interface-3.4.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradox-alarm-interface
-Version: 3.4.0
+Version: 3.4.2.dev0
 Summary: Interface to Paradox Alarm Panels
 Home-page: https://github.com/ParadoxAlarmInterface/pai
 Author: Jevgeni Kiski, João Paulo Barraca
 Author-email: yozik04@gmail.com, jpbarraca@gmail.com
 License: EPL
 Project-URL: Bug Tracker, https://github.com/ParadoxAlarmInterface/pai/issues
 Keywords: paradox alarm ip150 serial home-assistant smarthome mqtt
@@ -14,22 +14,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: construct~=2.9.43
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: python-slugify>=4.0.1
 Requires-Dist: pytz>=2021.3
-Requires-Dist: paho_mqtt>=1.5.0
+Requires-Dist: paho_mqtt<2,>=1.5.0
 Requires-Dist: requests>=2.20.0
 Requires-Dist: pyserial-asyncio>=0.4
 Provides-Extra: yaml
 Requires-Dist: pyyaml>=5.2.0; extra == "yaml"
 Provides-Extra: pushbullet
 Requires-Dist: pushbullet.py>=0.11.0; extra == "pushbullet"
 Requires-Dist: ws4py>=0.4.2; extra == "pushbullet"
@@ -103,16 +103,16 @@
 
 ## How to use
 See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/Installation)
 
 ## Tested Environment
 
 Tested in the following environment:
-* Python 3.6, 3.7, 3.8
-* Mosquitto MQTT Broker >v 1.4.8
+* Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
+* Mosquitto MQTT Broker > 1.4.8
 * OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..)
 * Ubuntu Server 16.04.3 LTS
 * Paradox MG5050, SP7000 and EVO panels
 * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS interface
 * Pushbullet.py
 * SIM900 module through a serial port
 * Serial over TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: paradox-alarm-interface Version: 3.4.0 Summary:
-Interface to Paradox Alarm Panels Home-page: https://github.com/
+Metadata-Version: 2.1 Name: paradox-alarm-interface Version: 3.4.2.dev0
+Summary: Interface to Paradox Alarm Panels Home-page: https://github.com/
 ParadoxAlarmInterface/pai Author: Jevgeni Kiski, JoÃ£o Paulo Barraca Author-
 email: yozik04@gmail.com, jpbarraca@gmail.com License: EPL Project-URL: Bug
 Tracker, https://github.com/ParadoxAlarmInterface/pai/issues Keywords: paradox
 alarm ip150 serial home-assistant smarthome mqtt Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Programming Language :: Python :: 3.11 Requires-Python: <3.12,>=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 construct~=2.9.43 Requires-Dist: argparse>=1.4.0 Requires-Dist: python-
-slugify>=4.0.1 Requires-Dist: pytz>=2021.3 Requires-Dist: paho_mqtt>=1.5.0
+slugify>=4.0.1 Requires-Dist: pytz>=2021.3 Requires-Dist: paho_mqtt<2,>=1.5.0
 Requires-Dist: requests>=2.20.0 Requires-Dist: pyserial-asyncio>=0.4 Provides-
 Extra: yaml Requires-Dist: pyyaml>=5.2.0; extra == "yaml" Provides-Extra:
 pushbullet Requires-Dist: pushbullet.py>=0.11.0; extra == "pushbullet"
 Requires-Dist: ws4py>=0.4.2; extra == "pushbullet" Provides-Extra: pushover
 Requires-Dist: chump>=1.6.0; extra == "pushover" Provides-Extra: signal
 Requires-Dist: pygobject>=3.20.0; extra == "signal" Requires-Dist:
 pydbus>=0.6.0; extra == "signal" Requires-Dist: gi>=1.2; extra == "signal"
@@ -58,85 +58,86 @@
 registered in the site** We do not recommend using SWAN because of https://
 github.com/CriticalSecurity/paradox ## Firmware Upgrade WARNING: **Do not
 upgrade EVO firmware versions to 7.50.000+ if you use Serial connection.
 Process is irreversible! Paradox introduces serial communication encryption
 which most probably will break our PAI ability to talk to the panel.** ## How
 to use See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/
 Installation) ## Tested Environment Tested in the following environment: *
-Python 3.6, 3.7, 3.8 * Mosquitto MQTT Broker >v 1.4.8 * OrangePi 2G-IOT, NanoPi
-NEO, and Raspberry Pi 3 through their built in Serial Port (with a level
-shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..) * Ubuntu
-Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO panels * [Signal Cli]
-(https://github.com/AsamK/signal-cli) through a DBUS interface * Pushbullet.py
-* SIM900 module through a serial port * Serial over TCP (ESP32 or Arduino
-connected to the panel's serial port acts as a proxy) ## Authors * JoÃ£o Paulo
-Barraca - [@jpbarraca](https://github.com/jpbarraca) - Main code and MG/SP
-devices * Jevgeni Kiski - [@yozik04](https://github.com/yozik04) - Main code
-and EVO devices * Ion Darie - [@iondarie](https://github.com/iondarie) - PAI
-Logo, Homebridge integration, testing ## Acknowledgments This work is inspired
-or uses parts from the following projects: * Tertiush at https://github.com/
-Tertiush/ParadoxIP150v2 * Spinza at https://github.com/spinza/paradox_mqtt ##
-Thanks * Ivan Markov - [@ivmarkov](https://github.com/ivmarkov) - Multi-
-platform Docker builds * Claudiu Bucur - [@clau-bucur](https://github.com/clau-
-bucur) - For fixing HomeAssistant plugin after Supervisor(2021.02.5) upgrade
-[#199](https://github.com/ParadoxAlarmInterface/pai/issues/199) * David Tekan -
-[@tekand](https://github.com/tekand) - For supporting different label
-encodings. ## Disclaimer Paradox, MG5050 and IP150 are registered marks of
-PARADOX. Other brands are owned by their respective owners. The code was
-developed as a way of integrating personally owned Paradox systems, and it
-cannot be used for other purposes. It is not affiliated with any company and it
-doesn't have have commercial intent. The code is provided AS IS and the
-developers will not be held responsible for failures in the alarm systems, or
-any other malfunction. ## Donations We have fully stopped accepting donations
-due to lack of free time to spend on this project. [//]: # (## With support
-from) [//]: # () [//]: # (_[_J_e_t_B_r_a_i_n_s_]) Eclipse Public License - v 2.0 THE
-ACCOMPANYING PROGRAM IS PROVIDED UNDER THE TERMS OF THIS ECLIPSE PUBLIC LICENSE
-("AGREEMENT"). ANY USE, REPRODUCTION OR DISTRIBUTION OF THE PROGRAM CONSTITUTES
-RECIPIENT'S ACCEPTANCE OF THIS AGREEMENT. 1. DEFINITIONS "Contribution" means:
-a) in the case of the initial Contributor, the initial content Distributed
-under this Agreement, and b) in the case of each subsequent Contributor: i)
-changes to the Program, and ii) additions to the Program; where such changes
-and/or additions to the Program originate from and are Distributed by that
-particular Contributor. A Contribution "originates" from a Contributor if it
-was added to the Program by such Contributor itself or anyone acting on such
-Contributor's behalf. Contributions do not include changes or additions to the
-Program that are not Modified Works. "Contributor" means any person or entity
-that Distributes the Program. "Licensed Patents" mean patent claims licensable
-by a Contributor which are necessarily infringed by the use or sale of its
-Contribution alone or when combined with the Program. "Program" means the
-Contributions Distributed in accordance with this Agreement. "Recipient" means
-anyone who receives the Program under this Agreement or any Secondary License
-(as applicable), including Contributors. "Derivative Works" shall mean any
-work, whether in Source Code or other form, that is based on (or derived from)
-the Program and for which the editorial revisions, annotations, elaborations,
-or other modifications represent, as a whole, an original work of authorship.
-"Modified Works" shall mean any work in Source Code or other form that results
-from an addition to, deletion from, or modification of the contents of the
-Program, including, for purposes of clarity any new file in Source Code form
-that contains any contents of the Program. Modified Works shall not include
-works that contain only declarations, interfaces, types, classes, structures,
-or files of the Program solely in each case in order to link to, bind by name,
-or subclass the Program or Modified Works thereof. "Distribute" means the acts
-of a) distributing or b) making available in any manner that enables the
-transfer of a copy. "Source Code" means the form of a Program preferred for
-making modifications, including but not limited to software source code,
-documentation source, and configuration files. "Secondary License" means either
-the GNU General Public License, Version 2.0, or any later versions of that
-license, including any exceptions or additional permissions as identified by
-the initial Contributor. 2. GRANT OF RIGHTS a) Subject to the terms of this
+Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11 * Mosquitto MQTT Broker > 1.4.8 *
+OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial
+Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303,
+CH340, etc..) * Ubuntu Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO
+panels * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS
+interface * Pushbullet.py * SIM900 module through a serial port * Serial over
+TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy) ##
+Authors * JoÃ£o Paulo Barraca - [@jpbarraca](https://github.com/jpbarraca) -
+Main code and MG/SP devices * Jevgeni Kiski - [@yozik04](https://github.com/
+yozik04) - Main code and EVO devices * Ion Darie - [@iondarie](https://
+github.com/iondarie) - PAI Logo, Homebridge integration, testing ##
+Acknowledgments This work is inspired or uses parts from the following
+projects: * Tertiush at https://github.com/Tertiush/ParadoxIP150v2 * Spinza at
+https://github.com/spinza/paradox_mqtt ## Thanks * Ivan Markov - [@ivmarkov]
+(https://github.com/ivmarkov) - Multi-platform Docker builds * Claudiu Bucur -
+[@clau-bucur](https://github.com/clau-bucur) - For fixing HomeAssistant plugin
+after Supervisor(2021.02.5) upgrade [#199](https://github.com/
+ParadoxAlarmInterface/pai/issues/199) * David Tekan - [@tekand](https://
+github.com/tekand) - For supporting different label encodings. ## Disclaimer
+Paradox, MG5050 and IP150 are registered marks of PARADOX. Other brands are
+owned by their respective owners. The code was developed as a way of
+integrating personally owned Paradox systems, and it cannot be used for other
+purposes. It is not affiliated with any company and it doesn't have have
+commercial intent. The code is provided AS IS and the developers will not be
+held responsible for failures in the alarm systems, or any other malfunction.
+## Donations We have fully stopped accepting donations due to lack of free time
+to spend on this project. [//]: # (## With support from) [//]: # () [//]: # (
+_[_J_e_t_B_r_a_i_n_s_]) Eclipse Public License - v 2.0 THE ACCOMPANYING PROGRAM IS
+PROVIDED UNDER THE TERMS OF THIS ECLIPSE PUBLIC LICENSE ("AGREEMENT"). ANY USE,
+REPRODUCTION OR DISTRIBUTION OF THE PROGRAM CONSTITUTES RECIPIENT'S ACCEPTANCE
+OF THIS AGREEMENT. 1. DEFINITIONS "Contribution" means: a) in the case of the
+initial Contributor, the initial content Distributed under this Agreement, and
+b) in the case of each subsequent Contributor: i) changes to the Program, and
+ii) additions to the Program; where such changes and/or additions to the
+Program originate from and are Distributed by that particular Contributor. A
+Contribution "originates" from a Contributor if it was added to the Program by
+such Contributor itself or anyone acting on such Contributor's behalf.
+Contributions do not include changes or additions to the Program that are not
+Modified Works. "Contributor" means any person or entity that Distributes the
+Program. "Licensed Patents" mean patent claims licensable by a Contributor
+which are necessarily infringed by the use or sale of its Contribution alone or
+when combined with the Program. "Program" means the Contributions Distributed
+in accordance with this Agreement. "Recipient" means anyone who receives the
+Program under this Agreement or any Secondary License (as applicable),
+including Contributors. "Derivative Works" shall mean any work, whether in
+Source Code or other form, that is based on (or derived from) the Program and
+for which the editorial revisions, annotations, elaborations, or other
+modifications represent, as a whole, an original work of authorship. "Modified
+Works" shall mean any work in Source Code or other form that results from an
+addition to, deletion from, or modification of the contents of the Program,
+including, for purposes of clarity any new file in Source Code form that
+contains any contents of the Program. Modified Works shall not include works
+that contain only declarations, interfaces, types, classes, structures, or
+files of the Program solely in each case in order to link to, bind by name, or
+subclass the Program or Modified Works thereof. "Distribute" means the acts of
+a) distributing or b) making available in any manner that enables the transfer
+of a copy. "Source Code" means the form of a Program preferred for making
+modifications, including but not limited to software source code, documentation
+source, and configuration files. "Secondary License" means either the GNU
+General Public License, Version 2.0, or any later versions of that license,
+including any exceptions or additional permissions as identified by the initial
+Contributor. 2. GRANT OF RIGHTS a) Subject to the terms of this Agreement, each
+Contributor hereby grants Recipient a non-exclusive, worldwide, royalty-free
+copyright license to reproduce, prepare Derivative Works of, publicly display,
+publicly perform, Distribute and sublicense the Contribution of such
+Contributor, if any, and such Derivative Works. b) Subject to the terms of this
 Agreement, each Contributor hereby grants Recipient a non-exclusive, worldwide,
-royalty-free copyright license to reproduce, prepare Derivative Works of,
-publicly display, publicly perform, Distribute and sublicense the Contribution
-of such Contributor, if any, and such Derivative Works. b) Subject to the terms
-of this Agreement, each Contributor hereby grants Recipient a non-exclusive,
-worldwide, royalty-free patent license under Licensed Patents to make, use,
-sell, offer to sell, import and otherwise transfer the Contribution of such
-Contributor, if any, in Source Code or other form. This patent license shall
-apply to the combination of the Contribution and the Program if, at the time
-the Contribution is added by the Contributor, such addition of the Contribution
+royalty-free patent license under Licensed Patents to make, use, sell, offer to
+sell, import and otherwise transfer the Contribution of such Contributor, if
+any, in Source Code or other form. This patent license shall apply to the
+combination of the Contribution and the Program if, at the time the
+Contribution is added by the Contributor, such addition of the Contribution
 causes such combination to be covered by the Licensed Patents. The patent
 license shall not apply to any other combinations which include the
 Contribution. No hardware per se is licensed hereunder. c) Recipient
 understands that although each Contributor grants the licenses to its
 Contributions set forth herein, no assurances are provided by any Contributor
 that the Program does not infringe the patent or other intellectual property
 rights of any other entity. Each Contributor disclaims any liability to
```

### Comparing `paradox-alarm-interface-3.4.0/README.md` & `paradox_alarm_interface-3.4.2.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
 ## How to use
 See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/Installation)
 
 ## Tested Environment
 
 Tested in the following environment:
-* Python 3.6, 3.7, 3.8
-* Mosquitto MQTT Broker >v 1.4.8
+* Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
+* Mosquitto MQTT Broker > 1.4.8
 * OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..)
 * Ubuntu Server 16.04.3 LTS
 * Paradox MG5050, SP7000 and EVO panels
 * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS interface
 * Pushbullet.py
 * SIM900 module through a serial port
 * Serial over TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy)
```

#### html2text {}

```diff
@@ -35,34 +35,35 @@
 registered in the site** We do not recommend using SWAN because of https://
 github.com/CriticalSecurity/paradox ## Firmware Upgrade WARNING: **Do not
 upgrade EVO firmware versions to 7.50.000+ if you use Serial connection.
 Process is irreversible! Paradox introduces serial communication encryption
 which most probably will break our PAI ability to talk to the panel.** ## How
 to use See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/
 Installation) ## Tested Environment Tested in the following environment: *
-Python 3.6, 3.7, 3.8 * Mosquitto MQTT Broker >v 1.4.8 * OrangePi 2G-IOT, NanoPi
-NEO, and Raspberry Pi 3 through their built in Serial Port (with a level
-shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..) * Ubuntu
-Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO panels * [Signal Cli]
-(https://github.com/AsamK/signal-cli) through a DBUS interface * Pushbullet.py
-* SIM900 module through a serial port * Serial over TCP (ESP32 or Arduino
-connected to the panel's serial port acts as a proxy) ## Authors * JoÃ£o Paulo
-Barraca - [@jpbarraca](https://github.com/jpbarraca) - Main code and MG/SP
-devices * Jevgeni Kiski - [@yozik04](https://github.com/yozik04) - Main code
-and EVO devices * Ion Darie - [@iondarie](https://github.com/iondarie) - PAI
-Logo, Homebridge integration, testing ## Acknowledgments This work is inspired
-or uses parts from the following projects: * Tertiush at https://github.com/
-Tertiush/ParadoxIP150v2 * Spinza at https://github.com/spinza/paradox_mqtt ##
-Thanks * Ivan Markov - [@ivmarkov](https://github.com/ivmarkov) - Multi-
-platform Docker builds * Claudiu Bucur - [@clau-bucur](https://github.com/clau-
-bucur) - For fixing HomeAssistant plugin after Supervisor(2021.02.5) upgrade
-[#199](https://github.com/ParadoxAlarmInterface/pai/issues/199) * David Tekan -
-[@tekand](https://github.com/tekand) - For supporting different label
-encodings. ## Disclaimer Paradox, MG5050 and IP150 are registered marks of
-PARADOX. Other brands are owned by their respective owners. The code was
-developed as a way of integrating personally owned Paradox systems, and it
-cannot be used for other purposes. It is not affiliated with any company and it
-doesn't have have commercial intent. The code is provided AS IS and the
-developers will not be held responsible for failures in the alarm systems, or
-any other malfunction. ## Donations We have fully stopped accepting donations
-due to lack of free time to spend on this project. [//]: # (## With support
-from) [//]: # () [//]: # (_[_J_e_t_B_r_a_i_n_s_])
+Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11 * Mosquitto MQTT Broker > 1.4.8 *
+OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial
+Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303,
+CH340, etc..) * Ubuntu Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO
+panels * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS
+interface * Pushbullet.py * SIM900 module through a serial port * Serial over
+TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy) ##
+Authors * JoÃ£o Paulo Barraca - [@jpbarraca](https://github.com/jpbarraca) -
+Main code and MG/SP devices * Jevgeni Kiski - [@yozik04](https://github.com/
+yozik04) - Main code and EVO devices * Ion Darie - [@iondarie](https://
+github.com/iondarie) - PAI Logo, Homebridge integration, testing ##
+Acknowledgments This work is inspired or uses parts from the following
+projects: * Tertiush at https://github.com/Tertiush/ParadoxIP150v2 * Spinza at
+https://github.com/spinza/paradox_mqtt ## Thanks * Ivan Markov - [@ivmarkov]
+(https://github.com/ivmarkov) - Multi-platform Docker builds * Claudiu Bucur -
+[@clau-bucur](https://github.com/clau-bucur) - For fixing HomeAssistant plugin
+after Supervisor(2021.02.5) upgrade [#199](https://github.com/
+ParadoxAlarmInterface/pai/issues/199) * David Tekan - [@tekand](https://
+github.com/tekand) - For supporting different label encodings. ## Disclaimer
+Paradox, MG5050 and IP150 are registered marks of PARADOX. Other brands are
+owned by their respective owners. The code was developed as a way of
+integrating personally owned Paradox systems, and it cannot be used for other
+purposes. It is not affiliated with any company and it doesn't have have
+commercial intent. The code is provided AS IS and the developers will not be
+held responsible for failures in the alarm systems, or any other malfunction.
+## Donations We have fully stopped accepting donations due to lack of free time
+to spend on this project. [//]: # (## With support from) [//]: # () [//]: # (
+_[_J_e_t_B_r_a_i_n_s_])
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/config.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         "IP_CONNECTION_PANEL_SERIAL": (
             None,
             [str, type(None)],
         ),  # Serial number to be used in multi-panel sites. None for first
         "IP_CONNECTION_BARE": False,  # IP endpoint connects directly to panel. Used for Serial Tunnels over TCP
         # Paradox
         "KEEP_ALIVE_INTERVAL": 10,  # Interval between status updates
+        "IO_TIMEOUT": 0.5,  # Timeout for IO operations
         "LIMITS": {},  # By default all zones will be monitored
         "LABEL_ENCODING": "paradox-en",  # Encoding to use when decoding labels. paradox-* or https://docs.python.org/3/library/codecs.html#standard-encodings
         "LABEL_REFRESH_INTERVAL": (
             15 * 60,
             int,
             (0, 0xFFFFFFFF),
         ),  # Interval between refresh of labels
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/connection.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/connection.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/handler.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/handler.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/ip/commands.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/commands.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/ip/connection.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# -*- coding: utf-8 -*-
-
+from abc import ABC, abstractmethod
 import asyncio
 import logging
-from abc import ABC, abstractmethod
 
 from construct import Container
 
+from paradox.config import config as cfg
 from paradox.connections.connection import Connection
 from paradox.connections.handler import IPConnectionHandler
 from paradox.connections.ip.commands import IPModuleConnectCommand
 from paradox.connections.ip.stun_session import StunSession
-from paradox.connections.protocols import (IPConnectionProtocol,
-                                           SerialConnectionProtocol)
+from paradox.connections.protocols import IPConnectionProtocol, SerialConnectionProtocol
 from paradox.exceptions import PAICriticalException
 from paradox.lib.handlers import FutureHandler, HandlerRegistry
 
 logger = logging.getLogger("PAI").getChild(__name__)
 
 
 class MultiAttemptConnection(Connection):
@@ -90,28 +88,31 @@
     def set_key(self, value):
         self.key = value
         self._protocol.key = value
 
     def on_ip_message(self, container: Container):
         return self.loop.create_task(self.ip_handler_registry.handle(container))
 
-    async def wait_for_ip_message(self, timeout=2) -> Container:
+    async def wait_for_ip_message(self, timeout=cfg.IO_TIMEOUT) -> Container:
         future = FutureHandler()
         return await self.ip_handler_registry.wait_until_complete(future, timeout)
 
     async def send_raw_ip_message(self, msg):
         self._protocol.send_raw(msg)
 
     def _make_protocol(self):
         return IPConnectionProtocol(self, self.key)
 
 
 class LocalIPConnection(IPConnectionWithEncryption):
     def __init__(
-        self, host, port, password,
+        self,
+        host,
+        port,
+        password,
     ):
         super().__init__(password)
         self.host = host
         self.port = port
 
     async def _try_connect(self) -> None:
         _, self._protocol = await self.loop.create_connection(
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/ip/parsers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/parsers.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/ip/stun_session.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/ip/stun_session.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/protocols.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+from abc import abstractmethod
 import asyncio
 import binascii
 import logging
-from abc import abstractmethod
 
 from paradox.config import config as cfg
 from paradox.connections.handler import ConnectionHandler, IPConnectionHandler
-from paradox.connections.ip.parsers import (IPMessageCommand, IPMessageRequest,
-                                            IPMessageResponse, IPMessageType)
+from paradox.connections.ip.parsers import (
+    IPMessageCommand,
+    IPMessageRequest,
+    IPMessageResponse,
+    IPMessageType,
+)
 
 logger = logging.getLogger("PAI").getChild(__name__)
 
 
 def checksum(data, min_message_length):
     """Calculates the 8bit checksum of Paradox messages"""
     c = 0
@@ -48,19 +52,19 @@
         if not self.is_active():
             raise ConnectionError("Transport does not exist or is already closed")
 
     async def close(self):
         if self.transport:
             try:
                 self.transport.close()
-            except:
+            except Exception:
                 logger.exception("Connection transport close raised Exception")
             self.transport = None
 
-        await asyncio.wait_for(self._closed, timeout=1)
+        await asyncio.wait_for(self._closed, timeout=cfg.IO_TIMEOUT)
 
     @abstractmethod
     def send_message(self, message):
         raise NotImplementedError("This function needs to be overridden in a subclass")
 
     def connection_lost(self, exc):
         logger.error(f"Connection was closed: {exc}")
@@ -90,15 +94,15 @@
         if closed.done() and not closed.cancelled():
             closed.exception()
 
 
 class SerialConnectionProtocol(ConnectionProtocol):
     def send_message(self, message):
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug("PAI -> SER {}".format(binascii.hexlify(message)))
+            logger.debug(f"PAI -> SER {binascii.hexlify(message)}")
 
         self.check_active()
 
         self.transport.write(message)
 
     def data_received(self, recv_data):
         self.buffer += recv_data
@@ -133,39 +137,39 @@
                 break
 
             frame = self.buffer[:potential_packet_length]
 
             if checksum(frame, min_length):
                 self.buffer = self.buffer[len(frame) :]  # Remove message
                 if cfg.LOGGING_DUMP_PACKETS:
-                    logger.debug("SER -> PAI {}".format(binascii.hexlify(frame)))
+                    logger.debug(f"SER -> PAI {binascii.hexlify(frame)}")
 
                 self.handler.on_message(frame)
             else:
                 self.buffer = self.buffer[1:]
 
 
 class IPConnectionProtocol(ConnectionProtocol):
     def __init__(self, handler: IPConnectionHandler, key):
-        super(IPConnectionProtocol, self).__init__(handler)
+        super().__init__(handler)
 
         self.handler = handler
         self.key = key
 
     def send_raw(self, raw):
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug("PAI -> IP (raw) {}".format(binascii.hexlify(raw)))
+            logger.debug(f"PAI -> IP (raw) {binascii.hexlify(raw)}")
 
         self.check_active()
 
         self.transport.write(raw)
 
     def send_message(self, message):
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug("PAI -> IP (payload) {}".format(binascii.hexlify(message)))
+            logger.debug(f"PAI -> IP (payload) {binascii.hexlify(message)}")
 
         self.check_active()
 
         msg = IPMessageRequest.build(
             dict(
                 header=dict(
                     length=len(message),
@@ -176,25 +180,23 @@
                     cryptor_code="aes_256_ecb",
                 ),
                 payload=message,
             ),
             password=self.key,
         )
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug("PAI -> IP (raw) {}".format(binascii.hexlify(msg)))
+            logger.debug(f"PAI -> IP (raw) {binascii.hexlify(msg)}")
 
         self.transport.write(msg)
 
     def _process_message(self, data):
         message = IPMessageResponse.parse(data, password=self.key)
 
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug(
-                "IP -> PAI (payload) {}".format(binascii.hexlify(message.payload))
-            )
+            logger.debug(f"IP -> PAI (payload) {binascii.hexlify(message.payload)}")
 
         if message.header.message_type == IPMessageType.serial_passthrough_response:
             self.handler.on_message(message.payload)
         elif message.header.message_type == IPMessageType.ip_response:
             self.handler.on_ip_message(message)
         else:
             logger.error(f"Wrong message detected: {message}")
@@ -214,11 +216,11 @@
         if len(recv_data) + 16 < self.buffer[1]:
             return
 
         if len(self.buffer) % 16 != 0:
             return
 
         if cfg.LOGGING_DUMP_PACKETS:
-            logger.debug("IP -> PAI (raw) {}".format(binascii.hexlify(self.buffer)))
+            logger.debug(f"IP -> PAI (raw) {binascii.hexlify(self.buffer)}")
 
         self._process_message(self.buffer)
         self.buffer = b""
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/connections/serial_connection.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/connections/serial_connection.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/console_scripts/ip150_connection_decrypt.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/ip150_connection_decrypt.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/console_scripts/pai_dump_memory.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/pai_dump_memory.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/console_scripts/pai_run.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/console_scripts/pai_run.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/data/element_type_container.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/data/element_type_container.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/data/enums.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/data/enums.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/data/memory_storage.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/data/memory_storage.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/event.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/event.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/exceptions.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/exceptions.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/__init__.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/common.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/common.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/adapters.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/adapters.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/event.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/event.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo192.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo192.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo48.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo48.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evo96.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evo96.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/models/evohd.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/models/evohd.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/panel.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/panel.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/parsers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/parsers.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/evo/property.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/evo/property.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/panel.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/panel.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/parsers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/parsers.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/adapters.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
-
 import datetime
+from enum import Enum
 
 from construct import Adapter
-from enum import Enum
+
 
 class DateAdapter(Adapter):
     def _decode(self, obj, context, path):
         return datetime.datetime(obj[0] * 100 + obj[1], obj[2], obj[3], obj[4], obj[5])
 
     def _encode(self, obj, context, path):
         return [
@@ -31,15 +30,14 @@
         )
 
 
 class PartitionStateAdapter(Adapter):
     states = dict(arm=4, disarm=5, arm_sleep=3, arm_stay=1, none=0)
 
     def _decode(self, obj, context, path):
-
         for k, v in enumerate(self.states):
             if v == obj[0]:
                 return k
 
         return "unknown"
 
     def _encode(self, obj, context, path):
@@ -49,15 +47,14 @@
         return 0
 
 
 class ZoneStateAdapter(Adapter):
     states = dict(bypass=0x10)
 
     def _decode(self, obj, context, path):
-
         for k, v in enumerate(self.states):
             if v == obj[0]:
                 return k
 
         return "unknown"
 
     def _encode(self, obj, context, path):
@@ -223,20 +220,28 @@
         force_zone_has_been_rearmed = 60
         system_status = 64
 
     def _decode(self, obj, context, path):
         disabled = sum(obj) == 0
 
         if disabled:
-            return 'disabled'
+            return "disabled"
 
         try:
-            activation_event = PGMDefinitionAdapter.PGMEvent(obj[0]) if sum(obj[:3]) != 0 else 'disabled'
-        except:
-            activation_event = 'unknown'
+            activation_event = (
+                PGMDefinitionAdapter.PGMEvent(obj[0])
+                if sum(obj[:3]) != 0
+                else "disabled"
+            )
+        except Exception:
+            activation_event = "unknown"
 
         try:
-            deactivation_event = PGMDefinitionAdapter.PGMEvent(obj[3]) if sum(obj[3:]) != 0 else 'disabled'
-        except:
-            deactivation_event = 'unknown'
+            deactivation_event = (
+                PGMDefinitionAdapter.PGMEvent(obj[3])
+                if sum(obj[3:]) != 0
+                else "disabled"
+            )
+        except Exception:
+            deactivation_event = "unknown"
 
         return dict(activation=activation_event, deactivation=deactivation_event)
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/event.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/event.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/panel.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/panel.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/parsers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/parsers.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/hardware/spectra_magellan/property.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/hardware/spectra_magellan/property.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/__init__.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/interface_manager.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/interface_manager.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/client_connection.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/client_connection.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/ip_interface/interface.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/ip_interface/interface.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/basic.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,23 +457,24 @@
             for element_type in self.definitions:  # zones, partitions
                 labels = self.labels[element_type]
                 definitions = self.definitions[element_type]
                 for i in definitions:  # numeric index
                     if i not in labels:
                         continue
 
-                    for attribute in definitions[i]:  # attribute
+                    definition = {**(definitions[i]), "id": i}
+                    for attribute in definition:  # attribute
                         if element_type == "user" and attribute == "code":
                             continue
                         self._publish(
                             f"{cfg.MQTT_BASE_TOPIC}/{cfg.MQTT_DEFINITION_TOPIC}",
                             element_type,
                             labels[i]["key"],
                             attribute,
-                            definitions[i][attribute],
+                            definition[attribute],
                         )
 
         if (
             cfg.MQTT_DASH_PUBLISH
             and len(list(self.labels.get("partition", {}).keys())) >= 2
         ):
             self._publish_dash(cfg.MQTT_DASH_TEMPLATE, self.labels.get("partition", {}))
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/core.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/core.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/abstract_entity.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/alarm_control_panel.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/alarm_control_panel.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/binary_sensors.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/binary_sensors.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/device.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/device.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/factory.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/factory.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/sensor.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/sensor.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/entities/switch.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/entities/switch.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/helpers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/helpers.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/mqtt/homeassistant.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/mqtt/homeassistant.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/core.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/core.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/dummy.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/dummy.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/gsm.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/gsm.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/homeassistant_notifications.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/homeassistant_notifications.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/pushbullet.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/pushbullet.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/pushover.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/pushover.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/interfaces/text/signal.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/interfaces/text/signal.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/async_message_manager.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/async_message_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 from typing import Callable, Optional
 
 from construct import Container
 
-from paradox.lib.handlers import (FutureHandler, HandlerRegistry,
-                                  PersistentHandler)
+from paradox.config import config as cfg
+from paradox.lib.handlers import FutureHandler, HandlerRegistry, PersistentHandler
 
 logger = logging.getLogger("PAI").getChild(__name__)
 
 
 class EventMessageHandler(PersistentHandler):
     def can_handle(self, data: Container) -> bool:
         assert isinstance(data, Container)
@@ -23,25 +23,27 @@
         return data.fields.value.po.command == 0x7 and hasattr(
             data.fields.value, "message"
         )
 
 
 class AsyncMessageManager:
     def __init__(self, loop=None):
-        super(AsyncMessageManager, self).__init__()
+        super().__init__()
 
         if not loop:
             loop = asyncio.get_event_loop()
         self.loop = loop
 
         self.handler_registry = HandlerRegistry()
         self.raw_handler_registry = HandlerRegistry()
 
     async def wait_for_message(
-        self, check_fn: Optional[Callable[[Container], bool]] = None, timeout=2
+        self,
+        check_fn: Optional[Callable[[Container], bool]] = None,
+        timeout=cfg.IO_TIMEOUT,
     ) -> Container:
         return await self.handler_registry.wait_until_complete(
             FutureHandler(check_fn), timeout
         )
 
     def register_raw_handler(self, handler):
         self.raw_handler_registry.append(handler)
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/crypto.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/__init__.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ar.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ar.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/de.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/de.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/el.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/el.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/en.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/en.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/et.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/et.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/he.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/he.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/hu.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/hu.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/pl.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/pl.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/pt.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/pt.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ro.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ro.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/ru.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/ru.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/encodings/charmaps/tr.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/encodings/charmaps/tr.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/event_filter.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/event_filter.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/format.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/format.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/handlers.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from abc import abstractmethod
 import asyncio
 import logging
-from abc import abstractmethod
 from typing import Any, Awaitable, Callable, List, Optional, Union
 
+from paradox.config import config as cfg
+
 logger = logging.getLogger("PAI").getChild(__name__)
 
 
 class Handler:
     def __init__(self, name=None):
         super().__init__()
         self.persistent = False
@@ -26,15 +28,17 @@
 
 class AlreadyHandledError(Exception):
     pass
 
 
 class FutureHandler(Handler, asyncio.Future):
     def __init__(
-        self, check_fn: Optional[Callable[[Any], bool]] = None, name=None,
+        self,
+        check_fn: Optional[Callable[[Any], bool]] = None,
+        name=None,
     ):
         super().__init__()
         self.name = name if name is not None else self.__class__.__name__
         self._check_fn = check_fn
 
     def can_handle(self, data) -> bool:
         if self.done():
@@ -49,15 +53,15 @@
         return data
 
 
 class PersistentHandler(Handler):
     def __init__(
         self, callback: Callable[[Any], Union[None, Awaitable[None]]], name=None
     ):
-        super(PersistentHandler, self).__init__(name)
+        super().__init__(name)
         self._handle = callback
         self.persistent = True
 
     async def __call__(self, data):
         result = self._handle(data)
 
         if isinstance(result, Awaitable):
@@ -86,15 +90,15 @@
         self._handlers.remove(handler)
 
     def remove_by_name(self, name: str):
         to_remove = filter(lambda x: x.name == name, self._handlers)
         for handler in to_remove:
             self.remove(handler)
 
-    async def wait_until_complete(self, handler: Handler, timeout=2):
+    async def wait_until_complete(self, handler: Handler, timeout=cfg.IO_TIMEOUT):
         self.append(handler)
         try:
             return await asyncio.wait_for(handler, timeout=timeout)
         finally:
             assert not handler.persistent
             self.remove(handler)
 
@@ -108,15 +112,15 @@
         for handler in self._handlers:
             try:
                 if handler.can_handle(data):
                     handled = True
                     await handler(data)
             except AlreadyHandledError:
                 logger.error("Already handled")
-            except:
+            except Exception:
                 logger.exception("Exception caught during message handling")
                 raise
 
         if not handled and not self._should_ignore_no_handlers:
             logger.error(
                 "No handler for message {}\nDetail: {}".format(
                     data.fields.value.po.command, data
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/help.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,36 +29,39 @@
     ),
     "requests": dict(
         mandatory=False, desc="the IP150 connection", install_name="requests>=2.20.0"
     ),
     "ws4py": dict(
         mandatory=False, desc="the Pushbullet interface", install_name="ws4py>=0.4.2"
     ),
-    "yaml": dict(mandatory=False, desc="the IP150 connection", install_name="pyyaml>=5.2.0"),
+    "yaml": dict(
+        mandatory=False, desc="the IP150 connection", install_name="pyyaml>=5.2.0"
+    ),
     "chump": dict(
         mandatory=False, desc="the Pushover interface", install_name="chump>=1.6.0"
     ),
     "pydbus": dict(
         mandatory=False, desc="the Signal interface", install_name="pydbus>=0.6.0"
     ),
     "pygobject": dict(
         mandatory=False, desc="the Signal interface", install_name="pygobject>=3.20.0"
     ),
     "gi": dict(mandatory=False, desc="the Signal interface", install_name="gi>=1.2"),
-    "pytz": dict(mandatory=False, desc="Panel time sync", install_name="pytz>=2023.3.post1"),
-    "mqtt": dict(mandatory=False, desc="MQTT", install_name="paho_mqtt>=1.5.0"),
-
+    "pytz": dict(
+        mandatory=False, desc="Panel time sync", install_name="pytz>=2023.3.post1"
+    ),
+    "mqtt": dict(mandatory=False, desc="MQTT", install_name="paho_mqtt>=1.5.0,<2"),
     "pre-commit": dict(mandatory=False, desc="Development", install_name="pre-commit"),
     "flake8": dict(mandatory=False, desc="Code checker", install_name="flake8"),
     "tox": dict(mandatory=False, desc="virtual env / testing", install_name="tox"),
 }
 
 
 def import_error_help(error):
-    logger.error("Could not import Python3 module '{}': {}\n".format(error.name, error))
+    logger.error(f"Could not import Python3 module '{error.name}': {error}\n")
 
     if error.name in MODULES:
         m = MODULES[error.name]
         logger.error(
             "The module is required for {} and IS{} mandatory.".format(
                 m["desc"], " NOT" if not m["mandatory"] else ""
             )
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/ps.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/ps.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/stun.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/stun.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/lib/utils.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/lib/utils.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/main.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/main.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox/paradox.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/paradox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# -*- coding: utf-8 -*-
-
 import asyncio
-import logging
-import time
-import pytz
 from binascii import hexlify
 from datetime import datetime
-from typing import Callable, Iterable, Optional, Sequence
+import logging
+import time
+from typing import Callable, Iterable, Optional
 
 from construct import Container
+import pytz
 
 from paradox.config import config as cfg, get_limits_for_type
 from paradox.connections.connection import Connection
 from paradox.data.enums import RunState
 from paradox.data.memory_storage import MemoryStorage as Storage
 from paradox.data.model import DetectedPanel
 from paradox.event import Change, ChangeEvent, Event, LiveEvent
-from paradox.exceptions import (AuthenticationFailed, PanelNotDetected,
-                                StatusRequestException,
-                                async_loop_unhandled_exception_handler, CodeLockout)
+from paradox.exceptions import (
+    AuthenticationFailed,
+    CodeLockout,
+    PanelNotDetected,
+    StatusRequestException,
+    async_loop_unhandled_exception_handler,
+)
 from paradox.hardware import Panel, create_panel
 from paradox.lib import ps
-from paradox.lib.async_message_manager import (ErrorMessageHandler,
-                                               EventMessageHandler)
+from paradox.lib.async_message_manager import ErrorMessageHandler, EventMessageHandler
 from paradox.lib.handlers import PersistentHandler
 from paradox.lib.utils import deep_merge
 from paradox.parsers.status import convert_raw_status
 
 logger = logging.getLogger("PAI").getChild(__name__)
 
 
 class Paradox:
     def __init__(self, retries=3):
         self.panel: Panel = None
         self._connection: Connection = None
         self.retries = retries
-        self.work_loop = asyncio.get_event_loop()  # type: asyncio.AbstractEventLoop
+        self.work_loop = asyncio.get_event_loop()
         self.work_loop.set_exception_handler(async_loop_unhandled_exception_handler)
 
         self.storage = Storage()
 
         self._run_state = RunState.STOP
         self.request_lock = asyncio.Lock()
         self.busy = asyncio.Lock()
@@ -66,29 +67,27 @@
             # Load a connection to the alarm
             if cfg.CONNECTION_TYPE == "Serial":
                 logger.info("Using Serial Connection")
 
                 from paradox.connections.serial_connection import SerialCommunication
 
                 self._connection = SerialCommunication(
-                    port=cfg.SERIAL_PORT, baud=cfg.SERIAL_BAUD,
+                    port=cfg.SERIAL_PORT,
+                    baud=cfg.SERIAL_BAUD,
                 )
             elif cfg.CONNECTION_TYPE == "IP":
                 logger.info("Using IP Connection")
 
                 if cfg.IP_CONNECTION_BARE:
                     from paradox.connections.ip.connection import BareIPConnection
 
                     self._connection = BareIPConnection(
                         host=cfg.IP_CONNECTION_HOST, port=cfg.IP_CONNECTION_PORT
                     )
-                elif (
-                    cfg.IP_CONNECTION_SITEID
-                    and cfg.IP_CONNECTION_EMAIL
-                ):
+                elif cfg.IP_CONNECTION_SITEID and cfg.IP_CONNECTION_EMAIL:
                     from paradox.connections.ip.connection import StunIPConnection
 
                     self._connection = StunIPConnection(
                         site_id=cfg.IP_CONNECTION_SITEID,
                         email=cfg.IP_CONNECTION_EMAIL,
                         panel_serial=cfg.IP_CONNECTION_PANEL_SERIAL,
                         password=cfg.IP_CONNECTION_PASSWORD,
@@ -98,17 +97,15 @@
 
                     self._connection = LocalIPConnection(
                         host=cfg.IP_CONNECTION_HOST,
                         port=cfg.IP_CONNECTION_PORT,
                         password=cfg.IP_CONNECTION_PASSWORD,
                     )
             else:
-                raise AssertionError(
-                    "Invalid connection type: {}".format(cfg.CONNECTION_TYPE)
-                )
+                raise AssertionError(f"Invalid connection type: {cfg.CONNECTION_TYPE}")
 
             self._register_connection_handlers()
 
         return self._connection
 
     def _register_connection_handlers(self):
         self.connection.register_raw_handler(
@@ -136,15 +133,15 @@
             self.panel = create_panel(self)
             self.connection.variable_message_length(self.panel.variable_message_length)
 
         try:
             initiate_reply = await self.send_wait(
                 self.panel.get_message("InitiateCommunication"),
                 None,
-                reply_expected=0x7
+                reply_expected=0x7,
             )
 
             if initiate_reply:
                 model = initiate_reply.fields.value.label.strip(b"\0 ").decode(
                     cfg.LABEL_ENCODING
                 )
                 firmware_version = "{}.{} build {}".format(
@@ -152,17 +149,15 @@
                     initiate_reply.fields.value.application.revision,
                     initiate_reply.fields.value.application.build,
                 )
                 serial_number = hexlify(
                     initiate_reply.fields.value.serial_number
                 ).decode()
 
-                logger.info(
-                    "Panel Identified {} version {}".format(model, firmware_version)
-                )
+                logger.info(f"Panel Identified {model} version {firmware_version}")
             else:
                 raise ConnectionError("Panel did not replied to InitiateCommunication")
 
             logger.info("Initiating panel connection")
             reply = await self.send_wait(
                 self.panel.get_message("StartCommunication"),
                 args=dict(source_id=0x2),
@@ -247,15 +242,17 @@
     async def sync_time(self):
         now = datetime.now().astimezone()
         if cfg.SYNC_TIME_TIMEZONE:
             try:
                 tzinfo = pytz.timezone(cfg.SYNC_TIME_TIMEZONE)
                 now = now.astimezone(tzinfo)
             except pytz.exceptions.UnknownTimeZoneError:
-                logger.debug(f"Panel Timezone Unknown ('{cfg.SYNC_TIME_TIMEZONE}'). Skipping sync")
+                logger.debug(
+                    f"Panel Timezone Unknown ('{cfg.SYNC_TIME_TIMEZONE}'). Skipping sync"
+                )
                 return
 
         if not self._is_time_sync_required(now.replace(tzinfo=None)):
             return
 
         args = dict(
             century=int(now.year / 100),
@@ -293,21 +290,21 @@
                     raise
                 except (StatusRequestException, asyncio.TimeoutError):
                     replies_missing += 1
                     if replies_missing > 3:
                         logger.error("Lost communication with panel")
                         await self.disconnect()
                         return
-                except:
+                except Exception:
                     logger.exception("Loop")
                 finally:
                     self.busy.release()
 
                 if replies_missing > 0:
-                    logger.debug("Loop: Replies missing: {}".format(replies_missing))
+                    logger.debug(f"Loop: Replies missing: {replies_missing}")
 
             # cfg.Listen for events
 
             max_wait_time = max((tstart + cfg.KEEP_ALIVE_INTERVAL) - time.time(), 0)
             try:
                 await asyncio.wait_for(self.loop_wait_event.wait(), max_wait_time)
             except asyncio.TimeoutError:
@@ -349,35 +346,33 @@
 
             if cfg.LOGGING_DUMP_MESSAGES:
                 logger.debug("Message received: %s", recv_message)
 
             # No message
             if recv_message is None:
                 logger.debug(
-                    "Unknown message: %s"
-                    % (" ".join("{:02x} ".format(c) for c in message))
+                    "Unknown message: %s" % (" ".join(f"{c:02x} " for c in message))
                 )
                 return
 
             self.connection.schedule_message_handling(
                 recv_message
             )  # schedule handling in the loop
-        except:
+        except Exception:
             logger.exception("Error parsing message")
 
     async def send_wait(
         self,
         message_type=None,
         args=None,
         message=None,
         retries=5,
-        timeout=0.5,
+        timeout=cfg.IO_TIMEOUT,
         reply_expected=None,
     ) -> Optional[Container]:
-
         # Connection closed
         if not self.connection.connected:
             raise ConnectionError("Not connected")
 
         if message is None and message_type is not None:
             message = message_type.build(dict(fields=dict(value=args)))
 
@@ -418,32 +413,30 @@
                 except asyncio.TimeoutError:
                     result = "timeout"
                     if attempt == retries:
                         raise
                 except ConnectionError:
                     result = "connection error"
                     raise
-                except:
+                except Exception:
                     result = "exception"
                     logger.exception("Unexpected exception during send_wait")
                     raise
-                #finally:
-                    #logger.debug("send/receive %s in %.4f s", result, time.time() - t1)
+                finally:
+                    logger.debug("send/receive %s in %.4f s", result, time.time() - t1)
 
             attempt += 1
 
         return None  # Probably it needs to throw an exception instead of returning None
 
     async def control_zone(self, zone: str, command: str) -> bool:
         command = command.lower()
-        logger.debug("Control Zone: {} - {}".format(zone, command))
+        logger.debug(f"Control Zone: {zone} - {command}")
 
-        zones_selected = self.storage.get_container("zone").select(
-            zone
-        )  # type: Sequence[int]
+        zones_selected = self.storage.get_container("zone").select(zone)
 
         # Not Found
         if len(zones_selected) == 0:
             logger.error("No zones selected")
             return False
 
         # Apply state changes
@@ -460,19 +453,17 @@
         # Refresh status
         self.request_status_refresh()  # Trigger status update
 
         return accepted
 
     async def control_partition(self, partition: str, command: str) -> bool:
         command = command.lower()
-        logger.debug("Control Partition: {} - {}".format(partition, command))
+        logger.debug(f"Control Partition: {partition} - {command}")
 
-        partitions_selected = self.storage.get_container("partition").select(
-            partition
-        )  # type: Sequence[int]
+        partitions_selected = self.storage.get_container("partition").select(partition)
 
         # Not Found
         if len(partitions_selected) == 0:
             logger.error("No partitions selected")
             return False
 
         # Apply state changes
@@ -489,15 +480,15 @@
         # Refresh status
         self.request_status_refresh()  # Trigger status update
 
         return accepted
 
     async def control_output(self, output, command) -> bool:
         command = command.lower()
-        logger.debug("Control Output: {} - {}".format(output, command))
+        logger.debug(f"Control Output: {output} - {command}")
 
         outputs_selected = self.storage.get_container("pgm").select(output)
 
         # Not Found
         if len(outputs_selected) == 0:
             logger.error("No outputs selected")
             return False
@@ -541,15 +532,15 @@
         except asyncio.CancelledError:
             logger.error("send_panic canceled")
         except asyncio.TimeoutError:
             logger.error("send_panic timeout")
 
     async def control_door(self, door, command) -> bool:
         command = command.lower()
-        logger.debug("Control Door: {} - {}".format(door, command))
+        logger.debug(f"Control Door: {door} - {command}")
 
         doors_selected = self.storage.get_container("door").select(door)
 
         # Not Found
         if len(doors_selected) == 0:
             logger.error("No doors selected")
             return False
@@ -581,15 +572,15 @@
         try:
             try:
                 evt = LiveEvent(
                     event=message,
                     event_map=self.panel.event_map,
                     label_provider=self.get_label,
                 )
-            except AssertionError as e:
+            except AssertionError:
                 logger.debug("Error creating event")
                 return
 
             element = self.storage.get_container_object(evt.type, evt.id)
 
             # Temporary to catch labels/properties in wrong places
             # TODO: REMOVE
@@ -629,26 +620,26 @@
 
             # The event has changes. Update the state
             if len(evt.change) > 0 and element:
                 self.storage.update_container_object(evt.type, evt.id, evt.change)
 
             ps.sendEvent(evt)
 
-        except:
+        except Exception:
             logger.exception("Handle live event")
 
     def handle_error_message(self, message):
         """Handle ErrorMessage"""
         error_enum = message.fields.value.message
 
         if error_enum == "panel_not_connected":
             asyncio.get_event_loop().create_task(self.disconnect())
         else:
             message = self.panel.get_error_message(error_enum)
-            logger.error("Got ERROR Message: {}".format(message))
+            logger.error(f"Got ERROR Message: {message}")
             if message == "Invalid PC Password":
                 raise AuthenticationFailed()
             elif "code lockout" in message:
                 raise CodeLockout()
 
     async def disconnect(self):
         logger.info("Disconnecting from the Alarm Panel")
@@ -705,15 +696,21 @@
         if "troubles" in status:
             self._process_trouble_statuses(status["troubles"])
 
         for element_type, element_items in status.items():
             if element_type in ["troubles"]:  # troubles was already parsed
                 continue
             for element_item_key, element_item_status in element_items.items():
-                if isinstance(element_item_status, (dict, list,)):
+                if isinstance(
+                    element_item_status,
+                    (
+                        dict,
+                        list,
+                    ),
+                ):
                     self.storage.update_container_object(
                         element_type, element_item_key, element_item_status
                     )
                 else:
                     logger.debug(
                         "%s/%s:%s ignored",
                         element_type,
@@ -742,21 +739,23 @@
         self.storage.update_container_object(
             "system", "troubles", {"trouble": global_trouble}
         )
 
     def _is_time_sync_required(self, now) -> bool:
         assert now.tzinfo is None
         try:
-           drift = (now - self.storage.get_container("system")["date"]["time"]).total_seconds()
-
-           if abs(drift) > cfg.SYNC_TIME_MIN_DRIFT:
-              logger.info(f"Time drifted more than allowed: {drift} seconds")
-              return True
-           else:
-              logger.debug(f"Time drifted within allowed range: {drift} seconds")
+            drift = (
+                now - self.storage.get_container("system")["date"]["time"]
+            ).total_seconds()
+
+            if abs(drift) > cfg.SYNC_TIME_MIN_DRIFT:
+                logger.info(f"Time drifted more than allowed: {drift} seconds")
+                return True
+            else:
+                logger.debug(f"Time drifted within allowed range: {drift} seconds")
 
         except KeyError:
             pass
 
         return False
 
     def _update_partition_states(self):
@@ -791,15 +790,15 @@
             if properties.get("exit_delay"):  # Redefine if pending
                 change["current_state"] = "arming"
 
             self.storage.update_container_object("partition", properties["key"], change)
 
     def _on_event(self, event: Event):
         if cfg.LOGGING_DUMP_EVENTS:
-            logger.debug("LiveEvent: {}".format(event))
+            logger.debug(f"LiveEvent: {event}")
 
         event.call_hook(storage=self.storage, alarm=self)
 
         if isinstance(event, LiveEvent):
             self._update_partition_states()
 
     def _on_property_change(self, change: Change):
@@ -809,11 +808,11 @@
         try:
             event = ChangeEvent(
                 change_object=change,
                 property_map=self.panel.property_map,
                 label_provider=self.get_label,
             )
             if cfg.LOGGING_DUMP_EVENTS:
-                logger.debug("ChangeEvent: {}".format(event))
+                logger.debug(f"ChangeEvent: {event}")
             ps.sendEvent(event)
         except AssertionError:
             logger.debug("Could not create event from change")
```

### Comparing `paradox-alarm-interface-3.4.0/paradox/parsers/status.py` & `paradox_alarm_interface-3.4.2.dev0/paradox/parsers/status.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/PKG-INFO` & `paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradox-alarm-interface
-Version: 3.4.0
+Version: 3.4.2.dev0
 Summary: Interface to Paradox Alarm Panels
 Home-page: https://github.com/ParadoxAlarmInterface/pai
 Author: Jevgeni Kiski, João Paulo Barraca
 Author-email: yozik04@gmail.com, jpbarraca@gmail.com
 License: EPL
 Project-URL: Bug Tracker, https://github.com/ParadoxAlarmInterface/pai/issues
 Keywords: paradox alarm ip150 serial home-assistant smarthome mqtt
@@ -14,22 +14,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: construct~=2.9.43
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: python-slugify>=4.0.1
 Requires-Dist: pytz>=2021.3
-Requires-Dist: paho_mqtt>=1.5.0
+Requires-Dist: paho_mqtt<2,>=1.5.0
 Requires-Dist: requests>=2.20.0
 Requires-Dist: pyserial-asyncio>=0.4
 Provides-Extra: yaml
 Requires-Dist: pyyaml>=5.2.0; extra == "yaml"
 Provides-Extra: pushbullet
 Requires-Dist: pushbullet.py>=0.11.0; extra == "pushbullet"
 Requires-Dist: ws4py>=0.4.2; extra == "pushbullet"
@@ -103,16 +103,16 @@
 
 ## How to use
 See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/Installation)
 
 ## Tested Environment
 
 Tested in the following environment:
-* Python 3.6, 3.7, 3.8
-* Mosquitto MQTT Broker >v 1.4.8
+* Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
+* Mosquitto MQTT Broker > 1.4.8
 * OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..)
 * Ubuntu Server 16.04.3 LTS
 * Paradox MG5050, SP7000 and EVO panels
 * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS interface
 * Pushbullet.py
 * SIM900 module through a serial port
 * Serial over TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: paradox-alarm-interface Version: 3.4.0 Summary:
-Interface to Paradox Alarm Panels Home-page: https://github.com/
+Metadata-Version: 2.1 Name: paradox-alarm-interface Version: 3.4.2.dev0
+Summary: Interface to Paradox Alarm Panels Home-page: https://github.com/
 ParadoxAlarmInterface/pai Author: Jevgeni Kiski, JoÃ£o Paulo Barraca Author-
 email: yozik04@gmail.com, jpbarraca@gmail.com License: EPL Project-URL: Bug
 Tracker, https://github.com/ParadoxAlarmInterface/pai/issues Keywords: paradox
 alarm ip150 serial home-assistant smarthome mqtt Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+Programming Language :: Python :: 3.11 Requires-Python: <3.12,>=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 construct~=2.9.43 Requires-Dist: argparse>=1.4.0 Requires-Dist: python-
-slugify>=4.0.1 Requires-Dist: pytz>=2021.3 Requires-Dist: paho_mqtt>=1.5.0
+slugify>=4.0.1 Requires-Dist: pytz>=2021.3 Requires-Dist: paho_mqtt<2,>=1.5.0
 Requires-Dist: requests>=2.20.0 Requires-Dist: pyserial-asyncio>=0.4 Provides-
 Extra: yaml Requires-Dist: pyyaml>=5.2.0; extra == "yaml" Provides-Extra:
 pushbullet Requires-Dist: pushbullet.py>=0.11.0; extra == "pushbullet"
 Requires-Dist: ws4py>=0.4.2; extra == "pushbullet" Provides-Extra: pushover
 Requires-Dist: chump>=1.6.0; extra == "pushover" Provides-Extra: signal
 Requires-Dist: pygobject>=3.20.0; extra == "signal" Requires-Dist:
 pydbus>=0.6.0; extra == "signal" Requires-Dist: gi>=1.2; extra == "signal"
@@ -58,85 +58,86 @@
 registered in the site** We do not recommend using SWAN because of https://
 github.com/CriticalSecurity/paradox ## Firmware Upgrade WARNING: **Do not
 upgrade EVO firmware versions to 7.50.000+ if you use Serial connection.
 Process is irreversible! Paradox introduces serial communication encryption
 which most probably will break our PAI ability to talk to the panel.** ## How
 to use See [wiki](https://github.com/ParadoxAlarmInterface/pai/wiki/
 Installation) ## Tested Environment Tested in the following environment: *
-Python 3.6, 3.7, 3.8 * Mosquitto MQTT Broker >v 1.4.8 * OrangePi 2G-IOT, NanoPi
-NEO, and Raspberry Pi 3 through their built in Serial Port (with a level
-shifter!), or a USB RS232 TTL adapter (CP2102, PL2303, CH340, etc..) * Ubuntu
-Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO panels * [Signal Cli]
-(https://github.com/AsamK/signal-cli) through a DBUS interface * Pushbullet.py
-* SIM900 module through a serial port * Serial over TCP (ESP32 or Arduino
-connected to the panel's serial port acts as a proxy) ## Authors * JoÃ£o Paulo
-Barraca - [@jpbarraca](https://github.com/jpbarraca) - Main code and MG/SP
-devices * Jevgeni Kiski - [@yozik04](https://github.com/yozik04) - Main code
-and EVO devices * Ion Darie - [@iondarie](https://github.com/iondarie) - PAI
-Logo, Homebridge integration, testing ## Acknowledgments This work is inspired
-or uses parts from the following projects: * Tertiush at https://github.com/
-Tertiush/ParadoxIP150v2 * Spinza at https://github.com/spinza/paradox_mqtt ##
-Thanks * Ivan Markov - [@ivmarkov](https://github.com/ivmarkov) - Multi-
-platform Docker builds * Claudiu Bucur - [@clau-bucur](https://github.com/clau-
-bucur) - For fixing HomeAssistant plugin after Supervisor(2021.02.5) upgrade
-[#199](https://github.com/ParadoxAlarmInterface/pai/issues/199) * David Tekan -
-[@tekand](https://github.com/tekand) - For supporting different label
-encodings. ## Disclaimer Paradox, MG5050 and IP150 are registered marks of
-PARADOX. Other brands are owned by their respective owners. The code was
-developed as a way of integrating personally owned Paradox systems, and it
-cannot be used for other purposes. It is not affiliated with any company and it
-doesn't have have commercial intent. The code is provided AS IS and the
-developers will not be held responsible for failures in the alarm systems, or
-any other malfunction. ## Donations We have fully stopped accepting donations
-due to lack of free time to spend on this project. [//]: # (## With support
-from) [//]: # () [//]: # (_[_J_e_t_B_r_a_i_n_s_]) Eclipse Public License - v 2.0 THE
-ACCOMPANYING PROGRAM IS PROVIDED UNDER THE TERMS OF THIS ECLIPSE PUBLIC LICENSE
-("AGREEMENT"). ANY USE, REPRODUCTION OR DISTRIBUTION OF THE PROGRAM CONSTITUTES
-RECIPIENT'S ACCEPTANCE OF THIS AGREEMENT. 1. DEFINITIONS "Contribution" means:
-a) in the case of the initial Contributor, the initial content Distributed
-under this Agreement, and b) in the case of each subsequent Contributor: i)
-changes to the Program, and ii) additions to the Program; where such changes
-and/or additions to the Program originate from and are Distributed by that
-particular Contributor. A Contribution "originates" from a Contributor if it
-was added to the Program by such Contributor itself or anyone acting on such
-Contributor's behalf. Contributions do not include changes or additions to the
-Program that are not Modified Works. "Contributor" means any person or entity
-that Distributes the Program. "Licensed Patents" mean patent claims licensable
-by a Contributor which are necessarily infringed by the use or sale of its
-Contribution alone or when combined with the Program. "Program" means the
-Contributions Distributed in accordance with this Agreement. "Recipient" means
-anyone who receives the Program under this Agreement or any Secondary License
-(as applicable), including Contributors. "Derivative Works" shall mean any
-work, whether in Source Code or other form, that is based on (or derived from)
-the Program and for which the editorial revisions, annotations, elaborations,
-or other modifications represent, as a whole, an original work of authorship.
-"Modified Works" shall mean any work in Source Code or other form that results
-from an addition to, deletion from, or modification of the contents of the
-Program, including, for purposes of clarity any new file in Source Code form
-that contains any contents of the Program. Modified Works shall not include
-works that contain only declarations, interfaces, types, classes, structures,
-or files of the Program solely in each case in order to link to, bind by name,
-or subclass the Program or Modified Works thereof. "Distribute" means the acts
-of a) distributing or b) making available in any manner that enables the
-transfer of a copy. "Source Code" means the form of a Program preferred for
-making modifications, including but not limited to software source code,
-documentation source, and configuration files. "Secondary License" means either
-the GNU General Public License, Version 2.0, or any later versions of that
-license, including any exceptions or additional permissions as identified by
-the initial Contributor. 2. GRANT OF RIGHTS a) Subject to the terms of this
+Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11 * Mosquitto MQTT Broker > 1.4.8 *
+OrangePi 2G-IOT, NanoPi NEO, and Raspberry Pi 3 through their built in Serial
+Port (with a level shifter!), or a USB RS232 TTL adapter (CP2102, PL2303,
+CH340, etc..) * Ubuntu Server 16.04.3 LTS * Paradox MG5050, SP7000 and EVO
+panels * [Signal Cli](https://github.com/AsamK/signal-cli) through a DBUS
+interface * Pushbullet.py * SIM900 module through a serial port * Serial over
+TCP (ESP32 or Arduino connected to the panel's serial port acts as a proxy) ##
+Authors * JoÃ£o Paulo Barraca - [@jpbarraca](https://github.com/jpbarraca) -
+Main code and MG/SP devices * Jevgeni Kiski - [@yozik04](https://github.com/
+yozik04) - Main code and EVO devices * Ion Darie - [@iondarie](https://
+github.com/iondarie) - PAI Logo, Homebridge integration, testing ##
+Acknowledgments This work is inspired or uses parts from the following
+projects: * Tertiush at https://github.com/Tertiush/ParadoxIP150v2 * Spinza at
+https://github.com/spinza/paradox_mqtt ## Thanks * Ivan Markov - [@ivmarkov]
+(https://github.com/ivmarkov) - Multi-platform Docker builds * Claudiu Bucur -
+[@clau-bucur](https://github.com/clau-bucur) - For fixing HomeAssistant plugin
+after Supervisor(2021.02.5) upgrade [#199](https://github.com/
+ParadoxAlarmInterface/pai/issues/199) * David Tekan - [@tekand](https://
+github.com/tekand) - For supporting different label encodings. ## Disclaimer
+Paradox, MG5050 and IP150 are registered marks of PARADOX. Other brands are
+owned by their respective owners. The code was developed as a way of
+integrating personally owned Paradox systems, and it cannot be used for other
+purposes. It is not affiliated with any company and it doesn't have have
+commercial intent. The code is provided AS IS and the developers will not be
+held responsible for failures in the alarm systems, or any other malfunction.
+## Donations We have fully stopped accepting donations due to lack of free time
+to spend on this project. [//]: # (## With support from) [//]: # () [//]: # (
+_[_J_e_t_B_r_a_i_n_s_]) Eclipse Public License - v 2.0 THE ACCOMPANYING PROGRAM IS
+PROVIDED UNDER THE TERMS OF THIS ECLIPSE PUBLIC LICENSE ("AGREEMENT"). ANY USE,
+REPRODUCTION OR DISTRIBUTION OF THE PROGRAM CONSTITUTES RECIPIENT'S ACCEPTANCE
+OF THIS AGREEMENT. 1. DEFINITIONS "Contribution" means: a) in the case of the
+initial Contributor, the initial content Distributed under this Agreement, and
+b) in the case of each subsequent Contributor: i) changes to the Program, and
+ii) additions to the Program; where such changes and/or additions to the
+Program originate from and are Distributed by that particular Contributor. A
+Contribution "originates" from a Contributor if it was added to the Program by
+such Contributor itself or anyone acting on such Contributor's behalf.
+Contributions do not include changes or additions to the Program that are not
+Modified Works. "Contributor" means any person or entity that Distributes the
+Program. "Licensed Patents" mean patent claims licensable by a Contributor
+which are necessarily infringed by the use or sale of its Contribution alone or
+when combined with the Program. "Program" means the Contributions Distributed
+in accordance with this Agreement. "Recipient" means anyone who receives the
+Program under this Agreement or any Secondary License (as applicable),
+including Contributors. "Derivative Works" shall mean any work, whether in
+Source Code or other form, that is based on (or derived from) the Program and
+for which the editorial revisions, annotations, elaborations, or other
+modifications represent, as a whole, an original work of authorship. "Modified
+Works" shall mean any work in Source Code or other form that results from an
+addition to, deletion from, or modification of the contents of the Program,
+including, for purposes of clarity any new file in Source Code form that
+contains any contents of the Program. Modified Works shall not include works
+that contain only declarations, interfaces, types, classes, structures, or
+files of the Program solely in each case in order to link to, bind by name, or
+subclass the Program or Modified Works thereof. "Distribute" means the acts of
+a) distributing or b) making available in any manner that enables the transfer
+of a copy. "Source Code" means the form of a Program preferred for making
+modifications, including but not limited to software source code, documentation
+source, and configuration files. "Secondary License" means either the GNU
+General Public License, Version 2.0, or any later versions of that license,
+including any exceptions or additional permissions as identified by the initial
+Contributor. 2. GRANT OF RIGHTS a) Subject to the terms of this Agreement, each
+Contributor hereby grants Recipient a non-exclusive, worldwide, royalty-free
+copyright license to reproduce, prepare Derivative Works of, publicly display,
+publicly perform, Distribute and sublicense the Contribution of such
+Contributor, if any, and such Derivative Works. b) Subject to the terms of this
 Agreement, each Contributor hereby grants Recipient a non-exclusive, worldwide,
-royalty-free copyright license to reproduce, prepare Derivative Works of,
-publicly display, publicly perform, Distribute and sublicense the Contribution
-of such Contributor, if any, and such Derivative Works. b) Subject to the terms
-of this Agreement, each Contributor hereby grants Recipient a non-exclusive,
-worldwide, royalty-free patent license under Licensed Patents to make, use,
-sell, offer to sell, import and otherwise transfer the Contribution of such
-Contributor, if any, in Source Code or other form. This patent license shall
-apply to the combination of the Contribution and the Program if, at the time
-the Contribution is added by the Contributor, such addition of the Contribution
+royalty-free patent license under Licensed Patents to make, use, sell, offer to
+sell, import and otherwise transfer the Contribution of such Contributor, if
+any, in Source Code or other form. This patent license shall apply to the
+combination of the Contribution and the Program if, at the time the
+Contribution is added by the Contributor, such addition of the Contribution
 causes such combination to be covered by the Licensed Patents. The patent
 license shall not apply to any other combinations which include the
 Contribution. No hardware per se is licensed hereunder. c) Recipient
 understands that although each Contributor grants the licenses to its
 Contributions set forth herein, no assurances are provided by any Contributor
 that the Program does not infringe the patent or other intellectual property
 rights of any other entity. Each Contributor disclaims any liability to
```

### Comparing `paradox-alarm-interface-3.4.0/paradox_alarm_interface.egg-info/SOURCES.txt` & `paradox_alarm_interface-3.4.2.dev0/paradox_alarm_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/pyproject.toml` & `paradox_alarm_interface-3.4.2.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/setup.cfg` & `paradox_alarm_interface-3.4.2.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 license = EPL
 
 [options]
 zip_safe = True
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.8,<3.12
 install_requires = 
 	construct~=2.9.43
 	argparse>=1.4.0
 	python-slugify>=4.0.1
 	pytz>=2021.3
-	paho_mqtt>=1.5.0
+	paho_mqtt>=1.5.0,<2
 	requests>=2.20.0
 	pyserial-asyncio>=0.4
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `paradox-alarm-interface-3.4.0/tests/test_async_queue.py` & `paradox_alarm_interface-3.4.2.dev0/tests/test_async_queue.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/tests/test_config.py` & `paradox_alarm_interface-3.4.2.dev0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `paradox-alarm-interface-3.4.0/tests/test_paradox.py` & `paradox_alarm_interface-3.4.2.dev0/tests/test_paradox.py`

 * *Files identical despite different names*

