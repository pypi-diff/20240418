# Comparing `tmp/storynavigator-0.0.8.tar.gz` & `tmp/storynavigator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storynavigator-0.0.8.tar", last modified: Mon Dec 11 20:39:52 2023, max compression
+gzip compressed data, was "storynavigator-0.0.9.tar", last modified: Mon Dec 11 21:21:59 2023, max compression
```

## Comparing `storynavigator-0.0.8.tar` & `storynavigator-0.0.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.356687 storynavigator-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-11 20:39:33.000000 storynavigator-0.0.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-11 20:39:33.000000 storynavigator-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-11 20:39:33.000000 storynavigator-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-12-11 20:39:52.356687 storynavigator-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-12-11 20:39:33.000000 storynavigator-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-11 20:39:33.000000 storynavigator-0.0.8/README.pypi
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2023-12-11 20:39:33.000000 storynavigator-0.0.8/distribute_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.336687 storynavigator-0.0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.336687 storynavigator-0.0.8/doc/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/dsgdepparser.md
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/dsgruleset.md
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/dsgsrl.md
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/dsgtagger.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.340687 storynavigator-0.0.8/doc/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    25652 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/icons/dsg_ruleset_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26587 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/icons/dsg_stanzadep_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    21161 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/icons/dsg_stanzasrl_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.344687 storynavigator-0.0.8/doc/widgets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   904633 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/images/dsgdepparser-example.png
--rw-r--r--   0 runner    (1001) docker     (127)   820676 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/images/dsgruleset-example.png
--rw-r--r--   0 runner    (1001) docker     (127)   629997 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/images/dsgsrl-example.png
--rw-r--r--   0 runner    (1001) docker     (127)   508321 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets/images/dsgtagger-example2.png
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-11 20:39:33.000000 storynavigator-0.0.8/doc/widgets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.344687 storynavigator-0.0.8/orangecontrib/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.344687 storynavigator-0.0.8/orangecontrib/storynavigation/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.344687 storynavigator-0.0.8/orangecontrib/storynavigation/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/modules/actionanalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    23685 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/modules/actoranalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/modules/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/modules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.348687 storynavigator-0.0.8/orangecontrib/storynavigation/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   284185 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/dictionary_verbs_halliday_dimensions.csv
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/dutchpronouns.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/dutchstopwords.txt
--rw-r--r--   0 runner    (1001) docker     (127)    81490 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_process.json
--rw-r--r--   0 runner    (1001) docker     (127)    82252 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_prosub.json
--rw-r--r--   0 runner    (1001) docker     (127)    81050 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_realm.json
--rw-r--r--   0 runner    (1001) docker     (127)    83176 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_sub.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.348687 storynavigator-0.0.8/orangecontrib/storynavigation/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_en.json
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_nl.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.348687 storynavigator-0.0.8/orangecontrib/storynavigation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGDepParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGRuleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGSRL.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.348687 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)    29645 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNActionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    31829 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNActorAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNAnthologyNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNBreachAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14726 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNMeansAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14766 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNNarrativeNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    14718 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNPurposeAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    30124 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNSentimentAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNSettingAnalysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.352687 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    39515 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/Category-NavigatingStories.png
--rw-r--r--   0 runner    (1001) docker     (127)      468 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/action_analysis_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/actor_analysis_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    17139 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/anthology_network_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   123378 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/breach_analysis_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/means_analysis_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/narrative_network_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/purpose_analysis_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)   335593 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/sentiment_analysis_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/setting_analysis_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23162 2023-12-11 20:39:33.000000 storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/tagger_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 20:39:52.356687 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-11 20:39:52.000000 storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-11 20:39:33.000000 storynavigator-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-11 20:39:33.000000 storynavigator-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-12-11 20:39:52.356687 storynavigator-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1444 2023-12-11 20:39:33.000000 storynavigator-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.114737 storynavigator-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-11 21:21:38.000000 storynavigator-0.0.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-11 21:21:38.000000 storynavigator-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-11 21:21:38.000000 storynavigator-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-12-11 21:21:59.114737 storynavigator-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-12-11 21:21:38.000000 storynavigator-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2023-12-11 21:21:38.000000 storynavigator-0.0.9/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2023-12-11 21:21:38.000000 storynavigator-0.0.9/distribute_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.094737 storynavigator-0.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.094737 storynavigator-0.0.9/doc/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/dsgdepparser.md
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/dsgruleset.md
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/dsgsrl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/dsgtagger.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.094737 storynavigator-0.0.9/doc/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    25652 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/icons/dsg_ruleset_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26587 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/icons/dsg_stanzadep_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21161 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/icons/dsg_stanzasrl_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.098737 storynavigator-0.0.9/doc/widgets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   904633 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/images/dsgdepparser-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   820676 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/images/dsgruleset-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   629997 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/images/dsgsrl-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   508321 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets/images/dsgtagger-example2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-11 21:21:38.000000 storynavigator-0.0.9/doc/widgets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.098737 storynavigator-0.0.9/orangecontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.098737 storynavigator-0.0.9/orangecontrib/storynavigation/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.102737 storynavigator-0.0.9/orangecontrib/storynavigation/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/modules/actionanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23685 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/modules/actoranalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/modules/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/modules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.102737 storynavigator-0.0.9/orangecontrib/storynavigation/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   284185 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/dictionary_verbs_halliday_dimensions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/dutchpronouns.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/dutchstopwords.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    81490 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_process.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82252 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_prosub.json
+-rw-r--r--   0 runner    (1001) docker     (127)    81050 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_realm.json
+-rw-r--r--   0 runner    (1001) docker     (127)    83176 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_sub.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.102737 storynavigator-0.0.9/orangecontrib/storynavigation/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_nl.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.106737 storynavigator-0.0.9/orangecontrib/storynavigation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGDepParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGRuleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGSRL.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.106737 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)    29011 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNActionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31489 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNActorAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNAnthologyNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNBreachAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14726 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNMeansAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14766 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNNarrativeNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14718 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNPurposeAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30124 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNSentimentAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNSettingAnalysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.110737 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    39515 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/Category-NavigatingStories.png
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/action_analysis_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/actor_analysis_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17139 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/anthology_network_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123378 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/breach_analysis_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/means_analysis_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/narrative_network_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/purpose_analysis_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   335593 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/sentiment_analysis_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/setting_analysis_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23162 2023-12-11 21:21:38.000000 storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/tagger_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:21:59.110737 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 21:21:58.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-11 21:21:59.000000 storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-11 21:21:38.000000 storynavigator-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-11 21:21:38.000000 storynavigator-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-12-11 21:21:59.114737 storynavigator-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1444 2023-12-11 21:21:38.000000 storynavigator-0.0.9/tox.ini
```

### Comparing `storynavigator-0.0.8/LICENSE` & `storynavigator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/PKG-INFO` & `storynavigator-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storynavigator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Narrative analysis add-on for the Orange 3 data mining software package.
 Home-page: https://github.com/navigating-stories/orange-story-navigator
 Author: Kody Moodley
 Project-URL: Bug Tracker, https://github.com/navigating-stories/orange-story-navigator/issues
 Keywords: orange3 add-on,story analysis,narrative theory,natural language processing,text mining,story networks,character networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `storynavigator-0.0.8/README.md` & `storynavigator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/README.pypi` & `storynavigator-0.0.9/README.pypi`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/distribute_setup.py` & `storynavigator-0.0.9/distribute_setup.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/Makefile` & `storynavigator-0.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/conf.py` & `storynavigator-0.0.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/make.bat` & `storynavigator-0.0.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/dsgdepparser.md` & `storynavigator-0.0.9/doc/widgets/dsgdepparser.md`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/dsgruleset.md` & `storynavigator-0.0.9/doc/widgets/dsgruleset.md`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/dsgsrl.md` & `storynavigator-0.0.9/doc/widgets/dsgsrl.md`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/dsgtagger.md` & `storynavigator-0.0.9/doc/widgets/dsgtagger.md`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/icons/dsg_ruleset_icon.png` & `storynavigator-0.0.9/doc/widgets/icons/dsg_ruleset_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/icons/dsg_stanzadep_icon.png` & `storynavigator-0.0.9/doc/widgets/icons/dsg_stanzadep_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/icons/dsg_stanzasrl_icon.png` & `storynavigator-0.0.9/doc/widgets/icons/dsg_stanzasrl_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/images/dsgdepparser-example.png` & `storynavigator-0.0.9/doc/widgets/images/dsgdepparser-example.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/images/dsgruleset-example.png` & `storynavigator-0.0.9/doc/widgets/images/dsgruleset-example.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/images/dsgsrl-example.png` & `storynavigator-0.0.9/doc/widgets/images/dsgsrl-example.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets/images/dsgtagger-example2.png` & `storynavigator-0.0.9/doc/widgets/images/dsgtagger-example2.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/doc/widgets.json` & `storynavigator-0.0.9/doc/widgets.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/modules/actionanalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/modules/actionanalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/modules/actoranalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/modules/actoranalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/modules/constants.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/modules/constants.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/modules/util.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/modules/util.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/dictionary_verbs_halliday_dimensions.csv` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/dictionary_verbs_halliday_dimensions.csv`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/dutchstopwords.txt` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/dutchstopwords.txt`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_process.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_process.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_prosub.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_prosub.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_realm.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_realm.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/resources/halliday_dimensions_sub.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/resources/halliday_dimensions_sub.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_en.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_en.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_nl.json` & `storynavigator-0.0.9/orangecontrib/storynavigation/rules/multilingual_dsg_patterns_nl.json`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGDepParser.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGDepParser.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGRuleset.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGRuleset.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/tests/testOWSNDSGSRL.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/tests/testOWSNDSGSRL.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNActionAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNActionAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,14 @@
     zero_pos = Setting(False)
 
     # Panels for POS and NER tag types or lists
     postags_box = None
 
     # original text (not tagged)
     original_text = ""
-    word_prominence_scores = {}
     sli = None
 
     # list of colour values for the background highlight for each entity type
     highlight_colors = {}
 
     # list of POS checkboxes for each POS type
     pos_checkboxes = []
@@ -565,42 +564,28 @@
         with disconnected(
             self.doc_list.selectionModel().selectionChanged, self.selection_changed
         ):
             view.selectionModel().select(selection, QItemSelectionModel.ClearAndSelect)
 
     def selection_changed(self) -> None:
         """Function is called every time the selection changes"""
-        self.agent_prominence_score_min = 0.0
-        self.actiontagger.word_prominence_scores = {}
         self.actiontagger.noun_action_dict = {}
         self.actiontagger.num_occurences_as_subject = {}
         self.actiontagger.num_occurences = {}
         self.actiontagger.sentence_count = 0
         self.actiontagger.word_count = 0
         self.actiontagger.word_count_nostops = 0
         self.actiontagger.html_result = ""
         self.actiontagger.sentence_nlp_models = []
 
         self.selected_documents = self.get_selected_indexes()
         self.show_docs()
         self.commit.deferred()
 
-    def prominence_metric_change(self):
-        self.agent_prominence_score_min = 0.0
-        self.actiontagger.word_prominence_scores = {}
-        self.show_docs(slider_engaged=False)
-        self.commit.deferred()
-
-    def slider_callback(self):
-        if self.agent_prominence_score_min > self.agent_prominence_score_max:
-            self.agent_prominence_score_min = self.agent_prominence_score_max
-        self.show_docs(slider_engaged=True)
-        self.commit.deferred()
-
-    def show_docs(self, slider_engaged=False):
+    def show_docs(self):
         if not hasattr(self, "actiontagger"):
             self.actiontagger = ActionTagger(constants.NL_SPACY_MODEL)
 
         """Show the selected documents in the right area"""
         if self.corpus is None:
             return
```

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNActorAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNActorAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -674,15 +674,15 @@
 
                 if feature.name == "content":
                     value = self.actortagger.postag_text(
                         value,
                         self.nouns,
                         self.subjs,
                         self.agent_prominence_metric,
-                        self.agent_prominence_score_min,
+                        self.agent_prominence_score_min
                     )
                     self.Outputs.metrics_freq_table.send(
                         table_from_frame(
                             self.actortagger.calculate_metrics_freq_table()
                         )
                     )
                     self.Outputs.metrics_subfreq_table.send(
@@ -716,25 +716,14 @@
             parts.append(text)
 
         joined = SEPARATOR.join(parts)
         html = f"<table>{joined}</table>"
         base = QUrl.fromLocalFile(__file__)
         self.doc_webview.setHtml(HTML.format(html), base)
 
-    def as_list(self, dw):
-        res = []
-        for item in dw:
-            if type(item) == str and item != "N/A":
-                words = item.split(" | ")
-                if len(words) > 0:
-                    for word in words:
-                        res.append(word.lower().strip())
-
-        return list(set(res))
-
     def __mark_text(self, text):
         search_keyword = self.regexp_filter.strip("|")
         if not search_keyword:
             return text
 
         try:
             reg = re.compile(search_keyword, re.IGNORECASE | re.MULTILINE)
@@ -873,14 +862,14 @@
                     attr: 1 if isinstance(v, list) else v
                     for attr, v in context.attributes + context.class_vars
                 }
                 context.metas = dict(context.metas)
                 delattr(context, "class_vars")
 
 
-# if __name__ == "__main__":
-#     from orangewidget.utils.widgetpreview import WidgetPreview
-#     from orangecontrib.text.preprocess import BASE_TOKENIZER
-#     corpus_ = Corpus.from_file("book-excerpts")
-#     corpus_ = corpus_[:3]
-#     corpus_ = BASE_TOKENIZER(corpus_)
-#     WidgetPreview(OWSNActorAnalysis).run(corpus_)
+if __name__ == "__main__":
+    from orangewidget.utils.widgetpreview import WidgetPreview
+    from orangecontrib.text.preprocess import BASE_TOKENIZER
+    corpus_ = Corpus.from_file("book-excerpts")
+    corpus_ = corpus_[:3]
+    corpus_ = BASE_TOKENIZER(corpus_)
+    WidgetPreview(OWSNActorAnalysis).run(corpus_)
```

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNAnthologyNetwork.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNAnthologyNetwork.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNBreachAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNBreachAnalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNMeansAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNMeansAnalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNNarrativeNetwork.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNNarrativeNetwork.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNPurposeAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNPurposeAnalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNSentimentAnalyzer.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNSentimentAnalyzer.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/OWSNSettingAnalysis.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/OWSNSettingAnalysis.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/__init__.py` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/Category-NavigatingStories.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/Category-NavigatingStories.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/actor_analysis_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/actor_analysis_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/anthology_network_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/anthology_network_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/breach_analysis_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/breach_analysis_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/means_analysis_icon.svg` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/means_analysis_icon.svg`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/narrative_network_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/narrative_network_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/purpose_analysis_icon.svg` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/purpose_analysis_icon.svg`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/sentiment_analysis_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/sentiment_analysis_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigation/widgets/icons/tagger_icon.png` & `storynavigator-0.0.9/orangecontrib/storynavigation/widgets/icons/tagger_icon.png`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/PKG-INFO` & `storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storynavigator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Narrative analysis add-on for the Orange 3 data mining software package.
 Home-page: https://github.com/navigating-stories/orange-story-navigator
 Author: Kody Moodley
 Project-URL: Bug Tracker, https://github.com/navigating-stories/orange-story-navigator/issues
 Keywords: orange3 add-on,story analysis,narrative theory,natural language processing,text mining,story networks,character networks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `storynavigator-0.0.8/orangecontrib/storynavigator.egg-info/SOURCES.txt` & `storynavigator-0.0.9/orangecontrib/storynavigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storynavigator-0.0.8/setup.cfg` & `storynavigator-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	character networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = storynavigator
 project_urls = 
 	Bug Tracker = https://github.com/navigating-stories/orange-story-navigator/issues
 url = https://github.com/navigating-stories/orange-story-navigator
-version = 0.0.8
+version = 0.0.9
 
 [options]
 packages = find:
 package_dir = 
 	= orangecontrib
 include_package_data = True
 zip_safe = False
```

### Comparing `storynavigator-0.0.8/tox.ini` & `storynavigator-0.0.9/tox.ini`

 * *Files identical despite different names*

