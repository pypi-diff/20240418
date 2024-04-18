# Comparing `tmp/cronitor-4.7.0.tar.gz` & `tmp/cronitor-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cronitor-4.7.0.tar", last modified: Thu Sep  7 17:53:39 2023, max compression
+gzip compressed data, was "cronitor-4.7.1.tar", last modified: Thu Apr 18 15:51:44 2024, max compression
```

## Comparing `cronitor-4.7.0.tar` & `cronitor-4.7.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 augustflanagan   (501) staff       (20)        0 2023-09-07 17:53:39.004157 cronitor-4.7.0/
--rw-r--r--   0 augustflanagan   (501) staff       (20)    13051 2023-09-07 17:53:39.004415 cronitor-4.7.0/PKG-INFO
--rw-r--r--   0 augustflanagan   (501) staff       (20)    10413 2023-09-07 17:51:55.000000 cronitor-4.7.0/README.md
-drwxr-xr-x   0 augustflanagan   (501) staff       (20)        0 2023-09-07 17:53:38.998773 cronitor-4.7.0/cronitor/
--rw-r--r--   0 augustflanagan   (501) staff       (20)     3569 2023-09-07 17:51:55.000000 cronitor-4.7.0/cronitor/__init__.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     2429 2021-09-21 23:04:53.000000 cronitor-4.7.0/cronitor/__main__.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     8600 2022-03-22 21:53:04.000000 cronitor-4.7.0/cronitor/celery.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     7450 2023-09-07 17:51:55.000000 cronitor-4.7.0/cronitor/monitor.py
-drwxr-xr-x   0 augustflanagan   (501) staff       (20)        0 2023-09-07 17:53:39.003441 cronitor-4.7.0/cronitor/tests/
--rw-r--r--   0 augustflanagan   (501) staff       (20)        0 2021-09-21 22:53:25.000000 cronitor-4.7.0/cronitor/tests/__init__.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     1144 2023-09-07 17:51:55.000000 cronitor-4.7.0/cronitor/tests/test_config.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     3037 2021-09-21 23:04:53.000000 cronitor-4.7.0/cronitor/tests/test_monitor.py
--rw-r--r--   0 augustflanagan   (501) staff       (20)     3192 2022-08-23 23:51:17.000000 cronitor-4.7.0/cronitor/tests/test_pings.py
-drwxr-xr-x   0 augustflanagan   (501) staff       (20)        0 2023-09-07 17:53:39.001067 cronitor-4.7.0/cronitor.egg-info/
--rw-r--r--   0 augustflanagan   (501) staff       (20)    13051 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/PKG-INFO
--rw-r--r--   0 augustflanagan   (501) staff       (20)      420 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/SOURCES.txt
--rw-r--r--   0 augustflanagan   (501) staff       (20)        1 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/dependency_links.txt
--rw-r--r--   0 augustflanagan   (501) staff       (20)       53 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/entry_points.txt
--rw-r--r--   0 augustflanagan   (501) staff       (20)       33 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/requires.txt
--rw-r--r--   0 augustflanagan   (501) staff       (20)        9 2023-09-07 17:53:38.000000 cronitor-4.7.0/cronitor.egg-info/top_level.txt
--rw-r--r--   0 augustflanagan   (501) staff       (20)      101 2023-09-07 17:53:39.004943 cronitor-4.7.0/setup.cfg
--rw-r--r--   0 augustflanagan   (501) staff       (20)      704 2023-09-07 17:52:12.000000 cronitor-4.7.0/setup.py
+drwxr-xr-x   0 au6ust     (501) staff       (20)        0 2024-04-18 15:51:44.383511 cronitor-4.7.1/
+-rw-r--r--   0 au6ust     (501) staff       (20)     1036 2024-04-18 15:47:42.000000 cronitor-4.7.1/LICENSE
+-rw-r--r--   0 au6ust     (501) staff       (20)    10699 2024-04-18 15:51:44.383568 cronitor-4.7.1/PKG-INFO
+-rw-r--r--   0 au6ust     (501) staff       (20)    10378 2024-04-18 15:47:42.000000 cronitor-4.7.1/README.md
+drwxr-xr-x   0 au6ust     (501) staff       (20)        0 2024-04-18 15:51:44.382223 cronitor-4.7.1/cronitor/
+-rw-r--r--   0 au6ust     (501) staff       (20)     3569 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/__init__.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     2429 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/__main__.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     8600 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/celery.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     7450 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/monitor.py
+drwxr-xr-x   0 au6ust     (501) staff       (20)        0 2024-04-18 15:51:44.383397 cronitor-4.7.1/cronitor/tests/
+-rw-r--r--   0 au6ust     (501) staff       (20)        0 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/tests/__init__.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     1144 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/tests/test_config.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     3037 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/tests/test_monitor.py
+-rw-r--r--   0 au6ust     (501) staff       (20)     3192 2024-04-18 15:47:42.000000 cronitor-4.7.1/cronitor/tests/test_pings.py
+drwxr-xr-x   0 au6ust     (501) staff       (20)        0 2024-04-18 15:51:44.382927 cronitor-4.7.1/cronitor.egg-info/
+-rw-r--r--   0 au6ust     (501) staff       (20)    10699 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/PKG-INFO
+-rw-r--r--   0 au6ust     (501) staff       (20)      428 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/SOURCES.txt
+-rw-r--r--   0 au6ust     (501) staff       (20)        1 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/dependency_links.txt
+-rw-r--r--   0 au6ust     (501) staff       (20)       53 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/entry_points.txt
+-rw-r--r--   0 au6ust     (501) staff       (20)       33 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/requires.txt
+-rw-r--r--   0 au6ust     (501) staff       (20)        9 2024-04-18 15:51:44.000000 cronitor-4.7.1/cronitor.egg-info/top_level.txt
+-rw-r--r--   0 au6ust     (501) staff       (20)      101 2024-04-18 15:51:44.383935 cronitor-4.7.1/setup.cfg
+-rw-r--r--   0 au6ust     (501) staff       (20)      704 2024-04-18 15:48:55.000000 cronitor-4.7.1/setup.py
```

### Comparing `cronitor-4.7.0/PKG-INFO` & `cronitor-4.7.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,302 +1,290 @@
-Metadata-Version: 2.1
-Name: cronitor
-Version: 4.7.0
-Summary: A lightweight Python client for Cronitor.
-Home-page: https://github.com/cronitorio/cronitor-python
-Author: August Flanagan
-Author-email: august@cronitor.io
-License: MIT License
-Description: # Cronitor Python Library
-        ![Test](https://github.com/cronitorio/cronitor-python/workflows/Test/badge.svg)
-        
-        [Cronitor](https://cronitor.io/) provides end-to-end monitoring for background jobs, websites, APIs, and anything else that can send or receive an HTTP request. This library provides convenient access to the Cronitor API from applications written in Python. See our [API docs](https://cronitor.io/docs/api) for detailed references on configuring monitors and sending telemetry pings.
-        
-        In this guide:
-        
-        - [Installation](#Installation)
-        - [Monitoring Background Jobs](#monitoring-background-jobs)
-        - [Sending Telemetry Events](#sending-telemetry-events)
-        - [Configuring Monitors](#configuring-monitors)
-        - [Package Configuration & Env Vars](#package-configuration)
-        - [Command Line Usage](#command-line-usage)
-        
-        ## Installation
-        
-        ```
-        pip install cronitor
-        ```
-        
-        ## Monitoring Background Jobs
-        
-        #### Celery Auto-Discover
-        `cronitor-python` can automatically discover all of your declared Celery tasks, including your Celerybeat scheduled tasks,
-        creating monitors for them and sending pings when tasks run, succeed, or fail. Your API keys can be found [here](https://cronitor.io/settings/api).
-        
-        Requires Celery 4.0 or higher. Celery auto-discover utilizes the Celery [message protocol version 2](https://docs.celeryproject.org/en/stable/internals/protocol.html#version-2).
-        
-        <details>
-        <summary>Some important notes on support</summary>
-        
-        * Tasks on [solar schedules](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#solar-schedules) are not supported and will be ignored.
-        * [`django-celery-beat`](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#using-custom-scheduler-classes) is not yet supported, but is in the works.
-        * If you use the default `PersistentScheduler`, the celerybeat integration overrides the celerybeat local task run database (as referenced [here](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler) in the docs), named `celerybeat-schedule` by default. If you currently specify a custom location for this database, this integration will override it. **Very** few people require setting custom locations for this database. If you fall into this group and want to use `cronitor-python`'s celerybeat integration, please reach out to Cronitor support.
-        </details>
-        
-        ```python
-        import cronitor.celery
-        from celery import Celery
-        
-        app = Celery()
-        app.conf.beat_schedule = {
-            'run-me-every-minute': {
-                'task': 'tasks.every_minute_celery_task',
-                'schedule': 60
-            }
-        }
-        
-        # Discover all of your celery tasks and automatically add monitoring.
-        cronitor.celery.initialize(app, api_key="apiKey123")
-        
-        @app.task
-        def every_minute_celery_task():
-            print("running a background job with celery...")
-        
-        @app.task
-        def non_scheduled_celery_task():
-            print("Even though I'm not on a schedule, I'll still be monitored!")
-        ```
-        
-        If you want only to monitor Celerybeat periodic tasks, and not tasks triggered any other way, you can set `celereybeat_only=True` when initializing:
-        ```python
-        app = Celery()
-        cronitor.celery.initialize(app, api_key="apiKey123", celerybeat_only=True)
-        ```
-        
-        #### Manual Integration
-        
-        The `@cronitor.job` is a lightweight way to monitor any background task regardless of how it is executed. It will send telemetry events before calling your function and after it exits. If your function raises an exception a `fail` event will be sent (and the exception re-raised).
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        # Apply the cronitor decorator to monitor any function.
-        # If no monitor matches the provided key, one will be created automatically.
-        @cronitor.job('send-invoices')
-        def send_invoices_task(*args, **kwargs):
-            ...
-        ```
-        
-        ## Sending Telemetry Events
-        
-        If you want to send a heartbeat events, or want finer control over when/how [telemetry events](https://cronitor.io/docs/telemetry-api) are sent for your jobs, you can create a monitor instance and call the `.ping` method.
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        # optionally, set an environment
-        cronitor.environment = 'staging'
-        
-        monitor = cronitor.Monitor('heartbeat-monitor')
-        monitor.ping() # send a heartbeat event
-        
-        # optional params can be passed as keyword arguements.
-        # for a complete list see https://cronitor.io/docs/telemetry-api#parameters
-        monitor.ping(
-            state='run|complete|fail|ok', # run|complete|fail used to measure lifecycle of a job, ok used for manual reset only.
-            message='', # message that will be displayed in alerts as well as monitor activity panel on your dashboard.
-            metrics={
-                'duration': 100, # how long the job ran (complete|fail only). cronitor will calculate this when not provided
-                'count': 4500, # if your job is processing a number of items you can report a count
-                'error_count': 10 # the number of errors that occurred while this job was running
-            }
-        )
-        ```
-        
-        ## Configuring Monitors
-        
-        You can configure all of your monitors using a single YAML file. This can be version controlled and synced to Cronitor as part of
-        a deployment or build process. For details on all of the attributes that can be set, see the [Monitor API](https://cronitor.io/docs/monitor-api) documentation.
-        
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        cronitor.read_config('./cronitor.yaml') # parse the yaml file of monitors
-        
-        cronitor.validate_config() # send monitors to Cronitor for configuration validation
-        
-        cronitor.apply_config() # sync the monitors from the config file to Cronitor
-        
-        cronitor.generate_config() # generate a new config file from the Cronitor API
-        ```
-        
-        The timeout value for validate_config, apply_config and generate_config is 10 seconds by default. The value can be rewritten by setting the environment variable `CRONITOR_TIMEOUT`. It can also be rewritten by assigning a value to cronitor.timeout.
-        
-        ```python
-        import cronitor
-        
-        cronitor.timeout = 30
-        cronitor.apply_config()
-        ```
-        
-        The `cronitor.yaml` file includes three top level keys `jobs`, `checks`, `heartbeats`. You can configure monitors under each key by defining [monitors](https://cronitor.io/docs/monitor-api#attributes).
-        
-        ```yaml
-        jobs:
-            nightly-database-backup:
-                schedule: 0 0 * * *
-                notify:
-                    - devops-alert-pagerduty
-                assertions:
-                    - metric.duration < 5 minutes
-        
-            send-welcome-email:
-                schedule: every 10 minutes
-                assertions:
-                    - metric.count > 0
-                    - metric.duration < 30 seconds
-        
-        checks:
-            cronitor-homepage:
-                request:
-                    url: https://cronitor.io
-                    regions:
-                        - us-east-1
-                        - eu-central-1
-                        - ap-northeast-1
-                assertions:
-                    - response.code = 200
-                    - response.time < 2s
-        
-            cronitor-ping-api:
-                request:
-                    url: https://cronitor.link/ping
-                assertions:
-                    - response.body contains ok
-                    - response.time < .25s
-        
-        heartbeats:
-            production-deploy:
-                notify:
-                    alerts: ['deploys-slack']
-                    events: true # send alert when the event occurs
-        
-        ```
-        
-        You can also create and update monitors by calling `Monitor.put`. For details on all of the attributes that can be set see the Monitor API [documentation)(https://cronitor.io/docs/monitor-api#attributes).
-        
-        ```python
-        import cronitor
-        
-        monitors = cronitor.Monitor.put([
-          {
-            'type': 'job',
-            'key': 'send-customer-invoices',
-            'schedule': '0 0 * * *',
-            'assertions': [
-                'metric.duration < 5 min'
-            ],
-            'notify': ['devops-alerts-slack']
-          },
-          {
-            'type': 'check',
-            'key': 'Cronitor Homepage',
-            'schedule': 'every 45 seconds',
-            'request': {
-                'url': 'https://cronitor.io'
-            },
-            'assertions': [
-                'response.code = 200',
-                'response.time < 600ms',
-            ]
-          }
-        ])
-        ```
-        
-        ### Pausing, Reseting, and Deleting
-        
-        ```python
-        import cronitor
-        
-        monitor = cronitor.Monitor('heartbeat-monitor');
-        
-        monitor.pause(24) # pause alerting for 24 hours
-        monitor.unpause() # alias for .pause(0)
-        monitor.ok() # manually reset to a passing state alias for monitor.ping({state: ok})
-        monitor.delete() # destroy the monitor
-        ```
-        
-        ## Package Configuration
-        
-        The package needs to be configured with your account's `API key`, which is available on the [account settings](https://cronitor.io/settings) page. You can also optionally specify an `api_version` and an `environment`. If not provided, your account default is used. These can also be supplied using the environment variables `CRONITOR_API_KEY`, `CRONITOR_API_VERSION`, `CRONITOR_ENVIRONMENT`.
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings
-        cronitor.api_key = 'apiKey123'
-        cronitor.api_version = '2020-10-01'
-        cronitor.environment = 'cluster_1_prod'
-        ```
-        
-        ## Command Line Usage
-        
-        ```bash
-        >> python -m cronitor -h
-        
-        usage: cronitor [-h] [--apikey APIKEY] [--key KEY] [--msg MSG]
-                        (--run | --complete | --fail | --ok | --pause PAUSE)
-        
-        Send status messages to Cronitor ping API.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --authkey AUTHKEY, -a AUTHKEY
-                                Auth Key from Account page
-          --key KEY, -k KEY     Unique key for the monitor to take ping
-          --msg MSG, -m MSG     Optional message to send with ping/fail
-          --tick, -t            Call ping on given monitor
-          --run, -r             Call ping with state=run on given monitor
-          --complete, -C        Call ping with state=complete on given monitor
-          --fail, -f            Call ping with state=fail on given monitor
-          --pause PAUSE, -P PAUSE
-                                Call pause on given monitor
-        ```
-        
-        
-        ## Contributing
-        
-        Pull requests and features are happily considered! By participating in this project you agree to abide by the [Code of Conduct](http://contributor-covenant.org/version/2/0).
-        
-        ### To contribute
-        
-        Fork, then clone the repo:
-        
-            git clone git@github.com:your-username/cronitor-python.git
-        
-        Set up your machine:
-        
-            pip install -r requirements
-        
-        Make sure the tests pass:
-        
-            pytest
-        
-        Make your change. Add tests for your change. Make the tests pass:
-        
-            pytest
-        
-        
-        Push to your fork and [submit a pull request]( https://github.com/cronitorio/cronitor-python/compare/)
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Cronitor Python Library
+![Test](https://github.com/cronitorio/cronitor-python/workflows/Test/badge.svg)
+
+[Cronitor](https://cronitor.io/) provides end-to-end monitoring for background jobs, websites, APIs, and anything else that can send or receive an HTTP request. This library provides convenient access to the Cronitor API from applications written in Python. See our [API docs](https://cronitor.io/docs/api) for detailed references on configuring monitors and sending telemetry pings.
+
+In this guide:
+
+- [Installation](#Installation)
+- [Monitoring Background Jobs](#monitoring-background-jobs)
+- [Sending Telemetry Events](#sending-telemetry-events)
+- [Configuring Monitors](#configuring-monitors)
+- [Package Configuration & Env Vars](#package-configuration)
+- [Command Line Usage](#command-line-usage)
+
+## Installation
+
+```
+pip install cronitor
+```
+
+## Monitoring Background Jobs
+
+#### Celery Auto-Discover
+`cronitor-python` can automatically discover all of your declared Celery tasks, including your Celerybeat scheduled tasks,
+creating monitors for them and sending pings when tasks run, succeed, or fail. Your API keys can be found [here](https://cronitor.io/settings/api).
+
+Requires Celery 4.0 or higher. Celery auto-discover utilizes the Celery [message protocol version 2](https://docs.celeryproject.org/en/stable/internals/protocol.html#version-2).
+
+**Some important notes on support**
+
+* Tasks on [solar schedules](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#solar-schedules) are not supported and will be ignored.
+* [`django-celery-beat`](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#using-custom-scheduler-classes) is not yet supported, but is in the works.
+* If you use the default `PersistentScheduler`, the celerybeat integration overrides the celerybeat local task run database (as referenced [here](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler) in the docs), named `celerybeat-schedule` by default. If you currently specify a custom location for this database, this integration will override it. **Very** few people require setting custom locations for this database. If you fall into this group and want to use `cronitor-python`'s celerybeat integration, please reach out to Cronitor support.
+
+
+```python
+import cronitor.celery
+from celery import Celery
+
+app = Celery()
+app.conf.beat_schedule = {
+    'run-me-every-minute': {
+        'task': 'tasks.every_minute_celery_task',
+        'schedule': 60
+    }
+}
+
+# Discover all of your celery tasks and automatically add monitoring.
+cronitor.celery.initialize(app, api_key="apiKey123")
+
+@app.task
+def every_minute_celery_task():
+    print("running a background job with celery...")
+
+@app.task
+def non_scheduled_celery_task():
+    print("Even though I'm not on a schedule, I'll still be monitored!")
+```
+
+If you want only to monitor Celerybeat periodic tasks, and not tasks triggered any other way, you can set `celereybeat_only=True` when initializing:
+```python
+app = Celery()
+cronitor.celery.initialize(app, api_key="apiKey123", celerybeat_only=True)
+```
+
+#### Manual Integration
+
+The `@cronitor.job` is a lightweight way to monitor any background task regardless of how it is executed. It will send telemetry events before calling your function and after it exits. If your function raises an exception a `fail` event will be sent (and the exception re-raised).
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+# Apply the cronitor decorator to monitor any function.
+# If no monitor matches the provided key, one will be created automatically.
+@cronitor.job('send-invoices')
+def send_invoices_task(*args, **kwargs):
+    ...
+```
+
+## Sending Telemetry Events
+
+If you want to send a heartbeat events, or want finer control over when/how [telemetry events](https://cronitor.io/docs/telemetry-api) are sent for your jobs, you can create a monitor instance and call the `.ping` method.
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+# optionally, set an environment
+cronitor.environment = 'staging'
+
+monitor = cronitor.Monitor('heartbeat-monitor')
+monitor.ping() # send a heartbeat event
+
+# optional params can be passed as keyword arguements.
+# for a complete list see https://cronitor.io/docs/telemetry-api#parameters
+monitor.ping(
+    state='run|complete|fail|ok', # run|complete|fail used to measure lifecycle of a job, ok used for manual reset only.
+    message='', # message that will be displayed in alerts as well as monitor activity panel on your dashboard.
+    metrics={
+        'duration': 100, # how long the job ran (complete|fail only). cronitor will calculate this when not provided
+        'count': 4500, # if your job is processing a number of items you can report a count
+        'error_count': 10 # the number of errors that occurred while this job was running
+    }
+)
+```
+
+## Configuring Monitors
+
+You can configure all of your monitors using a single YAML file. This can be version controlled and synced to Cronitor as part of
+a deployment or build process. For details on all of the attributes that can be set, see the [Monitor API](https://cronitor.io/docs/monitor-api) documentation.
+
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+cronitor.read_config('./cronitor.yaml') # parse the yaml file of monitors
+
+cronitor.validate_config() # send monitors to Cronitor for configuration validation
+
+cronitor.apply_config() # sync the monitors from the config file to Cronitor
+
+cronitor.generate_config() # generate a new config file from the Cronitor API
+```
+
+The timeout value for validate_config, apply_config and generate_config is 10 seconds by default. The value can be rewritten by setting the environment variable `CRONITOR_TIMEOUT`. It can also be rewritten by assigning a value to cronitor.timeout.
+
+```python
+import cronitor
+
+cronitor.timeout = 30
+cronitor.apply_config()
+```
+
+The `cronitor.yaml` file includes three top level keys `jobs`, `checks`, `heartbeats`. You can configure monitors under each key by defining [monitors](https://cronitor.io/docs/monitor-api#attributes).
+
+```yaml
+jobs:
+    nightly-database-backup:
+        schedule: 0 0 * * *
+        notify:
+            - devops-alert-pagerduty
+        assertions:
+            - metric.duration < 5 minutes
+
+    send-welcome-email:
+        schedule: every 10 minutes
+        assertions:
+            - metric.count > 0
+            - metric.duration < 30 seconds
+
+checks:
+    cronitor-homepage:
+        request:
+            url: https://cronitor.io
+            regions:
+                - us-east-1
+                - eu-central-1
+                - ap-northeast-1
+        assertions:
+            - response.code = 200
+            - response.time < 2s
+
+    cronitor-ping-api:
+        request:
+            url: https://cronitor.link/ping
+        assertions:
+            - response.body contains ok
+            - response.time < .25s
+
+heartbeats:
+    production-deploy:
+        notify:
+            alerts: ['deploys-slack']
+            events: true # send alert when the event occurs
+
+```
+
+You can also create and update monitors by calling `Monitor.put`. For details on all of the attributes that can be set see the Monitor API [documentation)(https://cronitor.io/docs/monitor-api#attributes).
+
+```python
+import cronitor
+
+monitors = cronitor.Monitor.put([
+  {
+    'type': 'job',
+    'key': 'send-customer-invoices',
+    'schedule': '0 0 * * *',
+    'assertions': [
+        'metric.duration < 5 min'
+    ],
+    'notify': ['devops-alerts-slack']
+  },
+  {
+    'type': 'check',
+    'key': 'Cronitor Homepage',
+    'schedule': 'every 45 seconds',
+    'request': {
+        'url': 'https://cronitor.io'
+    },
+    'assertions': [
+        'response.code = 200',
+        'response.time < 600ms',
+    ]
+  }
+])
+```
+
+### Pausing, Reseting, and Deleting
+
+```python
+import cronitor
+
+monitor = cronitor.Monitor('heartbeat-monitor');
+
+monitor.pause(24) # pause alerting for 24 hours
+monitor.unpause() # alias for .pause(0)
+monitor.ok() # manually reset to a passing state alias for monitor.ping({state: ok})
+monitor.delete() # destroy the monitor
+```
+
+## Package Configuration
+
+The package needs to be configured with your account's `API key`, which is available on the [account settings](https://cronitor.io/settings) page. You can also optionally specify an `api_version` and an `environment`. If not provided, your account default is used. These can also be supplied using the environment variables `CRONITOR_API_KEY`, `CRONITOR_API_VERSION`, `CRONITOR_ENVIRONMENT`.
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings
+cronitor.api_key = 'apiKey123'
+cronitor.api_version = '2020-10-01'
+cronitor.environment = 'cluster_1_prod'
+```
+
+## Command Line Usage
+
+```bash
+>> python -m cronitor -h
+
+usage: cronitor [-h] [--apikey APIKEY] [--key KEY] [--msg MSG]
+                (--run | --complete | --fail | --ok | --pause PAUSE)
+
+Send status messages to Cronitor ping API.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --authkey AUTHKEY, -a AUTHKEY
+                        Auth Key from Account page
+  --key KEY, -k KEY     Unique key for the monitor to take ping
+  --msg MSG, -m MSG     Optional message to send with ping/fail
+  --tick, -t            Call ping on given monitor
+  --run, -r             Call ping with state=run on given monitor
+  --complete, -C        Call ping with state=complete on given monitor
+  --fail, -f            Call ping with state=fail on given monitor
+  --pause PAUSE, -P PAUSE
+                        Call pause on given monitor
+```
+
+
+## Contributing
+
+Pull requests and features are happily considered! By participating in this project you agree to abide by the [Code of Conduct](http://contributor-covenant.org/version/2/0).
+
+### To contribute
+
+Fork, then clone the repo:
+
+    git clone git@github.com:your-username/cronitor-python.git
+
+Set up your machine:
+
+    pip install -r requirements
+
+Make sure the tests pass:
+
+    pytest
+
+Make your change. Add tests for your change. Make the tests pass:
+
+    pytest
+
+
+Push to your fork and [submit a pull request]( https://github.com/cronitorio/cronitor-python/compare/)
```

### Comparing `cronitor-4.7.0/README.md` & `cronitor-4.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cronitor
+Version: 4.7.1
+Summary: A lightweight Python client for Cronitor.
+Home-page: https://github.com/cronitorio/cronitor-python
+Author: August Flanagan
+Author-email: august@cronitor.io
+License: MIT License
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cronitor Python Library
 ![Test](https://github.com/cronitorio/cronitor-python/workflows/Test/badge.svg)
 
 [Cronitor](https://cronitor.io/) provides end-to-end monitoring for background jobs, websites, APIs, and anything else that can send or receive an HTTP request. This library provides convenient access to the Cronitor API from applications written in Python. See our [API docs](https://cronitor.io/docs/api) for detailed references on configuring monitors and sending telemetry pings.
 
 In this guide:
 
@@ -22,21 +34,20 @@
 
 #### Celery Auto-Discover
 `cronitor-python` can automatically discover all of your declared Celery tasks, including your Celerybeat scheduled tasks,
 creating monitors for them and sending pings when tasks run, succeed, or fail. Your API keys can be found [here](https://cronitor.io/settings/api).
 
 Requires Celery 4.0 or higher. Celery auto-discover utilizes the Celery [message protocol version 2](https://docs.celeryproject.org/en/stable/internals/protocol.html#version-2).
 
-<details>
-<summary>Some important notes on support</summary>
+**Some important notes on support**
 
 * Tasks on [solar schedules](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#solar-schedules) are not supported and will be ignored.
 * [`django-celery-beat`](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#using-custom-scheduler-classes) is not yet supported, but is in the works.
 * If you use the default `PersistentScheduler`, the celerybeat integration overrides the celerybeat local task run database (as referenced [here](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler) in the docs), named `celerybeat-schedule` by default. If you currently specify a custom location for this database, this integration will override it. **Very** few people require setting custom locations for this database. If you fall into this group and want to use `cronitor-python`'s celerybeat integration, please reach out to Cronitor support.
-</details>
+
 
 ```python
 import cronitor.celery
 from celery import Celery
 
 app = Celery()
 app.conf.beat_schedule = {
@@ -285,7 +296,9 @@
 
 Make your change. Add tests for your change. Make the tests pass:
 
     pytest
 
 
 Push to your fork and [submit a pull request]( https://github.com/cronitorio/cronitor-python/compare/)
+
+
```

### Comparing `cronitor-4.7.0/cronitor/__init__.py` & `cronitor-4.7.1/cronitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor/__main__.py` & `cronitor-4.7.1/cronitor/__main__.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor/celery.py` & `cronitor-4.7.1/cronitor/celery.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor/monitor.py` & `cronitor-4.7.1/cronitor/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         if not self.api_key:
             logger.error('No API key detected. Set cronitor.api_key or initialize Monitor with kwarg api_key.')
             return
 
         return self._req.get(url=self._ping_api_url(), params=self._clean_params(params), timeout=5, headers=self._headers)
 
     def ok(self):
-        self.ping(state=cronitor.Event.ok)
+        self.ping(state=cronitor.State.OK)
 
     def pause(self, hours):
         if not self.api_key:
             logger.error('No API key detected. Set cronitor.api_key or initialize Monitor with kwarg api_key.')
             return
 
         return self._req.get(url='{}/pause/{}'.format(self._monitor_api_url(self.key), hours), auth=(self.api_key, ''), timeout=5, headers=self._headers)
```

### Comparing `cronitor-4.7.0/cronitor/tests/test_config.py` & `cronitor-4.7.1/cronitor/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor/tests/test_monitor.py` & `cronitor-4.7.1/cronitor/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor/tests/test_pings.py` & `cronitor-4.7.1/cronitor/tests/test_pings.py`

 * *Files identical despite different names*

### Comparing `cronitor-4.7.0/cronitor.egg-info/PKG-INFO` & `cronitor-4.7.1/cronitor.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,302 +1,304 @@
 Metadata-Version: 2.1
 Name: cronitor
-Version: 4.7.0
+Version: 4.7.1
 Summary: A lightweight Python client for Cronitor.
 Home-page: https://github.com/cronitorio/cronitor-python
 Author: August Flanagan
 Author-email: august@cronitor.io
 License: MIT License
-Description: # Cronitor Python Library
-        ![Test](https://github.com/cronitorio/cronitor-python/workflows/Test/badge.svg)
-        
-        [Cronitor](https://cronitor.io/) provides end-to-end monitoring for background jobs, websites, APIs, and anything else that can send or receive an HTTP request. This library provides convenient access to the Cronitor API from applications written in Python. See our [API docs](https://cronitor.io/docs/api) for detailed references on configuring monitors and sending telemetry pings.
-        
-        In this guide:
-        
-        - [Installation](#Installation)
-        - [Monitoring Background Jobs](#monitoring-background-jobs)
-        - [Sending Telemetry Events](#sending-telemetry-events)
-        - [Configuring Monitors](#configuring-monitors)
-        - [Package Configuration & Env Vars](#package-configuration)
-        - [Command Line Usage](#command-line-usage)
-        
-        ## Installation
-        
-        ```
-        pip install cronitor
-        ```
-        
-        ## Monitoring Background Jobs
-        
-        #### Celery Auto-Discover
-        `cronitor-python` can automatically discover all of your declared Celery tasks, including your Celerybeat scheduled tasks,
-        creating monitors for them and sending pings when tasks run, succeed, or fail. Your API keys can be found [here](https://cronitor.io/settings/api).
-        
-        Requires Celery 4.0 or higher. Celery auto-discover utilizes the Celery [message protocol version 2](https://docs.celeryproject.org/en/stable/internals/protocol.html#version-2).
-        
-        <details>
-        <summary>Some important notes on support</summary>
-        
-        * Tasks on [solar schedules](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#solar-schedules) are not supported and will be ignored.
-        * [`django-celery-beat`](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#using-custom-scheduler-classes) is not yet supported, but is in the works.
-        * If you use the default `PersistentScheduler`, the celerybeat integration overrides the celerybeat local task run database (as referenced [here](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler) in the docs), named `celerybeat-schedule` by default. If you currently specify a custom location for this database, this integration will override it. **Very** few people require setting custom locations for this database. If you fall into this group and want to use `cronitor-python`'s celerybeat integration, please reach out to Cronitor support.
-        </details>
-        
-        ```python
-        import cronitor.celery
-        from celery import Celery
-        
-        app = Celery()
-        app.conf.beat_schedule = {
-            'run-me-every-minute': {
-                'task': 'tasks.every_minute_celery_task',
-                'schedule': 60
-            }
-        }
-        
-        # Discover all of your celery tasks and automatically add monitoring.
-        cronitor.celery.initialize(app, api_key="apiKey123")
-        
-        @app.task
-        def every_minute_celery_task():
-            print("running a background job with celery...")
-        
-        @app.task
-        def non_scheduled_celery_task():
-            print("Even though I'm not on a schedule, I'll still be monitored!")
-        ```
-        
-        If you want only to monitor Celerybeat periodic tasks, and not tasks triggered any other way, you can set `celereybeat_only=True` when initializing:
-        ```python
-        app = Celery()
-        cronitor.celery.initialize(app, api_key="apiKey123", celerybeat_only=True)
-        ```
-        
-        #### Manual Integration
-        
-        The `@cronitor.job` is a lightweight way to monitor any background task regardless of how it is executed. It will send telemetry events before calling your function and after it exits. If your function raises an exception a `fail` event will be sent (and the exception re-raised).
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        # Apply the cronitor decorator to monitor any function.
-        # If no monitor matches the provided key, one will be created automatically.
-        @cronitor.job('send-invoices')
-        def send_invoices_task(*args, **kwargs):
-            ...
-        ```
-        
-        ## Sending Telemetry Events
-        
-        If you want to send a heartbeat events, or want finer control over when/how [telemetry events](https://cronitor.io/docs/telemetry-api) are sent for your jobs, you can create a monitor instance and call the `.ping` method.
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        # optionally, set an environment
-        cronitor.environment = 'staging'
-        
-        monitor = cronitor.Monitor('heartbeat-monitor')
-        monitor.ping() # send a heartbeat event
-        
-        # optional params can be passed as keyword arguements.
-        # for a complete list see https://cronitor.io/docs/telemetry-api#parameters
-        monitor.ping(
-            state='run|complete|fail|ok', # run|complete|fail used to measure lifecycle of a job, ok used for manual reset only.
-            message='', # message that will be displayed in alerts as well as monitor activity panel on your dashboard.
-            metrics={
-                'duration': 100, # how long the job ran (complete|fail only). cronitor will calculate this when not provided
-                'count': 4500, # if your job is processing a number of items you can report a count
-                'error_count': 10 # the number of errors that occurred while this job was running
-            }
-        )
-        ```
-        
-        ## Configuring Monitors
-        
-        You can configure all of your monitors using a single YAML file. This can be version controlled and synced to Cronitor as part of
-        a deployment or build process. For details on all of the attributes that can be set, see the [Monitor API](https://cronitor.io/docs/monitor-api) documentation.
-        
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings/api
-        cronitor.api_key = 'apiKey123'
-        
-        cronitor.read_config('./cronitor.yaml') # parse the yaml file of monitors
-        
-        cronitor.validate_config() # send monitors to Cronitor for configuration validation
-        
-        cronitor.apply_config() # sync the monitors from the config file to Cronitor
-        
-        cronitor.generate_config() # generate a new config file from the Cronitor API
-        ```
-        
-        The timeout value for validate_config, apply_config and generate_config is 10 seconds by default. The value can be rewritten by setting the environment variable `CRONITOR_TIMEOUT`. It can also be rewritten by assigning a value to cronitor.timeout.
-        
-        ```python
-        import cronitor
-        
-        cronitor.timeout = 30
-        cronitor.apply_config()
-        ```
-        
-        The `cronitor.yaml` file includes three top level keys `jobs`, `checks`, `heartbeats`. You can configure monitors under each key by defining [monitors](https://cronitor.io/docs/monitor-api#attributes).
-        
-        ```yaml
-        jobs:
-            nightly-database-backup:
-                schedule: 0 0 * * *
-                notify:
-                    - devops-alert-pagerduty
-                assertions:
-                    - metric.duration < 5 minutes
-        
-            send-welcome-email:
-                schedule: every 10 minutes
-                assertions:
-                    - metric.count > 0
-                    - metric.duration < 30 seconds
-        
-        checks:
-            cronitor-homepage:
-                request:
-                    url: https://cronitor.io
-                    regions:
-                        - us-east-1
-                        - eu-central-1
-                        - ap-northeast-1
-                assertions:
-                    - response.code = 200
-                    - response.time < 2s
-        
-            cronitor-ping-api:
-                request:
-                    url: https://cronitor.link/ping
-                assertions:
-                    - response.body contains ok
-                    - response.time < .25s
-        
-        heartbeats:
-            production-deploy:
-                notify:
-                    alerts: ['deploys-slack']
-                    events: true # send alert when the event occurs
-        
-        ```
-        
-        You can also create and update monitors by calling `Monitor.put`. For details on all of the attributes that can be set see the Monitor API [documentation)(https://cronitor.io/docs/monitor-api#attributes).
-        
-        ```python
-        import cronitor
-        
-        monitors = cronitor.Monitor.put([
-          {
-            'type': 'job',
-            'key': 'send-customer-invoices',
-            'schedule': '0 0 * * *',
-            'assertions': [
-                'metric.duration < 5 min'
-            ],
-            'notify': ['devops-alerts-slack']
-          },
-          {
-            'type': 'check',
-            'key': 'Cronitor Homepage',
-            'schedule': 'every 45 seconds',
-            'request': {
-                'url': 'https://cronitor.io'
-            },
-            'assertions': [
-                'response.code = 200',
-                'response.time < 600ms',
-            ]
-          }
-        ])
-        ```
-        
-        ### Pausing, Reseting, and Deleting
-        
-        ```python
-        import cronitor
-        
-        monitor = cronitor.Monitor('heartbeat-monitor');
-        
-        monitor.pause(24) # pause alerting for 24 hours
-        monitor.unpause() # alias for .pause(0)
-        monitor.ok() # manually reset to a passing state alias for monitor.ping({state: ok})
-        monitor.delete() # destroy the monitor
-        ```
-        
-        ## Package Configuration
-        
-        The package needs to be configured with your account's `API key`, which is available on the [account settings](https://cronitor.io/settings) page. You can also optionally specify an `api_version` and an `environment`. If not provided, your account default is used. These can also be supplied using the environment variables `CRONITOR_API_KEY`, `CRONITOR_API_VERSION`, `CRONITOR_ENVIRONMENT`.
-        
-        ```python
-        import cronitor
-        
-        # your api keys can found here - https://cronitor.io/settings
-        cronitor.api_key = 'apiKey123'
-        cronitor.api_version = '2020-10-01'
-        cronitor.environment = 'cluster_1_prod'
-        ```
-        
-        ## Command Line Usage
-        
-        ```bash
-        >> python -m cronitor -h
-        
-        usage: cronitor [-h] [--apikey APIKEY] [--key KEY] [--msg MSG]
-                        (--run | --complete | --fail | --ok | --pause PAUSE)
-        
-        Send status messages to Cronitor ping API.
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --authkey AUTHKEY, -a AUTHKEY
-                                Auth Key from Account page
-          --key KEY, -k KEY     Unique key for the monitor to take ping
-          --msg MSG, -m MSG     Optional message to send with ping/fail
-          --tick, -t            Call ping on given monitor
-          --run, -r             Call ping with state=run on given monitor
-          --complete, -C        Call ping with state=complete on given monitor
-          --fail, -f            Call ping with state=fail on given monitor
-          --pause PAUSE, -P PAUSE
-                                Call pause on given monitor
-        ```
-        
-        
-        ## Contributing
-        
-        Pull requests and features are happily considered! By participating in this project you agree to abide by the [Code of Conduct](http://contributor-covenant.org/version/2/0).
-        
-        ### To contribute
-        
-        Fork, then clone the repo:
-        
-            git clone git@github.com:your-username/cronitor-python.git
-        
-        Set up your machine:
-        
-            pip install -r requirements
-        
-        Make sure the tests pass:
-        
-            pytest
-        
-        Make your change. Add tests for your change. Make the tests pass:
-        
-            pytest
-        
-        
-        Push to your fork and [submit a pull request]( https://github.com/cronitorio/cronitor-python/compare/)
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Cronitor Python Library
+![Test](https://github.com/cronitorio/cronitor-python/workflows/Test/badge.svg)
+
+[Cronitor](https://cronitor.io/) provides end-to-end monitoring for background jobs, websites, APIs, and anything else that can send or receive an HTTP request. This library provides convenient access to the Cronitor API from applications written in Python. See our [API docs](https://cronitor.io/docs/api) for detailed references on configuring monitors and sending telemetry pings.
+
+In this guide:
+
+- [Installation](#Installation)
+- [Monitoring Background Jobs](#monitoring-background-jobs)
+- [Sending Telemetry Events](#sending-telemetry-events)
+- [Configuring Monitors](#configuring-monitors)
+- [Package Configuration & Env Vars](#package-configuration)
+- [Command Line Usage](#command-line-usage)
+
+## Installation
+
+```
+pip install cronitor
+```
+
+## Monitoring Background Jobs
+
+#### Celery Auto-Discover
+`cronitor-python` can automatically discover all of your declared Celery tasks, including your Celerybeat scheduled tasks,
+creating monitors for them and sending pings when tasks run, succeed, or fail. Your API keys can be found [here](https://cronitor.io/settings/api).
+
+Requires Celery 4.0 or higher. Celery auto-discover utilizes the Celery [message protocol version 2](https://docs.celeryproject.org/en/stable/internals/protocol.html#version-2).
+
+**Some important notes on support**
+
+* Tasks on [solar schedules](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#solar-schedules) are not supported and will be ignored.
+* [`django-celery-beat`](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#using-custom-scheduler-classes) is not yet supported, but is in the works.
+* If you use the default `PersistentScheduler`, the celerybeat integration overrides the celerybeat local task run database (as referenced [here](https://docs.celeryproject.org/en/stable/userguide/periodic-tasks.html#starting-the-scheduler) in the docs), named `celerybeat-schedule` by default. If you currently specify a custom location for this database, this integration will override it. **Very** few people require setting custom locations for this database. If you fall into this group and want to use `cronitor-python`'s celerybeat integration, please reach out to Cronitor support.
+
+
+```python
+import cronitor.celery
+from celery import Celery
+
+app = Celery()
+app.conf.beat_schedule = {
+    'run-me-every-minute': {
+        'task': 'tasks.every_minute_celery_task',
+        'schedule': 60
+    }
+}
+
+# Discover all of your celery tasks and automatically add monitoring.
+cronitor.celery.initialize(app, api_key="apiKey123")
+
+@app.task
+def every_minute_celery_task():
+    print("running a background job with celery...")
+
+@app.task
+def non_scheduled_celery_task():
+    print("Even though I'm not on a schedule, I'll still be monitored!")
+```
+
+If you want only to monitor Celerybeat periodic tasks, and not tasks triggered any other way, you can set `celereybeat_only=True` when initializing:
+```python
+app = Celery()
+cronitor.celery.initialize(app, api_key="apiKey123", celerybeat_only=True)
+```
+
+#### Manual Integration
+
+The `@cronitor.job` is a lightweight way to monitor any background task regardless of how it is executed. It will send telemetry events before calling your function and after it exits. If your function raises an exception a `fail` event will be sent (and the exception re-raised).
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+# Apply the cronitor decorator to monitor any function.
+# If no monitor matches the provided key, one will be created automatically.
+@cronitor.job('send-invoices')
+def send_invoices_task(*args, **kwargs):
+    ...
+```
+
+## Sending Telemetry Events
+
+If you want to send a heartbeat events, or want finer control over when/how [telemetry events](https://cronitor.io/docs/telemetry-api) are sent for your jobs, you can create a monitor instance and call the `.ping` method.
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+# optionally, set an environment
+cronitor.environment = 'staging'
+
+monitor = cronitor.Monitor('heartbeat-monitor')
+monitor.ping() # send a heartbeat event
+
+# optional params can be passed as keyword arguements.
+# for a complete list see https://cronitor.io/docs/telemetry-api#parameters
+monitor.ping(
+    state='run|complete|fail|ok', # run|complete|fail used to measure lifecycle of a job, ok used for manual reset only.
+    message='', # message that will be displayed in alerts as well as monitor activity panel on your dashboard.
+    metrics={
+        'duration': 100, # how long the job ran (complete|fail only). cronitor will calculate this when not provided
+        'count': 4500, # if your job is processing a number of items you can report a count
+        'error_count': 10 # the number of errors that occurred while this job was running
+    }
+)
+```
+
+## Configuring Monitors
+
+You can configure all of your monitors using a single YAML file. This can be version controlled and synced to Cronitor as part of
+a deployment or build process. For details on all of the attributes that can be set, see the [Monitor API](https://cronitor.io/docs/monitor-api) documentation.
+
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings/api
+cronitor.api_key = 'apiKey123'
+
+cronitor.read_config('./cronitor.yaml') # parse the yaml file of monitors
+
+cronitor.validate_config() # send monitors to Cronitor for configuration validation
+
+cronitor.apply_config() # sync the monitors from the config file to Cronitor
+
+cronitor.generate_config() # generate a new config file from the Cronitor API
+```
+
+The timeout value for validate_config, apply_config and generate_config is 10 seconds by default. The value can be rewritten by setting the environment variable `CRONITOR_TIMEOUT`. It can also be rewritten by assigning a value to cronitor.timeout.
+
+```python
+import cronitor
+
+cronitor.timeout = 30
+cronitor.apply_config()
+```
+
+The `cronitor.yaml` file includes three top level keys `jobs`, `checks`, `heartbeats`. You can configure monitors under each key by defining [monitors](https://cronitor.io/docs/monitor-api#attributes).
+
+```yaml
+jobs:
+    nightly-database-backup:
+        schedule: 0 0 * * *
+        notify:
+            - devops-alert-pagerduty
+        assertions:
+            - metric.duration < 5 minutes
+
+    send-welcome-email:
+        schedule: every 10 minutes
+        assertions:
+            - metric.count > 0
+            - metric.duration < 30 seconds
+
+checks:
+    cronitor-homepage:
+        request:
+            url: https://cronitor.io
+            regions:
+                - us-east-1
+                - eu-central-1
+                - ap-northeast-1
+        assertions:
+            - response.code = 200
+            - response.time < 2s
+
+    cronitor-ping-api:
+        request:
+            url: https://cronitor.link/ping
+        assertions:
+            - response.body contains ok
+            - response.time < .25s
+
+heartbeats:
+    production-deploy:
+        notify:
+            alerts: ['deploys-slack']
+            events: true # send alert when the event occurs
+
+```
+
+You can also create and update monitors by calling `Monitor.put`. For details on all of the attributes that can be set see the Monitor API [documentation)(https://cronitor.io/docs/monitor-api#attributes).
+
+```python
+import cronitor
+
+monitors = cronitor.Monitor.put([
+  {
+    'type': 'job',
+    'key': 'send-customer-invoices',
+    'schedule': '0 0 * * *',
+    'assertions': [
+        'metric.duration < 5 min'
+    ],
+    'notify': ['devops-alerts-slack']
+  },
+  {
+    'type': 'check',
+    'key': 'Cronitor Homepage',
+    'schedule': 'every 45 seconds',
+    'request': {
+        'url': 'https://cronitor.io'
+    },
+    'assertions': [
+        'response.code = 200',
+        'response.time < 600ms',
+    ]
+  }
+])
+```
+
+### Pausing, Reseting, and Deleting
+
+```python
+import cronitor
+
+monitor = cronitor.Monitor('heartbeat-monitor');
+
+monitor.pause(24) # pause alerting for 24 hours
+monitor.unpause() # alias for .pause(0)
+monitor.ok() # manually reset to a passing state alias for monitor.ping({state: ok})
+monitor.delete() # destroy the monitor
+```
+
+## Package Configuration
+
+The package needs to be configured with your account's `API key`, which is available on the [account settings](https://cronitor.io/settings) page. You can also optionally specify an `api_version` and an `environment`. If not provided, your account default is used. These can also be supplied using the environment variables `CRONITOR_API_KEY`, `CRONITOR_API_VERSION`, `CRONITOR_ENVIRONMENT`.
+
+```python
+import cronitor
+
+# your api keys can found here - https://cronitor.io/settings
+cronitor.api_key = 'apiKey123'
+cronitor.api_version = '2020-10-01'
+cronitor.environment = 'cluster_1_prod'
+```
+
+## Command Line Usage
+
+```bash
+>> python -m cronitor -h
+
+usage: cronitor [-h] [--apikey APIKEY] [--key KEY] [--msg MSG]
+                (--run | --complete | --fail | --ok | --pause PAUSE)
+
+Send status messages to Cronitor ping API.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --authkey AUTHKEY, -a AUTHKEY
+                        Auth Key from Account page
+  --key KEY, -k KEY     Unique key for the monitor to take ping
+  --msg MSG, -m MSG     Optional message to send with ping/fail
+  --tick, -t            Call ping on given monitor
+  --run, -r             Call ping with state=run on given monitor
+  --complete, -C        Call ping with state=complete on given monitor
+  --fail, -f            Call ping with state=fail on given monitor
+  --pause PAUSE, -P PAUSE
+                        Call pause on given monitor
+```
+
+
+## Contributing
+
+Pull requests and features are happily considered! By participating in this project you agree to abide by the [Code of Conduct](http://contributor-covenant.org/version/2/0).
+
+### To contribute
+
+Fork, then clone the repo:
+
+    git clone git@github.com:your-username/cronitor-python.git
+
+Set up your machine:
+
+    pip install -r requirements
+
+Make sure the tests pass:
+
+    pytest
+
+Make your change. Add tests for your change. Make the tests pass:
+
+    pytest
+
+
+Push to your fork and [submit a pull request]( https://github.com/cronitorio/cronitor-python/compare/)
+
+
```

### Comparing `cronitor-4.7.0/setup.py` & `cronitor-4.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cronitor',
-    version='4.7.0',
+    version='4.7.1',
     packages=find_packages(),
     url='https://github.com/cronitorio/cronitor-python',
     license='MIT License',
     author='August Flanagan',
     author_email='august@cronitor.io',
     description='A lightweight Python client for Cronitor.',
     long_description = long_description,
```

