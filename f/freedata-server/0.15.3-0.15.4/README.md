# Comparing `tmp/freedata-server-0.15.3.tar.gz` & `tmp/freedata_server-0.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedata-server-0.15.3.tar", last modified: Wed Apr 17 20:03:14 2024, max compression
+gzip compressed data, was "freedata_server-0.15.4.tar", last modified: Thu Apr 18 09:06:46 2024, max compression
```

## Comparing `freedata-server-0.15.3.tar` & `freedata_server-0.15.4.tar`

### file list

```diff
@@ -1,87 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.822620 freedata-server-0.15.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-17 20:02:42.000000 freedata-server-0.15.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 20:03:14.822620 freedata-server-0.15.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-17 20:02:42.000000 freedata-server-0.15.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.822620 freedata-server-0.15.3/freedata_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 20:03:14.000000 freedata-server-0.15.3/freedata_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.818620 freedata-server-0.15.3/modem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/api_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/arq_data_type_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/arq_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/arq_session_irs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/arq_session_iss.py
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    24044 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/codec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_arq_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_cq.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_feq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_message_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_qrv.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/cw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20305 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/data_frame_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    13911 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/demodulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler_arq_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler_cq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler_p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/frame_handler_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    24901 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.810619 freedata-server-0.15.3/modem/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.818620 freedata-server-0.15.3/modem/lib/codec2/
--rw-r--r--   0 runner    (1001) docker     (127)  2264619 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/codec2/libcodec2.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.810619 freedata-server-0.15.3/modem/lib/pyaudio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:03:14.822620 freedata-server-0.15.3/modem/lib/pyaudio/windows/
--rw-r--r--   0 runner    (1001) docker     (127)    97711 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp310-cp310-win32.whl
--rw-r--r--   0 runner    (1001) docker     (127)   112489 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp310-cp310-win_amd64.whl
--rw-r--r--   0 runner    (1001) docker     (127)    98368 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp311-cp311-win32.whl
--rw-r--r--   0 runner    (1001) docker     (127)   113707 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp311-cp311-win_amd64.whl
--rw-r--r--   0 runner    (1001) docker     (127)    97698 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp39-cp39-win32.whl
--rw-r--r--   0 runner    (1001) docker     (127)   112479 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/PyAudio-0.2.11-cp39-cp39-win_amd64.whl
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/lib/pyaudio/windows/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/maidenhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    27414 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_p2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_system_db_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_system_db_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_system_db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_system_db_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/message_system_db_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/modem.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/modem_frametypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/modulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/radio_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/rigctld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/rigdummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/schedule_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/selftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/serial_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/socket_interface_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/tci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-17 20:02:42.000000 freedata-server-0.15.3/modem/websocket_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:03:14.822620 freedata-server-0.15.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-17 20:02:42.000000 freedata-server-0.15.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.661859 freedata_server-0.15.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 09:06:16.000000 freedata_server-0.15.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 09:06:46.661859 freedata_server-0.15.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 09:06:16.000000 freedata_server-0.15.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.653859 freedata_server-0.15.4/freedata_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/api_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_data_type_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session_irs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session_iss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24041 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/codec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_arq_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_feq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_message_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_qrv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20305 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/data_frame_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/demodulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_arq_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24901 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.645859 freedata_server-0.15.4/freedata_server/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.657859 freedata_server-0.15.4/freedata_server/lib/codec2/
+-rw-r--r--   0 runner    (1001) docker     (127)  2264619 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.dll
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2206856 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.so
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/maidenhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27414 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_p2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modem_frametypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/radio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/rigctld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/rigdummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/schedule_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/selftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/serial_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/socket_interface_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/tci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/websocket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.661859 freedata_server-0.15.4/freedata_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:06:46.661859 freedata_server-0.15.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 09:06:17.000000 freedata_server-0.15.4/setup.py
```

### Comparing `freedata-server-0.15.3/LICENSE` & `freedata_server-0.15.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/PKG-INFO` & `freedata_server-0.15.4/freedata_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedata-server
-Version: 0.15.3
+Version: 0.15.4
 Summary: A free, open-source, multi-platform application for sending files and messages, using the codec2 HF modems.
 Home-page: https://freedata.app
 Author: DJ2LS
 Author-email: dj2ls@proton.me
 License: GPL3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freedata-server-0.15.3/README.md` & `freedata_server-0.15.4/README.md`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/freedata_server.egg-info/PKG-INFO` & `freedata_server-0.15.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freedata-server
-Version: 0.15.3
+Name: freedata_server
+Version: 0.15.4
 Summary: A free, open-source, multi-platform application for sending files and messages, using the codec2 HF modems.
 Home-page: https://freedata.app
 Author: DJ2LS
 Author-email: dj2ls@proton.me
 License: GPL3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freedata-server-0.15.3/modem/api_validations.py` & `freedata_server-0.15.4/freedata_server/api_validations.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/arq_data_type_handler.py` & `freedata_server-0.15.4/freedata_server/arq_data_type_handler.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/arq_session.py` & `freedata_server-0.15.4/freedata_server/arq_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     }
 
     def __init__(self, config: dict, modem, dxcall: str, state_manager):
         self.logger = structlog.get_logger(type(self).__name__)
         self.config = config
 
         self.event_manager: EventManager = modem.event_manager
-        #self.states = modem.states
+        #self.states = freedata_server.states
         self.states = state_manager
         self.states.setARQ(True)
 
         self.protocol_version = 1
 
         self.snr = []
```

### Comparing `freedata-server-0.15.3/modem/arq_session_irs.py` & `freedata_server-0.15.4/freedata_server/arq_session_irs.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/arq_session_iss.py` & `freedata_server-0.15.4/freedata_server/arq_session_iss.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/audio.py` & `freedata_server-0.15.4/freedata_server/audio.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/codec2.py` & `freedata_server-0.15.4/freedata_server/codec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         files = glob.glob(os.path.join(script_dir, "**/*libcodec2*.dylib"), recursive=True)
 elif sys.platform in ["win32", "win64"]:
     files = glob.glob(os.path.join(script_dir, "**\\*libcodec2*.dll"), recursive=True)
 else:
     files = []
 api = None
 
-print(files)
 for file in files:
     try:
         api = ctypes.CDLL(file)
         #log.info("[C2 ] Libcodec2 loaded", path=file)
         break
     except OSError as err:
         pass
@@ -415,15 +414,15 @@
         ("fs", ctypes.c_float),  # Sample Frequency
         ("rs", ctypes.c_float),  # Symbol Rate
         ("ts", ctypes.c_float),  # Symbol duration
         ("tcp", ctypes.c_float),  # Cyclic Prefix duration
         ("timing_mx_thresh", ctypes.c_float),  # Threshold for timing metrics
         ("nc", ctypes.c_int),  # Number of carriers
         ("ns", ctypes.c_int),  # Number of Symbol frames
-        ("np", ctypes.c_int),  # Number of modem frames per packet
+        ("np", ctypes.c_int),  # Number of freedata_server frames per packet
         ("bps", ctypes.c_int),  # Bits per Symbol
         ("txtbits", ctypes.c_int),  # Number of auxiliary data bits
         ("nuwbits", ctypes.c_int),  # Number of unique word bits
         ("bad_uw_errors", ctypes.c_int),  # Threshold for bad unique word detection
         ("ftwindowwidth", ctypes.c_int),  # Filter window width
         ("edge_pilots", ctypes.c_int),  # Edge pilots configuration
         ("state_machine", ctypes.c_char_p),  # Name of sync state machine used
```

### Comparing `freedata-server-0.15.3/modem/command.py` & `freedata_server-0.15.4/freedata_server/command.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/command_arq_raw.py` & `freedata_server-0.15.4/freedata_server/command_arq_raw.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/command_feq.py` & `freedata_server-0.15.4/freedata_server/command_feq.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/command_message_send.py` & `freedata_server-0.15.4/freedata_server/command_message_send.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/command_p2p_connection.py` & `freedata_server-0.15.4/freedata_server/command_p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/command_ping.py` & `freedata_server-0.15.4/freedata_server/command_ping.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/config.py` & `freedata_server-0.15.4/freedata_server/config.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/cw.py` & `freedata_server-0.15.4/freedata_server/cw.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/data_frame_factory.py` & `freedata_server-0.15.4/freedata_server/data_frame_factory.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/demodulator.py` & `freedata_server-0.15.4/freedata_server/demodulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,26 +156,26 @@
             while self.stream.active:
                 threading.Event().wait(0.01)
                 while audiobuffer.nbuffer >= nin:
                     # demodulate audio
                     nbytes = codec2.api.freedv_rawdatarx(
                         freedv, bytes_out, audiobuffer.buffer.ctypes
                     )
-                    # get current modem states and write to list
+                    # get current freedata_server states and write to list
                     # 1 trial
                     # 2 sync
                     # 3 trial sync
                     # 6 decoded
                     # 10 error decoding == NACK
                     rx_status = codec2.api.freedv_get_rx_status(freedv)
 
                     if rx_status not in [0]:
                         self.is_codec2_traffic_counter = self.is_codec2_traffic_cooldown
                         self.log.debug(
-                            "[MDM] [demod_audio] modem state", mode=mode_name, rx_status=rx_status,
+                            "[MDM] [demod_audio] freedata_server state", mode=mode_name, rx_status=rx_status,
                             sync_flag=codec2.api.rx_sync_flags_to_text[rx_status]
                         )
 
                     # decrement codec traffic counter for making state smoother
                     if self.is_codec2_traffic_counter > 0:
                         self.is_codec2_traffic_counter -= 1
                         self.states.set_channel_busy_condition_codec2(True)
```

### Comparing `freedata-server-0.15.3/modem/event_manager.py` & `freedata_server-0.15.4/freedata_server/event_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,24 +78,24 @@
                 'state': state,
                 'data': data
             }
         }
         self.broadcast(event)
 
     def modem_started(self):
-        event = {"modem": "started"}
+        event = {"freedata_server": "started"}
         self.broadcast(event)
 
     def modem_restarted(self):
-        event = {"modem": "restarted"}
+        event = {"freedata_server": "restarted"}
         self.broadcast(event)
 
     def modem_stopped(self):
-        event = {"modem": "stopped"}
+        event = {"freedata_server": "stopped"}
         self.broadcast(event)
 
     def modem_failed(self):
-        event = {"modem": "failed"}
+        event = {"freedata_server": "failed"}
         self.broadcast(event)
 
     def freedata_message_db_change(self):
         self.broadcast({"message-db": "changed"})
```

### Comparing `freedata-server-0.15.3/modem/explorer.py` & `freedata_server-0.15.4/freedata_server/explorer.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_dispatcher.py` & `freedata_server-0.15.4/freedata_server/frame_dispatcher.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_handler.py` & `freedata_server-0.15.4/freedata_server/frame_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,16 +97,17 @@
 
         if "gridsquare" in frame:
             activity["gridsquare"] = frame["gridsquare"]
 
         if "session_id" in frame:
             activity["session_id"] = frame["session_id"]
 
-        if "AWAY_FROM_KEY" in frame["flag"]:
-            activity["away_from_key"] = frame["flag"]["AWAY_FROM_KEY"]
+        if "flag" in frame:
+            if "AWAY_FROM_KEY" in frame["flag"]:
+                activity["away_from_key"] = frame["flag"]["AWAY_FROM_KEY"]
 
         self.states.add_activity(activity)
 
     def add_to_heard_stations(self):
         frame = self.details['frame']
 
         if 'origin' not in frame:
@@ -117,25 +118,30 @@
         distance_km = None
         distance_miles = None
         if dxgrid != "------" and frame.get('gridsquare'):
             distance_dict = maidenhead.distance_between_locators(self.config['STATION']['mygrid'], frame['gridsquare'])
             distance_km = distance_dict['kilometers']
             distance_miles = distance_dict['miles']
 
+        away_from_key = False
+        if "flag" in self.details['frame']:
+            if "AWAY_FROM_KEY" in self.details['frame']["flag"]:
+                away_from_key = self.details['frame']["flag"]["AWAY_FROM_KEY"]
+
         helpers.add_to_heard_stations(
             frame['origin'],
             dxgrid,
             self.name,
             self.details['snr'],
             self.details['frequency_offset'],
             self.states.radio_frequency,
             self.states.heard_stations,
             distance_km=distance_km,  # Pass the kilometer distance
             distance_miles=distance_miles,  # Pass the miles distance
-            away_from_key=self.details['frame']["flag"]["AWAY_FROM_KEY"]
+            away_from_key=away_from_key
         )
     def make_event(self):
 
         event = {
             "type": "frame-handler",
             "received": self.details['frame']['frame_type'],
             "timestamp": int(time.time()),
```

### Comparing `freedata-server-0.15.3/modem/frame_handler_arq_session.py` & `freedata_server-0.15.4/freedata_server/frame_handler_arq_session.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_handler_beacon.py` & `freedata_server-0.15.4/freedata_server/frame_handler_beacon.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_handler_cq.py` & `freedata_server-0.15.4/freedata_server/frame_handler_cq.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_handler_p2p_connection.py` & `freedata_server-0.15.4/freedata_server/frame_handler_p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/frame_handler_ping.py` & `freedata_server-0.15.4/freedata_server/frame_handler_ping.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/helpers.py` & `freedata_server-0.15.4/freedata_server/helpers.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/lib/codec2/libcodec2.dll` & `freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.dll`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/log_handler.py` & `freedata_server-0.15.4/freedata_server/log_handler.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/maidenhead.py` & `freedata_server-0.15.4/freedata_server/maidenhead.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/mesh.py` & `freedata_server-0.15.4/freedata_server/mesh.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_p2p.py` & `freedata_server-0.15.4/freedata_server/message_p2p.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_system_db_attachments.py` & `freedata_server-0.15.4/freedata_server/message_system_db_attachments.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_system_db_beacon.py` & `freedata_server-0.15.4/freedata_server/message_system_db_beacon.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_system_db_manager.py` & `freedata_server-0.15.4/freedata_server/message_system_db_manager.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_system_db_messages.py` & `freedata_server-0.15.4/freedata_server/message_system_db_messages.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/message_system_db_model.py` & `freedata_server-0.15.4/freedata_server/message_system_db_model.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/modem.py` & `freedata_server-0.15.4/freedata_server/modem.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,23 +105,23 @@
                 raise RuntimeError("Unable to init audio devices")
             self.demodulator.start(self.sd_input_stream)
 
         return True
 
     def stop_modem(self):
         try:
-            # let's stop the modem service
+            # let's stop the freedata_server service
             self.service_queue.put("stop")
             # simulate audio class active state for reducing cli output
             # self.stream = lambda: None
             # self.stream.active = False
             # self.stream.stop
 
         except Exception:
-            self.log.error("[MDM] Error stopping modem")
+            self.log.error("[MDM] Error stopping freedata_server")
 
     def init_audio(self):
         self.log.info(f"[MDM] init: get audio devices", input_device=self.audio_input_device,
                       output_device=self.audio_output_device)
         try:
             result = audio.get_device_index_from_crc(self.audio_input_device, True)
             if result is None:
```

### Comparing `freedata-server-0.15.3/modem/modem_frametypes.py` & `freedata_server-0.15.4/freedata_server/modem_frametypes.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/modulator.py` & `freedata_server-0.15.4/freedata_server/modulator.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/p2p_connection.py` & `freedata_server-0.15.4/freedata_server/p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/radio_manager.py` & `freedata_server-0.15.4/freedata_server/radio_manager.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/rigctld.py` & `freedata_server-0.15.4/freedata_server/rigctld.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/rigdummy.py` & `freedata_server-0.15.4/freedata_server/rigdummy.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/schedule_manager.py` & `freedata_server-0.15.4/freedata_server/schedule_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def start(self, modem):
         """Start scheduling events and run the scheduler in a separate thread."""
 
         # wait some time
         threading.Event().wait(timeout=10)
 
-        # get actual modem instance
+        # get actual freedata_server instance
         self.modem = modem
 
         self.running = True  # Set the running flag to True
         for event_info in self.events.values():
             # Schedule each event for the first time
             self.scheduler.enter(0, 1, self.schedule_event, (event_info['function'], event_info['interval']))
```

### Comparing `freedata-server-0.15.3/modem/selftest.py` & `freedata_server-0.15.4/freedata_server/selftest.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/serial_ports.py` & `freedata_server-0.15.4/freedata_server/serial_ports.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/server.py` & `freedata_server-0.15.4/freedata_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from message_system_db_attachments import DatabaseManagerAttachments
 from message_system_db_beacon import DatabaseManagerBeacon
 from schedule_manager import ScheduleManager
 
 app = Flask(__name__)
 CORS(app, resources={r"/*": {"origins": "*"}})
 sock = Sock(app)
-MODEM_VERSION = "0.15.3-alpha"
+MODEM_VERSION = "0.15.4-alpha"
 
 # set config file to use
 def set_config():
     if 'FREEDATA_CONFIG' in os.environ:
         config_file = os.environ['FREEDATA_CONFIG']
     else:
         script_dir = os.path.dirname(os.path.abspath(__file__))
@@ -128,28 +128,28 @@
     return api_response(devices)
 
 @app.route('/devices/serial', methods=['GET'])
 def get_serial_devices():
     devices = serial_ports.get_ports()
     return api_response(devices)
 
-@app.route('/modem/state', methods=['GET'])
+@app.route('/freedata_server/state', methods=['GET'])
 def get_modem_state():
     return api_response(app.state_manager.sendState())
 
-@app.route('/modem/cqcqcq', methods=['POST', 'GET'])
+@app.route('/freedata_server/cqcqcq', methods=['POST', 'GET'])
 def post_cqcqcq():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for triggering a CQ via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     enqueue_tx_command(command_cq.CQCommand)
     return api_ok()
 
-@app.route('/modem/beacon', methods=['POST'])
+@app.route('/freedata_server/beacon', methods=['POST'])
 def post_beacon():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for controlling BEACON STATE via POST"})
     if not isinstance(request.json['enabled'], bool) or not isinstance(request.json['away_from_key'], bool):
         api_abort(f"Incorrect value for 'enabled'. Shoud be bool.")
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
@@ -161,85 +161,85 @@
         if not app.state_manager.getARQ():
             enqueue_tx_command(command_beacon.BeaconCommand, request.json)
     else:
         app.state_manager.set('is_beacon_running', request.json['enabled'])
 
     return api_response(request.json)
 
-@app.route('/modem/ping_ping', methods=['POST'])
+@app.route('/freedata_server/ping_ping', methods=['POST'])
 def post_ping():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for controlling PING via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     validate(request.json, 'dxcall', validations.validate_freedata_callsign)
     enqueue_tx_command(command_ping.PingCommand, request.json)
     return api_ok()
 
-@app.route('/modem/send_test_frame', methods=['POST'])
+@app.route('/freedata_server/send_test_frame', methods=['POST'])
 def post_send_test_frame():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for triggering a TEST_FRAME via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     enqueue_tx_command(command_test.TestCommand)
     return api_ok()
 
-@app.route('/modem/fec_transmit', methods=['POST'])
+@app.route('/freedata_server/fec_transmit', methods=['POST'])
 def post_send_fec_frame():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for triggering a FEC frame via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     enqueue_tx_command(command_feq.FecCommand, request.json)
     return api_ok()
 
-@app.route('/modem/fec_is_writing', methods=['POST'])
+@app.route('/freedata_server/fec_is_writing', methods=['POST'])
 def post_send_fec_is_writing():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for triggering a IS WRITING frame via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     #server_commands.modem_fec_is_writing(request.json)
     return 'Not implemented yet'
 
-@app.route('/modem/start', methods=['POST'])
+@app.route('/freedata_server/start', methods=['POST'])
 def post_modem_start():
     if request.method not in ['POST']:
-        return api_response({"info": "endpoint for STARTING modem via POST"})
+        return api_response({"info": "endpoint for STARTING freedata_server via POST"})
     print("start received...")
     app.modem_service.put("start")
     return api_response(request.json)
 
-@app.route('/modem/stop', methods=['POST'])
+@app.route('/freedata_server/stop', methods=['POST'])
 def post_modem_stop():
     if request.method not in ['POST']:
-        return api_response({"info": "endpoint for STOPPING modem via POST"})
+        return api_response({"info": "endpoint for STOPPING freedata_server via POST"})
     print("stop received...")
 
     app.modem_service.put("stop")
     return api_ok()
 
 @app.route('/version', methods=['GET'])
 def get_modem_version():
     return api_response({"version": app.MODEM_VERSION})
 
-@app.route('/modem/send_arq_raw', methods=['POST'])
+@app.route('/freedata_server/send_arq_raw', methods=['POST'])
 def post_modem_send_raw():
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for SENDING RAW DATA via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
     if app.state_manager.check_if_running_arq_session():
         api_abort('Modem busy', 503)
     if enqueue_tx_command(command_arq_raw.ARQRawCommand, request.json):
         return api_response(request.json)
     else:
         api_abort('Error executing command...', 500)
-@app.route('/modem/stop_transmission', methods=['POST'])
+@app.route('/freedata_server/stop_transmission', methods=['POST'])
 def post_modem_send_raw_stop():
 
     if request.method not in ['POST']:
         return api_response({"info": "endpoint for SENDING a STOP command via POST"})
     if not app.state_manager.is_modem_running:
         api_abort('Modem not running', 503)
 
@@ -337,42 +337,42 @@
             app.socket_interface_manager.stop_servers()
 
         if app.service_manager.modem:
             app.service_manager.modem.sd_input_stream.stop
         audio.sd._terminate()
     except Exception as e:
         print(e)
-        print("Error stopping modem")
+        print("Error stopping freedata_server")
     time.sleep(1)
     print('Server shutdown...')
     print("------------------------------------------")
 
 def main():
     app.config['SOCK_SERVER_OPTIONS'] = {'ping_interval': 10}
     # define global MODEM_VERSION
     app.MODEM_VERSION = MODEM_VERSION
 
     config_file = set_config()
     app.config_manager = CONFIG(config_file)
 
-    # start modem
+    # start freedata_server
     app.p2p_data_queue = queue.Queue() # queue which holds processing data of p2p connections
     app.state_queue = queue.Queue()  # queue which holds latest states
     app.modem_events = queue.Queue()  # queue which holds latest events
     app.modem_fft = queue.Queue()  # queue which holds latest fft data
-    app.modem_service = queue.Queue()  # start / stop modem service
+    app.modem_service = queue.Queue()  # start / stop freedata_server service
     app.event_manager = event_manager.EventManager([app.modem_events])  # TODO remove the app.modem_event custom queue
     # init state manager
     app.state_manager = state_manager.StateManager(app.state_queue)
     # initialize message system schedule manager
     app.schedule_manager = ScheduleManager(app.MODEM_VERSION, app.config_manager, app.state_manager, app.event_manager)
     # start service manager
     app.service_manager = service_manager.SM(app)
 
-    # start modem service
+    # start freedata_server service
     app.modem_service.put("start")
     # initialize database default values
     DatabaseManager(app.event_manager).initialize_default_values()
     wsm.startThreads(app)
 
     conf = app.config_manager.read()
     modemaddress = conf['NETWORK']['modemaddress']
```

### Comparing `freedata-server-0.15.3/modem/service_manager.py` & `freedata_server-0.15.4/freedata_server/service_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,38 +58,38 @@
                 self.config = self.app.config_manager.read()
                 self.start_radio_manager()
 
                 if self.start_modem():
                     self.event_manager.modem_restarted()
 
             else:
-                self.log.warning("[SVC] modem command processing failed", cmd=cmd, state=self.state_manager.is_modem_running)
+                self.log.warning("[SVC] freedata_server command processing failed", cmd=cmd, state=self.state_manager.is_modem_running)
 
 
     def start_modem(self):
 
         if self.config['STATION']['mycall'] in ['XX1XXX']:
             self.log.warning("wrong callsign in config! interrupting startup")
             return False
 
         if self.state_manager.is_modem_running:
-            self.log.warning("modem already running")
+            self.log.warning("freedata_server already running")
             return False
 
 
         # test audio devices
         audio_test = self.test_audio()
 
         if False in audio_test or None in audio_test or self.state_manager.is_modem_running:
-            self.log.warning("starting modem failed", input_test=audio_test[0], output_test=audio_test[1])
+            self.log.warning("starting freedata_server failed", input_test=audio_test[0], output_test=audio_test[1])
             self.state_manager.set("is_modem_running", False)
             self.event_manager.modem_failed()
             return False
 
-        self.log.info("starting modem....")
+        self.log.info("starting freedata_server....")
         self.modem = modem.RF(self.config, self.event_manager, self.modem_fft, self.modem_service, self.state_manager, self.app.radio_manager)
 
         self.frame_dispatcher = frame_dispatcher.DISPATCHER(self.config, 
                                                             self.event_manager,
                                                             self.state_manager,
                                                             self.modem)
         self.frame_dispatcher.start()
@@ -98,15 +98,15 @@
         self.state_manager.set("is_modem_running", True)
         self.modem.start_modem()
         self.schedule_manager.start(self.modem)
 
         return True
         
     def stop_modem(self):
-        self.log.info("stopping modem....")
+        self.log.info("stopping freedata_server....")
         del self.modem
         self.modem = False
         self.state_manager.set("is_modem_running", False)
         self.schedule_manager.stop()
         self.event_manager.modem_stopped()
 
     def test_audio(self):
```

### Comparing `freedata-server-0.15.3/modem/socket_interface.py` & `freedata_server-0.15.4/freedata_server/socket_interface.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/socket_interface_commands.py` & `freedata_server-0.15.4/freedata_server/socket_interface_commands.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/state_manager.py` & `freedata_server-0.15.4/freedata_server/state_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self, statequeue):
 
         # state related settings
         self.statequeue = statequeue
         self.newstate = None
         self.last = time.time()
 
-        # modem related states
+        # freedata_server related states
         # not every state is needed to publish, yet
         # TODO can we reduce them?
         self.channel_busy_slot = [False, False, False, False, False]
         self.channel_busy_event = threading.Event()
         self.channel_busy_condition_traffic = threading.Event()
         self.channel_busy_condition_codec2 = threading.Event()
```

### Comparing `freedata-server-0.15.3/modem/stats.py` & `freedata_server-0.15.4/freedata_server/stats.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/tci.py` & `freedata_server-0.15.4/freedata_server/tci.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/modem/websocket_manager.py` & `freedata_server-0.15.4/freedata_server/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `freedata-server-0.15.3/setup.py` & `freedata_server-0.15.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='freedata-server',
-    version='0.15.3',
+    name='freedata_server',
+    version='0.15.4',
     packages=find_packages(where='.'),
     package_dir={'': '.'},
     install_requires=required,
     python_requires='>=3.9',
     author='DJ2LS',
     author_email='dj2ls@proton.me',
     description='A free, open-source, multi-platform application for sending files and messages, using the codec2 HF modems.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://freedata.app',
     license='GPL3.0',
     entry_points={
         'console_scripts': [
-            'freedata-server=modem.server:main',  # Points to the main() function in server.py
+            'freedata_server=freedata_server.server:main',  # Points to the main() function in server.py
         ],
     },
     include_package_data=True,  # Ensure non-python files are included if specified
     package_data={
-        # Include all files under any directory within the 'modem' package
-        'modem': ['lib/**/*'],  # Recursive include for all files in 'lib' and its subdirectories
+        # Include all files under any directory within the 'freedata_server' package
+        'freedata_server': ['lib/**/*'],  # Recursive include for all files in 'lib' and its subdirectories
     },
 )
```

