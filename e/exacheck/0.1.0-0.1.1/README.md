# Comparing `tmp/exacheck-0.1.0.tar.gz` & `tmp/exacheck-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exacheck-0.1.0.tar", max compression
+gzip compressed data, was "exacheck-0.1.1.tar", max compression
```

## Comparing `exacheck-0.1.0.tar` & `exacheck-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1060 2024-02-08 17:18:51.304656 exacheck-0.1.0/LICENSE
--rw-r--r--   0        0        0     1813 2024-02-08 17:18:51.304656 exacheck-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-02-05 13:21:09.084737 exacheck-0.1.0/exacheck/__init__.py
--rw-r--r--   0        0        0      198 2024-02-06 16:22:20.120443 exacheck-0.1.0/exacheck/__version__.py
--rw-r--r--   0        0        0     9035 2024-02-06 16:22:28.956457 exacheck-0.1.0/exacheck/announcer.py
--rw-r--r--   0        0        0     5218 2024-02-21 08:10:52.814613 exacheck-0.1.0/exacheck/checkexecutor.py
--rw-r--r--   0        0        0     2413 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/checkresult.py
--rw-r--r--   0        0        0     1954 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/checkstate.py
--rw-r--r--   0        0        0     2693 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/cli.py
--rw-r--r--   0        0        0     7125 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/configuration.py
--rw-r--r--   0        0        0    20989 2024-03-20 15:22:48.053436 exacheck-0.1.0/exacheck/exacheck.py
--rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/__init__.py
--rw-r--r--   0        0        0      520 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/addressfamilyerror.py
--rw-r--r--   0        0        0      397 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/checktimeout.py
--rw-r--r--   0        0        0      447 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/dnsresolutionerror.py
--rw-r--r--   0        0        0      449 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/exceptions/workerprocesserror.py
--rw-r--r--   0        0        0    11129 2024-03-31 09:25:23.028122 exacheck-0.1.0/exacheck/logmanager.py
--rw-r--r--   0        0        0      606 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/__init__.py
--rw-r--r--   0        0        0     1644 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/_base.py
--rw-r--r--   0        0        0    12642 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/_remote.py
--rw-r--r--   0        0        0     9523 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/dns.py
--rw-r--r--   0        0        0     2403 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/file.py
--rw-r--r--   0        0        0     8192 2024-04-01 15:42:37.124154 exacheck-0.1.0/exacheck/methods/http.py
--rw-r--r--   0        0        0     7108 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/icmp.py
--rw-r--r--   0        0        0     6473 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/ntp.py
--rw-r--r--   0        0        0     2445 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/shell.py
--rw-r--r--   0        0        0     3485 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/methods/tcp.py
--rw-r--r--   0        0        0     7610 2024-03-20 15:22:48.053436 exacheck-0.1.0/exacheck/notifications.py
--rw-r--r--   0        0        0     2088 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/procname.py
--rw-r--r--   0        0        0        0 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/__init__.py
--rw-r--r--   0        0        0      528 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/_base.py
--rw-r--r--   0        0        0    10512 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/check.py
--rw-r--r--   0        0        0      589 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/__init__.py
--rw-r--r--   0        0        0      757 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/_base.py
--rw-r--r--   0        0        0     2217 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/_remote.py
--rw-r--r--   0        0        0     3969 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/dnsargs.py
--rw-r--r--   0        0        0     1351 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/fileargs.py
--rw-r--r--   0        0        0     7165 2024-04-01 15:42:37.124154 exacheck-0.1.0/exacheck/settings/checkargs/httpargs.py
--rw-r--r--   0        0        0     6955 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/icmpargs.py
--rw-r--r--   0        0        0     2166 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/ntpargs.py
--rw-r--r--   0        0        0      793 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/shellargs.py
--rw-r--r--   0        0        0     1477 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/checkargs/tcpargs.py
--rw-r--r--   0        0        0      764 2024-02-06 16:22:20.124443 exacheck-0.1.0/exacheck/settings/exacheck.py
--rw-r--r--   0        0        0      168 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/__init__.py
--rw-r--r--   0        0        0     2824 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/_base.py
--rw-r--r--   0        0        0     2795 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/logfile.py
--rw-r--r--   0        0        0     3251 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/loggers/syslog.py
--rw-r--r--   0        0        0     2750 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/settings/notifications.py
--rw-r--r--   0        0        0     1500 2024-02-06 16:22:28.956457 exacheck-0.1.0/exacheck/settings/sentry.py
--rw-r--r--   0        0        0     4560 2024-02-06 16:22:20.124443 exacheck-0.1.0/exacheck/settings/settings.py
--rw-r--r--   0        0        0     3222 2024-02-06 16:20:18.168247 exacheck-0.1.0/exacheck/sleeper.py
--rw-r--r--   0        0        0    13996 2024-02-21 08:01:57.744512 exacheck-0.1.0/exacheck/worker.py
--rw-r--r--   0        0        0     3320 2024-04-01 15:44:46.811009 exacheck-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 exacheck-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-02-08 17:18:51.000000 exacheck-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2372 2024-04-18 14:45:45.662572 exacheck-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-05 13:21:09.000000 exacheck-0.1.1/exacheck/__init__.py
+-rw-r--r--   0        0        0      198 2024-02-06 16:22:20.000000 exacheck-0.1.1/exacheck/__version__.py
+-rw-r--r--   0        0        0     9035 2024-02-06 16:22:28.000000 exacheck-0.1.1/exacheck/announcer.py
+-rw-r--r--   0        0        0     5218 2024-02-21 08:10:52.000000 exacheck-0.1.1/exacheck/checkexecutor.py
+-rw-r--r--   0        0        0     2413 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/checkresult.py
+-rw-r--r--   0        0        0     1954 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/checkstate.py
+-rw-r--r--   0        0        0     2693 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/cli.py
+-rw-r--r--   0        0        0     7125 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/configuration.py
+-rw-r--r--   0        0        0    20989 2024-03-20 15:22:48.000000 exacheck-0.1.1/exacheck/exacheck.py
+-rw-r--r--   0        0        0        0 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/exceptions/__init__.py
+-rw-r--r--   0        0        0      520 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/exceptions/addressfamilyerror.py
+-rw-r--r--   0        0        0      397 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/exceptions/checktimeout.py
+-rw-r--r--   0        0        0      447 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/exceptions/dnsresolutionerror.py
+-rw-r--r--   0        0        0      449 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/exceptions/workerprocesserror.py
+-rw-r--r--   0        0        0    11129 2024-03-31 09:25:23.000000 exacheck-0.1.1/exacheck/logmanager.py
+-rw-r--r--   0        0        0      606 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/__init__.py
+-rw-r--r--   0        0        0     1644 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/_base.py
+-rw-r--r--   0        0        0    12642 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/_remote.py
+-rw-r--r--   0        0        0     9523 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/dns.py
+-rw-r--r--   0        0        0     2403 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/file.py
+-rw-r--r--   0        0        0     8192 2024-04-01 15:42:37.000000 exacheck-0.1.1/exacheck/methods/http.py
+-rw-r--r--   0        0        0     7108 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/icmp.py
+-rw-r--r--   0        0        0     6473 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/ntp.py
+-rw-r--r--   0        0        0     2445 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/shell.py
+-rw-r--r--   0        0        0     3485 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/methods/tcp.py
+-rw-r--r--   0        0        0     7610 2024-03-20 15:22:48.000000 exacheck-0.1.1/exacheck/notifications.py
+-rw-r--r--   0        0        0     2088 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/procname.py
+-rw-r--r--   0        0        0        0 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/__init__.py
+-rw-r--r--   0        0        0      528 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/_base.py
+-rw-r--r--   0        0        0    10512 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/check.py
+-rw-r--r--   0        0        0      589 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/__init__.py
+-rw-r--r--   0        0        0      757 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/_base.py
+-rw-r--r--   0        0        0     2217 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/_remote.py
+-rw-r--r--   0        0        0     3969 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/dnsargs.py
+-rw-r--r--   0        0        0     1351 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/fileargs.py
+-rw-r--r--   0        0        0     7165 2024-04-01 15:42:37.000000 exacheck-0.1.1/exacheck/settings/checkargs/httpargs.py
+-rw-r--r--   0        0        0     6955 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/icmpargs.py
+-rw-r--r--   0        0        0     2166 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/ntpargs.py
+-rw-r--r--   0        0        0      793 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/shellargs.py
+-rw-r--r--   0        0        0     1477 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/checkargs/tcpargs.py
+-rw-r--r--   0        0        0      764 2024-02-06 16:22:20.000000 exacheck-0.1.1/exacheck/settings/exacheck.py
+-rw-r--r--   0        0        0      168 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/loggers/__init__.py
+-rw-r--r--   0        0        0     2824 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/loggers/_base.py
+-rw-r--r--   0        0        0     2795 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/loggers/logfile.py
+-rw-r--r--   0        0        0     3251 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/loggers/syslog.py
+-rw-r--r--   0        0        0     2750 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/settings/notifications.py
+-rw-r--r--   0        0        0     1500 2024-02-06 16:22:28.000000 exacheck-0.1.1/exacheck/settings/sentry.py
+-rw-r--r--   0        0        0     4560 2024-02-06 16:22:20.000000 exacheck-0.1.1/exacheck/settings/settings.py
+-rw-r--r--   0        0        0     3222 2024-02-06 16:20:18.000000 exacheck-0.1.1/exacheck/sleeper.py
+-rw-r--r--   0        0        0    13996 2024-02-21 08:01:57.000000 exacheck-0.1.1/exacheck/worker.py
+-rw-r--r--   0        0        0     3727 2024-04-18 14:45:45.664572 exacheck-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 exacheck-0.1.1/PKG-INFO
```

### Comparing `exacheck-0.1.0/LICENSE` & `exacheck-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/README.md` & `exacheck-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -17,8 +17,24 @@
 - Live configuration reloads (adding/modifying/removing services)
 - Health checks implemented in pure python where possible; no need to write scripts or use chains of commands to validate output
 - Detailed logging available
 - Configuration validation (if using live configuration reloads, configuration is validated before application)
 - Out of the box sane defaults where possible
 - JSON schema of configuration (see [schema.json][ExaCheck Configuration Schema] for the current schema)
 
+## Known Issues
+
+If installing Exacheck with Python 3.12 or higher, ExaBGP is not included as a requirement and you must install ExaBGP from source. If using ExaBGP from PyPi using Python 3.12 you will get the following error when running ExaBGP:
+
+```bash
+ModuleNotFoundError: No module named 'exabgp.vendoring.six.moves'
+```
+
+To work around the problem, install ExaBGP from source:
+
+```bash
+python3 -m pip --no-cache-dir install "git+https://github.com/Exa-Networks/exabgp.git@4.2"
+```
+
+If you are using the Docker container you do not need to do anything.
+
 [ExaCheck Configuration Schema]: https://github.com/exacheck/exacheck/blob/main/schema.json
```

### Comparing `exacheck-0.1.0/exacheck/announcer.py` & `exacheck-0.1.1/exacheck/announcer.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/checkexecutor.py` & `exacheck-0.1.1/exacheck/checkexecutor.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/checkresult.py` & `exacheck-0.1.1/exacheck/checkresult.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/checkstate.py` & `exacheck-0.1.1/exacheck/checkstate.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/cli.py` & `exacheck-0.1.1/exacheck/cli.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/configuration.py` & `exacheck-0.1.1/exacheck/configuration.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/exacheck.py` & `exacheck-0.1.1/exacheck/exacheck.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/exceptions/addressfamilyerror.py` & `exacheck-0.1.1/exacheck/exceptions/addressfamilyerror.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/logmanager.py` & `exacheck-0.1.1/exacheck/logmanager.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/__init__.py` & `exacheck-0.1.1/exacheck/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/_base.py` & `exacheck-0.1.1/exacheck/methods/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/_remote.py` & `exacheck-0.1.1/exacheck/methods/_remote.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/dns.py` & `exacheck-0.1.1/exacheck/methods/dns.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/file.py` & `exacheck-0.1.1/exacheck/methods/file.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/http.py` & `exacheck-0.1.1/exacheck/methods/http.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/icmp.py` & `exacheck-0.1.1/exacheck/methods/icmp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/ntp.py` & `exacheck-0.1.1/exacheck/methods/ntp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/shell.py` & `exacheck-0.1.1/exacheck/methods/shell.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/methods/tcp.py` & `exacheck-0.1.1/exacheck/methods/tcp.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/notifications.py` & `exacheck-0.1.1/exacheck/notifications.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/procname.py` & `exacheck-0.1.1/exacheck/procname.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/_base.py` & `exacheck-0.1.1/exacheck/settings/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/check.py` & `exacheck-0.1.1/exacheck/settings/check.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/__init__.py` & `exacheck-0.1.1/exacheck/settings/checkargs/__init__.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/_base.py` & `exacheck-0.1.1/exacheck/settings/checkargs/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/_remote.py` & `exacheck-0.1.1/exacheck/settings/checkargs/_remote.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/dnsargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/dnsargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/fileargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/fileargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/httpargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/httpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/icmpargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/icmpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/ntpargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/ntpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/shellargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/shellargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/checkargs/tcpargs.py` & `exacheck-0.1.1/exacheck/settings/checkargs/tcpargs.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/exacheck.py` & `exacheck-0.1.1/exacheck/settings/exacheck.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/loggers/_base.py` & `exacheck-0.1.1/exacheck/settings/loggers/_base.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/loggers/logfile.py` & `exacheck-0.1.1/exacheck/settings/loggers/logfile.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/loggers/syslog.py` & `exacheck-0.1.1/exacheck/settings/loggers/syslog.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/notifications.py` & `exacheck-0.1.1/exacheck/settings/notifications.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/sentry.py` & `exacheck-0.1.1/exacheck/settings/sentry.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/settings/settings.py` & `exacheck-0.1.1/exacheck/settings/settings.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/sleeper.py` & `exacheck-0.1.1/exacheck/sleeper.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/exacheck/worker.py` & `exacheck-0.1.1/exacheck/worker.py`

 * *Files identical despite different names*

### Comparing `exacheck-0.1.0/pyproject.toml` & `exacheck-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "networks",
   "routes",
   "routing",
 ]
 name = "exacheck"
 readme = "README.md"
 repository = "https://github.com/exacheck/exacheck"
-version = "0.1.0"
+version = "0.1.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry.urls]
 "Changelog" = "https://exacheck.net/development/changelog/"
@@ -42,20 +42,26 @@
 exacheck = 'exacheck.cli:cli'
 
 [tool.poetry.dependencies]
 # Python version required
 python = ">=3.10,<3.13"
 
 # ExaBGP itself
-exabgp = "^4.2.21"
+# Currently this will only be included as a dependancy when using Python 3.11 or below
+# To use Python 3.12 or above, ExaBGP must be installed from source due to the following error:
+#   ModuleNotFoundError: No module named 'exabgp.vendoring.six.moves'
+#
+# To install from source:
+#   python3 -m pip --no-cache-dir install "git+https://github.com/Exa-Networks/exabgp.git@4.2"
+exabgp = {version = "^4.2.21", python = "<=3.11"}
 
 # General ExaCheck requirements
-apprise = "^1.7.5"
+apprise = "^1.7.6"
 loguru = "^0.7.2"
-pydantic = "^2.6.4"
+pydantic = "^2.7.0"
 pyyaml = "^6.0.1"
 setproctitle = "^1.3.3"
 tabulate = "^0.9.0"
 ujson = "^5.9.0"
 
 # Requirements for the built in health checks
 dnspython = "^2.6.1"
@@ -63,15 +69,15 @@
 ntplib = "^0.4.0"
 httpx = {extras = ["http2"], version = "^0.27.0"}
 
 # For the CLI
 click = "^8.1.7"
 
 # For Sentry support; optional
-sentry-sdk = {version = "^1.44.0", optional = true}
+sentry-sdk = {version = "^1.45.0", optional = true}
 
 [tool.poetry.extras]
 sentry = [
   "sentry-sdk",
 ]
 full = [
   "sentry-sdk",
@@ -91,46 +97,46 @@
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # Packages for linting
 pycodestyle = "^2.11.1"
 pylint = "^3.1.0"
 pylint-pydantic = "^0.3.2"
-ruff = "^0.3.4"
-semgrep = "^1.67.0"
+ruff = "^0.3.7"
+semgrep = "^1.69.0"
 
 # Misc other development tools
 Cython = "^3.0.10"
 devtools = {extras = ["pygments"], version = "^0.12.2"}
 ipython = "^8.23.0"
 Markdown = "^3.6"
 pipenv = "^2023.12.1"
 rich = "^13.7.1"
 
 # Define the packages for the optional groups
 [tool.poetry.group.format.dependencies]
 # Packages for code formatting
 autopep8 = "^2.1.0"
-black = "^24.3.0"
+black = "^24.4.0"
 flake8 = "^7.0.0"
 
 [tool.poetry.group.test.dependencies]
 # Packages for testing
-hypothesis = {extras = ["cli"], version = "^6.100.0"}
+hypothesis = {extras = ["cli"], version = "^6.100.1"}
 pytest = "^8.1.1"
 pytest-html = "^4.1.1"
 
 [tool.poetry.group.typing.dependencies]
 # Packages for type checking
 mypy = "^1.9.0"
 pyre-check = "^0.9.19"
 
 # Extensions for type checking
 types-pyyaml = "^6.0.12.20240311"
-types-requests = "^2.31.0.20240311"
+types-requests = "^2.31.0.20240406"
 types-tabulate = "^0.9.0"
 types-ujson = "^5.9.0"
 
 [tool.autopep8]
 # Raise default maximum line length
 max_line_length = 120
```

### Comparing `exacheck-0.1.0/PKG-INFO` & `exacheck-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exacheck
-Version: 0.1.0
+Version: 0.1.1
 Summary: ExaCheck - ExaBGP Health Checker
 Home-page: https://exacheck.net
 Keywords: bgp,exabgp,healthcheck,monitoring,network,networking,networks,routes,routing
 Author: Chris
 Author-email: info@exacheck.net
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -17,25 +17,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Provides-Extra: full
 Provides-Extra: sentry
-Requires-Dist: apprise (>=1.7.5,<2.0.0)
+Requires-Dist: apprise (>=1.7.6,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
-Requires-Dist: exabgp (>=4.2.21,<5.0.0)
+Requires-Dist: exabgp (>=4.2.21,<5.0.0) ; python_full_version <= "3.11.0"
 Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: icmplib (>=3.0.4,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: sentry-sdk (>=1.44.0,<2.0.0) ; extra == "sentry" or extra == "full"
+Requires-Dist: sentry-sdk (>=1.45.0,<2.0.0) ; extra == "sentry" or extra == "full"
 Requires-Dist: setproctitle (>=1.3.3,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Project-URL: Changelog, https://exacheck.net/development/changelog/
 Project-URL: Configuration, https://exacheck.net/configuration/
 Project-URL: Documentation, https://exacheck.net/deployment/
 Project-URL: Docker Deployment, https://exacheck.net/deployment/docker/
@@ -61,9 +61,25 @@
 - Live configuration reloads (adding/modifying/removing services)
 - Health checks implemented in pure python where possible; no need to write scripts or use chains of commands to validate output
 - Detailed logging available
 - Configuration validation (if using live configuration reloads, configuration is validated before application)
 - Out of the box sane defaults where possible
 - JSON schema of configuration (see [schema.json][ExaCheck Configuration Schema] for the current schema)
 
+## Known Issues
+
+If installing Exacheck with Python 3.12 or higher, ExaBGP is not included as a requirement and you must install ExaBGP from source. If using ExaBGP from PyPi using Python 3.12 you will get the following error when running ExaBGP:
+
+```bash
+ModuleNotFoundError: No module named 'exabgp.vendoring.six.moves'
+```
+
+To work around the problem, install ExaBGP from source:
+
+```bash
+python3 -m pip --no-cache-dir install "git+https://github.com/Exa-Networks/exabgp.git@4.2"
+```
+
+If you are using the Docker container you do not need to do anything.
+
 [ExaCheck Configuration Schema]: https://github.com/exacheck/exacheck/blob/main/schema.json
```

