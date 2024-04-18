# Comparing `tmp/PatrowlEnginesUtils-1.2.0rc2.tar.gz` & `tmp/PatrowlEnginesUtils-1.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatrowlEnginesUtils-1.2.0rc2.tar", last modified: Thu Apr  4 07:46:41 2024, max compression
+gzip compressed data, was "PatrowlEnginesUtils-1.2.0rc3.tar", last modified: Fri Apr 12 09:41:17 2024, max compression
```

## Comparing `PatrowlEnginesUtils-1.2.0rc2.tar` & `PatrowlEnginesUtils-1.2.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    34523 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc2/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PKG-INFO
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    23779 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngine.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1074 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineExceptions.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5949 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineTest.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      252 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/__init__.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      365 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       20 2024-04-04 07:46:41.000000 PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      159 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc2/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       67 2024-04-04 07:46:41.481638 PatrowlEnginesUtils-1.2.0rc2/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      510 2024-04-03 15:51:44.000000 PatrowlEnginesUtils-1.2.0rc2/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-12 09:41:17.570214 PatrowlEnginesUtils-1.2.0rc3/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    34523 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc3/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      362 2024-04-12 09:41:17.570214 PatrowlEnginesUtils-1.2.0rc3/PKG-INFO
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-12 09:41:17.560214 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    26307 2024-04-12 09:36:44.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngine.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1074 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngineExceptions.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5949 2024-04-03 12:48:12.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngineTest.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      251 2024-04-12 08:31:38.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/__init__.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2024-04-12 09:41:17.570214 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      362 2024-04-12 09:41:17.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      365 2024-04-12 09:41:17.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2024-04-12 09:41:17.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       20 2024-04-12 09:41:17.000000 PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      159 2024-04-02 14:20:35.000000 PatrowlEnginesUtils-1.2.0rc3/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       67 2024-04-12 09:41:17.570214 PatrowlEnginesUtils-1.2.0rc3/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      509 2024-04-12 08:31:47.000000 PatrowlEnginesUtils-1.2.0rc3/setup.py
```

### Comparing `PatrowlEnginesUtils-1.2.0rc2/LICENSE` & `PatrowlEnginesUtils-1.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngine.py` & `PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # -*- coding: utf-8 -*-
 """This file manages PatrowlEngine and its common features."""
 
 import os
 
-import datetime
+from datetime import datetime, date, timezone
 from flask import jsonify, url_for, redirect, send_file
 import json
 import optparse
 import psutil
 import shutil
 import urllib
 import ssl
+import socket
 import time
 from uuid import UUID
+
 from .PatrowlEngineExceptions import PatrowlEngineExceptions
 
 APP_HOST = "127.0.0.1"
 APP_PORT = 5000
 APP_DEBUG = False
 APP_MAXSCANS = 25
 
 
 def _json_serial(obj):
     """JSON serializer for objects not serializable by default json code."""
-    if isinstance(obj, datetime.datetime) or isinstance(obj, datetime.date):
+    if isinstance(obj, datetime) or isinstance(obj, date):
         return obj.isoformat()
     if isinstance(obj, UUID):
         # if the obj is uuid, we simply return the value of uuid
         return obj.hex
     raise TypeError("Type not serializable")
 
 
@@ -44,14 +46,15 @@
         self.allowed_asset_types = []
         self.options = {}
         self.scan_id = 1
         self.scanner = {}
         self.scans = {}
         self.max_scans = max_scans
         self.status = "INIT"
+        self.metadata = {}
 
     def __str__(self):
         """Return a string-formated object."""
         return "%s - %s" % (self.name, self.version)
 
     def __to_dict(self):
         """Return a dict-formated object."""
@@ -132,15 +135,15 @@
 
     def liveness(self):
         """Return the liveness status."""
         return jsonify({"page": "liveness", "status": "success"}), 200
 
     def readiness(self):
         """Return the readiness status."""
-        if self.status not in ["READY", "BUSY"]:
+        if self.scanner["status"] not in ["READY", "BUSY"]:
             return jsonify({"page": "readiness", "status": "error"}), 500
         else:
             return jsonify({"page": "readiness", "status": "success"}), 200
 
     def test(self):
         """Return the test page."""
         res = "<h2>Test Page (DEBUG):</h2>"
@@ -163,17 +166,17 @@
         conf_file = self.base_dir + "/" + self.name + ".json"
         if os.path.exists(conf_file):
             engine_config = json.load(open(conf_file))
             self.version = engine_config["version"]
             self.description = engine_config["description"]
             self.options = engine_config["options"]
             self.allowed_asset_types = engine_config["allowed_asset_types"]
-            self.status = "READY"
+            self.scanner["status"] = "READY"
         else:
-            self.status = "ERROR"
+            self.scanner["status"] = "ERROR"
             return {"status": "ERROR", "reason": "config file not found"}
 
     def reloadconfig(self):
         """Reload the configuration file."""
         res = {"page": "reloadconfig"}
         self._loadconfig()
         res.update({"status": "success", "config": self.scanner})
@@ -216,18 +219,19 @@
         return context
 
     def clean(self, scan_id):
         """Clean all the scans."""
         res = {"page": "clean"}
         # Terminate processes
         for scan_id in self.scans.keys():
-            thread = self.scans[scan_id]["thread"]
-            if "proc" in thread and hasattr(thread["proc"], "pid"):
-                if psutil.pid_exists(thread["proc"].pid):
-                    psutil.Process(thread["proc"].pid).terminate()
+            for thread_id in self.scans[scan_id]["threads"]:
+                thread = self.scans[scan_id]["threads"][thread_id]
+                if "proc" in thread and hasattr(thread["proc"], "pid"):
+                    if psutil.pid_exists(thread["proc"].pid):
+                        psutil.Process(thread["proc"].pid).terminate()
         # Remove scans from memory
         self.scans.clear()
         # Update scanner status
         self.get_status()
         res.update({"status": "success"})
         return jsonify(res), 200
 
@@ -237,16 +241,25 @@
         res.update({"scan_id": scan_id})
 
         if scan_id not in self.scans.keys():
             raise PatrowlEngineExceptions(
                 1002, "scan_id '{}' not found".format(scan_id)
             )
 
+        # Terminate thread if any
+        for thread_id in self.scans[scan_id]["threads"]:
+            try:
+                thread = self.scans[scan_id][thread_id]
+                thread.join()
+                self.scans[scan_id]["threads"].remove(thread)
+            except Exception as e:
+                print(e)
+                pass
+
         self.scans.pop(scan_id)
-        # Todo: force terminating all threads
         res.update({"status": "removed"})
         return jsonify(res)
 
     def _engine_is_busy(self):
         """Returns if engine is busy scanning."""
         scans_count = 0
         # for scan_id, scan_infos in this.scans:
@@ -272,48 +285,62 @@
                 all_threads_finished = False
                 break
 
         if all_threads_finished and len(self.scans[scan_id]["threads"]) >= 1:
             if self.scans[scan_id]["status"] == "SCANNING":
                 # all threads are finished, ensure scan status is no more SCANNING
                 self.scans[scan_id]["status"] = "FINISHED"
+                self.scans[scan_id]["finished_at"] = datetime.now(
+                    timezone.utc
+                ).isoformat()
 
             if "finished_at" not in self.scans[scan_id].keys():
                 # update finished time if not already set
-                self.scans[scan_id]["finished_at"] = int(time.time() * 1000)
+                self.scans[scan_id]["finished_at"] = datetime.now(
+                    timezone.utc
+                ).isoformat()
 
         return jsonify({"status": self.scans[scan_id]["status"]})
 
-    def get_status(self):
+    def get_full_status(self):
+        """Return engine status with all assets on scans."""
+        return self.get_status(True)
+
+    def get_status(self, full_status=False):
         """Get the status of the engine and all its scans."""
         res = {"page": "status"}
         self.scanner["status"] = "READY"
         status_code = 200
 
-        # display info on the scanner
-        res.update({"scanner": self.scanner})
+        # display host + info on the scanner
+        res.update({"scanner": self.scanner, "hostname": socket.gethostname()})
 
         # display the status of scans performed
         scans = {}
         all_scans = list(self.scans.keys()).copy()
+
         for scan in all_scans:
             try:
-                self.status_scan(scan)
+                data = self.status_scan(scan).json
                 scans.update(
                     {
                         scan: {
-                            "status": self.scans[scan]["status"],
-                            "options": self.scans[scan]["options"],
-                            "nb_findings": self.scans[scan]["nb_findings"],
-                            "assets": self.scans[scan]["assets"],
-                            "position": self.scans[scan]["position"],
-                            "root_scan_id": self.scans[scan]["root_scan_id"],
+                            "status": data["status"],
+                            "options": data["options"],
+                            "nb_findings": data["nb_findings"],
+                            "nb_assets": len(data["assets"]),
+                            "position": data["position"],
+                            "root_scan_id": data["root_scan_id"],
+                            "created_at": data["created_at"],
+                            "finished_at": data["finished_at"],
                         }
                     }
                 )
+                if full_status:
+                    scans[scan].update({"assets": data["assets"]})
             except Exception:
                 pass
         res.update({"scans": scans})
 
         if self._engine_is_busy() is True:
             self.scanner["status"] = "BUSY"
 
@@ -322,108 +349,132 @@
             self.scanner["status"] = "ERROR"
 
         res.update({"status": self.scanner["status"]})
         if self.scanner["status"] == "ERROR":
             status_code = 500
         return jsonify(res), status_code
 
-    def status_scan(self, scan_id):
+    def _get_attr(self, data: dict, value: str, return_value=None):
+        if value in data:
+            return data[value]
+        return return_value
+
+    def status_scan(self, scan_id: int):
         """Get status on scan identified by id."""
-        res = {"page": "status_scan", "status": "UNKNOWN"}
+        res = {
+            "page": "status_scan",
+            "hostname": socket.gethostname(),
+            "status": "UNKNOWN",
+            "assets": [],
+        }
         info_thread_in_progress = []
         if scan_id not in self.scans.keys():
             res.update({"status": "error", "reason": f"scan_id '{scan_id}' not found"})
             return jsonify(res)
+        res.update({"scan_id": scan_id})
 
         if self.scans[scan_id]["status"] == "ERROR":
             res.update({"status": "error", "reason": "Something wrong happened"})
             return jsonify(res)
 
         # Fix when a scan is started but the thread has not been created yet
         if self.scans[scan_id]["status"] == "STARTED":
             res.update({"status": "SCANNING"})
 
-        if "assets" in self.scans[scan_id]:
-            res.update({"assets": self.scans[scan_id]["assets"]})
-        if "position" in self.scans[scan_id]:
-            res.update({"position": self.scans[scan_id]["position"]})
-        if "root_scan_id" in self.scans[scan_id]:
-            res.update({"root_scan_id": self.scans[scan_id]["root_scan_id"]})
-
-        thread = self.scans[scan_id]["thread"]
-        if "status" in thread and thread["status"] == "STARTED":
-            res.update({"status": "SCANNING"})
-            return jsonify(res)
-        elif "proc" not in thread:
-            res.update(
-                {"status": "error", "reason": "Process for this scan not found."}
-            )
-            return jsonify(res)
-
-        if not psutil.pid_exists(thread["proc"].pid):
-            thread["status"] = "FINISHED"
-
-        elif psutil.pid_exists(thread["proc"].pid) and psutil.Process(
-            thread["proc"].pid
-        ).status() in ["sleeping", "running"]:
-            thread["status"] = "SCANNING"
-            info = {
-                "thread_id": thread["thread_id"],
-                "cmd": thread["cmd"],
-                "pid": thread["proc"].pid,
+        res.update(
+            {
+                "options": self._get_attr(self.scans[scan_id], "options", {}),
+                "nb_findings": self._get_attr(self.scans[scan_id], "nb_findings"),
+                "nb_assets": len(self._get_attr(self.scans[scan_id], "assets", [])),
+                "assets": self._get_attr(self.scans[scan_id], "assets", []),
+                "position": self._get_attr(self.scans[scan_id], "position", 0),
+                "root_scan_id": self._get_attr(self.scans[scan_id], "root_scan_id", 0),
+                "created_at": self._get_attr(self.scans[scan_id], "created_at"),
+                "finished_at": self._get_attr(self.scans[scan_id], "finished_at"),
             }
-            info_thread_in_progress.append(info)
+        )
 
-        elif (
-            psutil.pid_exists(thread["proc"].pid)
-            and psutil.Process(thread["proc"].pid).status() == "zombie"
-        ):
-            thread["status"] = "FINISHED"
-            psutil.Process(thread["proc"].pid).terminate()
+        for thread_id in self.scans[scan_id]["threads"]:
+            thread = self.scans[scan_id]["threads"][thread_id]
+            if "proc" not in thread:
+                res.update(
+                    {"status": "error", "reason": "Process for this scan not found."}
+                )
+                return jsonify(res)
 
-        # Debug in case of status pf disk-sleep
-        else:
-            # print(psutil.Process(thread['proc'].pid).status())
-            thread["status"] = "SCANNING"
+            if not psutil.pid_exists(thread["proc"].pid):
+                thread["status"] = "FINISHED"
+            elif psutil.pid_exists(thread["proc"].pid) and psutil.Process(
+                thread["proc"].pid
+            ).status() in ["sleeping", "running"]:
+                thread["status"] = "SCANNING"
+                info = {
+                    "thread_id": thread["thread_id"],
+                    "cmd": thread["cmd"],
+                    "pid": thread["proc"].pid,
+                }
+                info_thread_in_progress.append(info)
 
-        thread = self.scans[scan_id]["thread"]
-        # if one thread is not finished, global scan is not finished
-        if thread["status"] == "SCANNING":
-            self.scans[scan_id]["status"] = "SCANNING"
-            res.update(
-                {"status": "SCANNING", "info": [t for t in info_thread_in_progress]}
-            )
-            return jsonify(res)
-        else:
-            self.scans[scan_id]["status"] = "FINISHED"
-            res.update({"status": "FINISHED"})
+            elif (
+                psutil.pid_exists(thread["proc"].pid)
+                and psutil.Process(thread["proc"].pid).status() == "zombie"
+            ):
+                thread["status"] = "FINISHED"
+                psutil.Process(thread["proc"].pid).terminate()
+
+            # Debug in case of status pf disk-sleep
+            else:
+                # print(psutil.Process(thread['proc'].pid).status())
+                thread["status"] = "SCANNING"
+
+        for thread_id in self.scans[scan_id]["threads"]:
+            thread = self.scans[scan_id]["threads"][thread_id]
+            # if one thread is not finished, global scan is not finished
+            if thread["status"] in ["SCANNING", "STARTED", "RUNNING"]:
+                self.scans[scan_id]["status"] = "SCANNING"
+                res.update(
+                    {"status": "SCANNING", "info": [t for t in info_thread_in_progress]}
+                )
+                return jsonify(res)
+            else:
+                self.scans[scan_id]["status"] = "FINISHED"
+                self.scans[scan_id]["finished_at"] = datetime.now(
+                    timezone.utc
+                ).isoformat()
+                res.update({"status": "FINISHED"})
         return jsonify(res)
 
     def info(self):
         """Return the info page."""
         scans = {}
         for scan in self.scans.keys():
-            self.status_scan(scan)
+            # self.status_scan(scan)
             scans.update(
                 {
                     scan: {
                         "status": self.scans[scan]["status"],
+                        "nb_assets": len(self.scans[scan]["assets"]),
                         "options": self.scans[scan]["options"],
                         "nb_findings": self.scans[scan]["nb_findings"],
                     }
                 }
             )
 
-        res = {"page": "info", "engine_config": self.scanner, "scans": scans}
+        res = {
+            "page": "info",
+            "hostname": socket.gethostname(),
+            "engine_config": self.scanner,
+            "scans": scans,
+        }
         return jsonify(res), 200
 
     def stop_scan(self, scan_id):
         """Stop a scan identified by his 'id'."""
         res = {"page": "stop_scan"}
-
+        pids = ""
         if scan_id not in self.scans.keys():
             raise PatrowlEngineExceptions(
                 1002, "scan_id '{}' not found".format(scan_id)
             )
 
         # Update scan status
         self.status_scan(scan_id)
@@ -433,26 +484,30 @@
                     "status": "ERROR",
                     "reason": "scan '{}' is not running (status={})".format(
                         scan_id, self.scans[scan_id]["status"]
                     ),
                 }
             )
             return jsonify(res)
+        for thread_id in self.scans[scan_id]["threads"]:
+            thread = self.scans[scan_id][thread_id]
+            if hasattr(thread["proc"], "pid"):
+                if psutil.pid_exists(thread["proc"].pid):
+                    psutil.Process(thread["proc"].pid).terminate()
+                    pids += " " + str(thread["proc"].pid)
 
-        thread = self.scans[scan_id]["thread"]
-        if hasattr(thread["proc"], "pid"):
-            if psutil.pid_exists(thread["proc"].pid):
-                psutil.Process(thread["proc"].pid).terminate()
-                pids += " " + str(thread["proc"].pid)
-
-        # Stop scan thread
-        thread["thread"].join()
+            # Stop scan
+            try:
+                thread.join()
+                self.scans[scan_id]["threads"].pop(thread_id)
+            except Exception:
+                pass
 
         self.scans[scan_id]["status"] = "STOPPED"
-        self.scans[scan_id]["finished_at"] = int(time.time() * 1000)
+        self.scans[scan_id]["finished_at"] = datetime.now(timezone.utc).isoformat()
 
         res.update({"status": "success", "details": {"pid": pids, "scan_id": scan_id}})
         return jsonify(res), 200
 
     # Stop all scans
     def stop(self):
         """Stop all the scans."""
@@ -474,19 +529,22 @@
                     "reason": "Scan refused: max concurrent active scans reached \
                     ({})".format(self.max_scans),
                 }
             )
             return res
 
         self.get_status()
-        if self.status != "READY":
+        if self.scanner["status"] != "READY":
             res.update(
                 {
                     "status": "ERROR",
-                    "details": {"reason": "scanner not ready", "status": self.status},
+                    "details": {
+                        "reason": "scanner not ready",
+                        "status": self.scanner["status"],
+                    },
                 }
             )
             return res
 
         data = json.loads(params)
         if "assets" not in data.keys():
             res.update(
@@ -553,15 +611,17 @@
             )
 
         # check if the scan is finished (thread as well)
         self.status_scan(scan_id)
         if self.scans[scan_id]["status"] != "FINISHED":
             raise PatrowlEngineExceptions(
                 1003,
-                "scan_id '{}' not finished (status={})".format(scan_id, scan["status"]),
+                "scan_id '{}' not finished (status={})".format(
+                    scan_id, self.scans[scan_id]["status"]
+                ),
             )
 
         issues = []
         summary = {}
         issues, summary = self._parse_results(scan_id)
 
         with open(
```

### Comparing `PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineExceptions.py` & `PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngineExceptions.py`

 * *Files identical despite different names*

### Comparing `PatrowlEnginesUtils-1.2.0rc2/PatrowlEnginesUtils/PatrowlEngineTest.py` & `PatrowlEnginesUtils-1.2.0rc3/PatrowlEnginesUtils/PatrowlEngineTest.py`

 * *Files identical despite different names*

