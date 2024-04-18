# Comparing `tmp/gotrackit-0.2.0.tar.gz` & `tmp/gotrackit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.2.0.tar", last modified: Fri Apr 12 07:59:26 2024, max compression
+gzip compressed data, was "gotrackit-0.2.1.tar", last modified: Thu Apr 18 13:37:55 2024, max compression
```

## Comparing `gotrackit-0.2.0.tar` & `gotrackit-0.2.1.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.428638 gotrackit-0.2.0/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4886 2024-04-12 07:59:26.427641 gotrackit-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4140 2024-04-12 07:45:08.000000 gotrackit-0.2.0/README.md
--rw-rw-rw-   0        0        0      795 2024-04-12 03:50:07.000000 gotrackit-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 07:59:26.428638 gotrackit-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.339875 gotrackit-0.2.0/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.345859 gotrackit-0.2.0/src/gotrackit/
--rw-rw-rw-   0        0        0    15398 2024-04-04 05:30:17.000000 gotrackit-0.2.0/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0    11426 2024-04-12 07:23:48.000000 gotrackit-0.2.0/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.0/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.0/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.351843 gotrackit-0.2.0/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.0/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.0/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.354836 gotrackit-0.2.0/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4291 2024-04-10 08:42:29.000000 gotrackit-0.2.0/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     8007 2024-04-12 03:06:11.000000 gotrackit-0.2.0/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0    21814 2024-04-11 02:47:55.000000 gotrackit-0.2.0/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.360824 gotrackit-0.2.0/src/gotrackit/map/
--rw-rw-rw-   0        0        0    19202 2024-04-11 02:00:49.000000 gotrackit-0.2.0/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    23292 2024-04-11 01:53:49.000000 gotrackit-0.2.0/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.0/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.362814 gotrackit-0.2.0/src/gotrackit/model/
--rw-rw-rw-   0        0        0    52888 2024-04-12 02:40:08.000000 gotrackit-0.2.0/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.367801 gotrackit-0.2.0/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.0/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    26881 2024-04-12 03:06:11.000000 gotrackit-0.2.0/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.368798 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.377774 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.378772 gotrackit-0.2.0/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.380766 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.382760 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.390740 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.393736 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.397720 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.401710 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.403705 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.410686 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.412680 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.413678 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.415672 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     5765 2024-04-12 02:47:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.0/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.0/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.417668 gotrackit-0.2.0/src/gotrackit/netxfer/
--rw-rw-rw-   0        0        0    17197 2024-03-31 15:04:35.000000 gotrackit-0.2.0/src/gotrackit/netxfer/SumoConvert.py
--rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.0/src/gotrackit/netxfer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.418665 gotrackit-0.2.0/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9181 2024-04-03 02:13:18.000000 gotrackit-0.2.0/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.425646 gotrackit-0.2.0/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.0/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.0/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.0/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.0/src/gotrackit/tools/group.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.0/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0     5360 2024-04-04 06:01:58.000000 gotrackit-0.2.0/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.426643 gotrackit-0.2.0/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     4886 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3666 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.916367 gotrackit-0.2.1/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4833 2024-04-18 13:37:55.915368 gotrackit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4087 2024-04-18 13:20:15.000000 gotrackit-0.2.1/README.md
+-rw-rw-rw-   0        0        0      795 2024-04-18 13:35:20.000000 gotrackit-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:37:55.916367 gotrackit-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.807293 gotrackit-0.2.1/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.812836 gotrackit-0.2.1/src/gotrackit/
+-rw-rw-rw-   0        0        0    15660 2024-04-18 05:53:17.000000 gotrackit-0.2.1/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    11926 2024-04-18 13:10:23.000000 gotrackit-0.2.1/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.1/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.1/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.817859 gotrackit-0.2.1/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.1/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.1/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.829264 gotrackit-0.2.1/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4259 2024-04-18 12:43:12.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8007 2024-04-14 02:50:11.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0     3888 2024-04-16 14:22:42.000000 gotrackit-0.2.1/src/gotrackit/gps/GpsXfer.py
+-rw-rw-rw-   0        0        0    22376 2024-04-18 06:27:36.000000 gotrackit-0.2.1/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.831283 gotrackit-0.2.1/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    19341 2024-04-18 02:38:44.000000 gotrackit-0.2.1/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    23345 2024-04-18 12:46:18.000000 gotrackit-0.2.1/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.1/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.835290 gotrackit-0.2.1/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    55598 2024-04-18 13:18:05.000000 gotrackit-0.2.1/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.841865 gotrackit-0.2.1/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.1/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    26881 2024-04-12 03:06:11.000000 gotrackit-0.2.1/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.845738 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.849740 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.853738 gotrackit-0.2.1/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.857739 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.862703 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.869965 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.875968 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.882864 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.889779 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.889779 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.897275 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.898273 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.900268 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.902413 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5765 2024-04-12 02:47:41.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.1/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.1/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.1/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.904216 gotrackit-0.2.1/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-04-16 10:06:45.000000 gotrackit-0.2.1/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.1/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.905960 gotrackit-0.2.1/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9181 2024-04-03 02:13:18.000000 gotrackit-0.2.1/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.1/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.912248 gotrackit-0.2.1/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.1/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.1/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.1/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.1/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.1/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0     9708 2024-04-18 13:24:10.000000 gotrackit-0.2.1/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:37:55.914372 gotrackit-0.2.1/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     4833 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3695 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-18 13:37:55.000000 gotrackit-0.2.1/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.2.0/LICENSE` & `gotrackit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/PKG-INFO` & `gotrackit-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,62 +30,62 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**04.12已更新: v0.2.0**
+**04.18已更新: v0.2.1**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
+- 地图匹配接口移除geo_res_fldr, geojson文件和html存储在一个目录下，指定html_fldr即可，以及增加其他存储参数(见文档)
 
-- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
+- HTML文件中新增警告路段信息，若该次匹配中出现警告, 则在HTML文件中会多一个图层，该图层记录了GPS状态转移出错的路段
 
-- 增加GPS点停留点识别功能
+- 停留点识别功能改进
 
-- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
+- BUG修复
 
-- 增加依据GPS数据提取带途径点OD的功能
 
-- 增加了路网处理函数：路段、节点重塑
-
-- 修复了部分BUG
+遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
 
-遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
+稀疏轨迹匹配与路径补全：
 
 <div align="center">
-    <img src="docs/_static/images/l_f.gif" />
+    <img src="docs/_static/images/极稀疏轨迹匹配.gif" />
 </div>
 
+
 <div align="center">
-    <img src="docs/_static/images/m_h_f.gif" />
+    <img src="docs/_static/images/匹配动画样例3.gif" />
 </div>
 
-稀疏轨迹增密匹配：
+
+常规匹配：
 
 <div align="center">
-    <img src="docs/_static/images/dense_gps.gif" />
+    <img src="docs/_static/images/匹配动画样例1.gif" />
 </div>
 
-
 <div align="center">
-    <img src="docs/_static/images/taxi_xishu.gif" />
+    <img src="docs/_static/images/匹配动画样例2.gif" />
 </div>
 
 
 <div align="center">
-    <img src="docs/_static/images/xa_sample.gif" />
+    <img src="docs/_static/images/匹配动画样例4.gif" />
 </div>
 
 
-![car_gps.png](docs/_static/images/wxq.jpg)
-
+用户交流群：
+<div align="center">
+    <img src="docs/_static/images/wxq.jpg" />
+</div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
 **数据无忧**
 - 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
@@ -115,16 +115,14 @@
 - networkx(3.2.1)
 - pandas(2.0.3)
 - numpy(1.26.2)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
-geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
-
 #### __使用pip安装__
 
 安装：
 
 ``` shell
 pip install -i https://pypi.org/simple/ gotrackit
 ```
```

### Comparing `gotrackit-0.2.0/README.md` & `gotrackit-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,62 +8,62 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**04.12已更新: v0.2.0**
+**04.18已更新: v0.2.1**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
+- 地图匹配接口移除geo_res_fldr, geojson文件和html存储在一个目录下，指定html_fldr即可，以及增加其他存储参数(见文档)
 
-- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
+- HTML文件中新增警告路段信息，若该次匹配中出现警告, 则在HTML文件中会多一个图层，该图层记录了GPS状态转移出错的路段
 
-- 增加GPS点停留点识别功能
+- 停留点识别功能改进
 
-- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
+- BUG修复
 
-- 增加依据GPS数据提取带途径点OD的功能
 
-- 增加了路网处理函数：路段、节点重塑
-
-- 修复了部分BUG
+遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
 
-遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
+稀疏轨迹匹配与路径补全：
 
 <div align="center">
-    <img src="docs/_static/images/l_f.gif" />
+    <img src="docs/_static/images/极稀疏轨迹匹配.gif" />
 </div>
 
+
 <div align="center">
-    <img src="docs/_static/images/m_h_f.gif" />
+    <img src="docs/_static/images/匹配动画样例3.gif" />
 </div>
 
-稀疏轨迹增密匹配：
+
+常规匹配：
 
 <div align="center">
-    <img src="docs/_static/images/dense_gps.gif" />
+    <img src="docs/_static/images/匹配动画样例1.gif" />
 </div>
 
-
 <div align="center">
-    <img src="docs/_static/images/taxi_xishu.gif" />
+    <img src="docs/_static/images/匹配动画样例2.gif" />
 </div>
 
 
 <div align="center">
-    <img src="docs/_static/images/xa_sample.gif" />
+    <img src="docs/_static/images/匹配动画样例4.gif" />
 </div>
 
 
-![car_gps.png](docs/_static/images/wxq.jpg)
-
+用户交流群：
+<div align="center">
+    <img src="docs/_static/images/wxq.jpg" />
+</div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
 **数据无忧**
 - 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
@@ -93,16 +93,14 @@
 - networkx(3.2.1)
 - pandas(2.0.3)
 - numpy(1.26.2)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
-geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
-
 #### __使用pip安装__
 
 安装：
 
 ``` shell
 pip install -i https://pypi.org/simple/ gotrackit
 ```
```

### Comparing `gotrackit-0.2.0/pyproject.toml` & `gotrackit-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.2.0/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.1/src/gotrackit/GlobalVal.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 
         self.DENSE_GEO = '__dens_geo__'
         self.N_SEGMENTS = '__n__'
 
         self.DIFF_VEC = 'diff_vec'
 
 
+class RouteField(object):
+    """"""
+    def __init__(self):
+        self.PATH_ID_FIELD = 'path_id'
+        self.TIME_COST_FIELD = 'time_cost'
+        self.SEQ_FIELD = 'seq'
+        self.O_TIME_FIELD = 'o_time'
+
+
 class MarkovField(object):
     """HMM模型字段"""
     def __init__(self):
         self.FROM_STATE = 'from_state'
         self.TO_STATE = 'to_state'
         self.FROM_SEQ = 'from_seq'
         self.TO_SEQ = 'to_seq'
@@ -378,14 +387,15 @@
                 "radiusField": None,
                 "radiusScale": "linear"
             }
         }
 
         self.BASE_LINK_NAME = 'base_link'
         self.BASE_NODE_NAME = 'base_node'
+        self.ERROR_XFER = 'error_xfer'
         self.MIX_NAME = 'mix'
         self.GPS_NAME = 'gps'
         self.MATCH_LINK_NAME = 'match_link'
     def get_base_config(self):
         return copy.deepcopy(self.__BASE_CONFIG)
 
     def get_polygon_config(self):
```

### Comparing `gotrackit-0.2.0/src/gotrackit/MapMatch.py` & `gotrackit-0.2.1/src/gotrackit/MapMatch.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 
 import numpy as np
 import pandas as pd
 from .map.Net import Net
 from .gps.LocGps import GpsPointsGdf
 from .model.Markov import HiddenMarkov
 from .GlobalVal import NetField, GpsField
-from .visualization import VisualizationCombination
+from .visualization import export_visualization
 
 gps_field = GpsField()
 net_field = NetField()
-agent_if_field = gps_field.AGENT_ID_FIELD
+agent_id_field = gps_field.AGENT_ID_FIELD
 node_id_field = net_field.NODE_ID_FIELD
 
 
 class MapMatch(object):
     def __init__(self, flag_name: str = 'test', net: Net = None, use_sub_net: bool = True, gps_df: pd.DataFrame = None,
                  time_format: str = "%Y-%m-%d %H:%M:%S", time_unit: str = 's',
                  gps_buffer: float = 100, gps_route_buffer_gap: float = 25.0,
                  max_increment_times: int = 2, increment_buffer: float = 20.0,
                  beta: float = 20.0, gps_sigma: float = 20.0, dis_para: float = 0.1,
                  is_lower_f: bool = False, lower_n: int = 2,
                  use_heading_inf: bool = False, heading_para_array: np.ndarray = None,
-                 dense_gps: bool = True, dense_interval: float = 50.0,
-                 dwell_l_length: float = 10.0, dwell_n: int = 3, del_dwell: bool = True,
+                 dense_gps: bool = True, dense_interval: float = 80.0,
+                 dwell_l_length: float = 10.0, dwell_n: int = 2, del_dwell: bool = True,
                  dup_threshold: float = 10.0,
                  is_rolling_average: bool = False, window: int = 2,
                  export_html: bool = False, use_gps_source: bool = False, html_fldr: str = None,
-                 export_geo_res: bool = False, geo_res_fldr: str = None,
+                 export_geo_res: bool = False,
                  node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0, multi_core: bool = True,
                  core_num: int = 1, link_width: float = 1.5, node_radius: float = 1.5,
-                 match_link_width: float = 5.0, gps_radius: float = 6.0):
+                 match_link_width: float = 5.0, gps_radius: float = 6.0, export_all_agents: bool = False,
+                 visualization_cache_times: int = 50, multi_core_save: bool = False):
         """
-
         :param flag_name: 标记字符名称, 会用于标记输出的可视化文件, 默认"test"
         :param net: gotrackit路网对象, 必须指定
         :param use_sub_net: 是否在子网络上进行计算, 默认True
         :param gps_df: GPS数据, 必须指定
         :param time_format: GPS数据中时间列的格式, 默认"%Y-%m-%d %H:%M:%S"
         :param time_unit: GPS数据中时间列的单位, 如果时间列是数值(秒或者毫秒), 默认's'
         :param gps_buffer: GPS的搜索半径, 单位米, 意为只选取每个gps_buffer点附近100米范围内的路段作为候选路段, 默认100.0
@@ -59,20 +59,22 @@
         :param dup_threshold: 利用GPS轨迹计算sub_net时, 先对GPS点原始轨迹做简化, 重复点检测阈值, 默认5m
         :param is_rolling_average: 是否启用滑动窗口平均对GPS数据进行降噪, 默认False
         :param window: 滑动窗口大小, 默认2
         :param export_html: 是否输出网页可视化结果html文件, 默认True
         :param use_gps_source: 是否在可视化结果中使用GPS源数据进行展示, 默认False
         :param html_fldr: 保存网页可视化结果的文件目录, 默认当前目录
         :param export_geo_res: 是否输出匹配结果的几何可视化文件, 默认False
-        :param geo_res_fldr: 存储几何可视化文件的目录, 默认当前目录
         :param node_num_threshold: 默认2000
         :param omitted_l: 当某GPS点与前后GPS点的平均距离小于该距离(m)时, 该GPS点的方向限制作用被取消
         :param multi_core: 是否启用多核匹配, 默认True
         :param core_num: 用几个核, 默认1
         :param gps_radius: HTML可视化中GPS点的半径大小，单位米，默认8米
+        :param export_all_agents: 是否将所有agent的可视化存储于一个html文件中
+        :param visualization_cache_times: 每匹配完几辆车再进行结果的统一存储, 默认50
+        :param multi_core_save: 是否启用多进程进行结果存储
         """
         # 坐标系投影
         self.plain_crs = net.planar_crs
         self.geo_crs = net.geo_crs
 
         # 用于自动确定是否使用全局路网的指标
         self.node_num_threshold = node_num_threshold
@@ -105,15 +107,14 @@
         self.beta = beta  # 状态转移概率参数, 概率与之成正比
         self.gps_sigma = gps_sigma  # 发射概率参数, 概率与之成正比
         self.flag_name = flag_name
         self.dis_para = dis_para
 
         self.export_html = export_html
         self.export_geo_res = export_geo_res
-        self.geo_res_fldr = geo_res_fldr
         self.html_fldr = html_fldr
 
         self.may_error_list = dict()
 
         self.my_net = net
         self.not_conn_cost = self.my_net.not_conn_cost
         self.use_gps_source = use_gps_source
@@ -123,25 +124,31 @@
 
         # 网页可视化参数
         self.link_width = link_width
         self.node_radius = node_radius
         self.match_link_width = match_link_width
         self.gps_radius = gps_radius
 
-    def execute(self):
+        self.export_all_agents = export_all_agents
+        self.visualization_cache_times = visualization_cache_times
+        self.multi_core_save = multi_core_save
 
+    def execute(self):
         match_res_df = pd.DataFrame()
+        hmm_res_list = []  # save hmm_res
         if len(self.my_net.get_node_data()[node_id_field].unique()) <= self.node_num_threshold:
             self.use_sub_net = False
-
+        self.gps_df.dropna(subset=[agent_id_field], inplace=True)
+        agent_num = len(self.gps_df[gps_field.AGENT_ID_FIELD].unique())
+        if agent_num == 0:
+            raise ValueError('去除agent_id列空值行后, gps数据为空...')
         # 对每辆车的轨迹进行匹配
+        agent_count = 0
         for agent_id, _gps_df in self.gps_df.groupby(gps_field.AGENT_ID_FIELD):
-            file_name = '-'.join([self.flag_name, str(agent_id)])
-            print(rf'agent: {agent_id}')
-            _gps_df.reset_index(inplace=True, drop=True)
+            print(rf'- gotrackit ------> agent: {agent_id} ')
             gps_obj = GpsPointsGdf(gps_points_df=_gps_df, time_format=self.time_format,
                                    buffer=self.gps_buffer, time_unit=self.time_unit,
                                    plane_crs=self.plain_crs,
                                    max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
                                    dense_gps=self.dense_gps, dense_interval=self.dense_interval,
                                    dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n)
             del _gps_df
@@ -179,31 +186,26 @@
                                    top_k=self.top_k, omitted_l=self.omitted_l, multi_core=self.multi_core,
                                    core_num=self.core_num)
 
             # 求解参数
             hmm_obj.generate_markov_para()
             hmm_obj.solve()
             _match_res_df = hmm_obj.acquire_res()
+            hmm_obj.format_war_info()
             if hmm_obj.is_warn:
-                self.may_error_list[agent_id] = hmm_obj.warn_info
-
-            if self.export_geo_res:
-                hmm_obj.acquire_geo_res(out_fldr=self.geo_res_fldr,
-                                        flag_name=file_name)
-
+                self.may_error_list[agent_id] = hmm_obj.format_warn_info
             match_res_df = pd.concat([match_res_df, _match_res_df])
+            agent_count += 1
+
+            # if export files
+            if self.export_html or self.export_geo_res:
+                hmm_res_list.append(hmm_obj)
+                if len(hmm_res_list) >= self.visualization_cache_times or agent_count == agent_num:
+                    export_visualization(hmm_obj_list=hmm_res_list, use_gps_source=self.use_gps_source,
+                                         export_geo=self.export_geo_res, export_html=self.export_html,
+                                         gps_radius=self.gps_radius, export_all_agents=self.export_all_agents,
+                                         out_fldr=self.html_fldr, flag_name=self.flag_name,
+                                         multi_core_save=self.multi_core_save)
+                    del hmm_res_list
+                    hmm_res_list = []
 
-            if self.export_html:
-                # 4.初始化一个匹配结果管理器
-                vc = VisualizationCombination(use_gps_source=self.use_gps_source)
-                vc.collect_hmm(hmm_obj)
-                try:
-                    vc.visualization(zoom=15, out_fldr=self.html_fldr,
-                                     file_name=file_name, link_width=self.link_width,
-                                     node_radius=self.node_radius, match_link_width=self.match_link_width,
-                                     gps_radius=self.gps_radius)
-                except Exception as e:
-                    print(repr(e))
-                    print(rf'输出HTML可视化文件, 出现某些错误, 输出失败...')
-                del vc
-        match_res_df.reset_index(inplace=True, drop=True)
         return match_res_df, self.may_error_list
```

### Comparing `gotrackit-0.2.0/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.1/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.1/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.1/src/gotrackit/gps/GpsArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
         self.gps_points_gdf[gps_field.GEOMETRY_FIELD] = self.gps_points_gdf.apply(
             lambda item: Point(item[gps_field.LNG_FIELD], item[gps_field.LAT_FIELD]), axis=1)
         self.gps_points_gdf = gpd.GeoDataFrame(self.gps_points_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                                crs=self.geo_crs)
         try:
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
-        except Exception as e:
-            print(repr(e))
+        except ValueError:
             self.gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
         self.gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
 
         # 存储最原始的GPS信息
```

### Comparing `gotrackit-0.2.0/src/gotrackit/gps/GpsTrip.py` & `gotrackit-0.2.1/src/gotrackit/gps/GpsTrip.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.1/src/gotrackit/gps/LocGps.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,27 +67,28 @@
         self.increment_buffer = increment_buffer
         self.dense_gps = dense_gps
         self.dense_interval = dense_interval
         self.max_increment_times = 1 if max_increment_times <= 0 else max_increment_times
         self.dwell_l_length = dwell_l_length
         self.dwell_n = dwell_n
         self.__gps_point_dis_dict = dict()
+        gps_points_df.reset_index(inplace=True, drop=True)
         self.__gps_points_gdf = gps_points_df
+        self.agent_id = self.__gps_points_gdf.at[0, gps_field.AGENT_ID_FIELD]
         self.check()
         if gps_field.HEADING_FIELD not in self.__gps_points_gdf.columns:
             self.__gps_points_gdf[gps_field.HEADING_FIELD] = 0.0
         self.__gps_points_gdf[gps_field.GEOMETRY_FIELD] = self.__gps_points_gdf.apply(
             lambda item: Point(item[gps_field.LNG_FIELD], item[gps_field.LAT_FIELD]), axis=1)
         self.__gps_points_gdf = gpd.GeoDataFrame(self.__gps_points_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                                  crs=self.geo_crs)
         try:
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], format=time_format)
-        except Exception as e:
-            print(repr(e))
+        except ValueError:
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
         self.__gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
         self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
@@ -95,14 +96,15 @@
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.__gps_points_gdf.copy()
 
         self.done_diff_heading = False
 
     def check(self):
+        assert len(self.__gps_points_gdf) > 1, f'agent: {self.agent_id} GPS样本数据不足两个...'
         assert {gps_field.LNG_FIELD, gps_field.LAT_FIELD,
                 gps_field.AGENT_ID_FIELD, gps_field.TIME_FIELD}.issubset(
             set(self.__gps_points_gdf.columns)), \
             rf'GPS数据字段有误, 请至少包含如下字段: {gps_field.AGENT_ID_FIELD, gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD}'
 
     def dense(self):
 
@@ -402,33 +404,42 @@
     def del_dwell_points(self) -> None:
         # add field = dis_gap_field
         self.calc_adj_dis_gap()
         self.__gps_points_gdf['dwell_label'] = \
             (self.__gps_points_gdf[dis_gap_field] > self.dwell_l_length).astype(int)
 
         self.__gps_points_gdf = self.del_consecutive_zero(df=self.__gps_points_gdf, col='dwell_label', n=self.dwell_n)
-        self.__gps_points_gdf.drop(columns=[sub_group_field], axis=1, inplace=True)
+        try:
+            self.__gps_points_gdf.drop(columns=[sub_group_field], axis=1, inplace=True)
+        except KeyError:
+            pass
 
     @staticmethod
     def del_consecutive_zero(df: pd.DataFrame or gpd.GeoDataFrame = None,
-                             col: str = None, n: int = 3) -> pd.DataFrame or gpd.GeoDataFrame:
+                             col: str = None, n: int = 3,
+                             del_all_dwell: bool = True) -> pd.DataFrame or gpd.GeoDataFrame:
         """
         标记超过连续n行为0的行, 并且只保留最后一行
         :param df:
         :param col:
         :param n:
+        :param del_all_dwell
         :return:
         """
         m = df[col].ne(0)
         df['__del__'] = (df.groupby(m.cumsum())[col]
                          .transform('count').gt(n + 1)
                          & (~m)
                          )
-        df['__a__'] = df['__del__'].ne(1).cumsum()
-        df['__cut__'] = df['__a__'] & df['__del__']
-        df.drop_duplicates(subset=['__a__'], keep='last', inplace=True)
-        df[sub_group_field] = df['__cut__'].ne(0).cumsum()
-        df.drop(columns=['__del__', '__a__', '__cut__'], axis=1, inplace=True)
+        if del_all_dwell:
+            df.drop(index=df[df['__del__']].index, inplace=True, axis=0)
+            df.drop(columns=['__del__'], axis=1, inplace=True)
+        else:
+            df['__a__'] = df['__del__'].ne(1).cumsum()
+            df['__cut__'] = df['__a__'] & df['__del__']
+            df.drop_duplicates(subset=['__a__'], keep='last', inplace=True)
+            df[sub_group_field] = df['__cut__'].ne(0).cumsum()
+            df.drop(columns=['__del__', '__a__', '__cut__'], axis=1, inplace=True)
         return df
```

### Comparing `gotrackit-0.2.0/src/gotrackit/map/Link.py` & `gotrackit-0.2.1/src/gotrackit/map/Link.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,21 @@
         self.__single_link_gdf.set_index(net_field.SINGLE_LINK_ID_FIELD, inplace=True)
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = list(self.__single_link_gdf.index)
 
     def renew_length(self):
         _idx = list(self.link_gdf.index)[0]
         length_a, length_b = \
             self.link_gdf.at[_idx, net_field.GEOMETRY_FIELD].length, self.link_gdf.at[_idx, net_field.LENGTH_FIELD]
-        if 0.8 <= length_a / length_b <= 1.2:
-            return None
-        self.link_gdf[length_field] = self.link_gdf.apply(lambda row: row[geometry_field].length, axis=1)
+        if isinstance(length_a, (gpd.GeoSeries, pd.Series)):
+            if 0.8 <= max(length_a / length_b) <= 1.2:
+                return None
+        else:
+            if 0.8 <= length_a / length_b <= 1.2:
+                return None
+        self.link_gdf[length_field] = self.link_gdf[geometry_field].length
 
     def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None):
         """通过给定的single_link_gdf初始化link, 用在子net的初始化上"""
         self.__single_link_gdf = single_link_gdf.copy()
         self.__double_single_mapping = {single_link_id: (link_id, int(direction), f, t) for
                                         single_link_id, link_id, direction, f, t in
                                         zip(self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD],
```

### Comparing `gotrackit-0.2.0/src/gotrackit/map/Net.py` & `gotrackit-0.2.1/src/gotrackit/map/Net.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,18 @@
                                not_conn_cost=self.not_conn_cost)
         else:
             self.__link = Link(link_gdf=link_gdf, weight_field=self.weight_field, is_check=is_check,
                                planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
                                not_conn_cost=self.not_conn_cost)
         self.__planar_crs = self.__node.planar_crs
         self.to_plane_prj()
-        self.__link.renew_length()
+        try:
+            self.__link.renew_length()
+        except:
+            pass
         if not init_from_existing:
             if create_single:
                 self.__link.init_link()
         else:
             if create_single:
                 self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf)
         if not init_from_existing:
```

### Comparing `gotrackit-0.2.0/src/gotrackit/map/Node.py` & `gotrackit-0.2.1/src/gotrackit/map/Node.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/model/Markov.py` & `gotrackit-0.2.1/src/gotrackit/model/Markov.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,42 +55,41 @@
         self.gps_sigma = gps_sigma
         self.__emission_mat_dict = dict()
         self.__solver = None
         self.index_state_list = None
         self.gps_match_res_gdf = None
         # {(from_seq, to_seq): pd.DataFrame()}
         self.__s2s_route_l = dict()
-        self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf = None, None, None
+        self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf, self.__may_error = None, None, None, None
         self.path_cost_df = pd.DataFrame()
         self.is_warn = False
         self.not_conn_cost = not_conn_cost
         self.use_heading_inf = use_heading_inf
         if heading_para_array is None:
-            self.heading_para_array = np.array([1.0, 1.0, 1.0, 0.1, 0.00001, 0.00001, 0.00001, 0.000001, 0.000001])
+            self.heading_para_array = np.array([1.0, 1.0, 1.0, 0.1, 0.0001, 0.0001, 0.00001, 0.000001, 0.000001])
         else:
             self.heading_para_array = heading_para_array
         self.angle_slice = 180 / len(self.heading_para_array)
         self.dis_para = dis_para
-        self.warn_info = list()
+        self.warn_info = {'from_ft': [], 'to_ft': []}
+        self.format_warn_info = pd.DataFrame()
         self.top_k = top_k
         self.omitted_l = omitted_l
         self.multi_core = multi_core
         self.core_num = int(core_num) if int(core_num) <= os.cpu_count() else os.cpu_count()
         self.gps_candidate_link = None
 
+    @function_time_cost
     def generate_markov_para(self):
-
-        # self.__generate_markov_para()
         if self.multi_core and self.core_num >= 1:
             self.__generate_transition_mat_alpha_multi()
         else:
             self.__generate_transition_mat()
         self.__generate_emission_mat()
 
-    @function_time_cost
     def __generate_transition_mat(self):
 
         # 计算 初步候选
         seq_list = self.__generate_candidates()
 
         self.gps_points.calc_gps_point_dis()
         # _ = pd.DataFrame()
@@ -132,15 +131,14 @@
 
             self.__ft_transition_dict[seq_list[i]] = transition_mat
             self.__ft_mapping_dict[seq_list[i]] = f_mapping
             self.__ft_mapping_dict[seq_list[i + 1]] = t_mapping
 
         # print(_)
 
-    @function_time_cost
     def __generate_emission_mat(self):
 
         # 计算每个观测点的生成概率, 这是在计算状态转移概率之后, 已经将关联不到的GPS点删除了
         # 这里的向量是候选路段的投影点的方向向量
         emission_p_df = pd.DataFrame(self.__done_prj_dict).T.reset_index(drop=False).rename(
             columns={'level_0': gps_field.POINT_SEQ_FIELD, 'level_1': net_field.SINGLE_LINK_ID_FIELD,
                      1: markov_field.PRJ_L, 4: net_field.LINK_VEC_FIELD})[
@@ -233,18 +231,16 @@
 
         # 使用viterbi模型求解
         self.__solver = Viterbi(observation_list=self.gps_points.used_observation_seq_list,
                                 o_mat_dict=self.__emission_mat_dict,
                                 t_mat_dict=self.__ft_transition_dict, use_log_p=use_lop_p)
         self.__solver.init_model()
         self.index_state_list = self.__solver.iter_model()
+        # print(self.index_state_list)
 
-        print(self.index_state_list)
-
-    @function_time_cost
     def __generate_transition_mat_alpha_multi(self):
         n = self.core_num
 
         # 计算 初步候选, 经过这一步, 实际匹配用到的GPS点已经完全确定
         # 得到self.gps_candidate_link
         seq_list = self.__generate_candidates()
 
@@ -587,15 +583,15 @@
         """
         if (gps_seq, single_link_id) in self.__done_prj_dict.keys():
             # already calculated
             (prj_p, prj_dis, route_dis, l_length, p_vec) = self.__done_prj_dict[
                 (gps_seq, single_link_id)]
         else:
             # new calc and cache
-            print('# new calc and cache')
+            # print('# new calc and cache')
             (prj_p, prj_dis, route_dis, l_length, p_vec) = self.get_gps_prj_info(
                 target_link_id=single_link_id,
                 gps_seq=gps_seq)
             self.__done_prj_dict.update(
                 {(gps_seq, single_link_id): (prj_p, prj_dis, route_dis, l_length, p_vec)})
         return prj_p, prj_dis, route_dis, l_length, p_vec
 
@@ -748,21 +744,28 @@
 
             next_from_node, next_to_node = int(gps_link_state_df.at[i + 1, net_field.FROM_NODE_FIELD]), \
                 int(gps_link_state_df.at[i + 1, net_field.TO_NODE_FIELD])
 
             if ((now_from_node, now_to_node) == (next_from_node, next_to_node)) or now_to_node == next_from_node:
                 pass
             else:
+                pre_seq = int(gps_link_state_df.at[i, gps_field.POINT_SEQ_FIELD])
+                next_seq = int(gps_link_state_df.at[i + 1, gps_field.POINT_SEQ_FIELD])
                 if ft_state in self.__adj_seq_path_dict.keys():
-                    pre_seq = int(gps_link_state_df.at[i, gps_field.POINT_SEQ_FIELD])
-                    next_seq = int(gps_link_state_df.at[i + 1, gps_field.POINT_SEQ_FIELD])
+                    # pre_seq = int(gps_link_state_df.at[i, gps_field.POINT_SEQ_FIELD])
+                    # next_seq = int(gps_link_state_df.at[i + 1, gps_field.POINT_SEQ_FIELD])
                     node_seq = self.__adj_seq_path_dict[ft_state]
                     if node_seq[1] != now_to_node:
-                        warnings.warn(rf'相邻link状态不连通...ft:{(now_from_node, now_to_node)} -> ft:{(next_from_node, next_to_node)}, 可能是GPS太稀疏或者路网本身不连通')
-                        self.warn_info.append([(now_from_node, now_to_node), (next_from_node, next_to_node)])
+                        warnings.warn(
+                            rf'gps seq: {pre_seq} -> {next_seq} 状态转移出现问题, from_link:{(now_from_node, now_to_node)} -> to_link:{(next_from_node, next_to_node)}')
+                        # self.warn_info.append([(now_from_node, now_to_node), (next_from_node, next_to_node)])
+                        self.warn_info['from_ft'].append(
+                            (ft_state[0], now_from_node, now_to_node, rf'seq:{pre_seq}-{next_seq}'))
+                        self.warn_info['to_ft'].append(
+                            (ft_state[1], next_from_node, next_to_node, rf'seq:{pre_seq}-{next_seq}'))
                         _single_link_list = [ft_node_link_mapping[(node_seq[i], node_seq[i + 1])] for i in
                                              range(0, len(node_seq) - 1)]
                     else:
                         _single_link_list = [ft_node_link_mapping[(node_seq[i], node_seq[i + 1])] for i in
                                              range(1, len(node_seq) - 1)]
 
                     omitted_gps_state_item += [
@@ -780,16 +783,21 @@
                     pre_seq_time, next_seq_time = gps_match_res_gdf.at[pre_seq, gps_field.TIME_FIELD], \
                         gps_match_res_gdf.at[next_seq, gps_field.TIME_FIELD]
                     dt = (next_seq_time - pre_seq_time).total_seconds() / (len(omitted_gps_points) + 1)
                     omitted_gps_points_time.extend(
                         [pre_seq_time + timedelta(seconds=dt * n) for n in range(1, len(_single_link_list) + 1)])
                 else:
                     self.is_warn = True
-                    warnings.warn(rf'相邻link状态不连通...ft:{(now_from_node, now_to_node)} -> ft:{(next_from_node, next_to_node)}, 可能是GPS太稀疏或者路网本身不连通')
-                    self.warn_info.append([(now_from_node, now_to_node), (next_from_node, next_to_node)])
+                    warnings.warn(
+                        rf'gps seq: {pre_seq} -> {next_seq} 状态转移出现问题, from_link:{(now_from_node, now_to_node)} -> to_link:{(next_from_node, next_to_node)}')
+                    # self.warn_info.append([(now_from_node, now_to_node), (next_from_node, next_to_node)])
+                    self.warn_info['from_ft'].append(
+                        (ft_state[0], now_from_node, now_to_node, rf'seq:{pre_seq}-{next_seq}'))
+                    self.warn_info['to_ft'].append(
+                        (ft_state[1], next_from_node, next_to_node, rf'seq:{pre_seq}-{next_seq}'))
 
         omitted_gps_state_df = pd.DataFrame(omitted_gps_state_item, columns=[gps_field.POINT_SEQ_FIELD,
                                                                              net_field.SINGLE_LINK_ID_FIELD,
                                                                              gps_field.SUB_SEQ_FIELD,
                                                                              net_field.LINK_ID_FIELD,
                                                                              net_field.DIRECTION_FIELD,
                                                                              net_field.FROM_NODE_FIELD,
@@ -799,19 +807,21 @@
         omitted_gps_state_df[gps_field.TIME_FIELD] = omitted_gps_points_time
         omitted_gps_state_df[net_field.GEOMETRY_FIELD] = [Point(loc) for loc in omitted_gps_points]
 
         return omitted_gps_state_df
 
     def acquire_visualization_res(self, use_gps_source: bool = False,
                                   link_width: float = 1.5, node_radius: float = 1.5,
-                                  match_link_width: float = 5.0, gps_radius: float = 3.0) -> tuple[
-                                        gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
+                                  match_link_width: float = 5.0, gps_radius: float = 3.0) -> tuple[gpd.GeoDataFrame,
+                                  gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
         """获取可视化结果"""
         if self.__plot_mix_gdf is None:
+            # print('初次计算')
             single_link_gdf = self.net.get_link_data()
+            single_link_gdf.reset_index(inplace=True, drop=True)
             node_gdf = self.net.get_node_data()
             net_crs = self.net.crs
             plain_crs = self.net.planar_crs
             is_geo_crs = self.net.is_geo_crs()
             double_link_geo = {l: geo for l, geo in zip(single_link_gdf[net_field.LINK_ID_FIELD],
                                                         single_link_gdf[net_field.GEOMETRY_FIELD])}
 
@@ -829,56 +839,79 @@
                                              gps_field.LAT_FIELD, gps_field.TIME_FIELD,
                                              gps_field.GEOMETRY_FIELD]].copy()
 
             # GPS点转化为circle polygon
             plot_gps_gdf.drop(columns=[gps_field.LNG_FIELD, gps_field.LAT_FIELD], axis=1, inplace=True)
             if plot_gps_gdf.crs != plain_crs:
                 plot_gps_gdf = plot_gps_gdf.to_crs(plain_crs)
-            plot_gps_gdf[net_field.GEOMETRY_FIELD] = \
-                plot_gps_gdf[net_field.GEOMETRY_FIELD].apply(lambda p: p.buffer(gps_radius))
+            plot_gps_gdf[net_field.GEOMETRY_FIELD] = plot_gps_gdf[net_field.GEOMETRY_FIELD].buffer(gps_radius)
             plot_gps_gdf[gps_field.TYPE_FIELD] = 'gps'
 
             # 匹配路段GDF
             plot_match_link_gdf = self.gps_match_res_gdf.copy()
             plot_match_link_gdf.drop(columns=[markov_field.PRJ_GEO], axis=1, inplace=True)
             plot_match_link_gdf[gps_field.TYPE_FIELD] = 'link'
             plot_match_link_gdf[net_field.GEOMETRY_FIELD] = plot_match_link_gdf[net_field.LINK_ID_FIELD].apply(
                 lambda x: double_link_geo[x])
             plot_match_link_gdf.crs = net_crs
             plot_match_link_gdf.drop_duplicates(subset=net_field.LINK_ID_FIELD, keep='first', inplace=True)
             plot_match_link_gdf.reset_index(drop=True, inplace=True)
             if is_geo_crs:
                 plot_match_link_gdf = plot_match_link_gdf.to_crs(plain_crs)
-            plot_match_link_gdf[net_field.GEOMETRY_FIELD] = plot_match_link_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda l: l.buffer(match_link_width))
+            plot_match_link_gdf[net_field.GEOMETRY_FIELD] = \
+                plot_match_link_gdf[net_field.GEOMETRY_FIELD].buffer(match_link_width)
             plot_match_link_gdf.drop(columns=[gps_field.LNG_FIELD, gps_field.LAT_FIELD], axis=1, inplace=True)
 
             plot_gps_gdf = plot_gps_gdf.to_crs(self.net.geo_crs)
             plot_match_link_gdf = plot_match_link_gdf.to_crs(self.net.geo_crs)
             gps_link_gdf = pd.concat([plot_gps_gdf, plot_match_link_gdf])
             gps_link_gdf.reset_index(inplace=True, drop=True)
 
+            # 错误信息
+            may_error_gdf = gpd.GeoDataFrame()
+            if self.format_warn_info.empty:
+                pass
+            else:
+                self.format_warn_info[['from_single', 'to_single', 'ft_gps']] = self.format_warn_info.apply(
+                    lambda row: (row['from_ft'][0], row['to_ft'][0], row['from_ft'][3]),
+                    axis=1, result_type='expand')
+                format_warn_df = pd.concat([self.format_warn_info[['from_single', 'ft_gps']].rename(
+                    columns={'from_single': net_field.SINGLE_LINK_ID_FIELD}),
+                                            self.format_warn_info[['to_single', 'ft_gps']].rename(
+                                                columns={'to_single': net_field.SINGLE_LINK_ID_FIELD})])
+                format_warn_df.reset_index(inplace=True, drop=True)
+                may_error_gdf = pd.merge(format_warn_df,
+                                         single_link_gdf, on=net_field.SINGLE_LINK_ID_FIELD, how='left')
+                may_error_gdf = gpd.GeoDataFrame(may_error_gdf, geometry=net_field.GEOMETRY_FIELD,
+                                                 crs=single_link_gdf.crs.srs)
+
             # 路网底图
             origin_link_gdf = single_link_gdf.drop_duplicates(subset=[net_field.LINK_ID_FIELD], keep='first').copy()
+            del single_link_gdf
             if is_geo_crs:
                 origin_link_gdf = origin_link_gdf.to_crs(plain_crs)
                 node_gdf = node_gdf.to_crs(plain_crs)
-            origin_link_gdf[net_field.GEOMETRY_FIELD] = origin_link_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda x: x.buffer(link_width))
-            node_gdf[net_field.GEOMETRY_FIELD] = node_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda x: x.buffer(node_radius))
+                may_error_gdf = may_error_gdf.to_crs(plain_crs)
+            origin_link_gdf[net_field.GEOMETRY_FIELD] = origin_link_gdf[net_field.GEOMETRY_FIELD].buffer(link_width)
+            node_gdf[net_field.GEOMETRY_FIELD] = node_gdf[net_field.GEOMETRY_FIELD].buffer(node_radius)
+
+            if not may_error_gdf.empty:
+                may_error_gdf[net_field.GEOMETRY_FIELD] = may_error_gdf[net_field.GEOMETRY_FIELD].buffer(link_width)
 
             origin_link_gdf = origin_link_gdf.to_crs(self.net.geo_crs)
+            if not may_error_gdf.empty:
+                may_error_gdf = may_error_gdf.to_crs(self.net.geo_crs)
             node_gdf = node_gdf.to_crs(self.net.geo_crs)
 
-            self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf = gps_link_gdf, origin_link_gdf, node_gdf
-            return gps_link_gdf, origin_link_gdf, node_gdf
-
+            self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf, self.__may_error = \
+                gps_link_gdf, origin_link_gdf, node_gdf, may_error_gdf
+            return gps_link_gdf, origin_link_gdf, node_gdf, may_error_gdf
         else:
-            return self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf
+            # print('利用重复值')
+            return self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf, self.__may_error
 
     def acquire_geo_res(self, out_fldr: str = None, flag_name: str = 'flag'):
         """获取矢量结果文件, 可以在qgis中可视化"""
         out_fldr = r'./' if out_fldr is None else out_fldr
         if self.gps_match_res_gdf is None:
             self.acquire_res()
 
@@ -921,14 +954,19 @@
         match_link_gdf = gpd.GeoDataFrame(match_link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=self.net.planar_crs)
         match_link_gdf = match_link_gdf.to_crs(self.net.geo_crs)
 
         for gdf, name in zip([gps_layer, prj_p_layer, prj_l_layer, match_link_gdf],
                              ['gps', 'prj_p', 'prj_l', 'match_link']):
             gdf.to_file(os.path.join(out_fldr, '-'.join([flag_name, name]) + '.geojson'), driver='GeoJSON')
 
+    def format_war_info(self):
+        if self.warn_info['from_ft']:
+            self.format_warn_info = pd.DataFrame(self.warn_info)
+        del self.warn_info
+
 
 if __name__ == '__main__':
     pass
     # a = LineString([(0, 0), (0, 1)])
     # z = a.segmentize(1/3 + 0.1 * 1/ 3)
     # print(z)
```

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/NetGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.1/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/netxfer/SumoConvert.py` & `gotrackit-0.2.1/src/gotrackit/netxfer/SumoConvert.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,40 +60,40 @@
         :param plain_node_path:
         :param crs:
         :return:
         """
         # 先解析节点
         node_tree = ET.parse(plain_node_path)
         node_root = node_tree.getroot()
-        node_df = self.parse_node_palin(plain_node_root=node_root)
+        node_df = self.parse_node_plain(plain_node_root=node_root)
 
         node_loc_dict = {node_id: (x, y) for node_id, x, y in
                          zip(node_df[NODE_ID_KEY], node_df[NODE_X_KEY], node_df[NODE_Y_KEY])}
 
         node_df['geometry'] = node_df.apply(lambda xy: Point((xy[NODE_X_KEY], xy[NODE_Y_KEY])), axis=1)
         node_df.drop(columns=[NODE_X_KEY, NODE_Y_KEY], axis=1, inplace=True)
         node_gdf = gpd.GeoDataFrame(node_df, geometry='geometry', crs=crs)
         del node_df
 
         # 再解析edge
         edge_tree = ET.parse(plain_edge_path)
         edge_root = edge_tree.getroot()
-        edge_df = self.parse_edge_palin(plain_edge_root=edge_root, node_loc_dict=node_loc_dict)
+        edge_df = self.parse_edge_plain(plain_edge_root=edge_root, node_loc_dict=node_loc_dict)
 
         # 生产几何列
         edge_df['geometry'] = edge_df[EDGE_SHAPE_KEY].apply(lambda shape: LineString(shape))
         edge_df.drop(columns=[EDGE_SHAPE_KEY], axis=1, inplace=True)
 
         edge_gdf = gpd.GeoDataFrame(edge_df, geometry='geometry', crs=crs)
         del edge_df
 
         return edge_gdf, node_gdf
 
     @staticmethod
-    def parse_node_palin(plain_node_root: ET.Element = None) -> pd.DataFrame:
+    def parse_node_plain(plain_node_root: ET.Element = None) -> pd.DataFrame:
         """
         解析node文件
         :param plain_node_root:
         :return:
         """
         item_list: list[list[str, float, float, str]] = list()
         for child in plain_node_root:
@@ -101,15 +101,15 @@
                 node_id, node_x, node_y, node_type = child.get(NODE_ID_KEY), float(child.get(NODE_X_KEY)), float(
                     child.get(
                         NODE_Y_KEY)), child.get(NODE_TYPE_KEY)
                 item_list.append([node_id, node_x, node_y, node_type])
         return pd.DataFrame(item_list, columns=[NODE_ID_KEY, NODE_X_KEY, NODE_Y_KEY, NODE_TYPE_KEY])
 
     @staticmethod
-    def parse_edge_palin(plain_edge_root: ET.Element = None, node_loc_dict: dict = None) -> pd.DataFrame:
+    def parse_edge_plain(plain_edge_root: ET.Element = None, node_loc_dict: dict = None) -> pd.DataFrame:
         """
         解析edge文件
         :param plain_edge_root:
         :param node_loc_dict:
         :return:
         """
         edge_item_list = []
```

### Comparing `gotrackit-0.2.0/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.1/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.1/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/tools/geo_process.py` & `gotrackit-0.2.1/src/gotrackit/tools/geo_process.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/tools/group.py` & `gotrackit-0.2.1/src/gotrackit/tools/group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.1/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.2.0/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.1/src/gotrackit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,62 +30,62 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**04.12已更新: v0.2.0**
+**04.18已更新: v0.2.1**
 
 更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
+- 地图匹配接口移除geo_res_fldr, geojson文件和html存储在一个目录下，指定html_fldr即可，以及增加其他存储参数(见文档)
 
-- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
+- HTML文件中新增警告路段信息，若该次匹配中出现警告, 则在HTML文件中会多一个图层，该图层记录了GPS状态转移出错的路段
 
-- 增加GPS点停留点识别功能
+- 停留点识别功能改进
 
-- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
+- BUG修复
 
-- 增加依据GPS数据提取带途径点OD的功能
 
-- 增加了路网处理函数：路段、节点重塑
-
-- 修复了部分BUG
+遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
 
-遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
+稀疏轨迹匹配与路径补全：
 
 <div align="center">
-    <img src="docs/_static/images/l_f.gif" />
+    <img src="docs/_static/images/极稀疏轨迹匹配.gif" />
 </div>
 
+
 <div align="center">
-    <img src="docs/_static/images/m_h_f.gif" />
+    <img src="docs/_static/images/匹配动画样例3.gif" />
 </div>
 
-稀疏轨迹增密匹配：
+
+常规匹配：
 
 <div align="center">
-    <img src="docs/_static/images/dense_gps.gif" />
+    <img src="docs/_static/images/匹配动画样例1.gif" />
 </div>
 
-
 <div align="center">
-    <img src="docs/_static/images/taxi_xishu.gif" />
+    <img src="docs/_static/images/匹配动画样例2.gif" />
 </div>
 
 
 <div align="center">
-    <img src="docs/_static/images/xa_sample.gif" />
+    <img src="docs/_static/images/匹配动画样例4.gif" />
 </div>
 
 
-![car_gps.png](docs/_static/images/wxq.jpg)
-
+用户交流群：
+<div align="center">
+    <img src="docs/_static/images/wxq.jpg" />
+</div>
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
 **数据无忧**
 - 提供路网生产模块以及路网优化接口，您不需要准备任何路网和GPS数据即可玩转地图匹配；
@@ -115,16 +115,14 @@
 - networkx(3.2.1)
 - pandas(2.0.3)
 - numpy(1.26.2)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
-geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
-
 #### __使用pip安装__
 
 安装：
 
 ``` shell
 pip install -i https://pypi.org/simple/ gotrackit
 ```
```

### Comparing `gotrackit-0.2.0/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.1/src/gotrackit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/gotrackit.egg-info/dependency_links.txt
 src/gotrackit.egg-info/requires.txt
 src/gotrackit.egg-info/top_level.txt
 src/gotrackit/generation/GpsGen.py
 src/gotrackit/generation/__init__.py
 src/gotrackit/gps/GpsArray.py
 src/gotrackit/gps/GpsTrip.py
+src/gotrackit/gps/GpsXfer.py
 src/gotrackit/gps/LocGps.py
 src/gotrackit/gps/__init__.py
 src/gotrackit/map/Link.py
 src/gotrackit/map/Net.py
 src/gotrackit/map/Node.py
 src/gotrackit/map/__init__.py
 src/gotrackit/model/Markov.py
```

