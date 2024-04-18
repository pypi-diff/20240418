# Comparing `tmp/flightanalysis-0.2.5.tar.gz` & `tmp/flightanalysis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightanalysis-0.2.5.tar", last modified: Wed Mar 20 20:38:20 2024, max compression
+gzip compressed data, was "flightanalysis-0.2.6.tar", last modified: Thu Apr 18 12:15:24 2024, max compression
```

## Comparing `flightanalysis-0.2.5.tar` & `flightanalysis-0.2.6.tar`

### file list

```diff
@@ -1,113 +1,94 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.028771 flightanalysis-0.2.5/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35149 2023-03-28 15:54:19.000000 flightanalysis-0.2.5/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       35 2023-09-25 09:37:01.000000 flightanalysis-0.2.5/MANIFEST.in
--rw-r--r--   0 td6834    (1001) td6834    (1001)      464 2024-03-20 20:38:20.028771 flightanalysis-0.2.5/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      181 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:19.000000 flightanalysis-0.2.5/examples/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:19.000000 flightanalysis-0.2.5/examples/data/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/schedules_construction/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6939 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/examples/schedules_construction/AMA_Intermediate2024.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/examples/schedules_construction/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      662 2024-01-27 20:42:45.000000 flightanalysis-0.2.5/examples/schedules_construction/create_all.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8487 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3a_a25.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    10825 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3a_f25.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8466 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3a_p23.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8357 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3a_p25.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6573 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3auk_Intermediate.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7174 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/schedules_construction/f3auk_clubman.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4613 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/schedules_construction/imac_sport2024.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5682 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/schedules_construction/imac_unlim2024.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      521 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/schedules_construction/make_manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7342 2024-01-27 20:42:45.000000 flightanalysis-0.2.5/examples/schedules_construction/nsrca_inter2024.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/scoring/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      863 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/examples/scoring/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      526 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/examples/scoring/analysis_reprocess.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1850 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/examples/scoring/f3a_criteria_maker.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1244 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/examples/scoring/judging.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/scoring/manoeuvres/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      497 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/inter_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      906 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/intra_analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.004768 flightanalysis-0.2.5/examples/scoring/manoeuvres/mans/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/mans/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      994 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/mans/extract_mans.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      296 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/examples/scoring/manoeuvres/positioning_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1396 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/examples/scoring/split_optimisation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.008769 flightanalysis-0.2.5/flightanalysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      211 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.008769 flightanalysis-0.2.5/flightanalysis/analysis/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      127 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/analysis/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      949 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/analysis/el_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     9949 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/analysis/man_analysis.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2607 2024-01-27 20:42:45.000000 flightanalysis-0.2.5/flightanalysis/analysis/sch_analysis.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.016770 flightanalysis-0.2.5/flightanalysis/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    73468 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/IMAC_Unlimited2024_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      416 2023-11-09 20:21:46.000000 flightanalysis-0.2.5/flightanalysis/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    60657 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3a_a25_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)   100262 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3a_f25_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    87146 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3a_p23_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    94295 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3a_p25_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    45162 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3auk_clubman_schedule.json
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    40452 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/data/f3auk_inter_schedule.json
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.016770 flightanalysis-0.2.5/flightanalysis/definition/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      450 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/definition/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.016770 flightanalysis-0.2.5/flightanalysis/definition/builders/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/builders/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    10592 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/definition/builders/elbuilders.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/builders/lines.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     9692 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/definition/builders/manbuilder.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2142 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/collectors.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6433 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/definition/eldef.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5365 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/definition/mandef.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     4850 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/definition/maninfo.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6586 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/definition/manparm.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.020770 flightanalysis-0.2.5/flightanalysis/definition/operations/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       52 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/operations/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1652 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/operations/funopp.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1348 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/operations/itemopp.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2531 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/operations/mathopp.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3248 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/definition/operations/operation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5653 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/definition/scheddef.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.020770 flightanalysis-0.2.5/flightanalysis/elements/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      257 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/elements/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2256 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/flightanalysis/elements/autorotation.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6505 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/elements/element.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2812 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/elements/line.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5349 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/elements/loop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2581 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/flightanalysis/elements/nose_drop.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2029 2024-01-27 20:42:45.000000 flightanalysis-0.2.5/flightanalysis/elements/pitch_break.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1832 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/flightanalysis/elements/recovery.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2105 2024-01-27 20:42:45.000000 flightanalysis-0.2.5/flightanalysis/elements/stall_turn.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6467 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/manoeuvre.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1804 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/schedule.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.024771 flightanalysis-0.2.5/flightanalysis/scoring/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      219 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.024771 flightanalysis-0.2.5/flightanalysis/scoring/criteria/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      334 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1321 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/criteria.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      732 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/exponential.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1640 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/f3a_criteria.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.024771 flightanalysis-0.2.5/flightanalysis/scoring/criteria/inter/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/inter/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2071 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/inter/combination.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      467 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/inter/comparison.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.024771 flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-12-19 08:57:31.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2644 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/bounded.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3573 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/continuous.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1189 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/single.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1204 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/downgrade.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     9841 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/flightanalysis/scoring/measurement.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     6224 2024-01-16 15:47:18.000000 flightanalysis-0.2.5/flightanalysis/scoring/results.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.008769 flightanalysis-0.2.5/flightanalysis.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)      464 2024-03-20 20:38:19.000000 flightanalysis-0.2.5/flightanalysis.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3645 2024-03-20 20:38:19.000000 flightanalysis-0.2.5/flightanalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-03-20 20:38:19.000000 flightanalysis-0.2.5/flightanalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       27 2024-03-20 20:38:19.000000 flightanalysis-0.2.5/flightanalysis.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      444 2024-03-20 20:38:20.028771 flightanalysis-0.2.5/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      687 2023-06-14 11:51:46.000000 flightanalysis-0.2.5/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:38:20.028771 flightanalysis-0.2.5/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5944 2024-03-20 20:37:45.000000 flightanalysis-0.2.5/tests/test_criiteria.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      189 2024-02-18 20:32:51.000000 flightanalysis-0.2.5/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/el_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.035287 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/manoeuvre_analysis/scored.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/analysis/sch_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    72721 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/IMAC_Unlimited2024_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60591 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_a25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   100154 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_f25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    87050 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_p23_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3a_p25_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45110 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3auk_clubman_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40407 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/data/f3auk_inter_schedule.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/definition/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.039287 flightanalysis-0.2.6/flightanalysis/definition/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10578 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/elbuilders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/builders/manbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/eldef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/mandef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/maninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/manoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/manparm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/definition/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/funopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/itemopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/mathopp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/scheddef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/definition/scheduleinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/autorotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/nose_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/pitch_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/elements/stall_turn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/manoeuvre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.043287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/f3a_criteria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/bounded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/downgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/flightanalysis/scoring/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/flightanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 12:15:24.000000 flightanalysis-0.2.6/flightanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/batch_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/scripts/collect_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:15:24.047287 flightanalysis-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/tests/test_criiteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 12:14:41.000000 flightanalysis-0.2.6/tests/test_data.py
```

### Comparing `flightanalysis-0.2.5/LICENSE` & `flightanalysis-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/analysis/el_analysis.py` & `flightanalysis-0.2.6/flightanalysis/analysis/el_analysis.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/data/IMAC_Unlimited2024_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/IMAC_Unlimited2024_schedule.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731712962962963%*

 * *Differences: {"'Imm'": "{'mps': {'point_length': {'defaul': 20.0, delete: ['default']}, 'partial_roll_rate': "*

 * *          "{'defaul': 3.141592653589793, delete: ['default']}, 'full_roll_rate': {'defaul': "*

 * *          "3.141592653589793, delete: ['default']}, 'snap_rate': {'defaul': 12.566370614359172, "*

 * *          "delete: ['default']}, 'e_0_rolls': {'defaul': 0, delete: ['default']}, 'e_2_rolls': "*

 * *          "{'defaul': 0, delete: ['default']}}}",*

 * * "'Loop'": "{'mps': {'snap_rate': {'defaul': 12.566370614359172, delete: [' […]*

```diff
@@ -146,15 +146,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0_autorotation.roll": "e_2_0_autorotation.roll"
                 },
                 "criteria": {
@@ -169,15 +169,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -187,15 +187,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -205,15 +205,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_2_pause.length": "(e_0_2_pause.length+30)",
                     "e_0_3_pause.length": "(e_0_3_pause.length+30)"
@@ -222,30 +222,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_2_0_autorotation.rate": "e_2_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "Loop": {
         "eds": {
             "e_0_0": {
@@ -373,30 +373,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "e_0_radius"
             },
             "snap_rate": {
                 "collectors": {
                     "e_0_2_autorotation.rate": "e_0_2_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "TD": {
         "eds": {
             "e_0": {
@@ -604,15 +604,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll",
                     "e_1_2.roll": "e_1_2.roll"
@@ -633,15 +633,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -649,15 +649,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll",
                     "e_3_2_autorotation.roll": "e_3_2_autorotation.roll"
@@ -678,15 +678,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_1_2.rate": "e_1_2.rate",
@@ -697,15 +697,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_1_2.rate": "e_1_2.rate",
@@ -716,15 +716,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_1_2_pause.length": "(e_1_2_pause.length+30)",
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)",
@@ -734,30 +734,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_3_2_autorotation.rate": "e_3_2_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "dhb": {
         "eds": {
             "e_0_autorotation": {
@@ -975,15 +975,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 1,
+                "defaul": 1,
                 "name": "directions"
             },
             "e_1_pad_length": {
                 "collectors": {
                     "e_1_pad1.length": "(e_1_pad1.length+40)",
                     "e_1_pad2.length": "(e_1_pad2.length+40)"
                 },
@@ -991,15 +991,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0_autorotation.roll": "e_1_0_autorotation.roll"
                 },
                 "criteria": {
@@ -1014,15 +1014,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1030,15 +1030,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0_autorotation.roll": "e_3_0_autorotation.roll"
                 },
                 "criteria": {
@@ -1053,15 +1053,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -1069,30 +1069,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_5_roll.rate": "e_5_roll.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 6.283185307179586,
+                "defaul": 6.283185307179586,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0_break.length)+e_1_0_autorotation.length)+e_1_0_recovery.length)+e_1_pad2.length)",
                     "e_3": "(((((0+e_3_pad1.length)+e_3_0_break.length)+e_3_0_autorotation.length)+e_3_0_recovery.length)+e_3_pad2.length)"
                 },
@@ -1100,15 +1100,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_0_autorotation.rate": "e_1_0_autorotation.rate",
                     "e_3_0_autorotation.rate": "e_3_0_autorotation.rate"
                 },
@@ -1116,30 +1116,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "hcu": {
         "eds": {
             "e_0_0_autorotation": {
@@ -1289,15 +1289,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_pad_length": {
                 "collectors": {
                     "e_2_pad1.length": "(e_2_pad1.length+40)",
                     "e_2_pad2.length": "(e_2_pad2.length+40)"
                 },
@@ -1305,15 +1305,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_2_pad_length"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0.roll": "e_2_0.roll",
                     "e_2_1.roll": "e_2_1.roll",
                     "e_2_2.roll": "e_2_2.roll"
@@ -1334,15 +1334,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_2_0.rate": "e_2_0.rate",
                     "e_2_1.rate": "e_2_1.rate",
                     "e_2_2.rate": "e_2_2.rate"
@@ -1351,15 +1351,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.9269908169872414,
+                "defaul": 3.9269908169872414,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_2_0.rate": "e_2_0.rate",
                     "e_2_1.rate": "e_2_1.rate"
                 },
@@ -1367,15 +1367,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.9269908169872414,
+                "defaul": 3.9269908169872414,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_2_1_pause.length": "(e_2_1_pause.length+30)",
                     "e_2_2_pause.length": "(e_2_2_pause.length+30)"
                 },
@@ -1383,30 +1383,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 10,
+                "defaul": 10,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_0_0_autorotation.rate": "e_0_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "lhb": {
         "eds": {
             "e_0": {
@@ -1614,15 +1614,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0_autorotation.roll": "e_1_0_autorotation.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -1640,15 +1640,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1656,15 +1656,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll",
                     "e_3_2.roll": "e_3_2.roll",
@@ -1688,15 +1688,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_1.rate": "e_1_1.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate",
@@ -1707,15 +1707,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_1.rate": "e_1_1.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate",
@@ -1726,15 +1726,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)",
                     "e_3_2_pause.length": "(e_3_2_pause.length+30)",
@@ -1744,30 +1744,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_0_autorotation.rate": "e_1_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "qLoop": {
         "eds": {
             "e_0_0": {
@@ -1941,15 +1941,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_pad_length": {
                 "collectors": {
                     "e_2_pad1.length": "(e_2_pad1.length+40)",
                     "e_2_pad2.length": "(e_2_pad2.length+40)"
                 },
@@ -1957,15 +1957,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_2_pad_length"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0.roll": "e_2_0.roll",
                     "e_2_1.roll": "e_2_1.roll"
                 },
@@ -1983,15 +1983,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_2_0.rate": "e_2_0.rate",
@@ -2001,15 +2001,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_2_0.rate": "e_2_0.rate",
@@ -2019,15 +2019,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_2_pause.length": "(e_0_2_pause.length+30)",
                     "e_2_1_pause.length": "(e_2_1_pause.length+30)"
@@ -2036,43 +2036,43 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_0_2_autorotation.rate": "e_0_2_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "rcirc": {
         "eds": {
-            "e_0_rolls": {
+            "e_0": {
                 "Kind": "Loop",
-                "name": "e_0_rolls",
+                "name": "e_0",
                 "props": {
                     "angle": "directions[0]",
                     "ke": "1.5707963267948966",
-                    "radius": "e_0_radius",
+                    "radius": "loop_radius",
                     "roll": "directions[1]",
                     "speed": "30.0"
                 }
             },
             "e_1": {
                 "Kind": "Loop",
                 "name": "e_1",
@@ -2080,21 +2080,21 @@
                     "angle": "directions[2]",
                     "ke": "1.5707963267948966",
                     "radius": "loop_radius",
                     "roll": "0",
                     "speed": "30.0"
                 }
             },
-            "e_2_rolls": {
+            "e_2": {
                 "Kind": "Loop",
-                "name": "e_2_rolls",
+                "name": "e_2",
                 "props": {
                     "angle": "directions[3]",
                     "ke": "1.5707963267948966",
-                    "radius": "e_2_radius",
+                    "radius": "loop_radius",
                     "roll": "directions[4]",
                     "speed": "30.0"
                 }
             }
         },
         "info": {
             "centre_points": [],
@@ -2113,19 +2113,19 @@
                 "h": "BTM",
                 "o": "UPRIGHT"
             }
         },
         "mps": {
             "directions": {
                 "collectors": {
-                    "e_0_rolls.angle": "e_0_rolls.angle",
-                    "e_0_rolls.roll": "e_0_rolls.roll",
+                    "e_0.angle": "e_0.angle",
+                    "e_0.roll": "e_0.roll",
                     "e_1.angle": "e_1.angle",
-                    "e_2_rolls.angle": "e_2_rolls.angle",
-                    "e_2_rolls.roll": "e_2_rolls.roll"
+                    "e_2.angle": "e_2.angle",
+                    "e_2.roll": "e_2.roll"
                 },
                 "criteria": {
                     "desired": [
                         [
                             3.078760800517997,
                             -6.283185307179586,
                             0.12566370614359174,
@@ -2143,60 +2143,32 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 1,
+                "defaul": 1,
                 "name": "directions"
             },
-            "e_0_radius": {
-                "collectors": {
-                    "e_0_rolls.radius": "e_0_rolls.radius"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 1,
-                        "factor": 0,
-                        "limit": 10
-                    }
-                },
-                "default": 100,
-                "name": "e_0_radius"
-            },
-            "e_2_radius": {
-                "collectors": {
-                    "e_2_rolls.radius": "e_2_rolls.radius"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 1,
-                        "factor": 0,
-                        "limit": 10
-                    }
-                },
-                "default": 100,
-                "name": "e_2_radius"
-            },
             "loop_radius": {
                 "collectors": {
-                    "e_1.radius": "e_1.radius"
+                    "e_0.radius": "e_0.radius",
+                    "e_1.radius": "e_1.radius",
+                    "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             }
         }
     },
     "sTooth": {
         "eds": {
             "e_0": {
@@ -2404,15 +2376,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll",
                     "e_1_2.roll": "e_1_2.roll",
@@ -2436,15 +2408,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2452,15 +2424,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1_autorotation.roll": "e_3_1_autorotation.roll"
                 },
@@ -2478,15 +2450,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_1_2.rate": "e_1_2.rate",
@@ -2497,15 +2469,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 4.71238898038469,
+                "defaul": 4.71238898038469,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_1_2.rate": "e_1_2.rate",
@@ -2515,15 +2487,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_1_2_pause.length": "(e_1_2_pause.length+30)",
                     "e_1_3_pause.length": "(e_1_3_pause.length+30)",
@@ -2533,30 +2505,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_3_1_autorotation.rate": "e_3_1_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "sTurn": {
         "eds": {
             "e_0": {
@@ -2725,15 +2697,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1_autorotation.roll": "e_1_1_autorotation.roll"
                 },
@@ -2751,15 +2723,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2767,15 +2739,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll"
                 },
@@ -2793,15 +2765,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate"
@@ -2810,15 +2782,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate"
@@ -2827,15 +2799,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)"
                 },
@@ -2843,43 +2815,43 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_1_autorotation.rate": "e_1_1_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_2.yaw_rate": "e_2.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 6.283185307179586,
+                "defaul": 6.283185307179586,
                 "name": "stallturn_rate"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3a_a25_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3a_a25_schedule.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333338%*

 * *Differences: {"'Com'": "{'mps': {'loop_radius': {'defaul': 50, delete: ['default']}, 'line_length': {'defaul': "*

 * *          "180.0, delete: ['default']}}}",*

 * * "'Z'": "{'mps': {'loop_radius': {'defaul': 40, delete: ['default']}, 'line_length': {'defaul': "*

 * *        "130.0, delete: ['default']}, 'partial_roll_rate': {'defaul': 1.5707963267948966, delete: "*

 * *        "['default']}, 'e_1_rolls': {'defaul': 0, delete: ['default']}, 'e_1_pad_length': "*

 * *        "{'defaul': None, delete: ['default']}}}",*

 * * "'dImm'": "{'mps': {'loop_r […]*

```diff
@@ -81,15 +81,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 180.0,
+                "defaul": 180.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -98,15 +98,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 50,
+                "defaul": 50,
                 "name": "loop_radius"
             }
         }
     },
     "Z": {
         "eds": {
             "e_0": {
@@ -192,15 +192,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -215,30 +215,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -246,30 +246,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 40,
+                "defaul": 40,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "dImm": {
         "eds": {
             "e_0_0": {
@@ -366,15 +366,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0.roll": "e_2_0.roll"
                 },
                 "criteria": {
@@ -389,15 +389,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll"
                 },
                 "criteria": {
@@ -412,15 +412,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_1.radius": "e_1.radius",
                     "e_4.radius": "e_4.radius"
                 },
@@ -428,15 +428,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_2_0.rate": "e_2_0.rate",
                     "e_5_0.rate": "e_5_0.rate"
@@ -445,15 +445,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "fig9": {
         "eds": {
             "e_0": {
@@ -534,15 +534,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -557,30 +557,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -588,30 +588,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "figS": {
         "eds": {
             "e_0": {
@@ -669,15 +669,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "hB": {
         "eds": {
             "e_0": {
@@ -778,15 +778,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -801,15 +801,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -817,15 +817,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -834,30 +834,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hClov": {
         "eds": {
             "e_0": {
@@ -968,15 +968,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -986,15 +986,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "hSqL": {
         "eds": {
             "e_0": {
@@ -1075,15 +1075,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1098,30 +1098,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1129,30 +1129,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hSqL2": {
         "eds": {
             "e_0": {
@@ -1235,15 +1235,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 91.92388155425118,
+                "defaul": 91.92388155425118,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1252,15 +1252,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "iSpin": {
         "eds": {
             "e_0_autorotation": {
@@ -1339,30 +1339,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "loop": {
         "eds": {
             "e_0_0": {
@@ -1451,15 +1451,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_4_rolls": {
                 "collectors": {
                     "e_4_0.roll": "e_4_0.roll"
                 },
                 "criteria": {
@@ -1474,15 +1474,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_4_rolls"
             },
             "ee_pause": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_3.length": "e_3.length"
                 },
@@ -1490,30 +1490,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "ee_pause"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_4_0.rate": "e_4_0.rate"
                 },
@@ -1521,15 +1521,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "rEt": {
         "eds": {
             "e_0": {
@@ -1611,15 +1611,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1628,15 +1628,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "rollC": {
         "eds": {
             "e_0_0": {
@@ -1752,15 +1752,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -1770,15 +1770,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_2_pause.length": "(e_0_2_pause.length+30)",
                     "e_0_3_pause.length": "(e_0_3_pause.length+30)"
@@ -1787,15 +1787,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "sqL": {
         "eds": {
             "e_0": {
@@ -1962,15 +1962,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1985,15 +1985,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -2001,15 +2001,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll"
                 },
                 "criteria": {
@@ -2024,15 +2024,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)",
                     "e_5": "(((0+e_5_pad1.length)+e_5_0.length)+e_5_pad2.length)",
@@ -2042,15 +2042,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 80,
+                "defaul": 80,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -2061,15 +2061,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate",
                     "e_5_0.rate": "e_5_0.rate"
                 },
@@ -2077,15 +2077,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "stall": {
         "eds": {
             "e_0": {
@@ -2183,15 +2183,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -2206,15 +2206,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_4.radius": "e_4.radius"
                 },
@@ -2222,45 +2222,45 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_2.yaw_rate": "e_2.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     },
     "tHat": {
         "eds": {
             "e_0": {
@@ -2381,15 +2381,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2404,15 +2404,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_5.length": "e_5.length"
                 },
@@ -2420,15 +2420,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -2438,30 +2438,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "trgle": {
         "eds": {
             "e_0": {
@@ -2590,15 +2590,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -2613,30 +2613,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_5.length": "e_5.length"
                 },
@@ -2644,15 +2644,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 150,
+                "defaul": 150,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -2662,13 +2662,13 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3a_f25_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3a_f25_schedule.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333338%*

 * *Differences: {"'Aval'": "{'mps': {'loop_radius': {'defaul': 100, delete: ['default']}, 'snap_rate': {'defaul': "*

 * *           "12.566370614359172, delete: ['default']}, 'roll_option': {'defaul': 0, delete: "*

 * *           "['default']}, 'e_2_rolls': {'defaul': 0, delete: ['default']}}}",*

 * * "'dl45'": "{'mps': {'loop_radius': {'defaul': 55.0, delete: ['default']}, 'line_length': "*

 * *           "{'defaul': 281.11984104714446, delete: ['default']}, 'partial_roll_rate': {'defaul': "*

 * *           "1.5707963267948966, delete: ['default' […]*

```diff
@@ -115,15 +115,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_1.radius": "e_1.radius",
                     "e_3.radius": "e_3.radius",
@@ -133,15 +133,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "roll_option": {
                 "collectors": {
                     "e_0.roll": "e_0.roll",
                     "e_1.angle": "e_1.angle",
                     "e_3.angle": "e_3.angle",
@@ -168,30 +168,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             },
             "snap_rate": {
                 "collectors": {
                     "e_2_0_autorotation.rate": "e_2_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "dl45": {
         "eds": {
             "e_0": {
@@ -283,15 +283,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -309,15 +309,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate"
                 },
@@ -325,30 +325,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "((((0+e_1_pad1.length)+e_1_0.length)+e_1_1.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 281.11984104714446,
+                "defaul": 281.11984104714446,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -356,30 +356,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_1.rate": "e_1_1.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "fig9": {
         "eds": {
             "e_0": {
@@ -469,15 +469,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -495,45 +495,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "((((0+e_1_pad1.length)+e_1_0.length)+e_1_1.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -541,30 +541,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_1.rate": "e_1_1.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             }
         }
     },
     "h8L": {
         "eds": {
             "e_0": {
@@ -703,15 +703,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -719,15 +719,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_roll.length)+e_1_pad2.length)",
                     "e_3.length": "e_3.length",
                     "e_5": "(((0+e_5_pad1.length)+e_5_roll.length)+e_5_pad2.length)"
@@ -736,15 +736,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 65,
+                "defaul": 65,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -754,15 +754,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 35,
+                "defaul": 35,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_roll.rate": "e_1_roll.rate",
                     "e_5_roll.rate": "e_5_roll.rate"
                 },
@@ -770,15 +770,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_1_roll.roll": "e_1_roll.roll",
                     "e_2.angle": "e_2.angle",
                     "e_4.angle": "e_4.angle",
@@ -802,15 +802,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "hB": {
         "eds": {
             "e_0": {
@@ -951,15 +951,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0_autorotation.roll": "e_1_0_autorotation.roll"
                 },
                 "criteria": {
@@ -974,15 +974,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -990,15 +990,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1013,30 +1013,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0_break.length)+e_1_0_autorotation.length)+e_1_0_recovery.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1044,15 +1044,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1061,30 +1061,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_0_autorotation.rate": "e_1_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "hB2": {
         "eds": {
             "e_0": {
@@ -1203,15 +1203,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1226,15 +1226,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1242,15 +1242,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1265,30 +1265,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1296,15 +1296,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1313,30 +1313,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hCirc": {
         "eds": {
             "e_0": {
@@ -1410,15 +1410,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "roll_option": {
                 "collectors": {
                     "e_0.angle": "e_0.angle",
                     "e_0.roll": "e_0.roll",
                     "e_1.angle": "e_1.angle",
@@ -1448,15 +1448,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 1,
+                "defaul": 1,
                 "name": "roll_option"
             }
         }
     },
     "hLoop": {
         "eds": {
             "e_0": {
@@ -1498,15 +1498,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "hSLoop": {
         "eds": {
             "e_0": {
@@ -1596,15 +1596,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -1622,45 +1622,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "((((0+e_1_pad1.length)+e_1_0.length)+e_1_1.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1668,30 +1668,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_1.rate": "e_1_1.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             }
         }
     },
     "keS": {
         "eds": {
             "e_0_roll": {
@@ -1751,15 +1751,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 122.5,
+                "defaul": 122.5,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_roll.rate": "e_0_roll.rate",
                     "e_2_roll.rate": "e_2_roll.rate"
                 },
@@ -1767,15 +1767,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_0_roll.roll": "e_0_roll.roll",
                     "e_1.angle": "e_1.angle",
                     "e_2_roll.roll": "e_2_roll.roll"
@@ -1796,15 +1796,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "keTrg": {
         "eds": {
             "e_0": {
@@ -1928,15 +1928,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1951,15 +1951,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1967,15 +1967,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1990,15 +1990,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -2006,15 +2006,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -2023,15 +2023,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -2039,15 +2039,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_0.roll": "e_0.roll",
                     "e_2.angle": "e_2.angle",
                     "e_4.angle": "e_4.angle",
@@ -2071,15 +2071,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             },
             "top_roll_option": {
                 "collectors": {
                     "e_2.roll": "e_2.roll"
                 },
                 "criteria": {
@@ -2094,15 +2094,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "top_roll_option"
             }
         }
     },
     "rollC": {
         "eds": {
             "e_0_0": {
@@ -2284,15 +2284,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -2306,15 +2306,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_3_pause.length": "(e_0_3_pause.length+30)",
                     "e_0_4_pause.length": "(e_0_4_pause.length+30)",
@@ -2325,15 +2325,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "sFin": {
         "eds": {
             "e_0": {
@@ -2495,15 +2495,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2518,15 +2518,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2534,15 +2534,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0_autorotation.roll": "e_3_0_autorotation.roll",
                     "e_3_1_autorotation.roll": "e_3_1_autorotation.roll"
                 },
@@ -2560,45 +2560,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 80,
+                "defaul": 80,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -2607,15 +2607,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 40,
+                "defaul": 40,
                 "name": "loop_radius"
             },
             "snap_rate": {
                 "collectors": {
                     "e_3_0_autorotation.rate": "e_3_0_autorotation.rate",
                     "e_3_1_autorotation.rate": "e_3_1_autorotation.rate"
                 },
@@ -2623,15 +2623,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "sLoop": {
         "eds": {
             "e_0": {
@@ -2764,15 +2764,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 70,
+                "defaul": 70,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -2783,15 +2783,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "roll_option": {
                 "collectors": {
                     "e_0.roll": "e_0.roll",
                     "e_2.angle": "e_2.angle",
                     "e_4.angle": "e_4.angle",
@@ -2821,15 +2821,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "sV8": {
         "eds": {
             "e_0": {
@@ -3151,15 +3151,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_11_pad_length"
             },
             "e_11_rolls": {
                 "collectors": {
                     "e_11_0.roll": "e_11_0.roll"
                 },
                 "criteria": {
@@ -3174,15 +3174,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_11_rolls"
             },
             "e_13_pad_length": {
                 "collectors": {
                     "e_13_pad1.length": "(e_13_pad1.length+40)",
                     "e_13_pad2.length": "(e_13_pad2.length+40)"
                 },
@@ -3190,15 +3190,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_13_pad_length"
             },
             "e_13_rolls": {
                 "collectors": {
                     "e_13_0.roll": "e_13_0.roll"
                 },
                 "criteria": {
@@ -3213,15 +3213,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_13_rolls"
             },
             "e_1_pad_length": {
                 "collectors": {
                     "e_1_pad1.length": "(e_1_pad1.length+40)",
                     "e_1_pad2.length": "(e_1_pad2.length+40)"
                 },
@@ -3229,15 +3229,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -3252,15 +3252,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -3268,15 +3268,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -3291,15 +3291,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -3307,15 +3307,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_7_pad_length": {
                 "collectors": {
                     "e_7_pad1.length": "(e_7_pad1.length+40)",
                     "e_7_pad2.length": "(e_7_pad2.length+40)"
                 },
@@ -3323,15 +3323,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_7_pad_length"
             },
             "e_7_rolls": {
                 "collectors": {
                     "e_7_0.roll": "e_7_0.roll"
                 },
                 "criteria": {
@@ -3346,15 +3346,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_7_rolls"
             },
             "e_9_pad_length": {
                 "collectors": {
                     "e_9_pad1.length": "(e_9_pad1.length+40)",
                     "e_9_pad2.length": "(e_9_pad2.length+40)"
                 },
@@ -3362,15 +3362,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_9_pad_length"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_11_0.rate": "e_11_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_7_0.rate": "e_7_0.rate"
@@ -3379,15 +3379,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 4.71238898038469,
+                "defaul": 4.71238898038469,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_11": "(((0+e_11_pad1.length)+e_11_0.length)+e_11_pad2.length)",
                     "e_13": "(((0+e_13_pad1.length)+e_13_0.length)+e_13_pad2.length)",
@@ -3400,15 +3400,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 60,
+                "defaul": 60,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_10.radius": "e_10.radius",
                     "e_12.radius": "e_12.radius",
@@ -3422,15 +3422,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 35,
+                "defaul": 35,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_13_0.rate": "e_13_0.rate",
                     "e_1_0.rate": "e_1_0.rate",
                     "e_5_roll.rate": "e_5_roll.rate",
@@ -3440,15 +3440,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 4.71238898038469,
+                "defaul": 4.71238898038469,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_5_roll.roll": "e_5_roll.roll",
                     "e_6.angle": "e_6.angle",
                     "e_8.angle": "e_8.angle",
@@ -3472,15 +3472,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "spin": {
         "eds": {
             "e_0_autorotation": {
@@ -3576,15 +3576,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -3599,60 +3599,60 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "stall": {
         "eds": {
             "e_0_0": {
@@ -3866,15 +3866,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -3882,15 +3882,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll",
                     "e_3_2.roll": "e_3_2.roll"
@@ -3911,15 +3911,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -3927,15 +3927,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0_autorotation.roll": "e_5_0_autorotation.roll"
                 },
                 "criteria": {
@@ -3950,15 +3950,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "e_8_rolls": {
                 "collectors": {
                     "e_8_0.roll": "e_8_0.roll"
                 },
                 "criteria": {
@@ -3973,15 +3973,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_8_rolls"
             },
             "ee_pause": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_7.length": "e_7.length"
                 },
@@ -3989,15 +3989,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 10,
+                "defaul": 10,
                 "name": "ee_pause"
             },
             "line_length": {
                 "collectors": {
                     "e_3": "(((((((0+e_3_pad1.length)+e_3_0.length)+e_3_1_pause.length)+e_3_1.length)+e_3_2_pause.length)+e_3_2.length)+e_3_pad2.length)",
                     "e_5": "(((((0+e_5_pad1.length)+e_5_0_break.length)+e_5_0_autorotation.length)+e_5_0_recovery.length)+e_5_pad2.length)"
                 },
@@ -4005,15 +4005,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 150,
+                "defaul": 150,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius",
                     "e_6.radius": "e_6.radius"
                 },
@@ -4021,15 +4021,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate",
@@ -4040,15 +4040,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)",
                     "e_3_2_pause.length": "(e_3_2_pause.length+30)"
                 },
@@ -4056,43 +4056,43 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             },
             "snap_rate": {
                 "collectors": {
                     "e_5_0_autorotation.rate": "e_5_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_4.yaw_rate": "e_4.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3a_p23_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3a_p23_schedule.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333338%*

 * *Differences: {"'M'": "{'mps': {'loop_radius': {'defaul': 55.0, delete: ['default']}, 'line_length': {'defaul': "*

 * *        "150.0, delete: ['default']}, 'partial_roll_rate': {'defaul': 1.5707963267948966, delete: "*

 * *        "['default']}, 'stallturn_rate': {'defaul': 3.141592653589793, delete: ['default']}, "*

 * *        "'roll_option': {'defaul': 1, delete: ['default']}, 'e_1_pad_length': {'defaul': None, "*

 * *        "delete: ['default']}, 'e_7_pad_length': {'defaul': None, delete: ['default']}}}",*

 * * "'fTrn'": "{'mps': {'loop_ra […]*

```diff
@@ -153,15 +153,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_7_pad_length": {
                 "collectors": {
                     "e_7_pad1.length": "(e_7_pad1.length+40)",
                     "e_7_pad2.length": "(e_7_pad2.length+40)"
                 },
@@ -169,15 +169,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_7_pad_length"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_roll.length)+e_1_pad2.length)",
                     "e_3.length": "e_3.length",
                     "e_5.length": "e_5.length",
@@ -187,15 +187,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 150.0,
+                "defaul": 150.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_4.radius": "e_4.radius",
                     "e_8.radius": "e_8.radius"
@@ -204,15 +204,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_roll.rate": "e_1_roll.rate",
                     "e_7_roll.rate": "e_7_roll.rate"
                 },
@@ -220,15 +220,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_1_roll.roll": "e_1_roll.roll",
                     "e_7_roll.roll": "e_7_roll.roll"
                 },
@@ -246,15 +246,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 1,
+                "defaul": 1,
                 "name": "roll_option"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_2.yaw_rate": "e_2.yaw_rate",
                     "e_6.yaw_rate": "e_6.yaw_rate"
                 },
@@ -262,15 +262,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     },
     "fTrn": {
         "eds": {
             "e_0": {
@@ -389,15 +389,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -405,15 +405,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_roll.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_roll.length)+e_3_pad2.length)"
                 },
@@ -421,15 +421,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -438,15 +438,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_roll.rate": "e_1_roll.rate",
                     "e_3_roll.rate": "e_3_roll.rate"
                 },
@@ -454,15 +454,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_1_roll.roll": "e_1_roll.roll",
                     "e_3_roll.roll": "e_3_roll.roll"
                 },
@@ -480,15 +480,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "h8L": {
         "eds": {
             "e_0": {
@@ -592,15 +592,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 50,
+                "defaul": 50,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -610,15 +610,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "hB": {
         "eds": {
             "e_0": {
@@ -745,15 +745,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -768,15 +768,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -784,15 +784,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -807,30 +807,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -838,15 +838,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -855,30 +855,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hB2": {
         "eds": {
             "e_0": {
@@ -997,15 +997,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1013,15 +1013,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_roll.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_roll.length)+e_3_pad2.length)"
                 },
@@ -1029,15 +1029,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1046,15 +1046,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_roll.rate": "e_1_roll.rate",
                     "e_3_roll.rate": "e_3_roll.rate"
                 },
@@ -1062,15 +1062,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_1_roll.roll": "e_1_roll.roll",
                     "e_3_roll.roll": "e_3_roll.roll"
                 },
@@ -1104,15 +1104,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "hSqL": {
         "eds": {
             "e_0": {
@@ -1193,15 +1193,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1216,30 +1216,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1247,30 +1247,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hSqLC": {
         "eds": {
             "e_0": {
@@ -1389,15 +1389,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1412,15 +1412,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1428,15 +1428,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1451,15 +1451,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1467,15 +1467,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 91.92388155425118,
+                "defaul": 91.92388155425118,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1484,15 +1484,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -1500,15 +1500,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "iSp": {
         "eds": {
             "e_0_autorotation": {
@@ -1587,45 +1587,45 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "loop": {
         "eds": {
             "e_0": {
@@ -1697,15 +1697,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 80,
+                "defaul": 80,
                 "name": "e_1_radius"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1713,15 +1713,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 80,
+                "defaul": 80,
                 "name": "loop_radius"
             }
         }
     },
     "pImm": {
         "eds": {
             "e_0": {
@@ -1780,45 +1780,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "rEt": {
         "eds": {
             "e_0": {
@@ -1966,15 +1966,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -1992,15 +1992,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2008,15 +2008,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll"
                 },
@@ -2034,15 +2034,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -2051,15 +2051,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 70,
+                "defaul": 70,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_3_0.rate": "e_3_0.rate",
@@ -2069,30 +2069,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "rollC": {
         "eds": {
             "e_0_0": {
@@ -2196,15 +2196,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -2214,15 +2214,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_3_pause.length": "(e_0_3_pause.length+30)"
                 },
@@ -2230,15 +2230,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "sFin": {
         "eds": {
             "e_0": {
@@ -2375,15 +2375,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2398,15 +2398,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2414,15 +2414,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll"
                 },
@@ -2440,15 +2440,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -2457,15 +2457,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 30,
+                "defaul": 30,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate"
@@ -2474,30 +2474,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "sqL": {
         "eds": {
             "e_0": {
@@ -2578,15 +2578,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2601,30 +2601,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -2632,30 +2632,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "tHat": {
         "eds": {
             "e_0": {
@@ -2853,15 +2853,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -2879,15 +2879,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2895,15 +2895,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -2918,15 +2918,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -2934,15 +2934,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll",
                     "e_5_1.roll": "e_5_1.roll"
                 },
@@ -2960,15 +2960,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0.length)+e_1_1_pause.length)+e_1_1.length)+e_1_pad2.length)",
                     "e_5": "(((((0+e_5_pad1.length)+e_5_0.length)+e_5_1_pause.length)+e_5_1.length)+e_5_pad2.length)"
                 },
@@ -2976,15 +2976,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -2994,15 +2994,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_3_0.rate": "e_3_0.rate",
@@ -3013,15 +3013,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_5_1_pause.length": "(e_5_1_pause.length+30)"
                 },
@@ -3029,15 +3029,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "trgle": {
         "eds": {
             "e_0_0": {
@@ -3248,15 +3248,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -3264,15 +3264,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll"
                 },
@@ -3290,15 +3290,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -3306,15 +3306,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll",
                     "e_5_1.roll": "e_5_1.roll"
                 },
@@ -3332,15 +3332,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "e_8_rolls": {
                 "collectors": {
                     "e_8_0.roll": "e_8_0.roll"
                 },
                 "criteria": {
@@ -3355,15 +3355,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_8_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_3": "(((((0+e_3_pad1.length)+e_3_0.length)+e_3_1_pause.length)+e_3_1.length)+e_3_pad2.length)",
                     "e_5": "(((((0+e_5_pad1.length)+e_5_0.length)+e_5_1_pause.length)+e_5_1.length)+e_5_pad2.length)"
                 },
@@ -3371,15 +3371,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
                     "e_6.radius": "e_6.radius"
@@ -3388,15 +3388,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate",
@@ -3408,15 +3408,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)",
                     "e_5_1_pause.length": "(e_5_1_pause.length+30)"
                 },
@@ -3424,15 +3424,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "upL": {
         "eds": {
             "e_0": {
@@ -3535,15 +3535,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0_autorotation.roll": "e_1_0_autorotation.roll"
                 },
                 "criteria": {
@@ -3558,30 +3558,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0_break.length)+e_1_0_autorotation.length)+e_1_0_recovery.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 293.84776310850236,
+                "defaul": 293.84776310850236,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -3589,28 +3589,28 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_0_autorotation.rate": "e_1_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3a_p25_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3a_p25_schedule.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9475554128076595%*

 * *Differences: {"'Com'": "{'mps': {'loop_radius': {'defaul': 50, delete: ['default']}, 'line_length': {'defaul': "*

 * *          "180.0, delete: ['default']}, 'point_length': {'defaul': 20.0, delete: ['default']}, "*

 * *          "'partial_roll_rate': {'defaul': 1.5707963267948966, delete: ['default']}, "*

 * *          "'full_roll_rate': {'defaul': 2.356194490192345, delete: ['default']}, 'e_1_rolls': "*

 * *          "{'criteria': {'lookup': {'limit': None}}, 'defaul': 0, delete: ['default']}, "*

 * *          "'e_1_pad_length': {'defaul': No […]*

```diff
@@ -135,15 +135,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -158,18 +158,18 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -177,15 +177,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -197,33 +197,33 @@
                             -6.283185307179586
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0.length)+e_1_1_pause.length)+e_1_1.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -231,15 +231,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 180.0,
+                "defaul": 180.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -248,15 +248,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 50,
+                "defaul": 50,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate"
                 },
@@ -264,30 +264,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "Z": {
         "eds": {
             "e_0": {
@@ -390,15 +390,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0_autorotation.roll": "e_1_0_autorotation.roll"
                 },
                 "criteria": {
@@ -410,33 +410,33 @@
                             -6.283185307179586
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0_break.length)+e_1_0_autorotation.length)+e_1_0_recovery.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 60,
+                "defaul": 60,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -444,30 +444,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 50,
+                "defaul": 50,
                 "name": "loop_radius"
             },
             "snap_rate": {
                 "collectors": {
                     "e_1_0_autorotation.rate": "e_1_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 12.566370614359172,
+                "defaul": 12.566370614359172,
                 "name": "snap_rate"
             }
         }
     },
     "dImm": {
         "eds": {
             "e_0_0": {
@@ -575,18 +575,18 @@
                             -6.283185307179586
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_6_rolls": {
                 "collectors": {
                     "e_6_0.roll": "e_6_0.roll"
                 },
                 "criteria": {
@@ -598,33 +598,33 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_6_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "loop_radius": {
                 "collectors": {
                     "e_1.radius": "e_1.radius",
                     "e_5.radius": "e_5.radius"
                 },
@@ -632,15 +632,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_2_roll.rate": "e_2_roll.rate",
                     "e_4_roll.rate": "e_4_roll.rate",
                     "e_6_0.rate": "e_6_0.rate"
@@ -649,15 +649,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "roll_option": {
                 "collectors": {
                     "e_2_roll.roll": "e_2_roll.roll",
                     "e_4_roll.roll": "e_4_roll.roll"
                 },
@@ -672,18 +672,18 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "roll_option"
             }
         }
     },
     "fig9": {
         "eds": {
             "e_0": {
@@ -764,15 +764,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -784,33 +784,33 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -818,30 +818,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "figS": {
         "eds": {
             "e_0": {
@@ -851,21 +851,21 @@
                     "angle": "2.356194490192345",
                     "ke": "0",
                     "radius": "loop_radius",
                     "roll": "0.0",
                     "speed": "30.0"
                 }
             },
-            "e_1_rolls": {
+            "e_1": {
                 "Kind": "Loop",
-                "name": "e_1_rolls",
+                "name": "e_1",
                 "props": {
                     "angle": "0.7853981633974483",
                     "ke": "0",
-                    "radius": "e_1_radius",
+                    "radius": "loop_radius",
                     "roll": "rke_opt[0]",
                     "speed": "30.0"
                 }
             },
             "e_2": {
                 "Kind": "Loop",
                 "name": "e_2",
@@ -873,21 +873,21 @@
                     "angle": "rke_opt[1]",
                     "ke": "1.5707963267948966",
                     "radius": "loop_radius",
                     "roll": "0.0",
                     "speed": "30.0"
                 }
             },
-            "e_3_rolls": {
+            "e_3": {
                 "Kind": "Loop",
-                "name": "e_3_rolls",
+                "name": "e_3",
                 "props": {
                     "angle": "rke_opt[2]",
                     "ke": "1.5707963267948966",
-                    "radius": "e_3_radius",
+                    "radius": "loop_radius",
                     "roll": "rke_opt[3]",
                     "speed": "30.0"
                 }
             }
         },
         "info": {
             "centre_points": [
@@ -908,66 +908,38 @@
             "start": {
                 "d": "UPWIND",
                 "h": "BTM",
                 "o": "UPRIGHT"
             }
         },
         "mps": {
-            "e_1_radius": {
-                "collectors": {
-                    "e_1_rolls.radius": "e_1_rolls.radius"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 1,
-                        "factor": 0,
-                        "limit": 10
-                    }
-                },
-                "default": 55.0,
-                "name": "e_1_radius"
-            },
-            "e_3_radius": {
-                "collectors": {
-                    "e_3_rolls.radius": "e_3_rolls.radius"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 1,
-                        "factor": 0,
-                        "limit": 10
-                    }
-                },
-                "default": 55.0,
-                "name": "e_3_radius"
-            },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
-                    "e_2.radius": "e_2.radius"
+                    "e_1.radius": "e_1.radius",
+                    "e_2.radius": "e_2.radius",
+                    "e_3.radius": "e_3.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "rke_opt": {
                 "collectors": {
-                    "e_1_rolls.roll": "e_1_rolls.roll",
+                    "e_1.roll": "e_1.roll",
                     "e_2.angle": "e_2.angle",
-                    "e_3_rolls.angle": "e_3_rolls.angle",
-                    "e_3_rolls.roll": "e_3_rolls.roll"
+                    "e_3.angle": "e_3.angle",
+                    "e_3.roll": "e_3.roll"
                 },
                 "criteria": {
                     "desired": [
                         [
                             1.5707963267948966,
                             2.356194490192345,
                             0.7853981633974483,
@@ -980,18 +952,18 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "rke_opt"
             }
         }
     },
     "hB": {
         "eds": {
             "e_0": {
@@ -1119,15 +1091,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -1142,18 +1114,18 @@
                             3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1161,15 +1133,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1181,18 +1153,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "((((0+e_1_pad1.length)+e_1_0.length)+e_1_1.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1200,15 +1172,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1217,15 +1189,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_3_0.rate": "e_3_0.rate"
@@ -1234,15 +1206,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hClov": {
         "eds": {
             "e_0": {
@@ -1407,15 +1379,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1427,18 +1399,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1446,15 +1418,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1466,18 +1438,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -1485,15 +1457,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll"
                 },
                 "criteria": {
@@ -1505,18 +1477,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_5": "(((0+e_5_pad1.length)+e_5_0.length)+e_5_pad2.length)"
                 },
@@ -1524,15 +1496,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -1542,15 +1514,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_5_0.rate": "e_5_0.rate"
@@ -1559,15 +1531,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hSqL": {
         "eds": {
             "e_0": {
@@ -1648,15 +1620,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1668,48 +1640,48 @@
                             -6.283185307179586
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1717,15 +1689,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "hSqL2": {
         "eds": {
             "e_0": {
@@ -1844,15 +1816,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1864,18 +1836,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -1883,15 +1855,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1903,18 +1875,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1922,15 +1894,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 91.92388155425118,
+                "defaul": 91.92388155425118,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1939,15 +1911,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -1955,15 +1927,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "iSpin": {
         "eds": {
             "e_0_autorotation": {
@@ -2061,15 +2033,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2081,88 +2053,88 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "loop": {
         "eds": {
             "e_0_0": {
                 "Kind": "Loop",
                 "name": "e_0_0",
                 "props": {
                     "angle": "1.5707963267948966",
                     "ke": "0",
                     "radius": "e_0_radius",
-                    "roll": "3.141592653589793",
+                    "roll": "e_0_rolls[0]",
                     "speed": "30.0"
                 }
             },
             "e_0_1": {
                 "Kind": "Loop",
                 "name": "e_0_1",
                 "props": {
                     "angle": "1.5707963267948966",
-                    "ke": "-3.141592653589793",
+                    "ke": "(0-e_0_rolls[2])",
                     "radius": "e_0_radius",
-                    "roll": "-3.141592653589793",
+                    "roll": "e_0_rolls[1]",
                     "speed": "30.0"
                 }
             },
             "e_0_pad1": {
                 "Kind": "Loop",
                 "name": "e_0_pad1",
                 "props": {
@@ -2174,15 +2146,15 @@
                 }
             },
             "e_0_pad2": {
                 "Kind": "Loop",
                 "name": "e_0_pad2",
                 "props": {
                     "angle": "1.5707963267948966",
-                    "ke": "0.0",
+                    "ke": "(0-e_0_rolls[3])",
                     "radius": "e_0_radius",
                     "roll": "0",
                     "speed": "30.0"
                 }
             }
         },
         "info": {
@@ -2212,19 +2184,49 @@
                     "e_0_pad2.radius": "e_0_pad2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "e_0_radius"
+            },
+            "e_0_rolls": {
+                "collectors": {
+                    "e_0_0.roll": "e_0_0.roll",
+                    "e_0_1.roll": "e_0_1.roll"
+                },
+                "criteria": {
+                    "desired": [
+                        [
+                            3.141592653589793,
+                            -3.141592653589793,
+                            3.141592653589793,
+                            0.0
+                        ],
+                        [
+                            -3.141592653589793,
+                            3.141592653589793,
+                            -3.141592653589793,
+                            0.0
+                        ]
+                    ],
+                    "kind": "Combination",
+                    "lookup": {
+                        "exponent": 1,
+                        "factor": 0,
+                        "limit": null
+                    }
+                },
+                "defaul": 0,
+                "name": "e_0_rolls"
             }
         }
     },
     "rEt": {
         "eds": {
             "e_0": {
                 "Kind": "Loop",
@@ -2360,15 +2362,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2380,18 +2382,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2399,15 +2401,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll",
                     "e_3_1.roll": "e_3_1.roll"
                 },
@@ -2422,33 +2424,33 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_3": "(((((0+e_3_pad1.length)+e_3_0.length)+e_3_1_pause.length)+e_3_1.length)+e_3_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -2457,15 +2459,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_3_1.rate": "e_3_1.rate"
@@ -2474,30 +2476,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_3_1_pause.length": "(e_3_1_pause.length+30)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "rollC": {
         "eds": {
             "e_0_0": {
@@ -2640,18 +2642,18 @@
                             1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -2663,15 +2665,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_2_pause.length": "(e_0_2_pause.length+30)",
                     "e_0_4_pause.length": "(e_0_4_pause.length+30)",
@@ -2681,15 +2683,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "sqL": {
         "eds": {
             "e_0": {
@@ -2892,15 +2894,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -2912,18 +2914,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -2931,15 +2933,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -2951,18 +2953,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -2970,15 +2972,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll"
                 },
                 "criteria": {
@@ -2990,18 +2992,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "e_7_pad_length": {
                 "collectors": {
                     "e_7_pad1.length": "(e_7_pad1.length+40)",
                     "e_7_pad2.length": "(e_7_pad2.length+40)"
                 },
@@ -3009,15 +3011,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_7_pad_length"
             },
             "e_7_rolls": {
                 "collectors": {
                     "e_7_0.roll": "e_7_0.roll"
                 },
                 "criteria": {
@@ -3029,18 +3031,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_7_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)",
                     "e_5": "(((0+e_5_pad1.length)+e_5_0.length)+e_5_pad2.length)",
@@ -3050,15 +3052,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 80,
+                "defaul": 80,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -3069,15 +3071,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate",
                     "e_5_0.rate": "e_5_0.rate",
@@ -3087,15 +3089,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "stall": {
         "eds": {
             "e_0": {
@@ -3193,15 +3195,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -3213,18 +3215,18 @@
                             -3.141592653589793
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_4.radius": "e_4.radius"
                 },
@@ -3232,287 +3234,528 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_2.yaw_rate": "e_2.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     },
-    "tHat": {
-        "eds": {
-            "e_0": {
-                "Kind": "Loop",
-                "name": "e_0",
-                "props": {
-                    "angle": "1.5707963267948966",
-                    "ke": "0",
-                    "radius": "loop_radius",
-                    "roll": "0.0",
-                    "speed": "30.0"
+    "tHat": [
+        {
+            "eds": {
+                "e_0": {
+                    "Kind": "Loop",
+                    "name": "e_0",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_0": {
+                    "Kind": "Line",
+                    "name": "e_1_0",
+                    "props": {
+                        "length": "((abs(e_1_rolls[0])*30.0)/partial_roll_rate)",
+                        "roll": "e_1_rolls[0]",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_1": {
+                    "Kind": "Line",
+                    "name": "e_1_1",
+                    "props": {
+                        "length": "((abs(e_1_rolls[1])*30.0)/partial_roll_rate)",
+                        "roll": "e_1_rolls[1]",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_1_pause": {
+                    "Kind": "Line",
+                    "name": "e_1_1_pause",
+                    "props": {
+                        "length": "20.0",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_pad1": {
+                    "Kind": "Line",
+                    "name": "e_1_pad1",
+                    "props": {
+                        "length": "(0.5*(line_length-(((0+((abs(e_1_rolls[0])*30.0)/partial_roll_rate))+20.0)+((abs(e_1_rolls[1])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_pad2": {
+                    "Kind": "Line",
+                    "name": "e_1_pad2",
+                    "props": {
+                        "length": "(0.5*(line_length-(((0+((abs(e_1_rolls[0])*30.0)/partial_roll_rate))+20.0)+((abs(e_1_rolls[1])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_2": {
+                    "Kind": "Loop",
+                    "name": "e_2",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_3": {
+                    "Kind": "Line",
+                    "name": "e_3",
+                    "props": {
+                        "length": "50",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_4": {
+                    "Kind": "Loop",
+                    "name": "e_4",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_5": {
+                    "Kind": "Line",
+                    "name": "e_5",
+                    "props": {
+                        "length": "line_length",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_6": {
+                    "Kind": "Loop",
+                    "name": "e_6",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                }
+            },
+            "info": {
+                "centre_points": [],
+                "centred_els": [],
+                "end": {
+                    "d": "DRIVEN",
+                    "h": "BTM",
+                    "o": "DRIVEN"
+                },
+                "k": 3,
+                "name": "Top Hat",
+                "position": "END",
+                "short_name": "tHat",
+                "start": {
+                    "d": "UPWIND",
+                    "h": "BTM",
+                    "o": "UPRIGHT"
+                }
+            },
+            "mps": {
+                "e_1_pad_length": {
+                    "collectors": {
+                        "e_1_pad1.length": "(e_1_pad1.length+40)",
+                        "e_1_pad2.length": "(e_1_pad2.length+40)"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": null,
+                    "name": "e_1_pad_length"
+                },
+                "e_1_rolls": {
+                    "collectors": {
+                        "e_1_0.roll": "e_1_0.roll",
+                        "e_1_1.roll": "e_1_1.roll"
+                    },
+                    "criteria": {
+                        "desired": [
+                            [
+                                1.5707963267948966,
+                                1.5707963267948966
+                            ],
+                            [
+                                -1.5707963267948966,
+                                -1.5707963267948966
+                            ]
+                        ],
+                        "kind": "Combination",
+                        "lookup": {
+                            "exponent": 1,
+                            "factor": 0,
+                            "limit": null
+                        }
+                    },
+                    "defaul": 0,
+                    "name": "e_1_rolls"
+                },
+                "line_length": {
+                    "collectors": {
+                        "e_1": "(((((0+e_1_pad1.length)+e_1_0.length)+e_1_1_pause.length)+e_1_1.length)+e_1_pad2.length)",
+                        "e_5.length": "e_5.length"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": 130.0,
+                    "name": "line_length"
+                },
+                "loop_radius": {
+                    "collectors": {
+                        "e_0.radius": "e_0.radius",
+                        "e_2.radius": "e_2.radius",
+                        "e_4.radius": "e_4.radius",
+                        "e_6.radius": "e_6.radius"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.4306765580733931,
+                            "factor": 1.0,
+                            "limit": 2
+                        }
+                    },
+                    "defaul": 55.0,
+                    "name": "loop_radius"
+                },
+                "partial_roll_rate": {
+                    "collectors": {
+                        "e_1_0.rate": "e_1_0.rate",
+                        "e_1_1.rate": "e_1_1.rate"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 1.1132827525593783,
+                            "factor": 0.25,
+                            "limit": 2
+                        }
+                    },
+                    "defaul": 1.5707963267948966,
+                    "name": "partial_roll_rate"
+                },
+                "point_length": {
+                    "collectors": {
+                        "e_1_1_pause.length": "(e_1_1_pause.length+30)"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": 20.0,
+                    "name": "point_length"
+                }
+            }
+        },
+        {
+            "eds": {
+                "e_0": {
+                    "Kind": "Loop",
+                    "name": "e_0",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_pad1": {
+                    "Kind": "Line",
+                    "name": "e_1_pad1",
+                    "props": {
+                        "length": "(0.5*(line_length-(0+((abs(opt[0])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_pad2": {
+                    "Kind": "Line",
+                    "name": "e_1_pad2",
+                    "props": {
+                        "length": "(0.5*(line_length-(0+((abs(opt[0])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_1_roll": {
+                    "Kind": "Line",
+                    "name": "e_1_roll",
+                    "props": {
+                        "length": "((abs(opt[0])*30.0)/partial_roll_rate)",
+                        "roll": "opt[0]",
+                        "speed": "30.0"
+                    }
+                },
+                "e_2": {
+                    "Kind": "Loop",
+                    "name": "e_2",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_3": {
+                    "Kind": "Line",
+                    "name": "e_3",
+                    "props": {
+                        "length": "50",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_4": {
+                    "Kind": "Loop",
+                    "name": "e_4",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_5_pad1": {
+                    "Kind": "Line",
+                    "name": "e_5_pad1",
+                    "props": {
+                        "length": "(0.5*(line_length-(0+((abs(opt[1])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_5_pad2": {
+                    "Kind": "Line",
+                    "name": "e_5_pad2",
+                    "props": {
+                        "length": "(0.5*(line_length-(0+((abs(opt[1])*30.0)/partial_roll_rate))))",
+                        "roll": "0",
+                        "speed": "30.0"
+                    }
+                },
+                "e_5_roll": {
+                    "Kind": "Line",
+                    "name": "e_5_roll",
+                    "props": {
+                        "length": "((abs(opt[1])*30.0)/partial_roll_rate)",
+                        "roll": "opt[1]",
+                        "speed": "30.0"
+                    }
+                },
+                "e_6": {
+                    "Kind": "Loop",
+                    "name": "e_6",
+                    "props": {
+                        "angle": "1.5707963267948966",
+                        "ke": "0",
+                        "radius": "loop_radius",
+                        "roll": "0.0",
+                        "speed": "30.0"
+                    }
+                }
+            },
+            "info": {
+                "centre_points": [],
+                "centred_els": [],
+                "end": {
+                    "d": "DRIVEN",
+                    "h": "BTM",
+                    "o": "DRIVEN"
+                },
+                "k": 3,
+                "name": "Top Hat Option",
+                "position": "END",
+                "short_name": "tHat",
+                "start": {
+                    "d": "UPWIND",
+                    "h": "BTM",
+                    "o": "UPRIGHT"
+                }
+            },
+            "mps": {
+                "e_1_pad_length": {
+                    "collectors": {
+                        "e_1_pad1.length": "(e_1_pad1.length+40)",
+                        "e_1_pad2.length": "(e_1_pad2.length+40)"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": null,
+                    "name": "e_1_pad_length"
+                },
+                "e_5_pad_length": {
+                    "collectors": {
+                        "e_5_pad1.length": "(e_5_pad1.length+40)",
+                        "e_5_pad2.length": "(e_5_pad2.length+40)"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": null,
+                    "name": "e_5_pad_length"
+                },
+                "line_length": {
+                    "collectors": {
+                        "e_1": "(((0+e_1_pad1.length)+e_1_roll.length)+e_1_pad2.length)",
+                        "e_5": "(((0+e_5_pad1.length)+e_5_roll.length)+e_5_pad2.length)"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.6826061944859854,
+                            "factor": 1.0,
+                            "limit": 3
+                        }
+                    },
+                    "defaul": 130.0,
+                    "name": "line_length"
+                },
+                "loop_radius": {
+                    "collectors": {
+                        "e_0.radius": "e_0.radius",
+                        "e_2.radius": "e_2.radius",
+                        "e_4.radius": "e_4.radius",
+                        "e_6.radius": "e_6.radius"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 0.4306765580733931,
+                            "factor": 1.0,
+                            "limit": 2
+                        }
+                    },
+                    "defaul": 55.0,
+                    "name": "loop_radius"
+                },
+                "opt": {
+                    "collectors": {
+                        "e_1_roll.roll": "e_1_roll.roll",
+                        "e_5_roll.roll": "e_5_roll.roll"
+                    },
+                    "criteria": {
+                        "desired": [
+                            [
+                                1.5707963267948966,
+                                -1.5707963267948966
+                            ],
+                            [
+                                1.5707963267948966,
+                                1.5707963267948966
+                            ]
+                        ],
+                        "kind": "Combination",
+                        "lookup": {
+                            "exponent": 1,
+                            "factor": 0,
+                            "limit": null
+                        }
+                    },
+                    "defaul": 0,
+                    "name": "opt"
+                },
+                "partial_roll_rate": {
+                    "collectors": {
+                        "e_1_roll.rate": "e_1_roll.rate",
+                        "e_5_roll.rate": "e_5_roll.rate"
+                    },
+                    "criteria": {
+                        "kind": "Comparison",
+                        "lookup": {
+                            "exponent": 1.1132827525593783,
+                            "factor": 0.25,
+                            "limit": 2
+                        }
+                    },
+                    "defaul": 1.5707963267948966,
+                    "name": "partial_roll_rate"
                 }
-            },
-            "e_1_0": {
-                "Kind": "Line",
-                "name": "e_1_0",
-                "props": {
-                    "length": "((abs(e_1_rolls[0])*30.0)/partial_roll_rate)",
-                    "roll": "e_1_rolls[0]",
-                    "speed": "30.0"
-                }
-            },
-            "e_1_1": {
-                "Kind": "Line",
-                "name": "e_1_1",
-                "props": {
-                    "length": "((abs(e_1_rolls[1])*30.0)/partial_roll_rate)",
-                    "roll": "e_1_rolls[1]",
-                    "speed": "30.0"
-                }
-            },
-            "e_1_1_pause": {
-                "Kind": "Line",
-                "name": "e_1_1_pause",
-                "props": {
-                    "length": "20.0",
-                    "roll": "0",
-                    "speed": "30.0"
-                }
-            },
-            "e_1_pad1": {
-                "Kind": "Line",
-                "name": "e_1_pad1",
-                "props": {
-                    "length": "(0.5*(line_length-(((0+((abs(e_1_rolls[0])*30.0)/partial_roll_rate))+20.0)+((abs(e_1_rolls[1])*30.0)/partial_roll_rate))))",
-                    "roll": "0",
-                    "speed": "30.0"
-                }
-            },
-            "e_1_pad2": {
-                "Kind": "Line",
-                "name": "e_1_pad2",
-                "props": {
-                    "length": "(0.5*(line_length-(((0+((abs(e_1_rolls[0])*30.0)/partial_roll_rate))+20.0)+((abs(e_1_rolls[1])*30.0)/partial_roll_rate))))",
-                    "roll": "0",
-                    "speed": "30.0"
-                }
-            },
-            "e_2": {
-                "Kind": "Loop",
-                "name": "e_2",
-                "props": {
-                    "angle": "1.5707963267948966",
-                    "ke": "0",
-                    "radius": "loop_radius",
-                    "roll": "0.0",
-                    "speed": "30.0"
-                }
-            },
-            "e_3": {
-                "Kind": "Line",
-                "name": "e_3",
-                "props": {
-                    "length": "50",
-                    "roll": "0.0",
-                    "speed": "30.0"
-                }
-            },
-            "e_4": {
-                "Kind": "Loop",
-                "name": "e_4",
-                "props": {
-                    "angle": "1.5707963267948966",
-                    "ke": "0",
-                    "radius": "loop_radius",
-                    "roll": "0.0",
-                    "speed": "30.0"
-                }
-            },
-            "e_5": {
-                "Kind": "Line",
-                "name": "e_5",
-                "props": {
-                    "length": "line_length",
-                    "roll": "0.0",
-                    "speed": "30.0"
-                }
-            },
-            "e_6": {
-                "Kind": "Loop",
-                "name": "e_6",
-                "props": {
-                    "angle": "1.5707963267948966",
-                    "ke": "0",
-                    "radius": "loop_radius",
-                    "roll": "0.0",
-                    "speed": "30.0"
-                }
-            }
-        },
-        "info": {
-            "centre_points": [],
-            "centred_els": [],
-            "end": {
-                "d": "DRIVEN",
-                "h": "BTM",
-                "o": "DRIVEN"
-            },
-            "k": 3,
-            "name": "Top Hat",
-            "position": "END",
-            "short_name": "tHat",
-            "start": {
-                "d": "UPWIND",
-                "h": "BTM",
-                "o": "UPRIGHT"
-            }
-        },
-        "mps": {
-            "e_1_pad_length": {
-                "collectors": {
-                    "e_1_pad1.length": "(e_1_pad1.length+40)",
-                    "e_1_pad2.length": "(e_1_pad2.length+40)"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 0.6826061944859854,
-                        "factor": 1.0,
-                        "limit": 3
-                    }
-                },
-                "default": null,
-                "name": "e_1_pad_length"
-            },
-            "e_1_rolls": {
-                "collectors": {
-                    "e_1_0.roll": "e_1_0.roll",
-                    "e_1_1.roll": "e_1_1.roll"
-                },
-                "criteria": {
-                    "desired": [
-                        [
-                            1.5707963267948966,
-                            1.5707963267948966
-                        ],
-                        [
-                            -1.5707963267948966,
-                            -1.5707963267948966
-                        ]
-                    ],
-                    "kind": "Combination",
-                    "lookup": {
-                        "exponent": 1,
-                        "factor": 0,
-                        "limit": 10
-                    }
-                },
-                "default": 0,
-                "name": "e_1_rolls"
-            },
-            "line_length": {
-                "collectors": {
-                    "e_1": "(((((0+e_1_pad1.length)+e_1_0.length)+e_1_1_pause.length)+e_1_1.length)+e_1_pad2.length)",
-                    "e_5.length": "e_5.length"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 0.6826061944859854,
-                        "factor": 1.0,
-                        "limit": 3
-                    }
-                },
-                "default": 130.0,
-                "name": "line_length"
-            },
-            "loop_radius": {
-                "collectors": {
-                    "e_0.radius": "e_0.radius",
-                    "e_2.radius": "e_2.radius",
-                    "e_4.radius": "e_4.radius",
-                    "e_6.radius": "e_6.radius"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 0.4306765580733931,
-                        "factor": 1.0,
-                        "limit": 2
-                    }
-                },
-                "default": 55.0,
-                "name": "loop_radius"
-            },
-            "partial_roll_rate": {
-                "collectors": {
-                    "e_1_0.rate": "e_1_0.rate",
-                    "e_1_1.rate": "e_1_1.rate"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 1.1132827525593783,
-                        "factor": 0.25,
-                        "limit": 2
-                    }
-                },
-                "default": 1.5707963267948966,
-                "name": "partial_roll_rate"
-            },
-            "point_length": {
-                "collectors": {
-                    "e_1_1_pause.length": "(e_1_1_pause.length+30)"
-                },
-                "criteria": {
-                    "kind": "Comparison",
-                    "lookup": {
-                        "exponent": 0.6826061944859854,
-                        "factor": 1.0,
-                        "limit": 3
-                    }
-                },
-                "default": 20.0,
-                "name": "point_length"
             }
         }
-    },
+    ],
     "trgle": {
         "eds": {
             "e_0": {
                 "Kind": "Loop",
                 "name": "e_0",
                 "props": {
                     "angle": "0.7853981633974483",
@@ -3709,15 +3952,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll",
                     "e_1_1.roll": "e_1_1.roll"
                 },
@@ -3732,18 +3975,18 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -3751,15 +3994,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -3771,18 +4014,18 @@
                             -6.283185307179586
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "e_5_pad_length": {
                 "collectors": {
                     "e_5_pad1.length": "(e_5_pad1.length+40)",
                     "e_5_pad2.length": "(e_5_pad2.length+40)"
                 },
@@ -3790,15 +4033,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_5_pad_length"
             },
             "e_5_rolls": {
                 "collectors": {
                     "e_5_0.roll": "e_5_0.roll",
                     "e_5_1.roll": "e_5_1.roll"
                 },
@@ -3813,33 +4056,33 @@
                             -1.5707963267948966
                         ]
                     ],
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
-                        "limit": 10
+                        "limit": null
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_5_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((((0+e_1_pad1.length)+e_1_0.length)+e_1_1_pause.length)+e_1_1.length)+e_1_pad2.length)",
                     "e_5": "(((((0+e_5_pad1.length)+e_5_0.length)+e_5_1_pause.length)+e_5_1.length)+e_5_pad2.length)"
                 },
@@ -3847,15 +4090,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 150,
+                "defaul": 150,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -3865,15 +4108,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_1_1.rate": "e_1_1.rate",
                     "e_5_0.rate": "e_5_0.rate",
@@ -3883,15 +4126,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_1_1_pause.length": "(e_1_1_pause.length+30)",
                     "e_5_1_pause.length": "(e_5_1_pause.length+30)"
                 },
@@ -3899,13 +4142,13 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3auk_clubman_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3auk_clubman_schedule.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9844444444444449%*

 * *Differences: {"'Immel'": "{'mps': {'loop_radius': {'defaul': 100, delete: ['default']}, 'partial_roll_rate': "*

 * *            "{'defaul': 1.5707963267948966, delete: ['default']}, 'e_1_rolls': {'defaul': 0, "*

 * *            "delete: ['default']}, 'e_3_rolls': {'defaul': 0, delete: ['default']}}}",*

 * * "'fullcuban8'": "{'mps': {'loop_radius': {'defaul': 100, delete: ['default']}, 'line_length': "*

 * *                 "{'defaul': 200, delete: ['default']}, 'partial_roll_rate': {'defaul': "*

 * *                 "1.5707963267948966, delete: […]*

```diff
@@ -86,15 +86,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -109,15 +109,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_4.radius": "e_4.radius"
                 },
@@ -125,15 +125,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -141,15 +141,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "fullcuban8": {
         "eds": {
             "e_0": {
@@ -277,15 +277,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -300,15 +300,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -316,15 +316,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -339,15 +339,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -355,15 +355,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 200,
+                "defaul": 200,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -372,15 +372,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -388,15 +388,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hcuban": {
         "eds": {
             "e_0": {
@@ -482,15 +482,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -505,15 +505,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -521,30 +521,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 45,
+                "defaul": 45,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "hsqrloop": {
         "eds": {
             "e_0": {
@@ -630,15 +630,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -653,30 +653,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -684,30 +684,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "inloop": {
         "eds": {
             "e_0": {
@@ -845,15 +845,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -868,15 +868,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3.length": "e_3.length"
                 },
@@ -884,15 +884,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -901,30 +901,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "inverted": {
         "eds": {
             "e_0_0": {
@@ -990,15 +990,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0.roll": "e_2_0.roll"
                 },
                 "criteria": {
@@ -1013,15 +1013,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_2_0.rate": "e_2_0.rate"
                 },
@@ -1029,15 +1029,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "land": {
         "eds": {
             "e_0": {
@@ -1077,15 +1077,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             }
         }
     },
     "outerhB": {
         "eds": {
             "e_0": {
@@ -1186,15 +1186,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -1209,15 +1209,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -1225,15 +1225,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1242,30 +1242,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_3_0.rate": "e_3_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "outloop": {
         "eds": {
             "e_0_0": {
@@ -1354,15 +1354,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_4_rolls": {
                 "collectors": {
                     "e_4_0.roll": "e_4_0.roll"
                 },
                 "criteria": {
@@ -1377,15 +1377,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_4_rolls"
             },
             "ee_pause": {
                 "collectors": {
                     "e_1.length": "e_1.length",
                     "e_3.length": "e_3.length"
                 },
@@ -1393,15 +1393,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "ee_pause"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_4_0.rate": "e_4_0.rate"
                 },
@@ -1409,15 +1409,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "rcuban": {
         "eds": {
             "e_0": {
@@ -1503,15 +1503,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1526,15 +1526,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1542,30 +1542,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 65,
+                "defaul": 65,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "slowroll": {
         "eds": {
             "e_0_0": {
@@ -1613,15 +1613,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             }
         }
     },
     "spin": {
         "eds": {
             "e_0_autorotation": {
@@ -1700,45 +1700,45 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "stall": {
         "eds": {
             "e_0": {
@@ -1836,30 +1836,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_4.yaw_rate": "e_4.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     },
     "trnround": {
         "eds": {
             "e_0": {
@@ -1945,15 +1945,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1968,15 +1968,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1984,28 +1984,28 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 65,
+                "defaul": 65,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/data/f3auk_inter_schedule.json` & `flightanalysis-0.2.6/flightanalysis/data/f3auk_inter_schedule.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333337%*

 * *Differences: {"'4pRoll'": "{'mps': {'point_length': {'defaul': 20.0, delete: ['default']}, 'partial_roll_rate': "*

 * *             "{'defaul': 1.5707963267948966, delete: ['default']}, 'e_0_rolls': {'defaul': 0, "*

 * *             "delete: ['default']}}}",*

 * * "'cuban'": "{'mps': {'loop_radius': {'defaul': 100, delete: ['default']}, 'line_length': "*

 * *            "{'defaul': 200, delete: ['default']}, 'partial_roll_rate': {'defaul': "*

 * *            "1.5707963267948966, delete: ['default']}, 'e_1_rolls': {'defaul': 0, delete: "*

 * *        […]*

```diff
@@ -114,15 +114,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_0_1.rate": "e_0_1.rate",
                     "e_0_2.rate": "e_0_2.rate",
@@ -132,15 +132,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             },
             "point_length": {
                 "collectors": {
                     "e_0_1_pause.length": "(e_0_1_pause.length+30)",
                     "e_0_2_pause.length": "(e_0_2_pause.length+30)",
                     "e_0_3_pause.length": "(e_0_3_pause.length+30)"
@@ -149,15 +149,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 20.0,
+                "defaul": 20.0,
                 "name": "point_length"
             }
         }
     },
     "cuban": {
         "eds": {
             "e_0": {
@@ -285,15 +285,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -308,15 +308,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "e_3_pad_length": {
                 "collectors": {
                     "e_3_pad1.length": "(e_3_pad1.length+40)",
                     "e_3_pad2.length": "(e_3_pad2.length+40)"
                 },
@@ -324,15 +324,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_3_pad_length"
             },
             "e_3_rolls": {
                 "collectors": {
                     "e_3_0.roll": "e_3_0.roll"
                 },
                 "criteria": {
@@ -347,15 +347,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_3_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3": "(((0+e_3_pad1.length)+e_3_0.length)+e_3_pad2.length)"
                 },
@@ -363,15 +363,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 200,
+                "defaul": 200,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -380,15 +380,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate",
                     "e_3_0.rate": "e_3_0.rate"
                 },
@@ -396,15 +396,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "fig6": {
         "eds": {
             "e_0": {
@@ -485,15 +485,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -508,30 +508,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -539,30 +539,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "figS": {
         "eds": {
             "e_0": {
@@ -620,15 +620,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "humpty": {
         "eds": {
             "e_0": {
@@ -711,15 +711,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -728,15 +728,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "immel": {
         "eds": {
             "e_0": {
@@ -795,45 +795,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 125,
+                "defaul": 125,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "knife": {
         "eds": {
             "e_0_0": {
@@ -904,15 +904,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "e_2_rolls": {
                 "collectors": {
                     "e_2_0.roll": "e_2_0.roll"
                 },
                 "criteria": {
@@ -927,15 +927,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_2_rolls"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate",
                     "e_2_0.rate": "e_2_0.rate"
                 },
@@ -943,15 +943,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     },
     "outloop": {
         "eds": {
             "e_0": {
@@ -993,15 +993,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 75,
+                "defaul": 75,
                 "name": "loop_radius"
             }
         }
     },
     "spin": {
         "eds": {
             "e_0_autorotation": {
@@ -1080,45 +1080,45 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 130.0,
+                "defaul": 130.0,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_2.radius": "e_2.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "spin_rate": {
                 "collectors": {
                     "e_0_autorotation.rate": "e_0_autorotation.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 5.340707511102648,
+                "defaul": 5.340707511102648,
                 "name": "spin_rate"
             }
         }
     },
     "splitS": {
         "eds": {
             "e_0_0": {
@@ -1177,45 +1177,45 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_0_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_0_0.rate": "e_0_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "loop_radius": {
                 "collectors": {
                     "e_1.radius": "e_1.radius"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 125,
+                "defaul": 125,
                 "name": "loop_radius"
             }
         }
     },
     "sqrl": {
         "eds": {
             "e_0": {
@@ -1324,15 +1324,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 100,
+                "defaul": 100,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius",
@@ -1342,15 +1342,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "stall": {
         "eds": {
             "e_0": {
@@ -1453,15 +1453,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1476,30 +1476,30 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "full_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 2.356194490192345,
+                "defaul": 2.356194490192345,
                 "name": "full_roll_rate"
             },
             "line_length": {
                 "collectors": {
                     "e_1": "(((0+e_1_pad1.length)+e_1_0.length)+e_1_pad2.length)",
                     "e_3.length": "e_3.length"
                 },
@@ -1507,15 +1507,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 200,
+                "defaul": 200,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_4.radius": "e_4.radius"
                 },
@@ -1523,30 +1523,30 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             },
             "stallturn_rate": {
                 "collectors": {
                     "e_2.yaw_rate": "e_2.yaw_rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 3.141592653589793,
+                "defaul": 3.141592653589793,
                 "name": "stallturn_rate"
             }
         }
     },
     "trgle": {
         "eds": {
             "e_0": {
@@ -1634,15 +1634,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": 150,
+                "defaul": 150,
                 "name": "line_length"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius",
                     "e_4.radius": "e_4.radius"
@@ -1651,15 +1651,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 55.0,
+                "defaul": 55.0,
                 "name": "loop_radius"
             }
         }
     },
     "trnround": {
         "eds": {
             "e_0": {
@@ -1740,15 +1740,15 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.6826061944859854,
                         "factor": 1.0,
                         "limit": 3
                     }
                 },
-                "default": null,
+                "defaul": null,
                 "name": "e_1_pad_length"
             },
             "e_1_rolls": {
                 "collectors": {
                     "e_1_0.roll": "e_1_0.roll"
                 },
                 "criteria": {
@@ -1763,15 +1763,15 @@
                     "kind": "Combination",
                     "lookup": {
                         "exponent": 1,
                         "factor": 0,
                         "limit": 10
                     }
                 },
-                "default": 0,
+                "defaul": 0,
                 "name": "e_1_rolls"
             },
             "loop_radius": {
                 "collectors": {
                     "e_0.radius": "e_0.radius",
                     "e_2.radius": "e_2.radius"
                 },
@@ -1779,28 +1779,28 @@
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 0.4306765580733931,
                         "factor": 1.0,
                         "limit": 2
                     }
                 },
-                "default": 65,
+                "defaul": 65,
                 "name": "loop_radius"
             },
             "partial_roll_rate": {
                 "collectors": {
                     "e_1_0.rate": "e_1_0.rate"
                 },
                 "criteria": {
                     "kind": "Comparison",
                     "lookup": {
                         "exponent": 1.1132827525593783,
                         "factor": 0.25,
                         "limit": 2
                     }
                 },
-                "default": 1.5707963267948966,
+                "defaul": 1.5707963267948966,
                 "name": "partial_roll_rate"
             }
         }
     }
 }
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/builders/elbuilders.py` & `flightanalysis-0.2.6/flightanalysis/definition/builders/elbuilders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from ..eldef import ElDef, ElDefs, ManParm, ManParms
-from flightanalysis.elements import *
-from flightdata import Collection
+from flightanalysis.elements import Line, Loop, StallTurn, PitchBreak, Autorotation, Recovery, NoseDrop
 from flightanalysis.definition.collectors import Collectors
-from flightanalysis.definition import Opp, ItemOpp
+from flightanalysis.definition import ItemOpp
 from flightanalysis.scoring.criteria.f3a_criteria import F3A
-from flightanalysis.scoring import Combination
 from numbers import Number
 import numpy as np
 
 
 def line(name, speed, length, roll):
     return ElDef.build(Line, name, speed, length, roll), ManParms()
 
@@ -78,15 +76,15 @@
 
 def snap_duration(roll, break_angle, break_rate, snap_rate):
     return (2 * abs(break_angle) / break_rate + abs(roll) / snap_rate)
 
 
 def short_line(name, speed, length, roll, extra_length):
     if length.__class__.__name__ == 'ManParm':
-        el = ElDef.build(Line, name, speed, length.default, roll)
+        el = ElDef.build(Line, name, speed, length.defaul, roll)
         length.append(el.get_collector('length') + extra_length), ManParms()
         return el
     else:
         return line(name, speed, length, roll)
 
 
 def parse_rolltypes(rolltypes, n):
@@ -224,35 +222,31 @@
     internal_rad = ManParm(f'{name}_radius', F3A.inter.free, rad )
 
 
     rolls = mps.parse_rolls(rolls, name, reversible) if not rolls==0 else 0
 
     try:
         rvs = rolls.value
-    except Exception as e:
+    except Exception:
         rvs = None
     
     if rvs is None:
         multi_rolls = False 
         rvs = [rolls]
     else:
         multi_rolls = True
 
 
     rolltypes = parse_rolltypes(rolltypes, len(rvs))
 
     angle = ManParm.parse(angle, mps)
 
-
-
     if not rollangle == angle:
         eds.add(loop(f"{name}_pad1", speed, internal_rad, (angle - rollangle) / 2, 0, ke)[0])
 
-
-
     if multi_rolls:
         
         #TODO cannot cope with options that change whether a pause is required or not.
         #this will need to be covered in some other way
         if mode == 'f3a':
             has_pause = np.concatenate([np.diff(np.sign(rvs)), np.ones(1)]) == 0
         else:
@@ -272,39 +266,38 @@
 
         only_rolls = []
         for i, rt in enumerate(rolltypes):
             only_rolls.append(abs(rvs[i]) if rt=='r' else 0)
         only_rolls = np.array(only_rolls)
         
         rolls.criteria.append_roll_sum(inplace=True)
-        rvs = rolls.value
+        #rvs = rolls.value
 
         loop_proportions = (np.abs(only_rolls) / np.sum(np.abs(only_rolls)))
 
         loop_angles = [remaining_rollangle * rp for rp in loop_proportions]
 
         n = len(loop_angles)
 
         for i, r in enumerate(loop_angles):    
-            roll_done = rvs[i+n-1] if i > 0 else 0
+            roll_done = rolls[i+n-1] if i > 0 else 0
             if rolltypes[i] == 'r':
                 
-                eds.add(loop(f"{name}_{i}", speed, internal_rad, r, rvs[i], ke=ke-roll_done)[0])
+                eds.add(loop(f"{name}_{i}", speed, internal_rad, r, rolls[i], ke=ke - roll_done)[0]) 
             else:
                 ed, mps = snap(
-                    f"{name}_{i}", rvs[i], break_angle, snap_rate, speed, break_rate
+                    f"{name}_{i}", rolls[i], break_angle, snap_rate, speed, break_rate
                 )
                 eds.add(ed)
                 snap_rate.collectors.add(eds[-2].get_collector("rate"))
             
             if has_pause[i]:
-                eds.add(loop(f"{name}_{i}_pause", speed, internal_rad, pause_angle, 0, ke=ke-rvs[i+n])[0])
-
+                eds.add(loop(f"{name}_{i}_pause", speed, internal_rad, pause_angle, 0, ke=ke - rolls[i+n])[0]) 
 
-        ke=ke-rvs[i+n]
+        ke=ke-rolls[i+n]
         
     else:
         eds.add(loop(f"{name}_rolls", speed, internal_rad, rollangle, rolls, ke=ke)[0])
         ke = ke - rolls
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/builders/manbuilder.py` & `flightanalysis-0.2.6/flightanalysis/definition/builders/manbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from flightanalysis.definition import ManDef, ManParm, ManParms, ElDef, ElDefs, DummyMPs, Opp
 from typing import Dict, Callable
 from functools import partial
 from .elbuilders import line, loopmaker, rollmaker, stallturn, spin
 import numpy as np
+from flightanalysis.scoring.criteria.f3a_criteria import F3A
+
 
 class MBTags:
     CENTRE=0
 
 def centred(elb):
     setattr(elb, 'centred', True)
     return elb
@@ -16,15 +18,14 @@
 
 def r(turns):
     return 2 * np.pi * np.array(turns)
 
 dp = DummyMPs()
 
 
-
 class ManBuilder():
     def __init__(self, mps: ManParms, mpmaps:Dict[str, dict]):
         self.mps = mps
         self.mpmaps = mpmaps
 
     def __getattr__(self, name):
         if name in self.mpmaps:
@@ -65,15 +66,15 @@
     def create(self, maninfo, elmakers: list[Callable[[ManDef], ElDef]], **kwargs) -> ManDef:
         mps = self.mps.copy()
         for k, v in kwargs.items():
             if isinstance(v, ManParm):
                 mps.add(v)
             elif isinstance(k, str):
                 if k in mps.data:
-                    mps[k].default=v
+                    mps[k].defaul=v
                 else:
                     mps.add(ManParm.parse(v, mps, k))
         md = ManDef(maninfo, mps)
         for i, em in enumerate(elmakers):
             if isinstance(em, int):
                 if em == MBTags.CENTRE:
                     md.info.centre_points.append(len(md.eds.data))
@@ -97,16 +98,16 @@
                         if abs(int(fac) - fac) < 0.05:
                             md.info.centre_points.append(c1 + ceid + int(fac))
                         else:
                             md.info.centred_els.append((ceid + c1, fac))  
 
         md.mps = md.mps.remove_unused()
         return md
-        
-from flightanalysis.scoring.criteria.f3a_criteria import F3A
+    
+
 
 f3amb = ManBuilder(
     ManParms([
         ManParm("speed", F3A.inter.speed, 30.0),
         ManParm("loop_radius", F3A.inter.radius, 55.0),
         ManParm("line_length", F3A.inter.length, 130.0),
         ManParm("point_length", F3A.inter.length, 20.0),
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/collectors.py` & `flightanalysis-0.2.6/flightanalysis/definition/collectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """The collectors are serializable functions that return parameters from elements"""
-from flightdata import Collection, State
+from flightdata import Collection
 from . import Opp
 from uuid import uuid1
-from typing import Self
 
 
 class Collector(Opp):
     def __init__(self, elname, pname):
         self.pname = pname
         self.elname = elname
         super().__init__(f"{self.elname}.{self.pname}")
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/eldef.py` & `flightanalysis-0.2.6/flightanalysis/definition/eldef.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import enum
 from typing import List, Callable, Union, Dict, Tuple
 import numpy as np
-from flightanalysis.elements import *
+from flightanalysis.elements import Element
 from inspect import getfullargspec
-from functools import partial
 from . import ManParm, ManParms, Opp, ItemOpp
 from flightdata import Collection
 from numbers import Number
 from . import Collector, Collectors
 import inspect
 from uuid import uuid1
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/mandef.py` & `flightanalysis-0.2.6/flightanalysis/definition/mandef.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 from flightanalysis.manoeuvre import Manoeuvre
 from flightanalysis.definition.maninfo import ManInfo
 from flightdata import State
 from geometry import Transformation, Euler, Point
 from . import ManParms, ElDef, ElDefs, Position, Direction
 
 
+
 class ManDef:
     """This is a class to define a manoeuvre for template generation and judging.
-
-    It also contains lots of helper functions for creating elements and common combinations
-    of elements.
+    It contains information on the location of the manoeuvre (ManInfo), a set
+    of parameters that are used to define the scale of the manoevre (ManParms)
+    and a list of element definitions that are used to create the elements that
+    form the manoeuvre (ElDefs).
     """
 
     def __init__(self, info: ManInfo, mps: ManParms = None, eds: ElDefs = None):
         self.info: ManInfo = info
         self.mps: ManParms = ManParms.create_defaults_f3a() if mps is None else mps
         self.eds: ElDefs = ElDefs() if eds is None else eds
 
@@ -40,19 +42,25 @@
         return dict(
             info = self.info.to_dict(),
             mps = self.mps.to_dict(),
             eds = self.eds.to_dict()
         )
 
     @staticmethod
-    def from_dict(data: dict) -> ManDef:
-        info = ManInfo.from_dict(data["info"])
-        mps = ManParms.from_dict(data["mps"])
-        eds = ElDefs.from_dict(data["eds"], mps)
-        return ManDef(info, mps, eds)
+    def from_dict(data: dict | list) -> ManDef | ManOption:
+        if isinstance(data, list):
+            return ManOption.from_dict(data)
+        elif 'options' in data and data['options'] is not None and len(data['options']) > 0:
+            opts = data.pop('options')
+            return ManOption.from_dict([data] + opts)
+        else:
+            info = ManInfo.from_dict(data["info"])
+            mps = ManParms.from_dict(data["mps"])
+            eds = ElDefs.from_dict(data["eds"], mps)
+            return ManDef(info, mps, eds)
 
     def create_entry_line(self, itrans: Transformation=None, target_depth=170) -> ElDef:
         """Create a line definition connecting Transformation to the start of this manoeuvre.
 
         The length of the line is set so that the manoeuvre is centred or extended to box
         edge as required.
 
@@ -125,7 +133,10 @@
         itrans = self.info.initial_transform(170, 1)
         man = self.create(itrans)
         template = man.create_template(itrans)
         from flightplotting import plotsec, plotdtw
         fig = plotdtw(template, template.data.element.unique())
         fig = plotsec(template, fig=fig, nmodels=20, scale=3)
         return fig
+
+
+from .manoption import ManOption  # noqa: E402
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/maninfo.py` & `flightanalysis-0.2.6/flightanalysis/definition/maninfo.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/manparm.py` & `flightanalysis-0.2.6/flightanalysis/definition/manparm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 from typing import Dict, Callable, Union, Tuple
 import numpy as np
 from flightdata import Collection
 from flightanalysis.manoeuvre import Manoeuvre
 from flightdata import State
-from flightanalysis.scoring import *
+from flightanalysis.scoring import Criteria, Combination, Measurement, Result, Comparison, Results, Single
 from . import Collector, Collectors, Opp
 from dataclasses import dataclass, field
 from typing import Any, Self
-import numpy as np
 import pandas as pd
 from geometry import Point
 from numbers import Number
-from copy import deepcopy
+
 
 @dataclass
 class ManParm(Opp):
     """This class represents a parameter that can be used to characterise the geometry of a manoeuvre.
     For example, the loop diameters, line lengths, roll direction. 
         name (str): a short name, must work as an attribute so no spaces or funny characters
         criteria (Comparison): The comparison criteria function to be used when judging this parameter
-        default (float): A default value (or default option if specified in criteria)
+        defaul (float): A defaul value (or defaul option if specified in criteria)
         collectors (Collectors): a list of functions that will pull values for this parameter from an Elements 
             collection. If the manoeuvre was flown correctly these should all be the same. The resulting list 
             can be passed through the criteria (Comparison callable) to calculate a downgrade.
 
     """
     criteria: Criteria
-    default:Any=None
+    defaul:Any=None
     collectors:Collectors=field(default_factory=lambda : Collectors())
 
 
     @property
     def n(self):
         return len(self.criteria.desired[0]) if isinstance(self.criteria, Combination) else None
         
     def to_dict(self):
         return dict(
             name = self.name,
             criteria = self.criteria.to_dict(),
-            default = self.default,
+            defaul = self.defaul,# because default is reserverd in javascript
             collectors = self.collectors.to_dict()
         )
     
     @staticmethod
     def from_dict(data: dict):
         return ManParm(
             name = data["name"],
             criteria = Criteria.from_dict(data["criteria"]),
-            default = data["default"] if 'default' in data else data['defaul'], # because default is reserverd in javascript
+            defaul = data['defaul'], 
             collectors = Collectors.from_dict(data["collectors"])
         )
 
     def append(self, collector: Union[Opp, Collector, Collectors]):
         if isinstance(collector, Opp) or isinstance(collector, Collector):
             self.collectors.add(collector)    
         elif isinstance(collector, Collectors):
@@ -75,44 +74,44 @@
     def get_downgrades(self, els, state: State):
         coll = self.collect(els)
         values = list(coll.values())
         direction, vis = self.collect_vis(els, state)
 
         meas = Measurement(
             values,
-            self.default,
+            self.defaul,
             direction,
             vis
         )
 
         keys, errors, dgs = self.criteria(list(coll.keys()), list(coll.values())) 
         return Result(self.name, meas, values, errors, dgs * meas.visibility, keys)
 
     @property
     def value(self):
         if isinstance(self.criteria, Comparison):
-            return self.default
+            return self.defaul
         elif isinstance(self.criteria, Combination):
-            return self.criteria[self.default]
+            return self.criteria[self.defaul]
         else:
             raise AttributeError("This type of ManParm has no value")
 
 
     @property
     def kind(self):
         return self.criteria.__class__.__name__    
 
     def copy(self):
-        return ManParm(name=self.name, criteria=self.criteria, default=self.default, collectors=self.collectors.copy())
+        return ManParm(name=self.name, criteria=self.criteria, defaul=self.defaul, collectors=self.collectors.copy())
 
     def list_parms(self):
         return [self]
 
     def __repr__(self):
-        return f'ManParm({self.name}, {self.criteria.__class__.__name__}, {self.default})'
+        return f'ManParm({self.name}, {self.criteria.__class__.__name__}, {self.defaul})'
 
 
 
 class ManParms(Collection):
     VType=ManParm
     uid="name"
 
@@ -134,20 +133,20 @@
 
         Args:
             intended (Manoeuvre): Usually a Manoeuvre that has been resized based on an alinged state
         """
         mps = []
         for mp in self:
             flown_parm = list(mp.collect(intended.all_elements()).values())
-            if len(flown_parm) > 0 and mp.default is not None:
+            if len(flown_parm) > 0 and mp.defaul is not None:
                 if isinstance(mp.criteria, Combination):
-                    default = mp.criteria.check_option(flown_parm)
+                    defaul = mp.criteria.check_option(flown_parm)
                 else:
-                    default = np.mean(np.abs(flown_parm)) * np.sign(mp.default)
-                mps.append(ManParm(mp.name, mp.criteria, default, mp.collectors))
+                    defaul = np.mean(np.abs(flown_parm)) * np.sign(mp.defaul)
+                mps.append(ManParm(mp.name, mp.criteria, defaul, mp.collectors))
             else: 
                 mps.append(mp)
         return ManParms(mps)
     
     def remove_unused(self):
         return ManParms([mp for mp in self if len(mp.collectors) > 0])
```

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/operations/funopp.py` & `flightanalysis-0.2.6/flightanalysis/definition/operations/funopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/operations/itemopp.py` & `flightanalysis-0.2.6/flightanalysis/definition/operations/itemopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/operations/mathopp.py` & `flightanalysis-0.2.6/flightanalysis/definition/operations/mathopp.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/operations/operation.py` & `flightanalysis-0.2.6/flightanalysis/definition/operations/operation.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/definition/scheddef.py` & `flightanalysis-0.2.6/flightanalysis/definition/scheddef.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,45 @@
-from . import ManDef, ManInfo, ManParms
+from . import ManDef, ManInfo, ManOption, ScheduleInfo, fcj_schedule_names
 from flightdata import State
-from typing import Dict, Tuple, Union, Self
+from typing import Tuple, Union, Self
 from geometry import Transformation
 from flightanalysis.schedule import Schedule
 from flightanalysis.elements import Line
-from flightdata import Collection, State
+from flightdata import Collection
 from json import dump, load
-from flightdata.base.numpy_encoder import NumpyEncoder
-from dataclasses import dataclass
-from flightanalysis.data import list_resources, get_json_resource
-from json import dump
-
-
-fcj_schedule_names = {
-    'f3a': ['F3A', 'F3A FAI'],
-    'nsrca': ['F3A US'],
-    'f3auk': ['F3A UK'],
-    'imac': ['IMAC']
-}
-
-@dataclass
-class ScheduleInfo:
-    category: str
-    name: str
-
-    @staticmethod
-    def from_str(fname):
-        if fname.endswith("_schedule.json"):
-            fname = fname[:-14]
-        info = fname.split("_")
-        if len(info) == 1:
-            return ScheduleInfo("f3a", info[0].lower())
-        else:
-            return ScheduleInfo(info[0].lower(), info[1].lower())
-
-    def __str__(self):
-        return f"{self.category}_{self.name}".lower()
-
-    def definition(self):
-        return SchedDef.load(self)
-
-    @staticmethod
-    def from_fcj_sch(fcj):
-        for k, v in fcj_schedule_names.items():
-            if fcj[0] in v:
-                return ScheduleInfo(k, fcj[1])
-        raise ValueError(f"Unknown schedule {fcj}")    
-
-    def to_fcj_sch(self):
-        return [fcj_schedule_names[self.category][-1], self.name]
-
-    @staticmethod
-    def build(category, name):
-        return ScheduleInfo(category.lower(), name.lower())
-
-
-schedule_library = [ScheduleInfo.from_str(fname) for fname in list_resources('schedule')]
+from flightdata import NumpyEncoder
+from flightanalysis.data import get_json_resource
 
 
 class SchedDef(Collection):
     VType=ManDef
+    def __init__(self, data: dict[str, VType] | list[VType] = None):
+        super().__init__(data, check_types=False)
+        assert all([v.__class__.__name__ in ['ManOption', 'ManDef'] for v in self])
+
     def add_new_manoeuvre(self, info: ManInfo, defaults=None):
         return self.add(ManDef(info,defaults))
 
-    def create_schedule(self, depth: float, wind: float) -> Schedule:
-        return Schedule(
-            {m.uid: m.create(m.info.initial_transform(depth, wind)) for m in self}
-        )      
-
     def create_template(self,depth:float=170, wind:int=-1) -> Tuple[Schedule, State]:
         templates = []
         ipos = self[0].info.initial_position(depth,wind)
         
         mans = []
         for md in self:
-
+            md = md[md.active] if isinstance(md, ManOption) else md
+                
             itrans=Transformation(
                 ipos if len(templates) == 0 else templates[-1][-1].pos,
                 md.info.start.initial_rotation(wind) if len(templates) == 0 else templates[-1][-1].att
             )
             man = md.create(itrans)
             templates.append(man.create_template(itrans))
             mans.append(man)
         return Schedule(mans), State.stack(templates)
 
-    def create_el_matched_template(self, intended: Schedule):
-        for md, man in zip(self, intended):
-            if isinstance(man, Line):
-                pass
-
-    def update_defaults(self, sched: Schedule):
-        # TODO need to consider the entry line
-        for md, man in zip(self, sched):
-            md.mps.update_defaults(man)
-
     def to_json(self, file: str) -> str:
         with open(file, "w") as f:
             dump(self.to_dict(), f, cls=NumpyEncoder, indent=2)
         return file
 
     @staticmethod
     def from_json(file:str):
@@ -109,15 +51,15 @@
         sinfo = ScheduleInfo.from_str(name) if isinstance(name, str) else name 
             
         return SchedDef.from_dict(get_json_resource(f"{str(sinfo).lower()}_schedule"))
     
 
     def plot(self):
         sched, template = self.create_template(170, 1)
-        from flightplotting import plotsec, plotdtw
+        from flightplotting import plotdtw
         return plotdtw(template, template.data.manoeuvre.unique())
 
     def label_exit_lines(self, sti: State):
         mans = list(self.data.keys()) + ['landing']
         
         meids = [sti.data.columns.get_loc(l) for l in ['manoeuvre', 'element']]
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/autorotation.py` & `flightanalysis-0.2.6/flightanalysis/elements/autorotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 import numpy as np
-from geometry import Transformation, Point, Quaternion, PX, PY, PZ, P0, Time
+from geometry import Transformation, P0, PY, Time
 from flightdata import State
-from .element import Element, Elements
+from .element import Element
 from flightanalysis.scoring.criteria.f3a_criteria import F3A
 from flightanalysis.scoring import Measurement, DownGrade, DownGrades
-from typing import Union
 
 
 class Autorotation(Element):
     """much like a line, but rolls happens around the velocity vector,
     rather than the body x axis"""
     parameters = Element.parameters + "length,roll,rate,angle".split(",")
     def __init__(self, speed: float, length: float, roll: float, uid: str):
@@ -23,25 +22,23 @@
         check the right number of turns was performed'''
         def roll_angle(fl, tp):
             return Measurement.roll_angle_proj(fl, tp, PY())
         return DownGrades([
             DownGrade(roll_angle, F3A.single.roll)
         ])
         
-    
     @property
     def angle(self):
         return self.roll
 
     @property
     def rate(self):
         return self.angle * self.speed / self.length
     
     def create_template(self, istate: State, time: Time=None):
-        
         return istate.copy(
             vel=istate.vel.scale(self.speed),
             rvel=P0()
         ).fill(
             Element.create_time(self.length / self.speed, time)
         ).superimpose_rotation(
             istate.vel.unit(),
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/element.py` & `flightanalysis-0.2.6/flightanalysis/elements/element.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pandas as pd
 from flightdata import State, Collection
 from flightanalysis.scoring.criteria.f3a_criteria import F3A
 from flightanalysis.scoring import Measurement, DownGrade, DownGrades, Results
 import geometry as g
 from json import load
 import inspect
-from typing import Self, Tuple
-
+from typing import Self, Tuple, Union
+from loguru import logger
 
 class ElementError(Exception):
     pass
 
 
 class Element:   
     parameters = ["speed"]
@@ -132,35 +132,36 @@
     
     def create_template(self, istate: State, time: g.Time=None) -> State:
         raise Exception('Not available on base class')
 
     def match_intention(self, itrans: g.Transformation, flown: State) -> Self:
         raise Exception('Not available on base class')
 
-    def score(self, istate: State, fl: State) -> Tuple[Results, State]:
+    def score(self, istate: Union[State, g.Transformation], fl: State) -> Tuple[Results, State]:
+        istate = istate if isinstance(istate, State) else State.from_transform(istate)
         tp = self.create_template(istate, fl.time)
         if self.uid=='entry_line':
             res = self.analyse_exit(fl, tp)
         else:
             res = self.analyse(fl, tp)
         return res, tp
         
     @staticmethod
-    def optimise_split(istate: State, el1: Element, el2: Element, fl1: State, fl2: State):
+    def optimise_split(itrans: g.Transformation, el1: Element, el2: Element, fl1: State, fl2: State):
         
         def get_score(cel1: Element, cel2: Element, cfl1: State, cfl2: State):
-            res, tp = cel1.match_intention(istate.transform, cfl1).score(istate, cfl1)
+            res, tp = cel1.match_intention(itrans, cfl1).score(itrans, cfl1)
             ist2=State.from_transform(g.Transformation(tp.att[-1], cfl2.pos[0]), vel=tp.vel[-1])
+            ist2= ist2.relocate(cfl2.pos[0])
             res2, tp2 = cel2.match_intention(ist2.transform, cfl2).score(ist2, cfl2)
             return res.total + res2.total
         
         dgs = {0: get_score(el1, el2, fl1, fl2)}
         
         steps=int(len(fl2) > len(fl1)) * 2 - 1
-        
         new_dg = get_score(el1, el2, *State.shift_multi(steps, fl1, fl2))
         if new_dg > dgs[0]:
             steps=-steps
         else:
             steps+=np.sign(steps)
             dgs[steps] = new_dg
             
@@ -171,15 +172,14 @@
             if new_dg < list(dgs.values())[-1]:
                 steps+=np.sign(steps)
                 dgs[steps] = new_dg
             else:
                 break
         min_dg_step = np.argmin(np.array(list(dgs.values())))
         out_steps = list(dgs.keys())[min_dg_step]
-        
         return out_steps
 
 
 class Elements(Collection):
     VType=Element
     def get_parameter_from_element(self, element_name: str, parameter_name: str):
         return getattr(self.data[element_name], parameter_name)
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/line.py` & `flightanalysis-0.2.6/flightanalysis/elements/line.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/loop.py` & `flightanalysis-0.2.6/flightanalysis/elements/loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,23 @@
         rads = self.measure_radius(itrans, flown)
         angles = np.arctan(abs(flown.vel) * flown.dt / rads)
         keep = ~np.isnan(rads * angles)
         
         return np.sum((rads * angles)[keep]) / np.sum(angles[keep])
 
     def match_intention(self, itrans: Transformation, flown: State) -> Loop:
-        rv = flown.rvel # .mean() if self.ke else flown.q.mean()
-        wrv = flown.att.transform_point(rv)
+        
+        wrv = flown.att.transform_point(Point.vector_rejection(flown.rvel, PX()))
         itrv = itrans.att.inverse().transform_point(wrv)
-        #TODO need to fix angle direction for new ke definitino.
+        itr = itrv.z * np.sin(self.ke) + itrv.y * np.cos(self.ke)
+        
         return self.set_parms(
-            radius = self.weighted_average_radius(itrans, flown), #self.measure_radius(itrans, flown).mean(), # 
+            radius = self.weighted_average_radius(itrans, flown), 
             roll=abs(self.roll) * np.sign(np.mean(flown.p)),
-            angle=abs(self.angle) * np.sign(itrv.z.mean() if self.ke else itrv.y.mean()),
+            angle=abs(self.angle) * np.sign(itr.mean()),
             speed=abs(flown.vel).mean()
         )
     
     def segment(self, transform:Transformation, flown: State, partitions=10):
         subsections = flown.segment(partitions)
         elms = [ self.match_intention( transform,sec) for sec in subsections ]
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/nose_drop.py` & `flightanalysis-0.2.6/flightanalysis/elements/nose_drop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from geometry import Transformation, PX, PY, PZ, Time, Point
+from geometry import Transformation, PX, PY, Time
 from flightdata import State
 from .element import Element
 from .loop import Loop
 from flightanalysis.scoring.criteria.f3a_criteria import F3A
 from flightanalysis.scoring import Measurement, DownGrade, DownGrades
 
 
@@ -24,15 +24,16 @@
         def length(fl, tp):
             return Measurement.length(fl, tp, PX())
         def roll_angle(fl, tp):
             return Measurement.roll_angle_proj(fl, tp, PY())
         
         return DownGrades([
             DownGrade(length, F3A.intra.spin_entry_length),
-            DownGrade(roll_angle, F3A.intra.roll)
+            DownGrade(roll_angle, F3A.intra.roll),
+            DownGrade(Measurement.nose_drop, F3A.intra.nose_drop_amount)
         ])
 
     def create_template(self, istate: State, time: Time=None) -> State:
         _inverted = 1 if istate.transform.rotation.is_inverted()[0] else -1
         
         alpha =  np.arctan2(istate.vel.z, istate.vel.x)[0]
 
@@ -43,15 +44,15 @@
             -alpha - abs(self.break_angle) * _inverted
         ).label(element=self.uid)
     
     def describe(self):
         return "nose drop"
 
     def match_intention(self, transform: Transformation, flown: State) -> NoseDrop:
-        _inverted = 1 if transform.rotation.is_inverted()[0] else -1
+        _inverted = 1 if transform.att.is_inverted()[0] else -1
         _speed = abs(flown.vel).mean()
 
         loop = Loop(_speed, self.radius, 0.5*np.pi*_inverted).match_intention(
             transform, flown
         )
 
         return self.set_parms(
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/pitch_break.py` & `flightanalysis-0.2.6/flightanalysis/elements/pitch_break.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 
     @property
     def intra_scoring(self) -> DownGrades:
         '''TODO check the pitch departure is in the right direction
         TODO perhaps limit the roll amount'''
         def length(fl, tp):
             return Measurement.length(fl, tp, PX())
+        def roll_angle(fl, tp):
+            return Measurement.roll_angle_proj(fl, tp, PY())
         return DownGrades([
-            DownGrade(length, F3A.intra.pitch_break_length),
+            DownGrade(length, F3A.intra.pitch_break_length)
         ])
 
     @property
     def exit_scoring(self) -> DownGrades:
         return DownGrades()
 
-
     def create_template(self, istate: State, time: Time=None) -> State:
         return Line(self.speed, self.length).create_template(
             istate, 
             time
         ).superimpose_rotation(
             PY(),
             self.break_angle
```

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/recovery.py` & `flightanalysis-0.2.6/flightanalysis/elements/recovery.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/elements/stall_turn.py` & `flightanalysis-0.2.6/flightanalysis/elements/stall_turn.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/manoeuvre.py` & `flightanalysis-0.2.6/flightanalysis/manoeuvre.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 from geometry import Transformation, PX
 from typing import List, Union, Tuple, Self
 import numpy as np
 from dataclasses import dataclass
-
-
 from flightdata.state import State
 from flightanalysis.elements import Elements, Element, Line, Autorotation
-from flightanalysis.scoring import *
+from flightanalysis.scoring import Results, ElementsResults
+from loguru import logger
 
 
 @dataclass
 class Manoeuvre:
     entry_line: Line
     elements: Elements
     exit_line: Line
@@ -77,17 +76,17 @@
     def create_template(self, initial: Union[Transformation, State], aligned:State=None) -> State:
         
         istate = State.from_transform(initial, vel=PX()) if isinstance(initial, Transformation) else initial
         aligned = self.get_data(aligned) if aligned else None
         templates = []
         els = self.all_elements()
         for i, element in enumerate(els):
-            time = element.get_data(aligned).time if not aligned is None else None
+            time = element.get_data(aligned).time if aligned is not None else None
 
-            if i < len(els)-1 and not time is None:
+            if i < len(els)-1 and time is not None:
                 time = time.extend()
             templates.append(element.create_template(istate, time))
             istate = templates[-1][-1]
         
         return State.stack(templates).label(manoeuvre=self.uid)
 
 
@@ -142,33 +141,44 @@
         )
 
     def analyse(self, flown: State, template: State):
         fl=self.entry_line.get_data(flown)
         tp=self.entry_line.get_data(template).relocate(fl.pos[0])
         
         ers = [Results(self.entry_line.uid, self.entry_line.analyse_exit(fl, tp))]
+        logger.debug(f'Intra analysis of entry line complete, total dg = {ers[-1].total}')
 
         for el in self.elements:
             fl = el.get_data(flown)
             tp = el.get_data(template).relocate(fl.pos[0])
             ers.append(Results(el.uid, el.analyse(fl, tp)))
+            logger.debug(f'Intra analysis of {el.uid} complete, total dg = {ers[-1].total}')
+
         return ElementsResults(ers)
 
-    def optimise_alignment(self, istate: State, aligned: State) -> Tuple(Self, State):
+    def optimise_alignment(self, template: State, aligned: State) -> State:
         els = self.all_elements()
         elns = list(els.data.keys())
-        
-        for eln1, eln2 in zip(elns[:-1], elns[1:]):
-            fl1, fl2 = aligned.get_element(eln1), aligned.get_element(eln2)
-            steps = Element.optimise_split(istate, els[eln1], els[eln2], fl1, fl2)
-            if not steps == 0:
-                aligned = aligned.shift_label(steps, 2, manoeuvre=self.uid, element=eln1)
-            istate = els[eln1].create_template(istate)[-1]
-        
-        return aligned
 
+        padjusted = set(elns)
+        count=0
+        while len(padjusted) > 0 and count < 2:
+            adjusted = set()
+            for eln1, eln2 in zip(elns[:-1], elns[1:]):
+                if (eln1 in padjusted) or (eln2 in padjusted):
+                    fl1, fl2 = aligned.get_element(eln1), aligned.get_element(eln2)
+                    tp0 = template.get_element(eln1)
+                    steps = Element.optimise_split(tp0[0].relocate(fl1[0].pos), els[eln1], els[eln2], fl1, fl2)
+                    logger.debug(f'Adjusting split between {eln1} and {eln2} by {steps} steps')
+                    if not steps == 0:
+                        aligned = aligned.shift_label(steps, 2, manoeuvre=self.uid, element=eln1)
+                        adjusted.update([eln1, eln2])
+            padjusted = adjusted
+            count+=1
+            logger.debug(f'pass {count}, {len(padjusted)} elements adjusted:\n{padjusted}')
+        return aligned
     
     def descriptions(self):
         return [e.describe() for e in self.elements]
     
     def __repr__(self):
         return f'Manoeuvre({self.uid}, len={len(self.elements)})'
```

### Comparing `flightanalysis-0.2.5/flightanalysis/schedule.py` & `flightanalysis-0.2.6/flightanalysis/schedule.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/criteria/criteria.py` & `flightanalysis-0.2.6/flightanalysis/scoring/criteria/criteria.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from .exponential import Exponential, free
 from dataclasses import dataclass, field
 
 
 def all_subclasses(cls):
     return set(cls.__subclasses__()).union(
         [s for c in cls.__subclasses__() for s in all_subclasses(c)])
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/criteria/exponential.py` & `flightanalysis-0.2.6/flightanalysis/scoring/criteria/exponential.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 from dataclasses import dataclass, field
 import numpy as np
+from typing import Union
 
 @dataclass
 class Exponential:
     factor: float
     exponent: float
-    limit: float = field(default=10)
+    limit: Union[float, None] = None
     def __call__(self, value):
         val = self.factor * value ** self.exponent
-        return np.minimum(val, self.limit)
-        
+        if self.limit:
+            val = np.minimum(val, self.limit)
+        return val
+    
     @staticmethod
     def linear(factor: float):
         return Exponential(factor, 1)
     
     @staticmethod
-    def fit_points(xs, ys, limit=10):
+    def fit_points(xs, ys, limit=None):
         from scipy.optimize import curve_fit
         res = curve_fit(
             lambda x, factor, exponent: factor * x ** exponent,
             xs, 
             ys)
-
+        assert np.all(np.isreal(res[0]))
         return Exponential(res[0][0], res[0][1], limit)
 
 free = Exponential(0,1)
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/criteria/f3a_criteria.py` & `flightanalysis-0.2.6/flightanalysis/scoring/criteria/f3a_criteria.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from flightanalysis.scoring.criteria import *
+from flightanalysis.scoring.criteria import Single, Exponential, ContAbs, ContRat, InsideBound, MaxBound, Comparison, OutsideBound
+
 
 class F3ASingle:
     track=Single(Exponential(3.8197186342054885,0.9999999999999999, 100 ))
     roll=Single(Exponential(2.872721387028467,1.6309297535714575, 100 ))
     angle=Single(Exponential(3.8197186342054885,0.9999999999999999, 100 ))
-    distance=Single(Exponential(0.02500000000000001,0.9999999999999999, 10 ))
 class F3AIntra:
-    track=ContAbs(Exponential(3.8197186342054885,0.9999999999999999, 10 ))
-    roll=ContAbs(Exponential(3.3937161800825275,1.2618595071429148, 10 ))
+    track=ContAbs(Exponential(3.8197186342054885,0.9999999999999999, None ))
+    roll=ContAbs(Exponential(3.3937161800825275,1.2618595071429148, None ))
     radius=ContRat(Exponential(0.5,1.2920296742201793, 2 ))
     speed=ContRat(Exponential(0.15,1.0, 1 ))
     roll_rate=ContRat(Exponential(0.15,1.0, 1 ))
-    stallturn_speed=InsideBound(Exponential(0.08879139070041006,1.75647079736603, 10 ), [-2, 2])
-    stallturn_width=InsideBound(Exponential(0.14798565116735013,1.75647079736603, 10 ), [-2, 2])
-    spin_entry_length=InsideBound(Exponential(0.08879139070041006,1.75647079736603, 10 ), [-5, 5])
-    pitch_break_length=InsideBound(Exponential(0.5,2.3219280948873626, 10 ), [-2, 2])
-    recovery_length=MaxBound(Exponential(0.5,2.3219280948873626, 10 ), 2)
+    stallturn_speed=InsideBound(Exponential(0.08879139070041006,1.75647079736603, None ), [-2, 2])
+    stallturn_width=InsideBound(Exponential(0.14798565116735013,1.75647079736603, None ), [-2, 2])
+    spin_entry_length=InsideBound(Exponential(0.08879139070041006,1.75647079736603, None ), [-5, 5])
+    pitch_break_length=InsideBound(Exponential(0.7,2.321928094887362, None ), [-2, 2])
+    nose_drop_amount=OutsideBound(Exponential(20,1, None ), [-0.2617993877991494, 0.2617993877991494])
+    recovery_length=MaxBound(Exponential(0.7,2.321928094887362, None ), 2)
+    box=InsideBound(Exponential(38.197186342054884,1, None ), [-1.0471975511965976, 1.0471975511965976])
+    depth=MaxBound(Exponential(0.02500000000000001,0.9999999999999999, None ), 170)
 class F3AInter:
     radius=Comparison(Exponential(1.0,0.4306765580733931, 2 ))
-    speed=Comparison(Exponential(0.25,0.8613531161467862, 10 ))
+    speed=Comparison(Exponential(0.25,0.8613531161467862, None ))
     roll_rate=Comparison(Exponential(0.25,1.1132827525593783, 2 ))
     length=Comparison(Exponential(1.0,0.6826061944859854, 3 ))
-    free=Comparison(Exponential(0,1, 10 ))
+    free=Comparison(Exponential(0,1, None ))
 
 
 
 class F3A:
     inter = F3AInter
     intra = F3AIntra
     single = F3ASingle
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/criteria/inter/combination.py` & `flightanalysis-0.2.6/flightanalysis/scoring/criteria/inter/combination.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from dataclasses import dataclass, field
 
 
 @dataclass
 class Combination(Criteria):
     desired: np.ndarray = field(default_factory=lambda : None)
     """Handles a series of criteria assessments.
-    for example a number of rolls in an element. 
+    for example a number of rolls in an element.
+    Warning - if not all of the desired values have collectors then the ones with collectors must
+    come first.
     """
     
     def __getitem__(self, value: int):
         return self.desired[value]
 
     def get_errors(self, values: npt.ArrayLike):
         """get the error between values and desired for all the options"""
-        return self.desired - np.array(values)
+        return np.array(self.desired)[:,:len(values)] - np.array(values)
 
     def get_option_error(self, option: int, values: npt.ArrayLike) -> npt.NDArray:
         """The difference between the values and a given option"""
         return np.array(values) - self.desired[option]
 
     def check_option(self, values) -> int:
         """Given a set of values, return the option id which gives the least error"""
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/criteria/intra/continuous.py` & `flightanalysis-0.2.6/flightanalysis/scoring/criteria/intra/continuous.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,26 +45,35 @@
     def visibility(self, measurement, ids):
         rids = np.concatenate([[0], ids])
         return np.array([np.mean(measurement.visibility[a:b]) for a, b in zip(rids[:-1], rids[1:])])
 
     @staticmethod
     def convolve(data, width):
         kernel = np.ones(width) / width
-        l = len(data)
-        outd = np.full(l, np.nan)
+        outd = np.full(len(data), np.nan)
         conv = np.convolve(data, kernel, mode='valid')
         ld = (len(data) - len(conv))/2
         outd[int(np.ceil(ld)):-int(np.floor(ld))] = conv
-        return pd.Series(outd).ffill().bfill().to_numpy()
+        outd[:width//2] = np.linspace(np.mean(data[0:width//4]), outd[width//2],width//2)
+        outd[-width//2:] = np.linspace(outd[-width//2], np.mean(data[-1-width//4:-1]),width//2)
+        return outd
 
 
 class ContAbs(Continuous):
-    def prepare(self, value: npt.NDArray, expected: float):
-        
-        return  value - expected
+#    def prepare(self, value: npt.NDArray, expected: float):
+#        
+#        return  value - expected
+
+    def prepare(self, values: npt.NDArray, expected: float):
+        window = 30
+        sample = values - expected
+        if len(sample) <= window:
+            return np.linspace(values[0],values[-1], len(sample))
+        else:
+            return Continuous.convolve(sample, window)
 
     @staticmethod
     def mistakes(data, peaks, troughs):
         '''All increases away from zero are downgraded (only peaks)'''
         last_trough = -1 if troughs[-1] else None
         first_peak = 1 if peaks[0] else 0
         return np.abs(data[first_peak:][peaks[first_peak:]] - data[:last_trough][troughs[:last_trough]])
@@ -74,24 +83,24 @@
         first_peak = 1 if peaks[0] else 0
         return ids[first_peak:][peaks[first_peak:]]
 
 
 class ContRat(Continuous):
     
     def prepare(self, values: npt.NDArray, expected: float):
-        endcut = 0
-        window = 20
-        sample = np.full(len(values), expected)
-        sample[endcut:-endcut-1] = values[endcut:-endcut-1]
-        sample = values
-        if len(sample) <= window + endcut * 2:
-            return np.full(len(sample), abs(np.mean(sample)))
+        window = 40
+        if len(values) <= window:
+            return np.abs(np.linspace(
+                np.mean(values[:1+len(values)//3]), 
+                np.mean(values[-1-len(values)//3:]), 
+                len(values)
+            ))
         else:
-            return np.abs(Continuous.convolve(sample, 20))
-        
+            return np.abs(Continuous.convolve(values, window))
+            
     @staticmethod
     def mistakes(data, peaks, troughs):
         '''All changes are downgraded (peaks and troughs)'''
         values = data[peaks + troughs]
         return np.maximum(values[:-1], values[1:]) / np.minimum(values[:-1], values[1:]) - 1
     
     @staticmethod
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/downgrade.py` & `flightanalysis-0.2.6/flightanalysis/scoring/downgrade.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/measurement.py` & `flightanalysis-0.2.6/flightanalysis/scoring/measurement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from flightdata import State
-from geometry import Point, Quaternion, PX, PY, PZ, P0, Transformation
+from geometry import Point, Quaternion, PX, PY, PZ
 import numpy as np
+import pandas as pd
 import numpy.typing as npt
 from dataclasses import dataclass
-from typing import Union, Any, Self
+from typing import Union, Self
 
 
 
 @dataclass()
 class Measurement:
     value: npt.NDArray
     expected: float
@@ -26,18 +27,24 @@
             self.visibility[sli],
         )
 
     def to_dict(self):
         return dict(
             value = list(self.value),
             expected = self.expected,
-            direction = self.direction.to_dict(),
+            direction = self.direction.to_dicts(),
             visibility = list(self.visibility)
         )
     
+    def __repr__(self):
+        if len(self.value) == 1:
+            return f'Measurement({self.value}, {self.expected}, {self.direction}, {self.visibility})'
+        else:
+            return f'Measurement(\nvalue:\n={pd.DataFrame(self.value).describe()}\nexpected:{self.expected}\nvisibility:\n{pd.DataFrame(self.visibility).describe()}\n)'
+
     def exit_only(self):
         fac = np.zeros(len(self.value))
         fac[-1] = 1
         return Measurement(
             self.value * fac,
             self.expected,
             self.direction,
@@ -45,20 +52,24 @@
         )
 
     @staticmethod
     def from_dict(data) -> Measurement:
         return Measurement(
             np.array(data['value']),
             data['expected'],
-            Point.from_dict(data['direction']),
+            Point.from_dicts(data['direction']),
             np.array(data['visibility'])
         )
 
     def _pos_vis(loc: Point):
-        return abs(Point.vector_rejection(loc, PY())) / abs(loc)
+        '''Accounts for how hard it is to see an error due to the distance from the pilot.
+        Assumes distance is a function only of x and z position, not the y position.
+        '''
+        res = abs(Point.vector_projection(loc, PY())) / abs(loc)
+        return np.nan_to_num(res, nan=1)
 
     @staticmethod
     def _vector_vis(direction: Point, loc: Point) -> Union[Point, npt.NDArray]:
         #a vector error is more visible if it is perpendicular to the viewing vector
         # 0 to np.pi, pi/2 gives max, 0&np.pi give min
         return direction,  (1 - 0.8* np.abs(Point.cos_angle_between(loc, direction))) * Measurement._pos_vis(loc)
 
@@ -70,15 +81,14 @@
         return world_tip_movement_direction, (1-0.8*np.abs(Point.cos_angle_between(loc, world_tip_movement_direction))) * Measurement._pos_vis(loc)
 
     @staticmethod
     def _rad_vis(loc:Point, axial_dir: Point) -> Union[Point, npt.NDArray]:
         #radial error more visible if axis is parallel to the view vector
         return axial_dir, (0.2+0.8*np.abs(Point.cos_angle_between(loc, axial_dir))) * Measurement._pos_vis(loc)
 
-    
     @staticmethod
     def speed(fl: State, tp: State, direction: Point=None, axis='body') -> Self:
         direction=Point(1,1,1) if direction is None else direction
         def get_body_direction(st: State):
             if axis == 'body':
                 return direction
             else:
@@ -113,29 +123,26 @@
         """Direction is the body X axis, value is equal to the roll angle error.
         roll angle error is the angle between the body proj vector axis and the 
         reference frame proj vector. 
         proj normal of the plane to measure roll angles against.
 
         """
         trfl = fl#.to_track() # flown in the track axis
-        
         rfproj=tp[0].att.transform_point(proj) # proj vector in the ref_frame
-        
         tr_rf_proj = trfl.att.inverse().transform_point(rfproj) # proj vector in track axis
-        
         tp_rf_proj = tp.att.inverse().transform_point(rfproj) # proj vector in template body axis (body == track for template)
-        
         with np.errstate(invalid='ignore'):
             fl_roll_angle = np.arcsin(Point.cross(tr_rf_proj, proj).x)
             tp_roll_angle = np.arcsin(Point.cross(tp_rf_proj, proj).x)
-        
 
+        flturns = np.sum(Point.scalar_projection(fl.rvel, fl.vel) * fl.dt) / (2*np.pi)
+        tpturns = np.sum(Point.scalar_projection(tp.rvel, tp.vel) * tp.dt) / (2*np.pi)
 
         return Measurement(
-            fl_roll_angle - tp_roll_angle,
+            int(flturns - tpturns) * 2 * np.pi + fl_roll_angle - tp_roll_angle,
             0, 
             *Measurement._roll_vis(fl.pos, fl.att)
         )
 
     @staticmethod
     def roll_angle_y(fl: State, tp: State) -> Self:
         return Measurement.roll_angle_proj(fl, tp, PY())
@@ -160,14 +167,21 @@
     @staticmethod
     def roll_rate(fl: State, tp: State) -> Measurement:
         """vector in the body X axis, length is equal to the roll rate"""
         wrvel = fl.att.transform_point(fl.p * PX())
         return Measurement(abs(wrvel) * np.sign(fl.p), np.mean(tp.p), *Measurement._roll_vis(fl.pos, fl.att))
     
     @staticmethod
+    def nose_drop(fl: State, tp: State) -> Measurement:
+        """Check the change in body pitch angle between the start and end of the element"""
+        flpit = Quaternion.body_axis_rates(fl.att[0], fl.att[-1]).y
+                
+        return Measurement(flpit, np.array([0]), *Measurement._roll_vis(fl.pos[-1], fl.att[-1]))
+    
+    @staticmethod
     def track_proj(fl: State, tp: State, proj: Point, fix='ang'):
         """
         Direction is the world frame scalar rejection of the velocity difference onto the template velocity 
         vector.
         proj defines the axis in the ref_frame (tp[0].transform) to work on.
         if fix=='vel' we are only interested in velocity errors in the proj vector. (loop axial track)
         if fix=='ang' we are only interested in angle errors about the proj vector. (loop exit track)
@@ -254,13 +268,60 @@
         return Measurement(
             c, np.mean(c), 
             *Measurement._rad_vis(
                 fl.pos, 
                 tp[0].att.transform_point(wproj)
             )  
         )
+
+    @staticmethod
+    def depth_vis(loc: Point):
+        '''Accounts for how hard it is to tell whether the aircraft is at a downgradable
+         distance (Y position). Assuming that planes look closer in the centre of the box than the end,
+         even if they are at the same Y position.
+        '''
+        rot = np.abs(np.arctan(loc.x / loc.y))
+        return loc, 0.4 + 0.6 * rot / np.radians(60)
+
+    @staticmethod
+    def depth(fl: State) -> Measurement:
+        return Measurement(
+            fl.pos.y,
+            0,
+            *Measurement.depth_vis(fl.pos)
+        )
+    
+    @staticmethod
+    def lateral_pos_vis(loc: Point):
+        '''How hard is it for the judge tell the lateral position. Based on the following principals: 
+        - its easier when the plane is lower as its closer to the box markers. (1 for low, 0.5 for high)
+        '''
+        r60 = np.radians(60)
+        return loc, (0.5 + 0.5 * (r60 - np.abs(np.arctan(loc.z / loc.y))) / r60)
     
     @staticmethod
-    def turns(fl: State, tp: State) -> Measurement:
-        fl_turns = fl.rvel.cumsum() * fl.dt
-        tp_turns = tp.rvel.cumsum() * fl.dt
-        
+    def side_box(fl: State):
+        vis = Measurement.lateral_pos_vis(fl.pos)
+        return Measurement(
+            np.arctan(fl.pos.x / fl.pos.y),
+            0.0,
+            vis[0],
+            vis[1] * 0.6 
+            # additional factor because the judge isn't aligned with the end marker so can't really tell
+        )
+    
+    @staticmethod
+    def top_box(fl: State):
+        return Measurement(
+            np.arctan(fl.pos.z / fl.pos.y),
+            0.0,
+            fl.pos,
+            np.full(len(fl), 0.5) # top box is always hard to tell
+        )
+
+    @staticmethod
+    def centre_box(fl: State):        
+        return Measurement(
+            np.arctan(fl.pos.x / fl.pos.y),
+            0.0,
+            *Measurement.lateral_pos_vis(fl.pos)
+        )
```

### Comparing `flightanalysis-0.2.5/flightanalysis/scoring/results.py` & `flightanalysis-0.2.6/flightanalysis/scoring/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,15 +109,16 @@
         return {r.name: r.dgs for r in self if len(r.dgs) > 0}
 
     def downgrade_df(self) -> pd.DataFrame:
         dgs = self.downgrade_summary()
         if len(dgs) == 0:
             return pd.DataFrame()
         max_len = max([len(v) for v in dgs.values()])
-        extend = lambda vals: [vals[i] if i < len(vals) else np.NaN for i in range(max_len)]
+        def extend(vals):
+            return [vals[i] if i < len(vals) else np.NaN for i in range(max_len)]
         df =  pd.DataFrame.from_dict({k:extend(v) for k,v in dgs.items()})
         
         return df
 
     def to_dict(self) -> dict[str, dict]:
         return dict(
             name = self.name,
@@ -143,45 +144,45 @@
 
     @property
     def total(self):
         return sum(self.downgrade_list)
     
     @property
     def downgrade_list(self):
-        return [er.total for er in self]
+        return list(self.downgrade_df().iloc[-1, :])
     
     def downgrade_df(self):
         df = pd.concat([idg.downgrade_df().sum() for idg in self], axis=1).T
-        df["Total"] = df.T.sum()
-        df["Element"] = self.data.keys()
+        df = pd.concat([df, pd.DataFrame(df.sum()).T])#(np.floor(df.sum())).T])
+        df.index = list(self.data.keys()) + ['Total']
         
-        return df.set_index("Element")
+        return df
     
     def to_dict(self) -> dict[str, dict]:
         return dict(
             data = {k: v.to_dict() for k, v in self.data.items()},
             summary = self.downgrade_list,
             total = self.total
         )
 
     @staticmethod
     def from_dict(data) -> Results:
-        return Results(
-            [Result.from_dict(v) for v in data['data'].values()]
+        return ElementsResults(
+            {k: Results.from_dict(v) for k, v in data['data'].items()}
         )
 
 
 @dataclass
 class ManoeuvreResults:
     inter: Results
     intra: ElementsResults
     positioning: Results
 
     def summary(self):
-        return {k: v.total for k, v in self.__dict__.items() if not v is None} 
+        return {k: v.total for k, v in self.__dict__.items() if v is not None} 
 
     def score(self):
         return max(0, 10 - sum([v for v in self.summary().values()]))
     
     def to_dict(self):
         return dict(
             inter=self.inter.to_dict(),
@@ -192,9 +193,9 @@
         )
 
     @staticmethod
     def from_dict(data):
         return ManoeuvreResults(
             Results.from_dict(data['inter']),
             ElementsResults.from_dict(data['intra']),
-            Result.from_dict(data['positioning']),
+            Results.from_dict(data['positioning']),
         )
```

### Comparing `flightanalysis-0.2.5/flightanalysis.egg-info/SOURCES.txt` & `flightanalysis-0.2.6/flightanalysis.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,46 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-examples/__init__.py
-examples/data/__init__.py
-examples/schedules_construction/AMA_Intermediate2024.py
-examples/schedules_construction/__init__.py
-examples/schedules_construction/create_all.py
-examples/schedules_construction/f3a_a25.py
-examples/schedules_construction/f3a_f25.py
-examples/schedules_construction/f3a_p23.py
-examples/schedules_construction/f3a_p25.py
-examples/schedules_construction/f3auk_Intermediate.py
-examples/schedules_construction/f3auk_clubman.py
-examples/schedules_construction/imac_sport2024.py
-examples/schedules_construction/imac_unlim2024.py
-examples/schedules_construction/make_manoeuvre.py
-examples/schedules_construction/nsrca_inter2024.py
-examples/scoring/__init__.py
-examples/scoring/analysis_reprocess.py
-examples/scoring/f3a_criteria_maker.py
-examples/scoring/judging.py
-examples/scoring/split_optimisation.py
-examples/scoring/manoeuvres/__init__.py
-examples/scoring/manoeuvres/inter_analysis.py
-examples/scoring/manoeuvres/intra_analysis.py
-examples/scoring/manoeuvres/positioning_analysis.py
-examples/scoring/manoeuvres/mans/__init__.py
-examples/scoring/manoeuvres/mans/extract_mans.py
 flightanalysis/__init__.py
 flightanalysis/manoeuvre.py
 flightanalysis/schedule.py
 flightanalysis.egg-info/PKG-INFO
 flightanalysis.egg-info/SOURCES.txt
 flightanalysis.egg-info/dependency_links.txt
+flightanalysis.egg-info/requires.txt
 flightanalysis.egg-info/top_level.txt
 flightanalysis/analysis/__init__.py
 flightanalysis/analysis/el_analysis.py
-flightanalysis/analysis/man_analysis.py
 flightanalysis/analysis/sch_analysis.py
+flightanalysis/analysis/manoeuvre_analysis/__init__.py
+flightanalysis/analysis/manoeuvre_analysis/alignment.py
+flightanalysis/analysis/manoeuvre_analysis/analysis.py
+flightanalysis/analysis/manoeuvre_analysis/basic.py
+flightanalysis/analysis/manoeuvre_analysis/complete.py
+flightanalysis/analysis/manoeuvre_analysis/scored.py
 flightanalysis/data/IMAC_Unlimited2024_schedule.json
 flightanalysis/data/__init__.py
 flightanalysis/data/f3a_a25_schedule.json
 flightanalysis/data/f3a_f25_schedule.json
 flightanalysis/data/f3a_p23_schedule.json
 flightanalysis/data/f3a_p25_schedule.json
 flightanalysis/data/f3auk_clubman_schedule.json
 flightanalysis/data/f3auk_inter_schedule.json
 flightanalysis/definition/__init__.py
 flightanalysis/definition/collectors.py
 flightanalysis/definition/eldef.py
 flightanalysis/definition/mandef.py
 flightanalysis/definition/maninfo.py
+flightanalysis/definition/manoption.py
 flightanalysis/definition/manparm.py
 flightanalysis/definition/scheddef.py
+flightanalysis/definition/scheduleinfo.py
 flightanalysis/definition/builders/__init__.py
 flightanalysis/definition/builders/elbuilders.py
 flightanalysis/definition/builders/lines.py
 flightanalysis/definition/builders/manbuilder.py
 flightanalysis/definition/operations/__init__.py
 flightanalysis/definition/operations/funopp.py
 flightanalysis/definition/operations/itemopp.py
@@ -84,9 +66,12 @@
 flightanalysis/scoring/criteria/inter/__init__.py
 flightanalysis/scoring/criteria/inter/combination.py
 flightanalysis/scoring/criteria/inter/comparison.py
 flightanalysis/scoring/criteria/intra/__init__.py
 flightanalysis/scoring/criteria/intra/bounded.py
 flightanalysis/scoring/criteria/intra/continuous.py
 flightanalysis/scoring/criteria/intra/single.py
+scripts/__init__.py
+scripts/batch_analyse.py
+scripts/collect_scores.py
 tests/test_criiteria.py
 tests/test_data.py
```

### Comparing `flightanalysis-0.2.5/setup.py` & `flightanalysis-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `flightanalysis-0.2.5/tests/test_criiteria.py` & `flightanalysis-0.2.6/tests/test_criiteria.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-from pytest import fixture, mark
+from pytest import fixture, mark, approx
 from flightanalysis.scoring.criteria import Single, Exponential, Criteria, Combination, ContRat, ContAbs, Comparison, MaxBound, InsideBound, OutsideBound, Continuous
 from flightanalysis.scoring import Measurement
+from flightanalysis import NoseDrop
+from flightdata import State
+from geometry import Transformation, Euldeg, P0, PX, PY
+
 from numpy.testing import assert_array_almost_equal
 import numpy as np
 import geometry as g
 
 @fixture
 def single():
     return Single(Exponential(1,1))
@@ -25,16 +29,14 @@
 
 
 @fixture
 def comparison():
     return Comparison(Exponential(1,1))
 
 
-
-
 def test_single_to_dict(single: Single):
     res = single.to_dict()
     
     assert res['kind'] == 'Single'
 
 def test_single_from_dict(single):
     res = Criteria.from_dict(single.to_dict())
@@ -138,15 +140,14 @@
     np.testing.assert_array_equal(sample, np.ones(11))
     
 
 @fixture
 def outside():
     return OutsideBound(Exponential(1,1), [-1, 1])
 
-
 def test_outside_allin(outside: OutsideBound):
     sample = outside.prepare(np.zeros(11), 0)
     np.testing.assert_array_equal(sample, np.ones(11))
     
 def test_outside_above(outside: InsideBound):
     sample = outside.prepare(np.full(11, 2), 0)
     np.testing.assert_array_equal(sample, np.zeros(11))
@@ -194,7 +195,33 @@
     )
 
     data = 4 - np.array([0,1,2,1,0,1,2,1,0,1,2,1,0])
     np.testing.assert_array_equal(
         ContRat.mistakes(*mistakes_inputs(data)), 
         [1,1,1,1,1,1]
     )
+
+
+@fixture
+def ndbound():
+    return OutsideBound(Exponential(20,1), [-np.radians(15), np.radians(15)])
+
+def make_nd(angle, inverted=False):
+    return NoseDrop(3, 5, np.radians(90-angle)).create_template(
+        State.from_transform(
+            Transformation(Euldeg(0 if inverted else 180, 0, 0), PY(100)),
+            vel=PX(3)
+        )
+    )
+
+def test_nose_drop_bound(ndbound: OutsideBound):
+    '''Check there is a big downgrade for nosedrop of less than 15 degrees'''
+    fl = make_nd(5)
+    res = ndbound('test', Measurement.nose_drop(fl, fl))
+    assert res.dgs[0] > 3
+
+def test_continuous_convolce():
+    data = np.linspace(0, 100, 100)
+    res = Continuous.convolve(data, 20)
+    assert len(res) == len(data)
+    assert data[0] == res[0]
+    assert data[-1] == res[-1]
```

