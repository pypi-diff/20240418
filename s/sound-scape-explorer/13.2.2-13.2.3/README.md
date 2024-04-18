# Comparing `tmp/sound_scape_explorer-13.2.2.tar.gz` & `tmp/sound_scape_explorer-13.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_scape_explorer-13.2.2.tar", last modified: Wed Apr 17 14:40:03 2024, max compression
+gzip compressed data, was "sound_scape_explorer-13.2.3.tar", last modified: Thu Apr 18 10:39:18 2024, max compression
```

## Comparing `sound_scape_explorer-13.2.2.tar` & `sound_scape_explorer-13.2.3.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.455557 sound_scape_explorer-13.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-17 14:40:03.455557 sound_scape_explorer-13.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.411558 sound_scape_explorer-13.2.2/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.415557 sound_scape_explorer-13.2.2/processing/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/autocluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/compute_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/export_computation_umaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/export_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/export_mdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/extract_and_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/fix_audio_windows_10_7_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/purge_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/refresh_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/repack_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/trace_relative_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/actions/trace_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.415557 sound_scape_explorer-13.2.2/processing/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/AggregatedLabelStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/AggregatedReduceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/AggregatedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/AutoclusteredStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/ComputationUmapStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/ContinuousTimeTrajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/FileLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/FileWalker.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/Interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/MeanDistancesMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/MenuChoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/RelativeTracedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/Timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/TimelineWalker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/TracedStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/TrajectoryConfigError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.415557 sound_scape_explorer-13.2.2/processing/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ConfigParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ExcelSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/autoclusters/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/autoclusters/AutoclusterConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/autoclusters/AutoclusterExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/autoclusters/AutoclusterStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/autoclusters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/bands/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/bands/BandConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/bands/BandExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/bands/BandStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/bands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/binary/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/binary/BinaryStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/digesters/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/digesters/DigesterConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/digesters/DigesterSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/digesters/DigesterStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/digesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.419557 sound_scape_explorer-13.2.2/processing/config/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/files/FileConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/files/FileSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/files/FileStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/integrations/IntegrationConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/integrations/IntegrationExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/integrations/IntegrationStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/labels/
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/labels/LabelConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/labels/LabelStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/labels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/ranges/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ranges/RangeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ranges/RangeExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ranges/RangeStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/ranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/reducers/
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/reducers/ReducerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/reducers/ReducerExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/reducers/ReducerStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/reducers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/SettingsConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/SettingsDefaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/SettingsRow.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/SettingsSheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/SettingsStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/sites/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/sites/SiteConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/sites/SiteStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.423557 sound_scape_explorer-13.2.2/processing/config/trajectories/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/trajectories/TrajectoryConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/trajectories/TrajectoryExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/trajectories/TrajectoryStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/config/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.427557 sound_scape_explorer-13.2.2/processing/digesters/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/ContingencyDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/Digester.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/DistanceDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/MeanSpreadingDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/MeanStandardDeviationDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/OverlapDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/SilhouetteDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/SumStandardDeviationDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/SumVarianceDigester.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/digesters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.427557 sound_scape_explorer-13.2.2/processing/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/errors/DatasetTypeError.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/errors/TimelineIntervalOverlapError.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.427557 sound_scape_explorer-13.2.2/processing/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/AcousticComplexityExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/AcousticDiversityIndexIndicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/BioacousticsIndexExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/FrequencyEntropyIndicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/LeqMaadExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/SoundscapeIndexExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/TemporalEntropyExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/TemporalMedianExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/VggExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.431557 sound_scape_explorer-13.2.2/processing/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/lib/ENES_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/lib/VAE_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/lib/VGG.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.431557 sound_scape_explorer-13.2.2/processing/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/SoundLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/SoundSlice.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/Spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/TorchLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.431557 sound_scape_explorer-13.2.2/processing/reducers/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/AbstractReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/PcaReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/SparsePcaReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/UmapReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/VaeReducer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/reducers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.431557 sound_scape_explorer-13.2.2/processing/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/storage/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/storage/StorageCompression.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/storage/StorageMode.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/storage/StoragePath.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.451557 sound_scape_explorer-13.2.2/processing/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/append_to_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_band.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_csv_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_for_repack_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/ask_npy_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/build_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/build_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/compute_relative_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/compute_starting_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/convert_dataframe_to_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/convert_date_to_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/convert_timestamp_to_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/create_timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/deep_getsizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/does_path_exist.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/extract_config_from_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/fill_symetrical_matrix_with_nans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/filter_features_by_label_and_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/filter_nn_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/get_absolute_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/get_file_full_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/get_uniques_sorted.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/get_uniques_unsorted.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/get_version_from_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/invoke_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/is_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/is_within_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/limit_memory_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/pack_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/prettify_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_digesters.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_file_indexes_by_site.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_menu_legend.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_new_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_aggregated_reduceables.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_autoclustered.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_computation_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_mean_distances_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_no_reduced.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_packed_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_timeline_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/print_welcome.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/quit_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/read_audio_path_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/read_audio_path_in_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/read_files_durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/read_trajectory_path_and_relative_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/reverse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/sort_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/split_array_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/trim_quotes_if_needed.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_aggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_autoclustered.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_autoclusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_computation_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_configuration_with_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_digesters.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_excel_booleans.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_excel_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_excel_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_int.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_mean_distances_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_mean_distances_matrix_with_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_reduced.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/validate_trajectory_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/walk_bands_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/walk_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/walk_packed_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-17 14:38:13.000000 sound_scape_explorer-13.2.2/processing/utils/wrap_menu_choice_with_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-17 14:40:01.000000 sound_scape_explorer-13.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:40:03.455557 sound_scape_explorer-13.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:40:03.455557 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 14:40:03.000000 sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.926490 sound_scape_explorer-13.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 10:39:18.926490 sound_scape_explorer-13.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.882490 sound_scape_explorer-13.2.3/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.886489 sound_scape_explorer-13.2.3/processing/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/autocluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/compute_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/export_computation_umaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/export_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/export_mdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/extract_and_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/fix_audio_windows_10_7_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/purge_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/refresh_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/repack_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/trace_relative_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/actions/trace_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.890489 sound_scape_explorer-13.2.3/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/AggregatedLabelStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/AggregatedReduceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/AggregatedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/AutoclusteredStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/ComputationUmapStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/ContinuousTimeTrajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/FileLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/FileWalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/Interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/MeanDistancesMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/MenuChoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/RelativeTracedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/Timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/TimelineWalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/TracedStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/TrajectoryConfigError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.890489 sound_scape_explorer-13.2.3/processing/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ConfigParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ExcelSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.890489 sound_scape_explorer-13.2.3/processing/config/autoclusters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/autoclusters/AutoclusterConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/autoclusters/AutoclusterExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/autoclusters/AutoclusterStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/autoclusters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.890489 sound_scape_explorer-13.2.3/processing/config/bands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/bands/BandConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/bands/BandExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/bands/BandStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/bands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.890489 sound_scape_explorer-13.2.3/processing/config/binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/binary/BinaryStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/digesters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/digesters/DigesterConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/digesters/DigesterSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/digesters/DigesterStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/digesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/files/FileConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/files/FileSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/files/FileStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/integrations/IntegrationConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/integrations/IntegrationExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/integrations/IntegrationStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/labels/LabelConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/labels/LabelStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/labels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.894490 sound_scape_explorer-13.2.3/processing/config/ranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ranges/RangeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ranges/RangeExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ranges/RangeStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/ranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.898490 sound_scape_explorer-13.2.3/processing/config/reducers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/reducers/ReducerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/reducers/ReducerExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/reducers/ReducerStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/reducers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.898490 sound_scape_explorer-13.2.3/processing/config/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/SettingsConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/SettingsDefaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/SettingsRow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/SettingsSheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/SettingsStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.898490 sound_scape_explorer-13.2.3/processing/config/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/sites/SiteConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/sites/SiteStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.898490 sound_scape_explorer-13.2.3/processing/config/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/trajectories/TrajectoryConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/trajectories/TrajectoryExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/trajectories/TrajectoryStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/config/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.902490 sound_scape_explorer-13.2.3/processing/digesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/ContingencyDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/Digester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/DistanceDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/MeanSpreadingDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/MeanStandardDeviationDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/OverlapDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/SilhouetteDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/SumStandardDeviationDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/SumVarianceDigester.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/digesters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.902490 sound_scape_explorer-13.2.3/processing/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/errors/DatasetTypeError.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/errors/TimelineIntervalOverlapError.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.902490 sound_scape_explorer-13.2.3/processing/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/AcousticComplexityExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/AcousticDiversityIndexIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/BioacousticsIndexExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/FrequencyEntropyIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/LeqMaadExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/SoundscapeIndexExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/TemporalEntropyExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/TemporalMedianExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/VggExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.906490 sound_scape_explorer-13.2.3/processing/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/lib/ENES_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/lib/VAE_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/lib/VGG.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.906490 sound_scape_explorer-13.2.3/processing/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/SoundLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/SoundSlice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/Spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/TorchLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.906490 sound_scape_explorer-13.2.3/processing/reducers/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/AbstractReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/PcaReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/SparsePcaReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/UmapReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/VaeReducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/reducers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.906490 sound_scape_explorer-13.2.3/processing/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/storage/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/storage/StorageCompression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/storage/StorageMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/storage/StoragePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.926490 sound_scape_explorer-13.2.3/processing/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/append_to_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_band.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_csv_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_for_repack_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/ask_npy_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/build_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/build_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/compute_relative_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/compute_starting_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/convert_dataframe_to_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/convert_date_to_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/convert_timestamp_to_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/create_timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/deep_getsizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/does_path_exist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/extract_config_from_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/fill_symetrical_matrix_with_nans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/filter_features_by_label_and_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/filter_nn_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/get_absolute_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/get_file_full_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/get_uniques_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/get_uniques_unsorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/get_version_from_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/invoke_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/is_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/is_within_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/limit_memory_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/pack_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/prettify_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_digesters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_file_indexes_by_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_menu_legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_new_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_aggregated_reduceables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_autoclustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_computation_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_mean_distances_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_no_reduced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_packed_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_timeline_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/print_welcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/quit_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/read_audio_path_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/read_audio_path_in_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/read_files_durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/read_trajectory_path_and_relative_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/reverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/sort_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/split_array_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/trim_quotes_if_needed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_autoclustered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_autoclusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_computation_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_configuration_with_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_digesters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_excel_booleans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_excel_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_excel_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_mean_distances_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_mean_distances_matrix_with_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_reduced.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/validate_trajectory_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/walk_bands_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/walk_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/walk_packed_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-18 10:37:24.000000 sound_scape_explorer-13.2.3/processing/utils/wrap_menu_choice_with_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-18 10:39:16.000000 sound_scape_explorer-13.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 10:39:18.926490 sound_scape_explorer-13.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:39:18.926490 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 10:39:18.000000 sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/top_level.txt
```

### Comparing `sound_scape_explorer-13.2.2/PKG-INFO` & `sound_scape_explorer-13.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-scape-explorer
-Version: 13.2.2
+Version: 13.2.3
 Summary: SoundScapeExplorer
 Author-email: Bamdad Sabbagh <hi@bamdad.fr>
 Requires-Dist: wheel
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: h5py==3.8.0
 Requires-Dist: torch==2.0.0
```

### Comparing `sound_scape_explorer-13.2.2/processing/actions/autocluster.py` & `sound_scape_explorer-13.2.3/processing/actions/autocluster.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/compute_requirements.py` & `sound_scape_explorer-13.2.3/processing/actions/compute_requirements.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/digest.py` & `sound_scape_explorer-13.2.3/processing/actions/digest.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/export_computation_umaps.py` & `sound_scape_explorer-13.2.3/processing/actions/export_computation_umaps.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/export_dataframe.py` & `sound_scape_explorer-13.2.3/processing/actions/export_dataframe.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/export_mdm.py` & `sound_scape_explorer-13.2.3/processing/actions/export_mdm.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/extract_and_aggregate.py` & `sound_scape_explorer-13.2.3/processing/actions/extract_and_aggregate.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/fix_audio_windows_10_7_2.py` & `sound_scape_explorer-13.2.3/processing/actions/fix_audio_windows_10_7_2.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/purge_requirements.py` & `sound_scape_explorer-13.2.3/processing/actions/purge_requirements.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/reduce.py` & `sound_scape_explorer-13.2.3/processing/actions/reduce.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/refresh_configuration.py` & `sound_scape_explorer-13.2.3/processing/actions/refresh_configuration.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/repack_storage.py` & `sound_scape_explorer-13.2.3/processing/actions/repack_storage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/trace_relative_trajectories.py` & `sound_scape_explorer-13.2.3/processing/actions/trace_relative_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/actions/trace_trajectories.py` & `sound_scape_explorer-13.2.3/processing/actions/trace_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/cli.py` & `sound_scape_explorer-13.2.3/processing/cli.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/AggregatedLabelStorage.py` & `sound_scape_explorer-13.2.3/processing/common/AggregatedLabelStorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,13 +60,13 @@
 
         aggregated_values_np = np.array(aggregated_values_strings)
 
         for index, values in enumerate(aggregated_values_np.T):
             property_ = properties[index]
             aggregated_label = LabelConfig(
                 index=index + len(autoclustereds),
-                property=property_,
+                property_=property_,
             )
             aggregated_label.load_values(values)
             aggregated_labels.append(aggregated_label)
 
         return aggregated_labels
```

### Comparing `sound_scape_explorer-13.2.2/processing/common/AggregatedReduceable.py` & `sound_scape_explorer-13.2.3/processing/common/AggregatedReduceable.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/AggregatedStorage.py` & `sound_scape_explorer-13.2.3/processing/common/AggregatedStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/AutoclusteredStorage.py` & `sound_scape_explorer-13.2.3/processing/common/AutoclusteredStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/ComputationUmapStorage.py` & `sound_scape_explorer-13.2.3/processing/common/ComputationUmapStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/ContinuousTimeTrajectory.py` & `sound_scape_explorer-13.2.3/processing/common/ContinuousTimeTrajectory.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/FileWalker.py` & `sound_scape_explorer-13.2.3/processing/common/FileWalker.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/MeanDistancesMatrix.py` & `sound_scape_explorer-13.2.3/processing/common/MeanDistancesMatrix.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/MenuChoice.py` & `sound_scape_explorer-13.2.3/processing/common/MenuChoice.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/RelativeTracedStorage.py` & `sound_scape_explorer-13.2.3/processing/common/RelativeTracedStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/Timeline.py` & `sound_scape_explorer-13.2.3/processing/common/Timeline.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/common/TimelineWalker.py` & `sound_scape_explorer-13.2.3/processing/common/TimelineWalker.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,59 +47,52 @@
 
     @property
     def timelines(self) -> List[Timeline]:
         assert self.__timelines is not None, "Please attach timelines"
         return self.__timelines
 
     @timelines.setter
-    def timelines(self, timelines: List[Timeline]) -> List[Timeline]:
+    def timelines(self, timelines: List[Timeline]):
         self.__timelines = timelines
-        return self.__timelines
 
     @property
     def bands(self) -> List[BandConfig]:
         assert self.__bands is not None, "Please attach bands"
         return self.__bands
 
     @bands.setter
-    def bands(self, bands: List[BandConfig]) -> List[BandConfig]:
+    def bands(self, bands: List[BandConfig]):
         self.__bands = bands
-        return self.__bands
 
     @property
     def integrations(self) -> List[IntegrationConfig]:
         assert self.__integrations is not None, "Please attach integrations"
         return self.__integrations
 
     @integrations.setter
-    def integrations(
-        self, integrations: List[IntegrationConfig]
-    ) -> List[IntegrationConfig]:
+    def integrations(self, integrations: List[IntegrationConfig]):
         self.__integrations = integrations
-        return self.__integrations
 
     @property
     def extractors(self) -> List[Extractor]:
         assert self.__extractors is not None, "Please attach extractors"
         return self.__extractors
 
     @extractors.setter
-    def extractors(self, extractors: List[Extractor]) -> List[Extractor]:
+    def extractors(self, extractors: List[Extractor]):
         self.__extractors = extractors
-        return self.__extractors
 
     @property
     def storage(self) -> Storage:
         assert self.__storage is not None, "Please attach storage"
         return self.__storage
 
     @storage.setter
-    def storage(self, storage: Storage) -> Storage:
+    def storage(self, storage: Storage):
         self.__storage = storage
-        return self.__storage
 
     def print_leftovers(self):
         print_new_line()
         print("Memory leftovers")
         # show extracted data
         for k, v in self.extracted.items():
             for kk, vv in v.items():
@@ -108,15 +101,15 @@
 
         # show loaded files
         for _, loader in self.loaders.items():
             print(type(loader.loader.torch.audio))
             loader.loader.sound.print_leftovers()
 
     def __enumerate(self):
-        for timeline in track(self.timelines, description=("Extracting...")):
+        for timeline in track(self.timelines, description="Extracting..."):
             for interval in timeline.intervals:
                 print_timeline_progress(timeline, interval)
                 for band_index, band in enumerate(self.bands):
                     for extractor in self.extractors:
                         yield (
                             timeline,
                             interval,
@@ -192,16 +185,16 @@
 
         file_data = self.extracted[block.file.index][band.index][extractor.index]
 
         block_data = file_data[start:end]
 
         return block_data
 
+    @staticmethod
     def get_block_details(
-        self,
         block: Block,
     ) -> str:
         file_relative_start = block.start - block.file.start
         block_details = f"{block.start}/{file_relative_start}/{block.file.path}"
         return block_details
 
     def purge(
```

### Comparing `sound_scape_explorer-13.2.2/processing/common/TracedStorage.py` & `sound_scape_explorer-13.2.3/processing/common/TracedStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/Config.py` & `sound_scape_explorer-13.2.3/processing/config/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from typing import List
 
 from rich import print
 from rich.console import Console
 from rich.table import Table
 
+from processing.config.ConfigParser import ConfigParser
 from processing.config.autoclusters.AutoclusterConfig import AutoclusterConfig
 from processing.config.autoclusters.AutoclusterStorage import AutoclusterStorage
 from processing.config.bands.BandConfig import BandConfig
 from processing.config.bands.BandStorage import BandStorage
 from processing.config.binary.BinaryStorage import BinaryStorage
-from processing.config.ConfigParser import ConfigParser
 from processing.config.digesters.DigesterConfig import DigesterConfig
 from processing.config.digesters.DigesterStorage import DigesterStorage
 from processing.config.extractors.ExtractorConfig import ExtractorConfig
 from processing.config.extractors.ExtractorStorage import ExtractorStorage
 from processing.config.files.FileConfig import FileConfig
 from processing.config.files.FileStorage import FileStorage
 from processing.config.integrations.IntegrationConfig import IntegrationConfig
@@ -33,25 +33,25 @@
 from processing.config.trajectories.TrajectoryConfig import TrajectoryConfig
 from processing.config.trajectories.TrajectoryStorage import TrajectoryStorage
 from processing.storage.Storage import Storage
 from processing.utils.convert_timestamp_to_date import convert_timestamp_to_date
 
 
 class Config:
+    settings: SettingsConfig
+
     def __init__(
         self,
         path: str,
     ) -> None:
         self.__print_load()
         self.path = os.path.abspath(path)
         self.folder = os.path.dirname(self.path)
         self.parser = ConfigParser(self.path, self.folder)
 
-        self.settings: SettingsConfig
-
         self.bands: List[BandConfig] = []
         self.integrations: List[IntegrationConfig] = []
         self.ranges: List[RangeConfig] = []
 
         self.labels: List[LabelConfig] = []
         self.files: List[FileConfig] = []
         self.sites: List[SiteConfig] = []
@@ -62,15 +62,16 @@
 
         self.reducers: List[ReducerConfig] = []
         self.digesters: List[DigesterConfig] = []
 
         self.parse()
         self.__print_success()
 
-    def __print_load(self) -> None:
+    @staticmethod
+    def __print_load() -> None:
         print("Loading configuration...")
 
     def __print_success(self) -> None:
         print(f"Config loaded: {self.parser.path}")
         self.print_settings()
 
     def print_settings(self) -> None:
@@ -116,15 +117,16 @@
             bands=self.bands,
             integrations=self.integrations,
             ranges=self.ranges,
         )
 
         self.digesters = DigesterStorage.read_from_config(self.parser)
 
-    def delete_from_storage(self, storage: Storage) -> None:
+    @staticmethod
+    def delete_from_storage(storage: Storage) -> None:
         BinaryStorage.delete_from_storage(storage)
         SettingsStorage.delete_from_storage(storage)
 
         BandStorage.delete_from_storage(storage)
         IntegrationStorage.delete_from_storage(storage)
         RangeStorage.delete_from_storage(storage)
 
@@ -139,22 +141,24 @@
 
         ReducerStorage.delete_from_storage(storage)
         DigesterStorage.delete_from_storage(storage)
 
     def write(self, storage: Storage) -> None:
         self.delete_from_storage(storage)
 
+        # noinspection DuplicatedCode
         BinaryStorage.write_to_storage(self.path, storage)
         SettingsStorage.write_to_storage(self.settings, storage)
 
         BandStorage.write_to_storage(self.bands, storage)
         IntegrationStorage.write_to_storage(self.integrations, storage)
         RangeStorage.write_to_storage(self.ranges, storage)
 
         LabelStorage.write_to_storage(self.labels, storage)
+        # noinspection DuplicatedCode
         FileStorage.write_to_storage(self.files, storage)
         SiteStorage.write_to_storage(self.sites, storage)
 
         ExtractorStorage.write_to_storage(self.extractors, storage)
 
         AutoclusterStorage.write_to_storage(self.autoclusters, storage)
         TrajectoryStorage.write_to_storage(self.trajectories, storage)
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/ConfigParser.py` & `sound_scape_explorer-13.2.3/processing/config/ConfigParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         path: str,
         folder: str,
     ) -> None:
         self.path = self.validate(path)
         self.folder = folder
         self.excel = ExcelFile(self.path)
 
-    def validate(self, path: str) -> str:
+    @staticmethod
+    def validate(path: str) -> str:
         assert path is not None, "Please define a path"
         assert Path(path).exists(), f"Path {path} does not exist"
         return path
 
     def parse(self, sheet: ExcelSheet) -> DataFrame:
         return self.excel.parse(sheet.value)  # type: ignore
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/autoclusters/AutoclusterConfig.py` & `sound_scape_explorer-13.2.3/processing/config/autoclusters/AutoclusterConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/autoclusters/AutoclusterStorage.py` & `sound_scape_explorer-13.2.3/processing/config/autoclusters/AutoclusterStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/bands/BandConfig.py` & `sound_scape_explorer-13.2.3/processing/config/bands/BandConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/bands/BandStorage.py` & `sound_scape_explorer-13.2.3/processing/config/bands/BandStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/binary/BinaryStorage.py` & `sound_scape_explorer-13.2.3/processing/config/binary/BinaryStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/digesters/DigesterConfig.py` & `sound_scape_explorer-13.2.3/processing/config/digesters/DigesterConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/digesters/DigesterStorage.py` & `sound_scape_explorer-13.2.3/processing/config/digesters/DigesterStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorConfig.py` & `sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/extractors/ExtractorStorage.py` & `sound_scape_explorer-13.2.3/processing/config/extractors/ExtractorStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/files/FileConfig.py` & `sound_scape_explorer-13.2.3/processing/config/files/FileConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/files/FileStorage.py` & `sound_scape_explorer-13.2.3/processing/config/files/FileStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/integrations/IntegrationConfig.py` & `sound_scape_explorer-13.2.3/processing/config/integrations/IntegrationConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/integrations/IntegrationStorage.py` & `sound_scape_explorer-13.2.3/processing/config/integrations/IntegrationStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/labels/LabelConfig.py` & `sound_scape_explorer-13.2.3/processing/config/labels/LabelConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     values: List[str]  # label values by file index
     uniques_sorted: List[str]  # by alphanumerical order
     uniques_unsorted: List[str]  # by order of occurrence
 
     def __init__(
         self,
         index: int,
-        property: str,
+        property_: str,
     ) -> None:
         self.index = index
-        self.property = property
+        self.property = property_
 
     @staticmethod
     def is_label_property(string: str) -> bool:
         prefix = FileSheet.label_prefix.value
         prefix_length = len(prefix)
         string_slice = string[:prefix_length]
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/labels/LabelStorage.py` & `sound_scape_explorer-13.2.3/processing/config/labels/LabelStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         files: List[FileConfig],
     ) -> List[LabelConfig]:
         properties_dataset = storage.read(LabelStorage.properties)
         properties = storage.convert_dataset_to_string_list(properties_dataset)
 
         labels: List[LabelConfig] = []
 
-        for index, property in enumerate(properties):
-            label: LabelConfig = LabelConfig(index, property)
+        for index, property_ in enumerate(properties):
+            label: LabelConfig = LabelConfig(index, property_)
             values = [file.labels[index] for file in files]
             label.load_values(values)
             labels.append(label)
 
         return labels
 
     @staticmethod
@@ -58,15 +58,15 @@
 
         index = 0
         for column in sheet:
             if not LabelConfig.is_label_property(column):
                 continue
 
             property_ = LabelConfig.trim_prefixed_property_from_config(column)
-            label: LabelConfig = LabelConfig(index=index, property=property_)
+            label: LabelConfig = LabelConfig(index=index, property_=property_)
 
             values = parser.get(
                 ExcelSheet.files,
                 FileSheet.label_prefix,
                 suffix=label.property,
             )
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/ranges/RangeConfig.py` & `sound_scape_explorer-13.2.3/processing/config/ranges/RangeConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/ranges/RangeStorage.py` & `sound_scape_explorer-13.2.3/processing/config/ranges/RangeStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/reducers/ReducerConfig.py` & `sound_scape_explorer-13.2.3/processing/config/reducers/ReducerConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         ranges: List[RangeConfig],
     ) -> List[RangeConfig]:
         if is_nan(ranges_names_string):
             return ranges
 
         ranges_names = ranges_names_string.split(",")
 
-        picked_ranges = [range for range in ranges if range.name in ranges_names]
+        picked_ranges = [range_ for range_ in ranges if range_.name in ranges_names]
 
         return picked_ranges
 
     @staticmethod
     def reconstruct(
         names: List[str],
         dimensions: List[int],
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/reducers/ReducerStorage.py` & `sound_scape_explorer-13.2.3/processing/config/reducers/ReducerStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
-from processing.config.bands.BandConfig import BandConfig
 from processing.config.ConfigParser import ConfigParser
 from processing.config.ExcelSheet import ExcelSheet
+from processing.config.bands.BandConfig import BandConfig
 from processing.config.integrations.IntegrationConfig import IntegrationConfig
 from processing.config.ranges.RangeConfig import RangeConfig
 from processing.config.reducers.ReducerConfig import ReducerConfig
 from processing.config.reducers.ReducerExcel import ReducerExcel
 from processing.constants import STRING_NONE
 from processing.storage.Storage import Storage
 from processing.storage.StoragePath import StoragePath
@@ -64,15 +64,15 @@
 
         integrations_names_strings = [
             ",".join(integrations_names_string)
             for integrations_names_string in integrations_names
         ]
 
         ranges_names_strings = [
-            ",".join(ranges_names_string) for ranges_names_string in integrations_names
+            ",".join(ranges_names_string) for ranges_names_string in ranges_names
         ]
 
         reducers = ReducerConfig.reconstruct(
             names=names,
             dimensions=dimensions,
             bands_names_strings=bands_names_strings,
             integrations_names_strings=integrations_names_strings,
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/settings/SettingsStorage.py` & `sound_scape_explorer-13.2.3/processing/config/settings/SettingsStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         sheet = ExcelSheet.settings
 
         properties = parser.get(sheet, SettingsSheet.setting)
         values = parser.get(sheet, SettingsSheet.value_)
 
         obj = {}
 
-        for property, value in zip(properties, values):
-            obj[property] = value
+        for property_, value in zip(properties, values):
+            obj[property_] = value
 
         storage_path = obj[SettingsRow.storage_path.value]
 
         if not os.path.isabs(storage_path):
             storage_path = os.path.join(parser.folder, storage_path)
 
         audio_path = obj[SettingsRow.audio_path.value]
```

### Comparing `sound_scape_explorer-13.2.2/processing/config/sites/SiteConfig.py` & `sound_scape_explorer-13.2.3/processing/config/sites/SiteConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/sites/SiteStorage.py` & `sound_scape_explorer-13.2.3/processing/config/sites/SiteStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/trajectories/TrajectoryConfig.py` & `sound_scape_explorer-13.2.3/processing/config/trajectories/TrajectoryConfig.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/config/trajectories/TrajectoryStorage.py` & `sound_scape_explorer-13.2.3/processing/config/trajectories/TrajectoryStorage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/ContingencyDigester.py` & `sound_scape_explorer-13.2.3/processing/digesters/ContingencyDigester.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/Digester.py` & `sound_scape_explorer-13.2.3/processing/digesters/Digester.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/DistanceDigester.py` & `sound_scape_explorer-13.2.3/processing/digesters/DistanceDigester.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from pandas import DataFrame, Index
 from sklearn import metrics
 
 from processing.digesters.Digester import Digester
 
 
 class DistanceDigester(Digester):
-    def get_centers(self, dataframe: DataFrame, values: Index):
+    @staticmethod
+    def get_centers(dataframe: DataFrame, values: Index):
         # medioids
         centers = np.empty((len(values), dataframe.shape[1]))
 
         for index, _ in enumerate(values):
             centers[index, :] = np.nanpercentile(dataframe, 50, axis=0)
 
         return centers
```

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/MeanSpreadingDigester.py` & `sound_scape_explorer-13.2.3/processing/digesters/MeanSpreadingDigester.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/OverlapDigester.py` & `sound_scape_explorer-13.2.3/processing/digesters/OverlapDigester.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/digesters/SilhouetteDigester.py` & `sound_scape_explorer-13.2.3/processing/digesters/SilhouetteDigester.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/errors/TimelineIntervalOverlapError.py` & `sound_scape_explorer-13.2.3/processing/errors/TimelineIntervalOverlapError.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/AcousticDiversityIndexIndicator.py` & `sound_scape_explorer-13.2.3/processing/extractors/AcousticDiversityIndexIndicator.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/BioacousticsIndexExtractor.py` & `sound_scape_explorer-13.2.3/processing/extractors/BioacousticsIndexExtractor.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/Extractor.py` & `sound_scape_explorer-13.2.3/processing/extractors/Extractor.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,47 +27,43 @@
     def expected_sample_rate(self) -> int:
         assert (
             self.__expected_sample_rate is not None
         ), "Please define expected sample rate"
         return self.__expected_sample_rate
 
     @expected_sample_rate.setter
-    def expected_sample_rate(self, expected_sample_rate: int) -> int:
+    def expected_sample_rate(self, expected_sample_rate: int):
         self.__expected_sample_rate = expected_sample_rate
-        return self.__expected_sample_rate
 
     @property
     def band(self) -> BandConfig:
         assert self.__band is not None, "Please define band"
         return self.__band
 
     @band.setter
-    def band(self, band: BandConfig) -> BandConfig:
+    def band(self, band: BandConfig):
         self.__band = band
-        return self.__band
 
     @property
     def offset(self) -> int:
         assert self.__offset is not None, "Please define offset"
         return self.__offset
 
     @offset.setter
-    def offset(self, offset: int) -> int:
+    def offset(self, offset: int):
         self.__offset = offset
-        return self.__offset
 
     @property
     def step(self) -> int:
         assert self.__step is not None, "Please define step"
         return self.__step
 
     @step.setter
-    def step(self, step: int) -> int:
+    def step(self, step: int):
         self.__step = step
-        return self.__step
 
     @abstractmethod
     def extract(self, loader: Loader) -> Extracted:
         pass
 
     def persist(self):
         self.is_persist = True
```

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/LeqMaadExtractor.py` & `sound_scape_explorer-13.2.3/processing/extractors/LeqMaadExtractor.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/SoundscapeIndexExtractor.py` & `sound_scape_explorer-13.2.3/processing/extractors/SoundscapeIndexExtractor.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/extractors/VggExtractor.py` & `sound_scape_explorer-13.2.3/processing/extractors/VggExtractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,51 +32,54 @@
         self.features = self.load_features()
         self.embeddings = self.load_embeddings()
         self.device = self.load_device()
         self.load_state_dict()
         self.to(self.device)
         self.eval()
 
-    def load_embeddings(self):
+    @staticmethod
+    def load_embeddings():
         return nn.Sequential(
             nn.Linear(512 * 4 * 6, 4096),
             nn.ReLU(True),
             nn.Linear(4096, 4096),
             nn.ReLU(True),
             nn.Linear(4096, 128),
             nn.ReLU(True),
         )
 
-    def load_features(self):
+    @staticmethod
+    def load_features():
         layers = []
         in_channels = 1
 
         for v in [64, "M", 128, "M", 256, 256, "M", 512, 512, "M"]:
             if v == "M":
                 layers += [nn.MaxPool2d(kernel_size=2, stride=2)]
             else:
                 conv2d = nn.Conv2d(in_channels, v, kernel_size=3, padding=1)
                 layers += [conv2d, nn.ReLU(inplace=True)]
                 in_channels = v
 
         return nn.Sequential(*layers)
 
-    def load_state_dict(self):
+    def load_state_dict(self, **kwargs):
         state_dict = self.fetch_state_dict()
         super().load_state_dict(state_dict)
 
     @staticmethod
     def fetch_state_dict():
         return hub.load_state_dict_from_url(
             "https://github.com/harritaylor/torchvggish/"
             "releases/download/v0.1/vggish-10086976.pth",
             progress=True,
         )
 
-    def load_device(self):
+    @staticmethod
+    def load_device():
         if cuda.is_available():
             print("Using GPU")
             return "cuda"
         else:
             print("Using CPU")
             return "cpu"
 
@@ -90,15 +93,16 @@
             # remain compatible with VGGish embeddings
             x = torch.transpose(x, 1, 3)
             x = torch.transpose(x, 1, 2)
             x = x.contiguous()
             x = x.view(x.size(0), -1)
             return self.embeddings(x)
 
-    def to_frames(self, data: Tensor) -> Tensor:
+    @staticmethod
+    def to_frames(data: Tensor) -> Tensor:
         window_length = hop_length = 100
 
         num_samples = data.shape[0]
         num_frames = 1 + int(np.floor((num_samples - window_length) / hop_length))
         shape = (num_frames, window_length) + data.shape[1:]
 
         strides = data.stride(0) * hop_length, data.stride(0), data.stride(1)
```

### Comparing `sound_scape_explorer-13.2.2/processing/lib/ENES_index.py` & `sound_scape_explorer-13.2.3/processing/lib/ENES_index.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/lib/VAE_v1.py` & `sound_scape_explorer-13.2.3/processing/lib/VAE_v1.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/lib/VGG.py` & `sound_scape_explorer-13.2.3/processing/lib/VGG.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/loaders/Loader.py` & `sound_scape_explorer-13.2.3/processing/loaders/Loader.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/loaders/SoundLoader.py` & `sound_scape_explorer-13.2.3/processing/loaders/SoundLoader.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/loaders/TorchLoader.py` & `sound_scape_explorer-13.2.3/processing/loaders/TorchLoader.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/main.py` & `sound_scape_explorer-13.2.3/processing/main.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/reducers/AbstractReducer.py` & `sound_scape_explorer-13.2.3/processing/reducers/AbstractReducer.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/reducers/PcaReducer.py` & `sound_scape_explorer-13.2.3/processing/reducers/PcaReducer.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/reducers/SparsePcaReducer.py` & `sound_scape_explorer-13.2.3/processing/reducers/SparsePcaReducer.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/reducers/UmapReducer.py` & `sound_scape_explorer-13.2.3/processing/reducers/UmapReducer.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/storage/Storage.py` & `sound_scape_explorer-13.2.3/processing/storage/Storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     def __get_path_as_string(path: Union[StoragePath, str]) -> str:
         if type(path) is StoragePath:
             path = path.value
 
         path = str(path)
         return path
 
+    @staticmethod
     def __write_version_to_dataset(
-        self,
         dataset: Dataset,
     ) -> Dataset:
         # Attach app version to all datasets
         dataset.attrs["version"] = get_version_from_setup()
         return dataset
 
     def write(
```

### Comparing `sound_scape_explorer-13.2.2/processing/storage/StoragePath.py` & `sound_scape_explorer-13.2.3/processing/storage/StoragePath.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/append_to_config.py` & `sound_scape_explorer-13.2.3/processing/utils/append_to_config.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/ask_band.py` & `sound_scape_explorer-13.2.3/processing/utils/ask_band.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/ask_csv_path.py` & `sound_scape_explorer-13.2.3/processing/utils/ask_csv_path.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/ask_integration.py` & `sound_scape_explorer-13.2.3/processing/utils/ask_integration.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/ask_menu.py` & `sound_scape_explorer-13.2.3/processing/utils/ask_menu.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/ask_npy_path.py` & `sound_scape_explorer-13.2.3/processing/utils/ask_npy_path.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/build_aggregated_reduceables.py` & `sound_scape_explorer-13.2.3/processing/utils/build_aggregated_reduceables.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/build_reducers.py` & `sound_scape_explorer-13.2.3/processing/utils/build_reducers.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/convert_date_to_timestamp.py` & `sound_scape_explorer-13.2.3/processing/utils/convert_date_to_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def convert_date_to_timestamp(date_string: Union[Timestamp, str]) -> int:
     """Converts a date to timestamp.
 
     The resulting timestamp is in UNIX format and milliseconds.
 
     Args:
-        date: A pandas Timestamp object.
+        date_string: A pandas Timestamp object.
 
     Returns:
         The timestamp in milliseconds as an integer.
     """
 
     if isinstance(date_string, str):
         date = datetime.datetime.strptime(date_string, "%Y-%m-%d %H:%M:%S")
```

### Comparing `sound_scape_explorer-13.2.2/processing/utils/create_timelines.py` & `sound_scape_explorer-13.2.3/processing/utils/create_timelines.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/extract_config_from_storage.py` & `sound_scape_explorer-13.2.3/processing/utils/extract_config_from_storage.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/filter_features_by_label_and_time.py` & `sound_scape_explorer-13.2.3/processing/utils/filter_features_by_label_and_time.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/is_within_interval.py` & `sound_scape_explorer-13.2.3/processing/utils/is_within_interval.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/pack_trajectories.py` & `sound_scape_explorer-13.2.3/processing/utils/pack_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_action.py` & `sound_scape_explorer-13.2.3/processing/utils/print_action.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_aggregated_reduceables.py` & `sound_scape_explorer-13.2.3/processing/utils/print_aggregated_reduceables.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_autoclusters.py` & `sound_scape_explorer-13.2.3/processing/utils/print_autoclusters.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_digesters.py` & `sound_scape_explorer-13.2.3/processing/utils/print_digesters.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_extractors.py` & `sound_scape_explorer-13.2.3/processing/utils/print_extractors.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_file_indexes_by_site.py` & `sound_scape_explorer-13.2.3/processing/utils/print_file_indexes_by_site.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_packed_trajectories.py` & `sound_scape_explorer-13.2.3/processing/utils/print_packed_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_reducers.py` & `sound_scape_explorer-13.2.3/processing/utils/print_reducers.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_timeline_progress.py` & `sound_scape_explorer-13.2.3/processing/utils/print_timeline_progress.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/print_trajectories.py` & `sound_scape_explorer-13.2.3/processing/utils/print_trajectories.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/read_files_durations.py` & `sound_scape_explorer-13.2.3/processing/utils/read_files_durations.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/read_trajectory_path_and_relative_timestamps.py` & `sound_scape_explorer-13.2.3/processing/utils/read_trajectory_path_and_relative_timestamps.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/split_array_by_length.py` & `sound_scape_explorer-13.2.3/processing/utils/split_array_by_length.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_aggregated.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_aggregated.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_autoclustered.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_autoclustered.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_autoclusters.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_autoclusters.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_computation_umap.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_computation_umap.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_configuration.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_configuration.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_configuration_with_config.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_configuration_with_config.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_digesters.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_digesters.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_mean_distances_matrix.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_mean_distances_matrix.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_mean_distances_matrix_with_config.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_mean_distances_matrix_with_config.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_reduced.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_reduced.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/processing/utils/validate_trajectory_labels.py` & `sound_scape_explorer-13.2.3/processing/utils/validate_trajectory_labels.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     names: List[str],
     properties: List[str],
     values: List[str],
     labels: List[LabelConfig],
 ) -> None:
     files_properties, files_values = LabelConfig.flatten(labels)
 
-    for i, property in enumerate(properties):
-        if property not in files_properties:
+    for i, property_ in enumerate(properties):
+        if property_ not in files_properties:
             raise TrajectoryConfigError(
-                f"Property {property} not found in files for trajectory {names[i]}."
+                f"Property {property_} not found in files for trajectory {names[i]}."
             )
 
-        property_index = files_properties.index(property)
+        property_index = files_properties.index(property_)
         value = values[i]
         files_value = files_values[property_index]
 
         if value not in files_value:
             raise TrajectoryConfigError(
                 f"Value {value} not found in files for property"
-                f" {property} for trajectory {names[i]}."
+                f" {property_} for trajectory {names[i]}."
             )
```

### Comparing `sound_scape_explorer-13.2.2/processing/utils/walk_directory.py` & `sound_scape_explorer-13.2.3/processing/utils/walk_directory.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 
 def walk_directory(path: str) -> List[str]:
     relative_paths = []
     supported_formats = [".wav", ".mp3", ".flac"]
 
     for dir_path, _, filenames in os.walk(path):
-        for f in filenames:
+        for filename in filenames:
             for format_ in supported_formats:
-                if f.endswith(format_):
-                    absolute_path = os.path.join(dir_path, f)
-                    relative_path = absolute_path.replace(path, "")
+                filename_lowercase = filename.lower()
 
-                    if platform.system() == "Windows":
-                        relative_path = relative_path.replace("\\", "/")
+                if not filename_lowercase.endswith(format_):
+                    continue
 
-                    relative_paths.append(relative_path)
+                absolute_path = os.path.join(dir_path, filename)
+                relative_path = absolute_path.replace(path, "")
+
+                if platform.system() == "Windows":
+                    relative_path = relative_path.replace("\\", "/")
+
+                relative_paths.append(relative_path)
 
     return relative_paths
```

### Comparing `sound_scape_explorer-13.2.2/processing/utils/wrap_menu_choice_with_state.py` & `sound_scape_explorer-13.2.3/processing/utils/wrap_menu_choice_with_state.py`

 * *Files identical despite different names*

### Comparing `sound_scape_explorer-13.2.2/pyproject.toml` & `sound_scape_explorer-13.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # INFO: When changing `name`, also change in `utils/get_version_from_setup.py`
 name = "sound-scape-explorer"
-version = "13.2.2"
+version = "13.2.3"
 description = "SoundScapeExplorer"
 authors = [{ name = "Bamdad Sabbagh", email = "hi@bamdad.fr" }]
 
 dependencies = [
   "wheel",
   "numpy==1.23.5",
   "pandas==1.5.3",
```

### Comparing `sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/PKG-INFO` & `sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-scape-explorer
-Version: 13.2.2
+Version: 13.2.3
 Summary: SoundScapeExplorer
 Author-email: Bamdad Sabbagh <hi@bamdad.fr>
 Requires-Dist: wheel
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas==1.5.3
 Requires-Dist: h5py==3.8.0
 Requires-Dist: torch==2.0.0
```

### Comparing `sound_scape_explorer-13.2.2/sound_scape_explorer.egg-info/SOURCES.txt` & `sound_scape_explorer-13.2.3/sound_scape_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

