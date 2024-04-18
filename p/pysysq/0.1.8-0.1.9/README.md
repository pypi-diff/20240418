# Comparing `tmp/pysysq-0.1.8.tar.gz` & `tmp/pysysq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysysq-0.1.8.tar", last modified: Thu Apr 18 13:57:30 2024, max compression
+gzip compressed data, was "pysysq-0.1.9.tar", last modified: Thu Apr 18 14:34:42 2024, max compression
```

## Comparing `pysysq-0.1.8.tar` & `pysysq-0.1.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.712205 pysysq-0.1.8/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.8/.gitignore
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.8/LICENSE
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-18 13:57:30.712205 pysysq-0.1.8/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.8/PysysQ.ipynb
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.8/README.md
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.8/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-18 13:57:25.000000 pysysq-0.1.8/pyproject.toml
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.8/requirements.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-18 13:57:30.712205 pysysq-0.1.8/setup.cfg
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.700205 pysysq-0.1.8/src/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.8/src/pysysq/__main__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      467 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq/_version.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/logging.conf
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_clock/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_clock/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_clock/sq_clock.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_event/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_event/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event_manager.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_factory/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_factory/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_factory/sq_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_filter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_filter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_filter/sq_filter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_logger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_logger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_logger/sq_logger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_merger/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_merger/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1584 2024-04-16 15:12:25.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_merger/sq_merger.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1981 2024-04-16 15:12:25.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7174 2024-04-18 13:57:25.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_object.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_packet/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       68 2024-04-15 18:02:36.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_packet/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_packet/sq_metadata.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      104 2024-04-15 19:03:53.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_packet/sq_packet.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.704205 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1683 2024-04-17 14:17:55.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      524 2024-04-17 14:20:02.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      762 2024-04-17 06:49:25.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3279 2024-04-06 20:39:45.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1101 2024-04-01 14:56:54.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1326 2024-04-01 14:56:54.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      787 2024-04-01 14:56:54.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_sink/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_sink/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1181 2024-04-15 17:58:00.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2748 2024-04-17 13:59:38.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      221 2024-04-15 19:03:53.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      974 2024-04-17 13:46:30.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/sq_helper.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/sq_plugin.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_queue/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_queue/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      383 2024-04-15 17:58:00.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_queue/sq_queue.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_queue/sq_single_queue.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/config/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/templates/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_simulator/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_simulator/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_simulator/sq_simulator.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_splitter/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_splitter/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_splitter/sq_splitter.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2506 2024-04-17 14:24:02.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/sq_plotter.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/sq_statistics.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.8/src/pysysq/sq_base/sq_time_base.py
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.712205 pysysq-0.1.8/src/pysysq.egg-info/
--rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq.egg-info/PKG-INFO
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3797 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq.egg-info/SOURCES.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq.egg-info/dependency_links.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq.egg-info/requires.txt
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-18 13:57:30.000000 pysysq-0.1.8/src/pysysq.egg-info/top_level.txt
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.700205 pysysq-0.1.8/tests/
-drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 13:57:30.708205 pysysq-0.1.8/tests/unittests/
--rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.8/tests/unittests/__init__.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2794 2024-04-15 19:40:28.000000 pysysq-0.1.8/tests/unittests/test_sq_demux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     2705 2024-04-15 19:40:28.000000 pysysq-0.1.8/tests/unittests/test_sq_mux.py
--rw-rw-r--   0 ajith     (1000) ajith     (1000)     3040 2024-04-15 19:52:19.000000 pysysq-0.1.8/tests/unittests/test_sq_splitter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.417098 pysysq-0.1.9/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3113 2024-03-31 20:14:07.000000 pysysq-0.1.9/.gitignore
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1073 2024-03-31 20:14:07.000000 pysysq-0.1.9/LICENSE
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-18 14:34:42.417098 pysysq-0.1.9/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)   607908 2024-03-31 20:14:07.000000 pysysq-0.1.9/PysysQ.ipynb
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     9238 2024-04-06 20:27:59.000000 pysysq-0.1.9/README.md
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-04-01 14:12:34.000000 pysysq-0.1.9/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1403 2024-04-18 14:34:36.000000 pysysq-0.1.9/pyproject.toml
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-03-31 20:14:07.000000 pysysq-0.1.9/requirements.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       38 2024-04-18 14:34:42.417098 pysysq-0.1.9/setup.cfg
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.401098 pysysq-0.1.9/src/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.405098 pysysq-0.1.9/src/pysysq/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      188 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      493 2024-03-31 20:20:58.000000 pysysq-0.1.9/src/pysysq/__main__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      467 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq/_version.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2138 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/logging.conf
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.405098 pysysq-0.1.9/src/pysysq/sq_base/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      475 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_clock/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       30 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_clock/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1117 2024-04-06 09:26:43.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_clock/sq_clock.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_event/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      127 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_event/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      843 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1965 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event_manager.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1183 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_factory/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       81 2024-04-06 10:06:37.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_factory/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1973 2024-04-06 13:21:28.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_factory/sq_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      443 2024-04-06 20:59:49.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_factory/sq_helper_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_filter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-04-01 14:12:25.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_filter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1446 2024-04-01 22:28:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_filter/sq_filter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_logger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       32 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_logger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      892 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_logger/sq_logger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_merger/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       31 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_merger/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1584 2024-04-16 15:12:25.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_merger/sq_merger.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       59 2024-04-06 10:07:28.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2168 2024-04-01 22:28:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1981 2024-04-16 15:12:25.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/sq_mux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7174 2024-04-18 13:57:25.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_object.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_packet/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       68 2024-04-15 18:02:36.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_packet/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      132 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_packet/sq_metadata.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      104 2024-04-15 19:03:53.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_packet/sq_packet.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       44 2024-04-06 10:07:36.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1683 2024-04-17 14:17:55.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      250 2024-04-01 14:46:29.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      410 2024-04-06 20:36:42.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      616 2024-04-01 14:46:29.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      524 2024-04-17 14:20:02.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      762 2024-04-17 06:49:25.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.409098 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       48 2024-04-06 10:07:43.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3027 2024-04-18 14:26:27.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       96 2024-04-06 20:39:45.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      886 2024-04-18 14:34:11.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1297 2024-04-18 14:30:55.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      594 2024-04-18 14:28:30.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      470 2024-04-01 14:56:54.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_processor_state.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      729 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_sink/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       34 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_sink/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1181 2024-04-15 17:58:00.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       77 2024-04-01 22:28:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       87 2024-04-06 20:59:49.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2670 2024-04-18 14:24:48.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      221 2024-04-15 19:03:53.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/sq_generic_packet.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      157 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/sq_packet_info.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      955 2024-04-18 14:24:22.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/sq_helper.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      112 2024-04-06 10:04:40.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/sq_plugin.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      632 2024-04-06 20:59:49.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_queue/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       73 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_queue/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      383 2024-04-15 17:58:00.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_queue/sq_queue.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1826 2024-04-01 20:12:38.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_queue/sq_single_queue.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       43 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/__init__.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/config/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2856 2024-04-06 20:08:42.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1961 2024-04-06 20:14:46.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1461 2024-04-06 10:02:05.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     7114 2024-04-06 20:08:42.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      312 2024-04-06 10:02:05.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_model.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1669 2024-04-06 10:02:05.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/templates/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1901 2024-04-06 13:11:59.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_simulator/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       37 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_simulator/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1330 2024-04-01 20:12:38.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_simulator/sq_simulator.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_splitter/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       36 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_splitter/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1517 2024-04-01 20:12:38.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_splitter/sq_splitter.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.413098 pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)       74 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2506 2024-04-17 14:24:02.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/sq_plotter.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     1172 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/sq_statistics.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      431 2024-03-31 20:14:07.000000 pysysq-0.1.9/src/pysysq/sq_base/sq_time_base.py
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.417098 pysysq-0.1.9/src/pysysq.egg-info/
+-rw-r--r--   0 ajith     (1000) ajith     (1000)    11852 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq.egg-info/PKG-INFO
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3797 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        1 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)      384 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq.egg-info/requires.txt
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        7 2024-04-18 14:34:42.000000 pysysq-0.1.9/src/pysysq.egg-info/top_level.txt
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.405098 pysysq-0.1.9/tests/
+drwxrwxr-x   0 ajith     (1000) ajith     (1000)        0 2024-04-18 14:34:42.417098 pysysq-0.1.9/tests/unittests/
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)        0 2024-03-31 20:14:07.000000 pysysq-0.1.9/tests/unittests/__init__.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2794 2024-04-15 19:40:28.000000 pysysq-0.1.9/tests/unittests/test_sq_demux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     2705 2024-04-15 19:40:28.000000 pysysq-0.1.9/tests/unittests/test_sq_mux.py
+-rw-rw-r--   0 ajith     (1000) ajith     (1000)     3040 2024-04-15 19:52:19.000000 pysysq-0.1.9/tests/unittests/test_sq_splitter.py
```

### Comparing `pysysq-0.1.8/.gitignore` & `pysysq-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/LICENSE` & `pysysq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/PKG-INFO` & `pysysq-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.8
+Version: 0.1.9
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.8/PysysQ.ipynb` & `pysysq-0.1.9/PysysQ.ipynb`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/README.md` & `pysysq-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/pyproject.toml` & `pysysq-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pysysq"
-version = "0.1.8"
+version = "0.1.9"
 authors =[
     {name = "Ajith Padman", email = "ajith.padman@gmail.com"}
 ]
 description= "A system functional flow simulation framework using Queuing Theory"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
```

### Comparing `pysysq-0.1.8/src/pysysq/logging.conf` & `pysysq-0.1.9/src/pysysq/logging.conf`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_clock/sq_clock.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_clock/sq_clock.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event_manager.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event_manager.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_event/sq_event_queue.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_event/sq_event_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_factory/sq_factory.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_factory/sq_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_filter/sq_filter.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_filter/sq_filter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_logger/sq_logger.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_logger/sq_logger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_merger/sq_merger.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_merger/sq_merger.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/sq_demux.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/sq_demux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_mux_demux/sq_mux.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_mux_demux/sq_mux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_object.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_object.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/sq_pkt_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_generator_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_gen_state.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_gen/states/sq_pkt_generator_queuing_state.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/sq_pkt_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,10 @@
         super().process_packet(evt)
         if evt.owner is self.clk:
             self.tick += 1
             self._state.process_packet(evt)
         else:
             self.logger.warning(f'{self.name} Ignoring Event {evt.data}')
 
-    def update_progress(self):
-        progress = (self.tick - self.start_tick) / self.processing_time * 100
-        progress_metadata = SQMetadata(name='progress', owner=self.name, value=progress)
-        self.data_indication(data=progress_metadata)
-
     def process_data(self, evt: SQEvent):
         super().process_data(evt)
         self.helper.process_data(evt.data, self.tick)
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_complete.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 
 class SQPktProcStateComplete(SQPktProcState):
     def process_packet(self, evt: SQEvent):
         self.owner.no_of_processed_pkts += 1
         self.owner.total_processing_time += self.owner.processing_time
         self.owner.avg_processing_time = self.owner.total_processing_time / self.owner.no_of_processed_pkts
         self.owner.load = self.owner.total_processing_time / self.owner.tick * 100
-        metadata = self.owner.helper.process_packet(self.owner.curr_pkt, self.owner.tick)
-        self.owner.update_progress()
-        if metadata is not None:
-            self.owner.data_indication(data=metadata)
-
         self.owner.logger.info(f'{self.owner.name} Packet {self.owner.curr_pkt} Processing Complete after ticks '
                                f'{self.owner.tick}')
         self.owner.output_queue.push(self.owner.curr_pkt)
         self.owner.finish_indication()
         self.owner.set_state(self.factory.create_state('IDLE', owner=self.owner))
 
     def get_state_name(self):
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_idle.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
     def process_packet(self, evt: SQEvent):
         self.owner.curr_pkt = self.owner.input_queue.pop()
         self.owner.start_tick = self.owner.tick
         if self.owner.curr_pkt is None:
             self.owner.logger.info(f'{self.owner.name} No Packet to Process')
         else:
+
             self.owner.pkt_size_sum += self.owner.curr_pkt.size
             self.owner.pkt_size_average = self.owner.pkt_size_sum / (self.owner.no_of_processed_pkts + 1)
             self.owner.processing_time = self.owner.helper.get_processing_cycles(self.owner.curr_pkt)
-            metadata = self.owner.helper.process_packet(self.owner.curr_pkt, self.owner.tick)
-            self.owner.update_progress()
-            if metadata is not None:
-                self.owner.data_indication(data=metadata)
-
             self.owner.logger.info(f'{self.owner.name} Start Processing Packet '
                                    f'{self.owner.curr_pkt} Expected processing time '
-                                   f'{self.owner.processing_time} current Tick {self.owner.tick}')
-            self.owner.set_state(self.factory.create_state('PROCESSING', owner=self.owner))
+                                   f'{self.owner.processing_time} ')
+            status = self.owner.helper.process_packet(self.owner.curr_pkt, self.owner.tick)
+            if status:
+                self.owner.set_state(self.factory.create_state('COMPLETE', owner=self.owner))
+            else:
+                self.owner.set_state(self.factory.create_state('PROCESSING', owner=self.owner))
 
     def get_state_name(self):
         return f'IDLE'
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_pkt_proc_processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from .sq_pkt_processor_state import SQPktProcState
 from ...sq_event import SQEvent
 
 
 class SQPktProcStateProcessing(SQPktProcState):
     def process_packet(self, evt: SQEvent):
-        metadata = self.owner.helper.process_packet(self.owner.curr_pkt, self.owner.tick)
-        if metadata is not None:
-            self.owner.data_indication(data=metadata)
-        self.owner.update_progress()
-        self.owner.logger.info(f'{self.owner.name} Continue Processing Packet '
-                               f'{self.owner.curr_pkt} Time {self.owner.tick}')
-        if self.owner.tick - self.owner.start_tick >= self.owner.processing_time - 2:
+        status = self.owner.helper.process_packet(self.owner.curr_pkt, self.owner.tick)
+
+        if status:
             self.owner.set_state(self.factory.create_state('COMPLETE', owner=self.owner))
+        else:
+            self.owner.logger.info(f'{self.owner.name} Continue Processing Packet '
+                                   f'{self.owner.curr_pkt}')
 
     def get_state_name(self):
         return f'PROCESSING'
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_processor/states/sq_state_factory.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_pkt_sink/sq_pkt_sink.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/default/sq_default_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,19 +35,19 @@
                                   priority=pkt_priority,
                                   timestamp=SQTimeBase.get_current_sim_time())
 
     def get_processing_cycles(self, pkt: SQPacket) -> int:
         np.random.seed(pkt.size)
         return np.random.randint(1, 10)
 
-    def process_packet(self, pkt: SQPacket, tick: int) -> Union[SQMetadata, None]:
+    def process_packet(self, pkt: SQPacket, tick: int) -> bool:
         self.owner.logger.info(f'Processing packet {pkt} at tick {tick}')
         if tick < self.get_processing_cycles(pkt):
-            return None
-        return SQMetadata(name='tick_count', owner=self.owner.name, value=tick)
+            return False
+        return True
 
     def filter_packet(self, pkt: SQPacket) -> bool:
         return True
 
     def process_data(self, data: SQEvent, tick: int):
         self.owner.logger.info(f'Consuming Metadata {data}')
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/sq_helper.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/sq_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         pass
 
     @abstractmethod
     def get_processing_cycles(self, pkt: SQPacket) -> int:
         pass
 
     @abstractmethod
-    def process_packet(self, pkt: SQPacket, tick: int) -> Union[SQMetadata, None]:
+    def process_packet(self, pkt: SQPacket, tick: int) -> bool:
         pass
 
     @abstractmethod
     def filter_packet(self, pkt: SQPacket) -> bool:
         pass
 
     @abstractmethod
```

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_plugin/sq_plugin_loader.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_queue/sq_single_queue.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_queue/sq_single_queue.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/config/input.json`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_code_gen_model.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_ctx.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_data_gen_strategy.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/sq_sim_setup_gen.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2` & `pysysq-0.1.9/src/pysysq/sq_base/sq_sim_setup_generator/templates/sim_setup.py.j2`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_simulator/sq_simulator.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_simulator/sq_simulator.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_splitter/sq_splitter.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_splitter/sq_splitter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/sq_plotter.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/sq_plotter.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq/sq_base/sq_statistics/sq_statistics.py` & `pysysq-0.1.9/src/pysysq/sq_base/sq_statistics/sq_statistics.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/src/pysysq.egg-info/PKG-INFO` & `pysysq-0.1.9/src/pysysq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysysq
-Version: 0.1.8
+Version: 0.1.9
 Summary: A system functional flow simulation framework using Queuing Theory
 Author-email: Ajith Padman <ajith.padman@gmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Ajith Padman]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysysq-0.1.8/src/pysysq.egg-info/SOURCES.txt` & `pysysq-0.1.9/src/pysysq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/tests/unittests/test_sq_demux.py` & `pysysq-0.1.9/tests/unittests/test_sq_demux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/tests/unittests/test_sq_mux.py` & `pysysq-0.1.9/tests/unittests/test_sq_mux.py`

 * *Files identical despite different names*

### Comparing `pysysq-0.1.8/tests/unittests/test_sq_splitter.py` & `pysysq-0.1.9/tests/unittests/test_sq_splitter.py`

 * *Files identical despite different names*

