# Comparing `tmp/freedata_server-0.15.4.tar.gz` & `tmp/freedata-server-0.15.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedata_server-0.15.4.tar", last modified: Thu Apr 18 09:06:46 2024, max compression
+gzip compressed data, was "freedata-server-0.15.4a1.tar", last modified: Thu Apr 18 09:15:19 2024, max compression
```

## Comparing `freedata_server-0.15.4.tar` & `freedata-server-0.15.4a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.661859 freedata_server-0.15.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 09:06:16.000000 freedata_server-0.15.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 09:06:46.661859 freedata_server-0.15.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 09:06:16.000000 freedata_server-0.15.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.653859 freedata_server-0.15.4/freedata_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/api_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_data_type_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session_irs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/arq_session_iss.py
--rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    24041 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/codec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_arq_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_cq.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_feq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_message_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_qrv.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/cw.py
--rw-r--r--   0 runner    (1001) docker     (127)    20305 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/data_frame_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/demodulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_arq_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_cq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/frame_handler_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    24901 2024-04-18 09:06:16.000000 freedata_server-0.15.4/freedata_server/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.645859 freedata_server-0.15.4/freedata_server/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.657859 freedata_server-0.15.4/freedata_server/lib/codec2/
--rw-r--r--   0 runner    (1001) docker     (127)  2264619 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.dll
--rwxr-xr-x   0 runner    (1001) docker     (127)  2206856 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.so
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/maidenhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    27414 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_p2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/message_system_db_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modem.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modem_frametypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/modulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/p2p_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/radio_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/rigctld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/rigdummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/schedule_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/selftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/serial_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/socket_interface_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/tci.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 09:06:17.000000 freedata_server-0.15.4/freedata_server/websocket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:06:46.661859 freedata_server-0.15.4/freedata_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:06:46.000000 freedata_server-0.15.4/freedata_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:06:46.661859 freedata_server-0.15.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 09:06:17.000000 freedata_server-0.15.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:19.176136 freedata-server-0.15.4a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 09:15:19.176136 freedata-server-0.15.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:19.168136 freedata-server-0.15.4a1/freedata_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/api_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/arq_data_type_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/arq_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/arq_session_irs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/arq_session_iss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24041 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/codec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_arq_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_feq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_message_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_qrv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20305 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/data_frame_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/demodulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler_arq_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler_cq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler_p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/frame_handler_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24901 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:19.160136 freedata-server-0.15.4a1/freedata_server/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:19.172136 freedata-server-0.15.4a1/freedata_server/lib/codec2/
+-rw-r--r--   0 runner    (1001) docker     (127)  2264619 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/lib/codec2/libcodec2.dll
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2206856 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/lib/codec2/libcodec2.so
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/maidenhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27414 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_p2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_system_db_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_system_db_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_system_db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_system_db_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/message_system_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/modem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/modem_frametypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/modulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/p2p_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/radio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/rigctld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/rigdummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/schedule_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/selftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/serial_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/socket_interface_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/tci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/freedata_server/websocket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:19.176136 freedata-server-0.15.4a1/freedata_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 09:15:19.000000 freedata-server-0.15.4a1/freedata_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:15:19.176136 freedata-server-0.15.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-18 09:14:48.000000 freedata-server-0.15.4a1/setup.py
```

### Comparing `freedata_server-0.15.4/LICENSE` & `freedata-server-0.15.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/PKG-INFO` & `freedata-server-0.15.4a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freedata_server
-Version: 0.15.4
+Name: freedata-server
+Version: 0.15.4a1
 Summary: A free, open-source, multi-platform application for sending files and messages, using the codec2 HF modems.
 Home-page: https://freedata.app
 Author: DJ2LS
 Author-email: dj2ls@proton.me
 License: GPL3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freedata_server-0.15.4/README.md` & `freedata-server-0.15.4a1/README.md`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/api_validations.py` & `freedata-server-0.15.4a1/freedata_server/api_validations.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/arq_data_type_handler.py` & `freedata-server-0.15.4a1/freedata_server/arq_data_type_handler.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/arq_session.py` & `freedata-server-0.15.4a1/freedata_server/arq_session.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/arq_session_irs.py` & `freedata-server-0.15.4a1/freedata_server/arq_session_irs.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/arq_session_iss.py` & `freedata-server-0.15.4a1/freedata_server/arq_session_iss.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/audio.py` & `freedata-server-0.15.4a1/freedata_server/audio.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/codec2.py` & `freedata-server-0.15.4a1/freedata_server/codec2.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command.py` & `freedata-server-0.15.4a1/freedata_server/command.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_arq_raw.py` & `freedata-server-0.15.4a1/freedata_server/command_arq_raw.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_beacon.py` & `freedata-server-0.15.4a1/freedata_server/command_beacon.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_feq.py` & `freedata-server-0.15.4a1/freedata_server/command_feq.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_message_send.py` & `freedata-server-0.15.4a1/freedata_server/command_message_send.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_p2p_connection.py` & `freedata-server-0.15.4a1/freedata_server/command_p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/command_ping.py` & `freedata-server-0.15.4a1/freedata_server/command_ping.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/config.py` & `freedata-server-0.15.4a1/freedata_server/config.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/cw.py` & `freedata-server-0.15.4a1/freedata_server/cw.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/data_frame_factory.py` & `freedata-server-0.15.4a1/freedata_server/data_frame_factory.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/demodulator.py` & `freedata-server-0.15.4a1/freedata_server/demodulator.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/event_manager.py` & `freedata-server-0.15.4a1/freedata_server/event_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/explorer.py` & `freedata-server-0.15.4a1/freedata_server/explorer.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_dispatcher.py` & `freedata-server-0.15.4a1/freedata_server/frame_dispatcher.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler_arq_session.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler_arq_session.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler_beacon.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler_beacon.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler_cq.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler_cq.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler_p2p_connection.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler_p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/frame_handler_ping.py` & `freedata-server-0.15.4a1/freedata_server/frame_handler_ping.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/helpers.py` & `freedata-server-0.15.4a1/freedata_server/helpers.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.dll` & `freedata-server-0.15.4a1/freedata_server/lib/codec2/libcodec2.dll`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/lib/codec2/libcodec2.so` & `freedata-server-0.15.4a1/freedata_server/lib/codec2/libcodec2.so`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/log_handler.py` & `freedata-server-0.15.4a1/freedata_server/log_handler.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/maidenhead.py` & `freedata-server-0.15.4a1/freedata_server/maidenhead.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/mesh.py` & `freedata-server-0.15.4a1/freedata_server/mesh.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_p2p.py` & `freedata-server-0.15.4a1/freedata_server/message_p2p.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_system_db_attachments.py` & `freedata-server-0.15.4a1/freedata_server/message_system_db_attachments.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_system_db_beacon.py` & `freedata-server-0.15.4a1/freedata_server/message_system_db_beacon.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_system_db_manager.py` & `freedata-server-0.15.4a1/freedata_server/message_system_db_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_system_db_messages.py` & `freedata-server-0.15.4a1/freedata_server/message_system_db_messages.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/message_system_db_model.py` & `freedata-server-0.15.4a1/freedata_server/message_system_db_model.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/modem.py` & `freedata-server-0.15.4a1/freedata_server/modem.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/modem_frametypes.py` & `freedata-server-0.15.4a1/freedata_server/modem_frametypes.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/modulator.py` & `freedata-server-0.15.4a1/freedata_server/modulator.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/p2p_connection.py` & `freedata-server-0.15.4a1/freedata_server/p2p_connection.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/radio_manager.py` & `freedata-server-0.15.4a1/freedata_server/radio_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/rigctld.py` & `freedata-server-0.15.4a1/freedata_server/rigctld.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/rigdummy.py` & `freedata-server-0.15.4a1/freedata_server/rigdummy.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/schedule_manager.py` & `freedata-server-0.15.4a1/freedata_server/schedule_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/selftest.py` & `freedata-server-0.15.4a1/freedata_server/selftest.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/serial_ports.py` & `freedata-server-0.15.4a1/freedata_server/serial_ports.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/server.py` & `freedata-server-0.15.4a1/freedata_server/server.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/service_manager.py` & `freedata-server-0.15.4a1/freedata_server/service_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/socket_interface.py` & `freedata-server-0.15.4a1/freedata_server/socket_interface.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/socket_interface_commands.py` & `freedata-server-0.15.4a1/freedata_server/socket_interface_commands.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/state_manager.py` & `freedata-server-0.15.4a1/freedata_server/state_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/stats.py` & `freedata-server-0.15.4a1/freedata_server/stats.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/tci.py` & `freedata-server-0.15.4a1/freedata_server/tci.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server/websocket_manager.py` & `freedata-server-0.15.4a1/freedata_server/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/freedata_server.egg-info/PKG-INFO` & `freedata-server-0.15.4a1/freedata_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedata-server
-Version: 0.15.4
+Version: 0.15.4a1
 Summary: A free, open-source, multi-platform application for sending files and messages, using the codec2 HF modems.
 Home-page: https://freedata.app
 Author: DJ2LS
 Author-email: dj2ls@proton.me
 License: GPL3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `freedata_server-0.15.4/freedata_server.egg-info/SOURCES.txt` & `freedata-server-0.15.4a1/freedata_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freedata_server-0.15.4/setup.py` & `freedata-server-0.15.4a1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='freedata_server',
-    version='0.15.4',
+    name='freedata-server',
+    version='0.15.4a1',
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
-            'freedata_server=freedata_server.server:main',  # Points to the main() function in server.py
+            'freedata-server=freedata_server.server:main',  # Points to the main() function in server.py
         ],
     },
     include_package_data=True,  # Ensure non-python files are included if specified
     package_data={
         # Include all files under any directory within the 'freedata_server' package
         'freedata_server': ['lib/**/*'],  # Recursive include for all files in 'lib' and its subdirectories
     },
```

