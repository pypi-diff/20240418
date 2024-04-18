# Comparing `tmp/cpg-utils-5.0.5.tar.gz` & `tmp/cpg-utils-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.5.tar", last modified: Tue Apr 16 22:31:25 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.6.tar", last modified: Thu Apr 18 05:51:26 2024, max compression
```

## Comparing `cpg-utils-5.0.5.tar` & `cpg-utils-5.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.986887 cpg-utils-5.0.5/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26173 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.990887 cpg-utils-5.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 22:31:25.000000 cpg-utils-5.0.5/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26201 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 05:51:25.000000 cpg-utils-5.0.6/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 05:51:26.000000 cpg-utils-5.0.6/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:51:25.000000 cpg-utils-5.0.6/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 05:51:25.000000 cpg-utils-5.0.6/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 05:51:25.000000 cpg-utils-5.0.6/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:26.021301 cpg-utils-5.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 05:51:24.000000 cpg-utils-5.0.6/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.5/LICENSE` & `cpg-utils-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/PKG-INFO` & `cpg-utils-5.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.5
+Version: 5.0.6
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.5/README.md` & `cpg-utils-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/__init__.py` & `cpg-utils-5.0.6/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/cloud.py` & `cpg-utils-5.0.6/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.6/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/config.py` & `cpg-utils-5.0.6/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/constants.py` & `cpg-utils-5.0.6/cpg_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/cromwell.py` & `cpg-utils-5.0.6/cpg_utils/cromwell.py`

 * *Files 3% similar despite different names*

```diff
@@ -366,14 +366,15 @@
     INNER Python function to watch workflow status, and write
     output paths to output_json_path on success.
     """
     # Re-importing dependencies here so the function is self-contained
     # and can be run in a Hail bash job.
 
     import json
+    import logging
     import math
     import subprocess
     import time
     from datetime import datetime
 
     import requests
     from cloudpathlib.anypath import to_anypath
@@ -415,15 +416,15 @@
         return max(
             min_poll_interval,
             int((1 - math.cos(math.pi * factor)) * max_poll_interval // 2),
         )
 
     with open(workflow_id_file, encoding='utf-8') as f:
         workflow_id = f.read().strip()
-    logger.info(f'Received workflow ID: {workflow_id}')
+    logging.info(f'Received workflow ID: {workflow_id}')
 
     failed_statuses = {'failed', 'aborted'}
     terminal_statuses = {'succeeded'} | failed_statuses
     status_reported = False
     subprocess.check_output(GCLOUD_ACTIVATE_AUTH_BASE)  # noqa: S603
     cromwell_workflow_root = f'{CROMWELL_URL}/api/workflows/v1/{workflow_id}'
     metadata_url = f'{cromwell_workflow_root}/metadata'
@@ -442,63 +443,63 @@
             exponential_decrease_seconds,
         )
         try:
             auth_header = {'Authorization': f'Bearer {_get_cromwell_oauth_token()}'}
             r = requests.get(status_url, headers=auth_header, timeout=60)
             if not r.ok:
                 _remaining_exceptions -= 1
-                logger.warning(
+                logging.warning(
                     f'Received "not okay" (status={r.status_code}) from cromwell '
                     f'(waiting={wait_time}): {r.text}',
                 )
                 time.sleep(wait_time)
                 continue
             status = r.json().get('status')
 
             # if workflow has concluded print logging to hail batch log
             if status.lower() in terminal_statuses and not status_reported:
-                logger.info('Cromwell workflow has concluded - fetching log')
+                logging.info('Cromwell workflow has concluded - fetching log')
                 # don't report multiple times if we fail fetching output
                 # also don't fail the whole run if we can't fetch metadata
                 status_reported = True
                 response = requests.get(metadata_url, headers=auth_header, timeout=60)
                 if response.ok:
                     meta_json = response.json()
                     print(WorkflowMetadataModel.parse(meta_json).display())
                 else:
                     print('Failed to collect run Metadata')
 
             if status.lower() == 'succeeded':
-                logger.info('Cromwell workflow moved to succeeded state')
+                logging.info('Cromwell workflow moved to succeeded state')
                 _remaining_exceptions = max_sequential_exception_count
                 # process outputs here
                 r_outputs = requests.get(outputs_url, headers=auth_header, timeout=60)
                 if not r_outputs.ok:
-                    logger.warning(
+                    logging.warning(
                         'Received error when fetching cromwell outputs, '
                         f'will retry in {wait_time} seconds',
                     )
                     time.sleep(wait_time)
                     continue
                 outputs = r_outputs.json()
-                logger.info(f'Received outputs from Cromwell: {outputs}')
+                logging.info(f'Received outputs from Cromwell: {outputs}')
                 with to_anypath(output_json_path).open('w') as fh:
                     json.dump(outputs.get('outputs'), fh)
                 break
             if status.lower() in failed_statuses:
-                logger.error(f'Got failed cromwell status: {status}')
+                logging.error(f'Got failed cromwell status: {status}')
                 raise CromwellError(status)
-            logger.info(f'Got cromwell status: {status} (sleeping={wait_time})')
+            logging.info(f'Got cromwell status: {status} (sleeping={wait_time})')
             time.sleep(wait_time)
         except CromwellError:
             # pass through
             raise
         except Exception as e:  # noqa: BLE001
             _remaining_exceptions -= 1
-            logger.error(
+            logging.error(
                 f'Cromwell status watch caught general exception (sleeping={wait_time}): {e}',
             )
             time.sleep(wait_time)
 
 
 def watch_workflow_and_get_output(
     b: Batch,
```

### Comparing `cpg-utils-5.0.5/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.6/cpg_utils/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/dataproc.py` & `cpg-utils-5.0.6/cpg_utils/dataproc.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/git.py` & `cpg-utils-5.0.6/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/hail_batch.py` & `cpg-utils-5.0.6/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/membership.py` & `cpg-utils-5.0.6/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils/slack.py` & `cpg-utils-5.0.6/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.6/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.5
+Version: 5.0.6
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.5/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.6/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/pyproject.toml` & `cpg-utils-5.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/setup.py` & `cpg-utils-5.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.5',
+    version='5.0.6',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.5/test/test_config.py` & `cpg-utils-5.0.6/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.5/test/test_cromwell.py` & `cpg-utils-5.0.6/test/test_cromwell.py`

 * *Files identical despite different names*

