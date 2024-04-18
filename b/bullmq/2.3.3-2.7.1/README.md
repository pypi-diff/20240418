# Comparing `tmp/bullmq-2.3.3.tar.gz` & `tmp/bullmq-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-2.3.3.tar", last modified: Sun Mar 24 17:30:07 2024, max compression
+gzip compressed data, was "bullmq-2.7.1.tar", last modified: Thu Apr 18 01:24:08 2024, max compression
```

## Comparing `bullmq-2.3.3.tar` & `bullmq-2.7.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.764309 bullmq-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-24 17:30:07.764309 bullmq-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-24 17:29:16.000000 bullmq-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.752309 bullmq-2.3.3/bullmq/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-24 17:30:06.000000 bullmq-2.3.3/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.760309 bullmq-2.3.3/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/addDelayedJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/addParentJob-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/addPrioritizedJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/addStandardJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/changeDelay-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/changePriority-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveJobFromActiveToWait-10.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveJobsToWait-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveStalledJobsToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveToActive-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveToDelayed-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    25897 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveToFinished-14.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/paginate-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/pause-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/promote-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/removeChildDependency-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/reprocessJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/retryJob-10.lua
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-24 17:29:45.000000 bullmq-2.3.3/bullmq/commands/updateProgress-3.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.760309 bullmq-2.3.3/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/flow_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/queue_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.760309 bullmq-2.3.3/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/promote_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/retry_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-03-24 17:29:16.000000 bullmq-2.3.3/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 17:30:07.764309 bullmq-2.3.3/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-24 17:30:07.000000 bullmq-2.3.3/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-24 17:30:07.000000 bullmq-2.3.3/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 17:30:07.000000 bullmq-2.3.3/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-24 17:30:07.000000 bullmq-2.3.3/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-24 17:30:07.000000 bullmq-2.3.3/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-24 17:30:06.000000 bullmq-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 17:30:07.764309 bullmq-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-24 17:29:16.000000 bullmq-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-18 01:24:08.097629 bullmq-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-18 01:22:34.000000 bullmq-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.089629 bullmq-2.7.1/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 01:24:06.000000 bullmq-2.7.1/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addDelayedJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addParentJob-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addPrioritizedJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addStandardJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/changeDelay-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/changePriority-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveJobFromActiveToWait-10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveJobsToWait-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveStalledJobsToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToActive-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    25897 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToFinished-14.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToWaitingChildren-5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/paginate-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/pause-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/promote-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeChildDependency-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/reprocessJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/retryJob-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/updateProgress-3.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/flow_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/queue_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/promote_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/retry_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 01:24:06.000000 bullmq-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:24:08.097629 bullmq-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 01:22:34.000000 bullmq-2.7.1/setup.py
```

### Comparing `bullmq-2.3.3/PKG-INFO` & `bullmq-2.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.3.3
+Version: 2.7.1
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.3.3/README.md` & `bullmq-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/backoffs.py` & `bullmq-2.7.1/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/addDelayedJob-6.lua` & `bullmq-2.7.1/bullmq/commands/addDelayedJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/addParentJob-4.lua` & `bullmq-2.7.1/bullmq/commands/addParentJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/addPrioritizedJob-7.lua` & `bullmq-2.7.1/bullmq/commands/addPrioritizedJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/addStandardJob-7.lua` & `bullmq-2.7.1/bullmq/commands/addStandardJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/changeDelay-4.lua` & `bullmq-2.7.1/bullmq/commands/changeDelay-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/changePriority-6.lua` & `bullmq-2.7.1/bullmq/commands/changePriority-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-2.7.1/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/drain-4.lua` & `bullmq-2.7.1/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/getCounts-1.lua` & `bullmq-2.7.1/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/getRanges-1.lua` & `bullmq-2.7.1/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/getState-8.lua` & `bullmq-2.7.1/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/getStateV2-8.lua` & `bullmq-2.7.1/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/isFinished-3.lua` & `bullmq-2.7.1/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/moveJobFromActiveToWait-10.lua` & `bullmq-2.7.1/bullmq/commands/moveJobFromActiveToWait-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/moveJobsToWait-7.lua` & `bullmq-2.7.1/bullmq/commands/moveJobsToWait-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/moveStalledJobsToWait-9.lua` & `bullmq-2.7.1/bullmq/commands/moveStalledJobsToWait-9.lua`

 * *Files 24% similar despite different names*

```diff
@@ -59,14 +59,131 @@
   if rcall("HEXISTS", queueMetaKey, "paused") ~= 1 then
     return waitKey, false
   else
     return pausedKey, true
   end
 end
 --[[
+  Function to recursively move from waitingChildren to failed.
+]]
+-- Includes
+--[[
+  Validate and move parent to active if needed.
+]]
+-- Includes
+--[[
+  Add delay marker if needed.
+]]
+-- Includes
+--[[
+  Function to return the next delayed job timestamp.
+]]
+local function getNextDelayedTimestamp(delayedKey)
+  local result = rcall("ZRANGE", delayedKey, 0, 0, "WITHSCORES")
+  if #result then
+    local nextTimestamp = tonumber(result[2])
+    if (nextTimestamp ~= nil) then 
+      nextTimestamp = nextTimestamp / 0x1000
+    end
+    return nextTimestamp
+  end
+end
+local function addDelayMarkerIfNeeded(markerKey, delayedKey)
+    local nextTimestamp = getNextDelayedTimestamp(delayedKey)
+    if nextTimestamp ~= nil then
+        -- Replace the score of the marker with the newest known
+        -- next timestamp.
+        rcall("ZADD", markerKey, nextTimestamp, "1")
+    end
+end
+--[[
+  Function to add job considering priority.
+]]
+-- Includes
+local function addJobWithPriority(markerKey, prioritizedKey, priority, jobId, priorityCounterKey, isPaused)
+  local prioCounter = rcall("INCR", priorityCounterKey)
+  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
+  rcall("ZADD", prioritizedKey, score, jobId)
+  addBaseMarkerIfNeeded(markerKey, isPaused)
+end
+--[[
+  Function to check for the meta.paused key to decide if we are paused or not
+  (since an empty list and !EXISTS are not really the same).
+]]
+local function isQueuePaused(queueMetaKey)
+    return rcall("HEXISTS", queueMetaKey, "paused") == 1
+end
+local function moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey,
+                                        parentKey, parentId, timestamp)
+    local isParentActive = rcall("ZSCORE",
+                                 parentQueueKey .. ":waiting-children", parentId)
+    if rcall("SCARD", parentDependenciesKey) == 0 and isParentActive then
+        rcall("ZREM", parentQueueKey .. ":waiting-children", parentId)
+        local parentWaitKey = parentQueueKey .. ":wait"
+        local parentPausedKey = parentQueueKey .. ":paused"
+        local parentMetaKey = parentQueueKey .. ":meta"
+        local parentMarkerKey = parentQueueKey .. ":marker"
+        local jobAttributes = rcall("HMGET", parentKey, "priority", "delay")
+        local priority = tonumber(jobAttributes[1]) or 0
+        local delay = tonumber(jobAttributes[2]) or 0
+        if delay > 0 then
+            local delayedTimestamp = tonumber(timestamp) + delay
+            local score = delayedTimestamp * 0x1000
+            local parentDelayedKey = parentQueueKey .. ":delayed"
+            rcall("ZADD", parentDelayedKey, score, parentId)
+            rcall("XADD", parentQueueKey .. ":events", "*", "event", "delayed",
+                  "jobId", parentId, "delay", delayedTimestamp)
+            addDelayMarkerIfNeeded(parentMarkerKey, parentDelayedKey)
+        else
+            if priority == 0 then
+                local parentTarget, isParentPaused =
+                    getTargetQueueList(parentMetaKey, parentWaitKey,
+                                       parentPausedKey)
+                addJobInTargetList(parentTarget, parentMarkerKey, "RPUSH", isParentPaused, parentId)
+            else
+                local isPaused = isQueuePaused(parentMetaKey)
+                addJobWithPriority(parentMarkerKey,
+                                   parentQueueKey .. ":prioritized", priority,
+                                   parentId, parentQueueKey .. ":pc", isPaused)
+            end
+            rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting",
+                  "jobId", parentId, "prev", "waiting-children")
+        end
+    end
+end
+local function moveParentFromWaitingChildrenToFailed( parentQueueKey, parentKey, parentId, jobIdKey, timestamp)
+  if rcall("ZREM", parentQueueKey .. ":waiting-children", parentId) == 1 then
+    rcall("ZADD", parentQueueKey .. ":failed", timestamp, parentId)
+    local failedReason = "child " .. jobIdKey .. " failed"
+    rcall("HMSET", parentKey, "failedReason", failedReason, "finishedOn", timestamp)
+    rcall("XADD", parentQueueKey .. ":events", "*", "event", "failed", "jobId", parentId, "failedReason",
+      failedReason, "prev", "waiting-children")
+    local rawParentData = rcall("HGET", parentKey, "parent")
+    if rawParentData ~= false then
+      local parentData = cjson.decode(rawParentData)
+      if parentData['fpof'] then
+        moveParentFromWaitingChildrenToFailed(
+          parentData['queueKey'],
+          parentData['queueKey'] .. ':' .. parentData['id'],
+          parentData['id'],
+          parentKey,
+          timestamp
+        )
+      elseif parentData['rdof'] then
+        local grandParentKey = parentData['queueKey'] .. ':' .. parentData['id']
+        local grandParentDependenciesSet = grandParentKey .. ":dependencies"
+        if rcall("SREM", grandParentDependenciesSet, parentKey) == 1 then
+          moveParentToWaitIfNeeded(parentData['queueKey'], grandParentDependenciesSet,
+            grandParentKey, parentData['id'], timestamp)
+        end
+      end
+    end
+  end
+end
+--[[
   Function to remove job.
 ]]
 -- Includes
 --[[
   Function to remove job keys.
 ]]
 local function removeJobKeys(jobKey)
@@ -243,25 +360,37 @@
                 --  Remove from the active queue.
                 local removed = rcall("LREM", activeKey, 1, jobId)
                 if (removed > 0) then
                     -- If this job has been stalled too many times, such as if it crashes the worker, then fail it.
                     local stalledCount =
                         rcall("HINCRBY", jobKey, "stalledCounter", 1)
                     if (stalledCount > MAX_STALLED_JOB_COUNT) then
-                        local rawOpts = rcall("HGET", jobKey, "opts")
+                        local jobAttributes = rcall("HMGET", jobKey, "opts", "parent")
+                        local rawOpts = jobAttributes[1]
+                        local rawParentData = jobAttributes[2]
                         local opts = cjson.decode(rawOpts)
                         local removeOnFailType = type(opts["removeOnFail"])
                         rcall("ZADD", failedKey, timestamp, jobId)
                         local failedReason =
                             "job stalled more than allowable limit"
                         rcall("HMSET", jobKey, "failedReason", failedReason,
                               "finishedOn", timestamp)
                         rcall("XADD", eventStreamKey, "*", "event",
                               "failed", "jobId", jobId, 'prev', 'active',
                               'failedReason', failedReason)
+                        if opts['fpof'] and rawParentData ~= false then
+                            local parentData = cjson.decode(rawParentData)
+                            moveParentFromWaitingChildrenToFailed(
+                                parentData['queueKey'],
+                                parentData['queueKey'] .. ':' .. parentData['id'],
+                                parentData['id'],
+                                jobKey,
+                                timestamp
+                            )
+                        end
                         if removeOnFailType == "number" then
                             removeJobsByMaxCount(opts["removeOnFail"],
                                                   failedKey, queueKeyPrefix)
                         elseif removeOnFailType == "boolean" then
                             if opts["removeOnFail"] then
                                 removeJob(jobId, false, queueKeyPrefix)
                                 rcall("ZREM", failedKey, jobId)
```

### Comparing `bullmq-2.3.3/bullmq/commands/moveToActive-11.lua` & `bullmq-2.7.1/bullmq/commands/moveToActive-11.lua`

 * *Files 1% similar despite different names*

```diff
@@ -202,9 +202,9 @@
     if jobId then
         return prepareJobForProcessing(ARGV[1], rateLimiterKey, eventStreamKey, jobId, ARGV[2],
                                        maxJobs, opts)
     end
 end
 -- Return the timestamp for the next delayed job if any.
 local nextTimestamp = getNextDelayedTimestamp(delayedKey)
-if (nextTimestamp ~= nil) then return {0, 0, 0, nextTimestamp} end
+if nextTimestamp ~= nil then return {0, 0, 0, nextTimestamp} end
 return {0, 0, 0, 0}
```

### Comparing `bullmq-2.3.3/bullmq/commands/moveToDelayed-7.lua` & `bullmq-2.7.1/bullmq/commands/moveToDelayed-8.lua`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     KEYS[1] marker key
     KEYS[2] active key
     KEYS[3] prioritized key
     KEYS[4] delayed key
     KEYS[5] job key
     KEYS[6] events stream
     KEYS[7] meta key
+    KEYS[8] stalled key
     ARGV[1] key prefix
     ARGV[2] timestamp
     ARGV[3] delayedTimestamp
     ARGV[4] the id of the job
     ARGV[5] queue token
     ARGV[6] delay value
     ARGV[7] skip attempt
@@ -63,26 +64,42 @@
 --[[
   Function to check for the meta.paused key to decide if we are paused or not
   (since an empty list and !EXISTS are not really the same).
 ]]
 local function isQueuePaused(queueMetaKey)
     return rcall("HEXISTS", queueMetaKey, "paused") == 1
 end
+local function removeLock(jobKey, stalledKey, token, jobId)
+  if token ~= "0" then
+    local lockKey = jobKey .. ':lock'
+    local lockToken = rcall("GET", lockKey)
+    if lockToken == token then
+      rcall("DEL", lockKey)
+      rcall("SREM", stalledKey, jobId)
+    else
+      if lockToken then
+        -- Lock exists but token does not match
+        return -6
+      else
+        -- Lock is missing completely
+        return -2
+      end
+    end
+  end
+  return 0
+end
 local jobKey = KEYS[5]
 local metaKey = KEYS[7]
+local token = ARGV[5] 
 if rcall("EXISTS", jobKey) == 1 then
-    local delayedKey = KEYS[4]
-    if ARGV[5] ~= "0" then
-        local lockKey = jobKey .. ':lock'
-        if rcall("GET", lockKey) == ARGV[5] then
-            rcall("DEL", lockKey)
-        else
-            return -2
-        end
+    local errorCode = removeLock(jobKey, KEYS[8], token, ARGV[4])
+    if errorCode < 0 then
+        return errorCode
     end
+    local delayedKey = KEYS[4]
     local jobId = ARGV[4]
     local score = tonumber(ARGV[3])
     local delayedTimestamp = (score / 0x1000)
     local numRemovedElements = rcall("LREM", KEYS[2], -1, jobId)
     if numRemovedElements < 1 then return -3 end
     if ARGV[7] == "0" then
         rcall("HINCRBY", jobKey, "atm", 1)
```

### Comparing `bullmq-2.3.3/bullmq/commands/moveToFinished-14.lua` & `bullmq-2.7.1/bullmq/commands/moveToFinished-14.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/obliterate-2.lua` & `bullmq-2.7.1/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/paginate-1.lua` & `bullmq-2.7.1/bullmq/commands/paginate-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/pause-7.lua` & `bullmq-2.7.1/bullmq/commands/pause-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/promote-8.lua` & `bullmq-2.7.1/bullmq/commands/promote-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/removeChildDependency-1.lua` & `bullmq-2.7.1/bullmq/commands/removeChildDependency-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/removeJob-1.lua` & `bullmq-2.7.1/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/removeRepeatable-2.lua` & `bullmq-2.7.1/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/reprocessJob-7.lua` & `bullmq-2.7.1/bullmq/commands/reprocessJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/commands/retryJob-10.lua` & `bullmq-2.7.1/bullmq/commands/retryJob-11.lua`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
       KEYS[4]  job key
       KEYS[5]  'meta'
       KEYS[6]  events stream
       KEYS[7]  delayed key
       KEYS[8]  prioritized key
       KEYS[9]  'pc' priority counter
       KEYS[10] 'marker'
+      KEYS[11] 'stalled'
       ARGV[1]  key prefix
       ARGV[2]  timestamp
       ARGV[3]  pushCmd
       ARGV[4]  jobId
       ARGV[5]  token
     Events:
       'waiting'
@@ -100,27 +101,42 @@
             -- Emit waiting event
             rcall("XADD", eventStreamKey, "*", "event", "waiting", "jobId",
                   jobId, "prev", "delayed")
             rcall("HSET", jobKey, "delay", 0)
         end
     end
 end
+local function removeLock(jobKey, stalledKey, token, jobId)
+  if token ~= "0" then
+    local lockKey = jobKey .. ':lock'
+    local lockToken = rcall("GET", lockKey)
+    if lockToken == token then
+      rcall("DEL", lockKey)
+      rcall("SREM", stalledKey, jobId)
+    else
+      if lockToken then
+        -- Lock exists but token does not match
+        return -6
+      else
+        -- Lock is missing completely
+        return -2
+      end
+    end
+  end
+  return 0
+end
 local target, paused = getTargetQueueList(KEYS[5], KEYS[2], KEYS[3])
 local markerKey = KEYS[10]
 -- Check if there are delayed jobs that we can move to wait.
 -- test example: when there are delayed jobs between retries
 promoteDelayedJobs(KEYS[7], markerKey, target, KEYS[8], KEYS[6], ARGV[1], ARGV[2], KEYS[9], paused)
 if rcall("EXISTS", KEYS[4]) == 1 then
-  if ARGV[5] ~= "0" then
-    local lockKey = KEYS[4] .. ':lock'
-    if rcall("GET", lockKey) == ARGV[5] then
-      rcall("DEL", lockKey)
-    else
-      return -2
-    end
+  local errorCode = removeLock(KEYS[4], KEYS[11], ARGV[5], ARGV[4]) 
+  if errorCode < 0 then
+    return errorCode
   end
   rcall("LREM", KEYS[1], 0, ARGV[4])
   local priority = tonumber(rcall("HGET", KEYS[4], "priority")) or 0
   -- Standard or priority add
   if priority == 0 then
     rcall(ARGV[3], target, ARGV[4])
     -- TODO: check if we need to add marker in this case too
```

### Comparing `bullmq-2.3.3/bullmq/commands/updateProgress-3.lua` & `bullmq-2.7.1/bullmq/commands/updateProgress-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/event_emitter.py` & `bullmq-2.7.1/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/flow_producer.py` & `bullmq-2.7.1/bullmq/flow_producer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/job.py` & `bullmq-2.7.1/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/queue.py` & `bullmq-2.7.1/bullmq/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,39 @@
 
     def getRateLimitTtl(self):
         """
         Returns the time to live for a rate limited key in milliseconds.
         """
         return self.client.pttl(self.keys["limiter"])
 
+    async def getJobLogs(self, job_id:str, start = 0, end = -1, asc = True):
+        """
+        Returns the logs for a given Job.
+
+        @param job_id: The id of the job to get the logs for.
+        @param start: Zero based index from where to start returning jobs.
+        @param end: Zero based index where to stop returning jobs.
+        @param asc: If true, the jobs will be returned in ascending order.
+        """
+
+        logs_key = self.toKey(job_id + ":logs")
+        pipe = self.redisConnection.conn.pipeline(transaction=True)
+        if asc:
+            pipe.lrange(logs_key, start, end)
+        else:
+            pipe.lrange(logs_key, -(end+1), -(start+1))
+        pipe.llen(logs_key)
+        result = await pipe.execute()
+        if not asc:
+            result[0].reverse()
+        return {
+            "logs": result[0],
+            "count": result[1]
+        }        
+   
     async def obliterate(self, force: bool = False):
         """
         Completely destroys the queue and all of its contents irreversibly.
         This method will the *pause* the queue and requires that there are no
         active jobs. It is possible to bypass this requirement, i.e. not
         having active jobs using the "force" option.
```

### Comparing `bullmq-2.3.3/bullmq/queue_keys.py` & `bullmq-2.7.1/bullmq/queue_keys.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/redis_connection.py` & `bullmq-2.7.1/bullmq/redis_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,26 @@
     RedisConnection class
     """
 
     minimum_version = '5.0.0'
     recommended_minimum_version = '6.2.0'
 
     capabilities = {
+        "canBlockFor1Ms": True,
         "canDoubleTimeout": False
     }
 
-    def __init__(self, redisOpts: dict | str = {}):
+    def __init__(self, redisOpts: dict | str | redis.Redis = {}):
         self.version = None
         retry = Retry(ExponentialBackoff(), 3)
         retry_errors = [BusyLoadingError, ConnectionError, TimeoutError]
 
-        if isinstance(redisOpts, dict):
+        if isinstance(redisOpts, redis.Redis):
+            self.conn = redisOpts
+        elif isinstance(redisOpts, dict):
             defaultOpts = {
                 "host": "localhost",
                 "port": 6379,
                 "db": 0,
                 "password": None,
                 "username": None,
             }
@@ -60,10 +63,11 @@
         doc = await self.conn.info()
         if doc.get("maxmemory_policy") != "noeviction":
             warnings.warn(f'IMPORTANT! Eviction policy is {doc.get("maxmemory_policy")}. It should be "noeviction"')
 
         self.version = doc.get("redis_version")
 
         self.capabilities = {
+            "canBlockFor1Ms": not isRedisVersionLowerThan(self.version, '7.0.8'),
             "canDoubleTimeout": not isRedisVersionLowerThan(self.version, '6.0.0')
         }
         return self.version
```

### Comparing `bullmq-2.3.3/bullmq/scripts.py` & `bullmq-2.7.1/bullmq/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
             "getCounts": self.redisClient.register_script(self.getScript("getCounts-1.lua")), #
             "getRanges": self.redisClient.register_script(self.getScript("getRanges-1.lua")), #
             "getState": self.redisClient.register_script(self.getScript("getState-8.lua")),
             "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-8.lua")),
             "isJobInList": self.redisClient.register_script(self.getScript("isJobInList-1.lua")),
             "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-9.lua")),
             "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-11.lua")),
-            "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-7.lua")),
+            "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-14.lua")),
-            "moveToWaitingChildren": self.redisClient.register_script(self.getScript("moveToWaitingChildren-4.lua")),
+            "moveToWaitingChildren": self.redisClient.register_script(self.getScript("moveToWaitingChildren-5.lua")),
             "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
             "pause": self.redisClient.register_script(self.getScript("pause-7.lua")),
             "promote": self.redisClient.register_script(self.getScript("promote-8.lua")),
             "removeJob": self.redisClient.register_script(self.getScript("removeJob-1.lua")),
             "reprocessJob": self.redisClient.register_script(self.getScript("reprocessJob-7.lua")),
-            "retryJob": self.redisClient.register_script(self.getScript("retryJob-10.lua")),
+            "retryJob": self.redisClient.register_script(self.getScript("retryJob-11.lua")),
             "moveJobsToWait": self.redisClient.register_script(self.getScript("moveJobsToWait-7.lua")),
             "saveStacktrace": self.redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
             "updateData": self.redisClient.register_script(self.getScript("updateData-1.lua")),
             "updateProgress": self.redisClient.register_script(self.getScript("updateProgress-3.lua")),
         }
 
         self.queue_keys = QueueKeys(prefix)
@@ -167,15 +167,16 @@
         keys, args = self.cleanJobsInSetArgs(set, grace, limit)
         return self.commands["cleanJobsInSet"](keys=keys, args=args)
 
     def moveToWaitingChildrenArgs(self, job_id, token, opts: dict = {}):
         keys = [self.toKey(job_id) + ":lock",
                 self.keys['active'],
                 self.keys['waiting-children'],
-                self.toKey(job_id)]
+                self.toKey(job_id),
+                self.keys['stalled']]
         child_key = opts.get("child") if opts else None
         args = [token, get_parent_key(child_key) or "", round(time.time() * 1000), job_id,
                 "1" if opts.get("skipAttempt") else "0"]
 
         return (keys, args)
 
     async def moveToWaitingChildren(self, job_id, token, opts):
@@ -247,14 +248,15 @@
         keys.append(self.toKey(job_id))
         keys.append(self.keys['meta'])
         keys.append(self.keys['events'])
         keys.append(self.keys['delayed'])
         keys.append(self.keys['prioritized'])
         keys.append(self.keys['pc'])
         keys.append(self.keys['marker'])
+        keys.append(self.keys['stalled'])
 
         push_cmd = "RPUSH" if lifo else "LPUSH"
 
         args = [self.keys[''], round(time.time() * 1000), push_cmd,
             job_id, token, "1" if opts.get("skipAttempt") else "0"]
 
         return (keys, args)
@@ -265,14 +267,15 @@
         if timestamp > 0:
             max_timestamp = max_timestamp * 0x1000 + (convert_to_int(job_id) & 0xfff)
 
         keys = self.getKeys(['marker', 'active', 'prioritized', 'delayed'])
         keys.append(self.toKey(job_id))
         keys.append(self.keys['events'])
         keys.append(self.keys['meta'])
+        keys.append(self.keys['stalled'])
 
         args = [self.keys[''], round(time.time() * 1000), str(max_timestamp),
             job_id, token, delay, "1" if opts.get("skipAttempt") else "0" ]
 
         return (keys, args)
 
     async def moveToDelayed(self, job_id: str, timestamp: int, delay: int, token: str = "0"):
```

### Comparing `bullmq-2.3.3/bullmq/timer.py` & `bullmq-2.7.1/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/types/job_options.py` & `bullmq-2.7.1/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/types/worker_options.py` & `bullmq-2.7.1/bullmq/types/worker_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from typing import TypedDict, Any
+import redis.asyncio as redis
 
 
 class WorkerOptions(TypedDict, total=False):
     autorun: bool
     """
     Condition to start processor at instance creation
 
@@ -46,11 +47,11 @@
     """
 
     prefix: str
     """
     Prefix for all queue keys.
     """
 
-    connection: dict[str, Any]
+    connection: dict[str, Any] | redis.Redis
     """
     Options for connecting to a Redis instance.
     """
```

### Comparing `bullmq-2.3.3/bullmq/utils.py` & `bullmq-2.7.1/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.3.3/bullmq/worker.py` & `bullmq-2.7.1/bullmq/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 class Worker(EventEmitter):
     def __init__(self, name: str, processor: Callable[[Job, str], asyncio.Future], opts: WorkerOptions = {}):
         super().__init__()
         self.name = name
         self.processor = processor
         final_opts = {
+            "drainDelay": 5,
             "concurrency": 1,
             "lockDuration": 30000,
             "maxStalledCount": 1,
             "stalledInterval": 30000,
         }
         final_opts.update(opts or {})
         self.opts = final_opts
@@ -149,35 +150,44 @@
             job_instance = Job.fromJSON(self, job_data, job_id)
             job_instance.token = token
             return job_instance
 
     async def waitForJob(self):
         block_timeout = self.getBlockTimeout(self.blockUntil)
         block_timeout = block_timeout if self.blockingRedisConnection.capabilities.get("canDoubleTimeout", False) else math.ceil(block_timeout)
-        block_timeout = min(block_timeout, maximum_block_timeout)
 
         result = await self.bclient.bzpopmin(self.scripts.keys["marker"], block_timeout)
         if result:
             [_key, member, score] = result
 
             if member:
                 return int(score)
             else:
                 return 0
         return 0
 
     def getBlockTimeout(self, block_until: int):
         if block_until:
+            block_timeout = None
             block_delay = block_until - int(time.time() * 1000)
-            if block_delay < 1:
-                return minimum_block_timeout
+            if block_delay < self.minimumBlockTimeout * 1000:
+                block_timeout = minimum_block_timeout
             else:
-                return block_delay / 1000
+                block_timeout = block_delay / 1000
+            # We restrict the maximum block timeout to 10 second to avoid
+            # blocking the connection for too long in the case of reconnections
+            # reference: https://github.com/taskforcesh/bullmq/issues/1658
+            return min(block_timeout, maximum_block_timeout)
         else:
-            return max(self.opts.get("drainDelay", 5), minimum_block_timeout)
+            return max(self.opts.get("drainDelay", 5), self.minimumBlockTimeout)
+
+    @property
+    def minimumBlockTimeout(self):
+        return minimum_block_timeout if self.blockingRedisConnection.capabilities.get("canBlockFor1Ms", True) else 0.002
+        
 
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
                 # Currently we do not support pre-fetching jobs as in NodeJS version.
```

### Comparing `bullmq-2.3.3/bullmq.egg-info/PKG-INFO` & `bullmq-2.7.1/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.3.3
+Version: 2.7.1
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.3.3/bullmq.egg-info/SOURCES.txt` & `bullmq-2.7.1/bullmq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 bullmq/commands/getStateV2-8.lua
 bullmq/commands/isFinished-3.lua
 bullmq/commands/isJobInList-1.lua
 bullmq/commands/moveJobFromActiveToWait-10.lua
 bullmq/commands/moveJobsToWait-7.lua
 bullmq/commands/moveStalledJobsToWait-9.lua
 bullmq/commands/moveToActive-11.lua
-bullmq/commands/moveToDelayed-7.lua
+bullmq/commands/moveToDelayed-8.lua
 bullmq/commands/moveToFinished-14.lua
-bullmq/commands/moveToWaitingChildren-4.lua
+bullmq/commands/moveToWaitingChildren-5.lua
 bullmq/commands/obliterate-2.lua
 bullmq/commands/paginate-1.lua
 bullmq/commands/pause-7.lua
 bullmq/commands/promote-8.lua
 bullmq/commands/releaseLock-1.lua
 bullmq/commands/removeChildDependency-1.lua
 bullmq/commands/removeJob-1.lua
 bullmq/commands/removeRepeatable-2.lua
 bullmq/commands/reprocessJob-7.lua
-bullmq/commands/retryJob-10.lua
+bullmq/commands/retryJob-11.lua
 bullmq/commands/saveStacktrace-1.lua
 bullmq/commands/updateData-1.lua
 bullmq/commands/updateProgress-3.lua
 bullmq/custom_errors/__init__.py
 bullmq/custom_errors/waiting_children_error.py
 bullmq/types/__init__.py
 bullmq/types/backoff_options.py
```

### Comparing `bullmq-2.3.3/pyproject.toml` & `bullmq-2.7.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "2.3.3"
+version = "2.7.1"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
```

