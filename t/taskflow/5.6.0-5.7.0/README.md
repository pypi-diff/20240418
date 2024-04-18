# Comparing `tmp/taskflow-5.6.0.tar.gz` & `tmp/taskflow-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskflow-5.6.0.tar", last modified: Fri Mar 15 15:02:40 2024, max compression
+gzip compressed data, was "taskflow-5.7.0.tar", last modified: Thu Apr 18 10:24:15 2024, max compression
```

## Comparing `taskflow-5.6.0.tar` & `taskflow-5.7.0.tar`

### file list

```diff
@@ -1,383 +1,384 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.158994 taskflow-5.6.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-03-15 15:02:10.000000 taskflow-5.6.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-15 15:02:10.000000 taskflow-5.6.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-03-15 15:02:10.000000 taskflow-5.6.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-03-15 15:02:10.000000 taskflow-5.6.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2024-03-15 15:02:10.000000 taskflow-5.6.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2024-03-15 15:02:39.000000 taskflow-5.6.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-03-15 15:02:10.000000 taskflow-5.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78531 2024-03-15 15:02:39.000000 taskflow-5.6.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-15 15:02:10.000000 taskflow-5.6.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-03-15 15:02:40.158994 taskflow-5.6.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2024-03-15 15:02:10.000000 taskflow-5.6.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-03-15 15:02:10.000000 taskflow-5.6.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.090996 taskflow-5.6.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.094996 taskflow-5.6.0/doc/diagrams/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/diagrams/area_of_influence.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16344 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/diagrams/core.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27254 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/diagrams/jobboard.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    99579 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/diagrams/tasks.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/diagrams/worker-engine.graffle.tgz
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.094996 taskflow-5.6.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.094996 taskflow-5.6.0/doc/source/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/templates/layout.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.098996 taskflow-5.6.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14336 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/arguments_and_results.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8573 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/atoms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/conductors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21501 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/engines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8567 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/examples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/exceptions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/history.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.102995 taskflow-5.6.0/doc/source/user/img/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/area_of_influence.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/conductor.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36940 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/conductor_cycle.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68549 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/distributed_flow_rpc.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24407 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/engine_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/flow_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/job_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   110260 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/jobboard.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21971 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/mandelbrot.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22538 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/retry_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20666 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/task_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   241180 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/tasks.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16727 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/wbe_request_states.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25165 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/img/worker-engine.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5696 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/inputs_and_outputs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13665 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/jobs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6370 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/patterns.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12122 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/persistence.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/resumption.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/shelf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10022 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/states.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/utils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16388 2024-03-15 15:02:10.000000 taskflow-5.6.0/doc/source/user/workers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2024-03-15 15:02:10.000000 taskflow-5.6.0/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.082996 taskflow-5.6.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.106995 taskflow-5.6.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/add-sentinel-redis-support-9fd16e2a5dd5c0c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/bug-2056656-871b67ddbc8cfc92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/fix-endless-loop-on-storage-error-dd4467f0bbc66abf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/fix-endless-loop-on-storage-failures-b98b30f0c34d25e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/fix-storage-failure-handling-5c115d92daa0eb82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/fix-zookeeper-option-parsing-f9d37fbc39af47f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/redis-username-df0eb33869db09a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/remove-strict-redis-f2a5a924b314de41.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/sentinel-fallbacks-6fe2ab0d68959cdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/sentinel-ssl-399c56ed7067d282.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/sentinel-use-redis-creds-63f58b12ad46a2b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.106995 taskflow-5.6.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.106995 taskflow-5.6.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.106995 taskflow-5.6.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-15 15:02:10.000000 taskflow-5.6.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-03-15 15:02:10.000000 taskflow-5.6.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1988 2024-03-15 15:02:10.000000 taskflow-5.6.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2024-03-15 15:02:40.162994 taskflow-5.6.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-15 15:02:10.000000 taskflow-5.6.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.110995 taskflow-5.6.0/taskflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17342 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/atom.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.110995 taskflow-5.6.0/taskflow/conductors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.114995 taskflow-5.6.0/taskflow/conductors/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/backends/impl_blocking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15160 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/backends/impl_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/backends/impl_nonblocking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/conductors/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.114995 taskflow-5.6.0/taskflow/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/deciders.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.114995 taskflow-5.6.0/taskflow/engines/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.114995 taskflow-5.6.0/taskflow/engines/action_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.118995 taskflow-5.6.0/taskflow/engines/action_engine/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/actions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/actions/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/actions/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17015 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/builder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16164 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/compiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9028 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/completer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7254 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/deciders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29532 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27828 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/process_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/runtime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/scopes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11558 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/selector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/action_engine/traversal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4865 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10952 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.118995 taskflow-5.6.0/taskflow/engines/worker_based/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7145 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/dispatcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13811 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20238 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9525 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11559 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6331 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/engines/worker_based/worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.130995 taskflow-5.6.0/taskflow/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8893 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/99_bottles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3255 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/alphabet_soup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6554 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/build_a_car.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/buildsystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3917 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/calculate_in_parallel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4614 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/calculate_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4336 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/create_parallel_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/delayed_return.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/distance_calculator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/dump_memory_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/echo_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/example_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6832 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/fake_billing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/hello_world.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/jobboard_produce_consume_colors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/parallel_table_multiply.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3906 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/persistence_example.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/pseudo_scoping.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/pseudo_scoping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_from_backend.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_from_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.134995 taskflow-5.6.0/taskflow/examples/resume_many_flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_many_flows/my_flows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_many_flows/resume_all.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_many_flows/run_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_many_flows.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_many_flows.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9636 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_vm_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/resume_volume_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/retry_flow.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/retry_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/reverting_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/reverting_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/run_by_iter.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/run_by_iter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/run_by_iter_enumerate.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/run_by_iter_enumerate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/share_engine_thread.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear_listening.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear_listening.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear_pass.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_linear_pass.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3762 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/simple_map_reduce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/switch_graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/timing_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8472 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/tox_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5547 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wbe_event_sender.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wbe_mandelbrot.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8842 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wbe_mandelbrot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wbe_simple_linear.out.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wbe_simple_linear.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/examples/wrapped_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/formatters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.134995 taskflow-5.6.0/taskflow/jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/jobs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.134995 taskflow-5.6.0/taskflow/jobs/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/jobs/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43925 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/jobs/backends/impl_redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37644 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/jobs/backends/impl_zookeeper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22463 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/jobs/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.134995 taskflow-5.6.0/taskflow/listeners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7391 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/capturing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8516 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/printing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6943 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/listeners/timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/logging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.134995 taskflow-5.6.0/taskflow/patterns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/patterns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15292 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/patterns/graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/patterns/linear_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/patterns/unordered_flow.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.138995 taskflow-5.6.0/taskflow/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.138995 taskflow-5.6.0/taskflow/persistence/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/impl_dir.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/impl_memory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25540 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/impl_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/impl_zookeeper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.138995 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.138995 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2467 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.142994 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4072 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40762 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/persistence/path_based.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14537 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6901 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52114 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10052 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10456 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.142994 taskflow-5.6.0/taskflow/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/test_examples.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.146994 taskflow-5.6.0/taskflow/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.146994 taskflow-5.6.0/taskflow/tests/unit/action_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12866 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/test_builder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23759 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/test_compile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/test_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/test_process_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11327 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/action_engine/test_scoping.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.150994 taskflow-5.6.0/taskflow/tests/unit/jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/jobs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8447 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/jobs/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/jobs/test_entrypoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7540 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/jobs/test_redis_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13789 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/jobs/test_zk_job.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.150994 taskflow-5.6.0/taskflow/tests/unit/patterns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/patterns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12452 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/patterns/test_graph_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/patterns/test_linear_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4981 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/patterns/test_unordered_flow.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.150994 taskflow-5.6.0/taskflow/tests/unit/persistence/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16547 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/test_dir_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7871 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/test_memory_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10260 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/test_sql_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/persistence/test_zk_persistence.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_arguments_passing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6173 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_check_transition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18996 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_conductors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_deciders.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_engine_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64393 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_engines.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4362 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17982 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18086 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_flow_dependencies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_formatters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_functor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15304 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_listeners.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_mapfunctor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7894 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_progress.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_reducefunctor_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56365 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_retries.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23520 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9900 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_suspend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15947 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20225 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11035 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils_async_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3168 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils_binary.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils_iter_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils_kazoo_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5503 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/test_utils_threading_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.154994 taskflow-5.6.0/taskflow/tests/unit/worker_based/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2915 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_dispatcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13622 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_message_pump.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3812 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7745 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/unit/worker_based/test_worker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11157 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.154994 taskflow-5.6.0/taskflow/types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/entity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21189 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/latch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14071 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/timing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15820 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/types/tree.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.158994 taskflow-5.6.0/taskflow/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/async_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/banner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/eventlet_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/iter_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9915 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/kazoo_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/kombu_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18504 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/persistence_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4345 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/redis_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1434 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/schema_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5849 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/utils/threading_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2024-03-15 15:02:10.000000 taskflow-5.6.0/taskflow/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.110995 taskflow-5.6.0/taskflow.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13056 2024-03-15 15:02:40.000000 taskflow-5.6.0/taskflow.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-03-15 15:02:39.000000 taskflow-5.6.0/taskflow.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-03-15 15:02:10.000000 taskflow-5.6.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 15:02:40.158994 taskflow-5.6.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/clear_zk.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/env_builder.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/pretty_tox.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3003 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/schema_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3999 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/speed_test.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7182 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/state_graph.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10573 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/subunit_trace.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/test-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1521 2024-03-15 15:02:10.000000 taskflow-5.6.0/tools/update_states.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2024-03-15 15:02:10.000000 taskflow-5.6.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.358343 taskflow-5.7.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-04-18 10:23:47.000000 taskflow-5.7.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-04-18 10:23:47.000000 taskflow-5.7.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-04-18 10:23:47.000000 taskflow-5.7.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-04-18 10:23:47.000000 taskflow-5.7.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2024-04-18 10:23:47.000000 taskflow-5.7.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2024-04-18 10:24:15.000000 taskflow-5.7.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-04-18 10:23:47.000000 taskflow-5.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78616 2024-04-18 10:24:15.000000 taskflow-5.7.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-18 10:23:47.000000 taskflow-5.7.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-04-18 10:24:15.358343 taskflow-5.7.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2024-04-18 10:23:47.000000 taskflow-5.7.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-04-18 10:23:47.000000 taskflow-5.7.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.318341 taskflow-5.7.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.318341 taskflow-5.7.0/doc/diagrams/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/diagrams/area_of_influence.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16344 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/diagrams/core.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27254 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/diagrams/jobboard.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    99579 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/diagrams/tasks.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6967 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/diagrams/worker-engine.graffle.tgz
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.318341 taskflow-5.7.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.318341 taskflow-5.7.0/doc/source/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/templates/layout.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.322341 taskflow-5.7.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14336 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/arguments_and_results.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8573 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/atoms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/conductors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21501 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/engines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8567 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/examples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/exceptions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/history.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.326341 taskflow-5.7.0/doc/source/user/img/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/area_of_influence.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/conductor.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36940 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/conductor_cycle.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68549 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/distributed_flow_rpc.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24407 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/engine_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/flow_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13531 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/job_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   110260 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/jobboard.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21971 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/mandelbrot.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22538 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/retry_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20666 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/task_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   241180 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/tasks.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16727 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/wbe_request_states.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25165 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/img/worker-engine.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5696 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/inputs_and_outputs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13665 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/jobs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6370 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/patterns.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12122 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/persistence.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/resumption.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/shelf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10022 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/states.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/utils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16388 2024-04-18 10:23:47.000000 taskflow-5.7.0/doc/source/user/workers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2024-04-18 10:23:47.000000 taskflow-5.7.0/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.314341 taskflow-5.7.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.326341 taskflow-5.7.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/add-sentinel-redis-support-9fd16e2a5dd5c0c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/bug-2056656-871b67ddbc8cfc92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/fix-endless-loop-on-storage-error-dd4467f0bbc66abf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/fix-endless-loop-on-storage-failures-b98b30f0c34d25e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/fix-storage-failure-handling-5c115d92daa0eb82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/fix-zookeeper-option-parsing-f9d37fbc39af47f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/redis-username-df0eb33869db09a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/remove-strict-redis-f2a5a924b314de41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/sentinel-fallbacks-6fe2ab0d68959cdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/sentinel-ssl-399c56ed7067d282.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/sentinel-use-redis-creds-63f58b12ad46a2b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-04-18 10:23:47.000000 taskflow-5.7.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-04-18 10:23:47.000000 taskflow-5.7.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1988 2024-04-18 10:23:47.000000 taskflow-5.7.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2024-04-18 10:24:15.358343 taskflow-5.7.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-18 10:23:47.000000 taskflow-5.7.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17342 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/atom.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow/conductors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow/conductors/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/backends/impl_blocking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15160 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/backends/impl_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3014 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/backends/impl_nonblocking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/conductors/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/deciders.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow/engines/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.334342 taskflow-5.7.0/taskflow/engines/action_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.334342 taskflow-5.7.0/taskflow/engines/action_engine/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/actions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/actions/retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/actions/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17015 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/builder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16164 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/compiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9028 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/completer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7254 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/deciders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29532 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27828 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/process_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/runtime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/scopes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11558 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/selector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4552 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/action_engine/traversal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4865 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10952 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.334342 taskflow-5.7.0/taskflow/engines/worker_based/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7145 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13811 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20238 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9525 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11559 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6331 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/engines/worker_based/worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.338342 taskflow-5.7.0/taskflow/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8893 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/99_bottles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3255 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/alphabet_soup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6554 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/build_a_car.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/buildsystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3917 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/calculate_in_parallel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4614 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/calculate_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4336 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/create_parallel_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/delayed_return.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/distance_calculator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/dump_memory_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/echo_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/example_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6832 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/fake_billing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/hello_world.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6821 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/jobboard_produce_consume_colors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/parallel_table_multiply.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3906 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/persistence_example.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/pseudo_scoping.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/pseudo_scoping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_from_backend.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_from_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/examples/resume_many_flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1288 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_many_flows/my_flows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_many_flows/resume_all.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_many_flows/run_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_many_flows.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3192 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_many_flows.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9636 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_vm_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/resume_volume_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/retry_flow.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/retry_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/reverting_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/reverting_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/run_by_iter.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2620 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/run_by_iter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/run_by_iter_enumerate.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/run_by_iter_enumerate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2742 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/share_engine_thread.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear_listening.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear_listening.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear_pass.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_linear_pass.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3762 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/simple_map_reduce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/switch_graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/timing_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8472 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/tox_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5547 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wbe_event_sender.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wbe_mandelbrot.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8842 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wbe_mandelbrot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wbe_simple_linear.out.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wbe_simple_linear.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4732 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/examples/wrapped_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4834 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/formatters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/jobs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/jobs/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2902 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/jobs/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43925 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/jobs/backends/impl_redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37644 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/jobs/backends/impl_zookeeper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22463 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/jobs/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/listeners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7391 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/capturing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4115 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8516 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/printing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6943 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/listeners/timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/logging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/patterns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/patterns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15292 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/patterns/graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/patterns/linear_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/patterns/unordered_flow.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/persistence/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/impl_dir.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/impl_memory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25540 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/impl_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/impl_zookeeper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.342342 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.346342 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2683 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.346342 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4072 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40762 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9545 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/persistence/path_based.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14537 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6901 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52114 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10052 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10456 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.346342 taskflow-5.7.0/taskflow/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/test_examples.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.350342 taskflow-5.7.0/taskflow/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.350342 taskflow-5.7.0/taskflow/tests/unit/action_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12866 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/test_builder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23759 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/test_compile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3517 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/test_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/test_process_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11327 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/action_engine/test_scoping.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.350342 taskflow-5.7.0/taskflow/tests/unit/jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/jobs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8447 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/jobs/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2220 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/jobs/test_entrypoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7394 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/jobs/test_redis_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13789 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/jobs/test_zk_job.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.350342 taskflow-5.7.0/taskflow/tests/unit/patterns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/patterns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12452 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/patterns/test_graph_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/patterns/test_linear_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4981 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/patterns/test_unordered_flow.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.350342 taskflow-5.7.0/taskflow/tests/unit/persistence/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16547 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/test_dir_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7871 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/test_memory_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10260 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/test_sql_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/persistence/test_zk_persistence.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9204 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_arguments_passing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6173 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_check_transition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18996 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_conductors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2733 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_deciders.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5399 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_engine_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64393 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_engines.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4362 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17982 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18086 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_flow_dependencies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_formatters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_functor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15304 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_listeners.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_mapfunctor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7894 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_progress.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_reducefunctor_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56365 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_retries.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23520 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9900 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_suspend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15947 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20225 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11035 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils_async_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3168 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils_binary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5716 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils_iter_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils_kazoo_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5503 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/test_utils_threading_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.354342 taskflow-5.7.0/taskflow/tests/unit/worker_based/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2915 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_dispatcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13622 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_message_pump.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3812 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_pipeline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7745 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14344 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/unit/worker_based/test_worker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11157 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.354342 taskflow-5.7.0/taskflow/types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/entity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21189 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/latch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14071 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/timing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15820 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/types/tree.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.354342 taskflow-5.7.0/taskflow/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/async_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/banner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/eventlet_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/iter_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9915 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/kazoo_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2528 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/kombu_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18504 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3899 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/persistence_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4345 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/redis_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1434 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/schema_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5849 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/utils/threading_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2024-04-18 10:23:47.000000 taskflow-5.7.0/taskflow/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.330341 taskflow-5.7.0/taskflow.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13087 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-18 10:24:15.000000 taskflow-5.7.0/taskflow.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-04-18 10:23:47.000000 taskflow-5.7.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 10:24:15.358343 taskflow-5.7.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      367 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/clear_zk.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/env_builder.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/pretty_tox.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3003 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/schema_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3999 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/speed_test.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7182 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/state_graph.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10573 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/subunit_trace.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/test-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1521 2024-04-18 10:23:47.000000 taskflow-5.7.0/tools/update_states.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2024-04-18 10:23:47.000000 taskflow-5.7.0/tox.ini
```

### Comparing `taskflow-5.6.0/.mailmap` & `taskflow-5.7.0/.mailmap`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/.pre-commit-config.yaml` & `taskflow-5.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/.zuul.yaml` & `taskflow-5.7.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/AUTHORS` & `taskflow-5.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/CONTRIBUTING.rst` & `taskflow-5.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/ChangeLog` & `taskflow-5.7.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 CHANGES
 =======
 
-5.6.0
+5.7.0
 -----
 
+* db: Don't rely on branched connections
+* Fix broken unit tests for redis jobboard driver
 * Revert "Use consistent credential for Redis and Redis Sentinel"
-* Update TOX\_CONSTRAINTS\_FILE for stable/2024.1
-* Update .gitreview for stable/2024.1
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/victoria
 
 5.5.0
 -----
 
 * Prevent potential ReDoS attack
 * redis: Support fallback servers
 * Use consistent credential for Redis and Redis Sentinel
```

### Comparing `taskflow-5.6.0/LICENSE` & `taskflow-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/PKG-INFO` & `taskflow-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflow
-Version: 5.6.0
+Version: 5.7.0
 Summary: Taskflow structured state management library.
 Home-page: https://docs.openstack.org/taskflow/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `taskflow-5.6.0/README.rst` & `taskflow-5.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/bindep.txt` & `taskflow-5.7.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/diagrams/area_of_influence.graffle.tgz` & `taskflow-5.7.0/doc/diagrams/area_of_influence.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/diagrams/core.graffle.tgz` & `taskflow-5.7.0/doc/diagrams/core.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/diagrams/jobboard.graffle.tgz` & `taskflow-5.7.0/doc/diagrams/jobboard.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/diagrams/tasks.graffle.tgz` & `taskflow-5.7.0/doc/diagrams/tasks.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/diagrams/worker-engine.graffle.tgz` & `taskflow-5.7.0/doc/diagrams/worker-engine.graffle.tgz`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/conf.py` & `taskflow-5.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/index.rst` & `taskflow-5.7.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/templates/layout.html` & `taskflow-5.7.0/doc/source/templates/layout.html`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/arguments_and_results.rst` & `taskflow-5.7.0/doc/source/user/arguments_and_results.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/atoms.rst` & `taskflow-5.7.0/doc/source/user/atoms.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/conductors.rst` & `taskflow-5.7.0/doc/source/user/conductors.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/engines.rst` & `taskflow-5.7.0/doc/source/user/engines.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/examples.rst` & `taskflow-5.7.0/doc/source/user/examples.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/area_of_influence.svg` & `taskflow-5.7.0/doc/source/user/img/area_of_influence.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/conductor.png` & `taskflow-5.7.0/doc/source/user/img/conductor.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/conductor_cycle.png` & `taskflow-5.7.0/doc/source/user/img/conductor_cycle.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/distributed_flow_rpc.png` & `taskflow-5.7.0/doc/source/user/img/distributed_flow_rpc.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/engine_states.svg` & `taskflow-5.7.0/doc/source/user/img/engine_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/flow_states.svg` & `taskflow-5.7.0/doc/source/user/img/flow_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/job_states.svg` & `taskflow-5.7.0/doc/source/user/img/job_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/jobboard.png` & `taskflow-5.7.0/doc/source/user/img/jobboard.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/mandelbrot.png` & `taskflow-5.7.0/doc/source/user/img/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/retry_states.svg` & `taskflow-5.7.0/doc/source/user/img/retry_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/task_states.svg` & `taskflow-5.7.0/doc/source/user/img/task_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/tasks.png` & `taskflow-5.7.0/doc/source/user/img/tasks.png`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/wbe_request_states.svg` & `taskflow-5.7.0/doc/source/user/img/wbe_request_states.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/img/worker-engine.svg` & `taskflow-5.7.0/doc/source/user/img/worker-engine.svg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/index.rst` & `taskflow-5.7.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/inputs_and_outputs.rst` & `taskflow-5.7.0/doc/source/user/inputs_and_outputs.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/jobs.rst` & `taskflow-5.7.0/doc/source/user/jobs.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/notifications.rst` & `taskflow-5.7.0/doc/source/user/notifications.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/persistence.rst` & `taskflow-5.7.0/doc/source/user/persistence.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/resumption.rst` & `taskflow-5.7.0/doc/source/user/resumption.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/shelf.rst` & `taskflow-5.7.0/doc/source/user/shelf.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/states.rst` & `taskflow-5.7.0/doc/source/user/states.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/types.rst` & `taskflow-5.7.0/doc/source/user/types.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/utils.rst` & `taskflow-5.7.0/doc/source/user/utils.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/doc/source/user/workers.rst` & `taskflow-5.7.0/doc/source/user/workers.rst`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/pylintrc` & `taskflow-5.7.0/pylintrc`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/releasenotes/source/conf.py` & `taskflow-5.7.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/requirements.txt` & `taskflow-5.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/run_tests.sh` & `taskflow-5.7.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/setup.cfg` & `taskflow-5.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/setup.py` & `taskflow-5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/atom.py` & `taskflow-5.7.0/taskflow/atom.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/conductors/backends/__init__.py` & `taskflow-5.7.0/taskflow/conductors/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/conductors/backends/impl_blocking.py` & `taskflow-5.7.0/taskflow/conductors/backends/impl_blocking.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/conductors/backends/impl_executor.py` & `taskflow-5.7.0/taskflow/conductors/backends/impl_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/conductors/backends/impl_nonblocking.py` & `taskflow-5.7.0/taskflow/conductors/backends/impl_nonblocking.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/conductors/base.py` & `taskflow-5.7.0/taskflow/conductors/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/deciders.py` & `taskflow-5.7.0/taskflow/deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/__init__.py` & `taskflow-5.7.0/taskflow/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/actions/base.py` & `taskflow-5.7.0/taskflow/engines/action_engine/actions/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/actions/retry.py` & `taskflow-5.7.0/taskflow/engines/action_engine/actions/retry.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/actions/task.py` & `taskflow-5.7.0/taskflow/engines/action_engine/actions/task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/builder.py` & `taskflow-5.7.0/taskflow/engines/action_engine/builder.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/compiler.py` & `taskflow-5.7.0/taskflow/engines/action_engine/compiler.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/completer.py` & `taskflow-5.7.0/taskflow/engines/action_engine/completer.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/deciders.py` & `taskflow-5.7.0/taskflow/engines/action_engine/deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/engine.py` & `taskflow-5.7.0/taskflow/engines/action_engine/engine.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/executor.py` & `taskflow-5.7.0/taskflow/engines/action_engine/executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/process_executor.py` & `taskflow-5.7.0/taskflow/engines/action_engine/process_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/runtime.py` & `taskflow-5.7.0/taskflow/engines/action_engine/runtime.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/scheduler.py` & `taskflow-5.7.0/taskflow/engines/action_engine/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/scopes.py` & `taskflow-5.7.0/taskflow/engines/action_engine/scopes.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/selector.py` & `taskflow-5.7.0/taskflow/engines/action_engine/selector.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/action_engine/traversal.py` & `taskflow-5.7.0/taskflow/engines/action_engine/traversal.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/base.py` & `taskflow-5.7.0/taskflow/engines/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/helpers.py` & `taskflow-5.7.0/taskflow/engines/helpers.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/dispatcher.py` & `taskflow-5.7.0/taskflow/engines/worker_based/dispatcher.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/endpoint.py` & `taskflow-5.7.0/taskflow/engines/worker_based/endpoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/engine.py` & `taskflow-5.7.0/taskflow/engines/worker_based/engine.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/executor.py` & `taskflow-5.7.0/taskflow/engines/worker_based/executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/protocol.py` & `taskflow-5.7.0/taskflow/engines/worker_based/protocol.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/proxy.py` & `taskflow-5.7.0/taskflow/engines/worker_based/proxy.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/server.py` & `taskflow-5.7.0/taskflow/engines/worker_based/server.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/types.py` & `taskflow-5.7.0/taskflow/engines/worker_based/types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/engines/worker_based/worker.py` & `taskflow-5.7.0/taskflow/engines/worker_based/worker.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/99_bottles.py` & `taskflow-5.7.0/taskflow/examples/99_bottles.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/alphabet_soup.py` & `taskflow-5.7.0/taskflow/examples/alphabet_soup.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/build_a_car.py` & `taskflow-5.7.0/taskflow/examples/build_a_car.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/buildsystem.py` & `taskflow-5.7.0/taskflow/examples/buildsystem.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/calculate_in_parallel.py` & `taskflow-5.7.0/taskflow/examples/calculate_in_parallel.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/calculate_linear.py` & `taskflow-5.7.0/taskflow/examples/calculate_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/create_parallel_volume.py` & `taskflow-5.7.0/taskflow/examples/create_parallel_volume.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/delayed_return.py` & `taskflow-5.7.0/taskflow/examples/delayed_return.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/distance_calculator.py` & `taskflow-5.7.0/taskflow/examples/distance_calculator.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/dump_memory_backend.py` & `taskflow-5.7.0/taskflow/examples/dump_memory_backend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/echo_listener.py` & `taskflow-5.7.0/taskflow/examples/echo_listener.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/example_utils.py` & `taskflow-5.7.0/taskflow/examples/example_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/fake_billing.py` & `taskflow-5.7.0/taskflow/examples/fake_billing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/graph_flow.py` & `taskflow-5.7.0/taskflow/examples/graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/hello_world.py` & `taskflow-5.7.0/taskflow/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/jobboard_produce_consume_colors.py` & `taskflow-5.7.0/taskflow/examples/jobboard_produce_consume_colors.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/parallel_table_multiply.py` & `taskflow-5.7.0/taskflow/examples/parallel_table_multiply.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/persistence_example.py` & `taskflow-5.7.0/taskflow/examples/persistence_example.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/pseudo_scoping.py` & `taskflow-5.7.0/taskflow/examples/pseudo_scoping.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_from_backend.out.txt` & `taskflow-5.7.0/taskflow/examples/resume_from_backend.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_from_backend.py` & `taskflow-5.7.0/taskflow/examples/resume_from_backend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_many_flows/my_flows.py` & `taskflow-5.7.0/taskflow/examples/resume_many_flows/my_flows.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_many_flows/resume_all.py` & `taskflow-5.7.0/taskflow/examples/resume_many_flows/resume_all.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_many_flows/run_flow.py` & `taskflow-5.7.0/taskflow/examples/resume_many_flows/run_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_many_flows.out.txt` & `taskflow-5.7.0/taskflow/examples/resume_many_flows.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_many_flows.py` & `taskflow-5.7.0/taskflow/examples/resume_many_flows.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_vm_boot.py` & `taskflow-5.7.0/taskflow/examples/resume_vm_boot.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/resume_volume_create.py` & `taskflow-5.7.0/taskflow/examples/resume_volume_create.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/retry_flow.py` & `taskflow-5.7.0/taskflow/examples/retry_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/reverting_linear.py` & `taskflow-5.7.0/taskflow/examples/reverting_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/run_by_iter.out.txt` & `taskflow-5.7.0/taskflow/examples/run_by_iter.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/run_by_iter.py` & `taskflow-5.7.0/taskflow/examples/run_by_iter.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/run_by_iter_enumerate.out.txt` & `taskflow-5.7.0/taskflow/examples/run_by_iter_enumerate.out.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/run_by_iter_enumerate.py` & `taskflow-5.7.0/taskflow/examples/run_by_iter_enumerate.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/share_engine_thread.py` & `taskflow-5.7.0/taskflow/examples/share_engine_thread.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/simple_linear.py` & `taskflow-5.7.0/taskflow/examples/simple_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/simple_linear_listening.py` & `taskflow-5.7.0/taskflow/examples/simple_linear_listening.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/simple_linear_pass.py` & `taskflow-5.7.0/taskflow/examples/simple_linear_pass.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/simple_map_reduce.py` & `taskflow-5.7.0/taskflow/examples/simple_map_reduce.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/switch_graph_flow.py` & `taskflow-5.7.0/taskflow/examples/switch_graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/timing_listener.py` & `taskflow-5.7.0/taskflow/examples/timing_listener.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/tox_conductor.py` & `taskflow-5.7.0/taskflow/examples/tox_conductor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/wbe_event_sender.py` & `taskflow-5.7.0/taskflow/examples/wbe_event_sender.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/wbe_mandelbrot.py` & `taskflow-5.7.0/taskflow/examples/wbe_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/wbe_simple_linear.py` & `taskflow-5.7.0/taskflow/examples/wbe_simple_linear.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/examples/wrapped_exception.py` & `taskflow-5.7.0/taskflow/examples/wrapped_exception.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/exceptions.py` & `taskflow-5.7.0/taskflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/flow.py` & `taskflow-5.7.0/taskflow/flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/formatters.py` & `taskflow-5.7.0/taskflow/formatters.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/jobs/backends/__init__.py` & `taskflow-5.7.0/taskflow/jobs/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/jobs/backends/impl_redis.py` & `taskflow-5.7.0/taskflow/jobs/backends/impl_redis.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/jobs/backends/impl_zookeeper.py` & `taskflow-5.7.0/taskflow/jobs/backends/impl_zookeeper.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/jobs/base.py` & `taskflow-5.7.0/taskflow/jobs/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/base.py` & `taskflow-5.7.0/taskflow/listeners/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/capturing.py` & `taskflow-5.7.0/taskflow/listeners/capturing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/claims.py` & `taskflow-5.7.0/taskflow/listeners/claims.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/logging.py` & `taskflow-5.7.0/taskflow/listeners/logging.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/printing.py` & `taskflow-5.7.0/taskflow/listeners/printing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/listeners/timing.py` & `taskflow-5.7.0/taskflow/listeners/timing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/logging.py` & `taskflow-5.7.0/taskflow/logging.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/patterns/graph_flow.py` & `taskflow-5.7.0/taskflow/patterns/graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/patterns/linear_flow.py` & `taskflow-5.7.0/taskflow/patterns/linear_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/patterns/unordered_flow.py` & `taskflow-5.7.0/taskflow/patterns/unordered_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/__init__.py` & `taskflow-5.7.0/taskflow/persistence/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/impl_dir.py` & `taskflow-5.7.0/taskflow/persistence/backends/impl_dir.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/impl_memory.py` & `taskflow-5.7.0/taskflow/persistence/backends/impl_memory.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/impl_sqlalchemy.py` & `taskflow-5.7.0/taskflow/persistence/backends/impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/impl_zookeeper.py` & `taskflow-5.7.0/taskflow/persistence/backends/impl_zookeeper.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,18 +59,23 @@
 
     """
     connectable = config.attributes.get('connection', None)
     if connectable is None:
         connectable = engine_from_config(
             config.get_section(config.config_ini_section),
             prefix='sqlalchemy.', poolclass=pool.NullPool)
-    with connectable.connect() as connection:
-        context.configure(connection=connection,
-                          target_metadata=target_metadata)
+        with connectable.connect() as connection:
+            context.configure(connection=connection,
+                              target_metadata=target_metadata)
+            with context.begin_transaction():
+                context.run_migrations()
+    else:
+        context.configure(
+            connection=connectable,
+            target_metadata=target_metadata)
         with context.begin_transaction():
             context.run_migrations()
 
-
 if context.is_offline_mode():
     run_migrations_offline()
 else:
     run_migrations_online()
```

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/0bc3e1a3c135_set_result_meduimtext_type.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/14b227d79a87_add_intention_column.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1c783c0c2875_replace_exception_an.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/1cea328f0f65_initial_logbook_deta.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/2ad4984f2864_switch_postgres_to_json_native.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/3162c0f3f8e4_add_revert_results_and_revert_failure_.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/40fc8c914bd2_fix_atomdetails_failure_size.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/589dccdf2b6e_rename_taskdetails_to_atomdetails.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/6df9422fcb43_fix_flowdetails_meta_size.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/alembic/versions/84d6e888850_add_task_detail_type.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/migration.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/backends/sqlalchemy/tables.py` & `taskflow-5.7.0/taskflow/persistence/backends/sqlalchemy/tables.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/base.py` & `taskflow-5.7.0/taskflow/persistence/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/models.py` & `taskflow-5.7.0/taskflow/persistence/models.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/persistence/path_based.py` & `taskflow-5.7.0/taskflow/persistence/path_based.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/retry.py` & `taskflow-5.7.0/taskflow/retry.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/states.py` & `taskflow-5.7.0/taskflow/states.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/storage.py` & `taskflow-5.7.0/taskflow/storage.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/task.py` & `taskflow-5.7.0/taskflow/task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/test.py` & `taskflow-5.7.0/taskflow/test.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/fixtures.py` & `taskflow-5.7.0/taskflow/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/test_examples.py` & `taskflow-5.7.0/taskflow/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/action_engine/test_builder.py` & `taskflow-5.7.0/taskflow/tests/unit/action_engine/test_builder.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/action_engine/test_compile.py` & `taskflow-5.7.0/taskflow/tests/unit/action_engine/test_compile.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/action_engine/test_creation.py` & `taskflow-5.7.0/taskflow/tests/unit/action_engine/test_creation.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/action_engine/test_process_executor.py` & `taskflow-5.7.0/taskflow/tests/unit/action_engine/test_process_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/action_engine/test_scoping.py` & `taskflow-5.7.0/taskflow/tests/unit/action_engine/test_scoping.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/jobs/base.py` & `taskflow-5.7.0/taskflow/tests/unit/jobs/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/jobs/test_entrypoint.py` & `taskflow-5.7.0/taskflow/tests/unit/jobs/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/jobs/test_redis_job.py` & `taskflow-5.7.0/taskflow/tests/unit/jobs/test_redis_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,41 +157,38 @@
                     '[::1]:26379', '127.0.0.2:26379', 'localhost:26379'
                 ]}
         with mock.patch('redis.sentinel.Sentinel') as mock_sentinel:
             impl_redis.RedisJobBoard('test-board', conf)
             test_conf = {
                 'username': 'default',
                 'password': 'secret',
+                'sentinel_kwargs': None,
             }
             mock_sentinel.assert_called_once_with(
                 [('127.0.0.1', 26379), ('::1', 26379),
                  ('127.0.0.2', 26379), ('localhost', 26379)],
-                sentinel_kwargs={
-                    'username': 'default',
-                    'password': 'secret'
-                },
                 **test_conf)
             mock_sentinel().master_for.assert_called_once_with('mymaster')
 
     def test__make_client_sentinel_ssl(self):
         conf = {'host': '127.0.0.1',
                 'port': 26379,
                 'username': 'default',
                 'password': 'secret',
                 'namespace': 'test',
                 'sentinel': 'mymaster',
-                'sentinel_kwargs': {'password': 'senitelsecret'},
+                'sentinel_kwargs': None,
                 'ssl': True,
                 'ssl_ca_certs': '/etc/ssl/certs'}
         with mock.patch('redis.sentinel.Sentinel') as mock_sentinel:
             impl_redis.RedisJobBoard('test-board', conf)
             test_conf = {
                 'username': 'default',
                 'password': 'secret',
                 'ssl': True,
                 'ssl_ca_certs': '/etc/ssl/certs',
             }
             mock_sentinel.assert_called_once_with(
                 [('127.0.0.1', 26379)],
-                sentinel_kwargs={'password': 'senitelsecret'},
+                sentinel_kwargs=None,
                 **test_conf)
             mock_sentinel().master_for.assert_called_once_with('mymaster')
```

### Comparing `taskflow-5.6.0/taskflow/tests/unit/jobs/test_zk_job.py` & `taskflow-5.7.0/taskflow/tests/unit/jobs/test_zk_job.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/patterns/test_graph_flow.py` & `taskflow-5.7.0/taskflow/tests/unit/patterns/test_graph_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/patterns/test_linear_flow.py` & `taskflow-5.7.0/taskflow/tests/unit/patterns/test_linear_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/patterns/test_unordered_flow.py` & `taskflow-5.7.0/taskflow/tests/unit/patterns/test_unordered_flow.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/persistence/base.py` & `taskflow-5.7.0/taskflow/tests/unit/persistence/base.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/persistence/test_dir_persistence.py` & `taskflow-5.7.0/taskflow/tests/unit/persistence/test_dir_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/persistence/test_memory_persistence.py` & `taskflow-5.7.0/taskflow/tests/unit/persistence/test_memory_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/persistence/test_sql_persistence.py` & `taskflow-5.7.0/taskflow/tests/unit/persistence/test_sql_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/persistence/test_zk_persistence.py` & `taskflow-5.7.0/taskflow/tests/unit/persistence/test_zk_persistence.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_arguments_passing.py` & `taskflow-5.7.0/taskflow/tests/unit/test_arguments_passing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_check_transition.py` & `taskflow-5.7.0/taskflow/tests/unit/test_check_transition.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_conductors.py` & `taskflow-5.7.0/taskflow/tests/unit/test_conductors.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_deciders.py` & `taskflow-5.7.0/taskflow/tests/unit/test_deciders.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_engine_helpers.py` & `taskflow-5.7.0/taskflow/tests/unit/test_engine_helpers.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_engines.py` & `taskflow-5.7.0/taskflow/tests/unit/test_engines.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_exceptions.py` & `taskflow-5.7.0/taskflow/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_failure.py` & `taskflow-5.7.0/taskflow/tests/unit/test_failure.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_flow_dependencies.py` & `taskflow-5.7.0/taskflow/tests/unit/test_flow_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_formatters.py` & `taskflow-5.7.0/taskflow/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_functor_task.py` & `taskflow-5.7.0/taskflow/tests/unit/test_functor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_listeners.py` & `taskflow-5.7.0/taskflow/tests/unit/test_listeners.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_mapfunctor_task.py` & `taskflow-5.7.0/taskflow/tests/unit/test_mapfunctor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_notifier.py` & `taskflow-5.7.0/taskflow/tests/unit/test_notifier.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_progress.py` & `taskflow-5.7.0/taskflow/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_reducefunctor_task.py` & `taskflow-5.7.0/taskflow/tests/unit/test_reducefunctor_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_retries.py` & `taskflow-5.7.0/taskflow/tests/unit/test_retries.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_states.py` & `taskflow-5.7.0/taskflow/tests/unit/test_states.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_storage.py` & `taskflow-5.7.0/taskflow/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_suspend.py` & `taskflow-5.7.0/taskflow/tests/unit/test_suspend.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_task.py` & `taskflow-5.7.0/taskflow/tests/unit/test_task.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_types.py` & `taskflow-5.7.0/taskflow/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils_async_utils.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils_async_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils_binary.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils_binary.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils_iter_utils.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils_iter_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils_kazoo_utils.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils_kazoo_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/test_utils_threading_utils.py` & `taskflow-5.7.0/taskflow/tests/unit/test_utils_threading_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_creation.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_creation.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_dispatcher.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_endpoint.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_executor.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_executor.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_message_pump.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_message_pump.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_pipeline.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_protocol.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_protocol.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_proxy.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_proxy.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_server.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_server.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_types.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_types.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/unit/worker_based/test_worker.py` & `taskflow-5.7.0/taskflow/tests/unit/worker_based/test_worker.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/tests/utils.py` & `taskflow-5.7.0/taskflow/tests/utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/entity.py` & `taskflow-5.7.0/taskflow/types/entity.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/failure.py` & `taskflow-5.7.0/taskflow/types/failure.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/graph.py` & `taskflow-5.7.0/taskflow/types/graph.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/latch.py` & `taskflow-5.7.0/taskflow/types/latch.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/notifier.py` & `taskflow-5.7.0/taskflow/types/notifier.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/sets.py` & `taskflow-5.7.0/taskflow/types/sets.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/timing.py` & `taskflow-5.7.0/taskflow/types/timing.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/types/tree.py` & `taskflow-5.7.0/taskflow/types/tree.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/async_utils.py` & `taskflow-5.7.0/taskflow/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/banner.py` & `taskflow-5.7.0/taskflow/utils/banner.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/eventlet_utils.py` & `taskflow-5.7.0/taskflow/utils/eventlet_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/iter_utils.py` & `taskflow-5.7.0/taskflow/utils/iter_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/kazoo_utils.py` & `taskflow-5.7.0/taskflow/utils/kazoo_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/kombu_utils.py` & `taskflow-5.7.0/taskflow/utils/kombu_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/misc.py` & `taskflow-5.7.0/taskflow/utils/misc.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/persistence_utils.py` & `taskflow-5.7.0/taskflow/utils/persistence_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/redis_utils.py` & `taskflow-5.7.0/taskflow/utils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/schema_utils.py` & `taskflow-5.7.0/taskflow/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/utils/threading_utils.py` & `taskflow-5.7.0/taskflow/utils/threading_utils.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow/version.py` & `taskflow-5.7.0/taskflow/version.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow.egg-info/PKG-INFO` & `taskflow-5.7.0/taskflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflow
-Version: 5.6.0
+Version: 5.7.0
 Summary: Taskflow structured state management library.
 Home-page: https://docs.openstack.org/taskflow/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `taskflow-5.6.0/taskflow.egg-info/SOURCES.txt` & `taskflow-5.7.0/taskflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 releasenotes/notes/remove-strict-redis-f2a5a924b314de41.yaml
 releasenotes/notes/sentinel-fallbacks-6fe2ab0d68959cdf.yaml
 releasenotes/notes/sentinel-ssl-399c56ed7067d282.yaml
 releasenotes/notes/sentinel-use-redis-creds-63f58b12ad46a2b5.yaml
 releasenotes/notes/zookeeper-ssl-support-b9abf24a39096b62.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
```

### Comparing `taskflow-5.6.0/taskflow.egg-info/entry_points.txt` & `taskflow-5.7.0/taskflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/taskflow.egg-info/requires.txt` & `taskflow-5.7.0/taskflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/test-requirements.txt` & `taskflow-5.7.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/env_builder.sh` & `taskflow-5.7.0/tools/env_builder.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/schema_generator.py` & `taskflow-5.7.0/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/speed_test.py` & `taskflow-5.7.0/tools/speed_test.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/state_graph.py` & `taskflow-5.7.0/tools/state_graph.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/subunit_trace.py` & `taskflow-5.7.0/tools/subunit_trace.py`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/test-setup.sh` & `taskflow-5.7.0/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tools/update_states.sh` & `taskflow-5.7.0/tools/update_states.sh`

 * *Files identical despite different names*

### Comparing `taskflow-5.6.0/tox.ini` & `taskflow-5.7.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [testenv]
 setenv =
 # TODO(stephenfin): Remove once we bump our upper-constraint to SQLAlchemy 2.0
   SQLALCHEMY_WARN_20=1
 # We need to install a bit more than just `test' because those drivers have
 # custom tests that we always run
 deps =
-  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2024.1}
+  -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
   -r{toxinidir}/requirements.txt
 commands =
   stestr run {posargs}
 
 [testenv:docs]
 deps =
```

