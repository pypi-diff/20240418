# Comparing `tmp/shipyard_googlesheets-0.2.0a0.tar.gz` & `tmp/shipyard_googlesheets-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_googlesheets-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_googlesheets-0.2.0a1.tar", max compression
```

## Comparing `shipyard_googlesheets-0.2.0a0.tar` & `shipyard_googlesheets-0.2.0a1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-26 19:00:30.088676 shipyard_googlesheets-0.2.0a0/README.md
--rw-r--r--   0        0        0      621 2024-03-28 03:57:10.868317 shipyard_googlesheets-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-12 18:48:21.832867 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436611 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/__init__.py
--rw-r--r--   0        0        0      619 2024-03-28 03:55:30.378620 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/authtest.py
--rw-r--r--   0        0        0     3332 2024-03-28 03:55:30.373405 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/clear_data.py
--rw-r--r--   0        0        0     4302 2024-03-28 03:57:27.411601 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/download.py
--rw-r--r--   0        0        0     5205 2024-03-28 03:57:27.419196 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/upload.py
--rw-r--r--   0        0        0     1238 2024-03-28 03:22:12.044908 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/googlesheets.py
--rw-r--r--   0        0        0     5075 2024-03-28 03:57:27.429937 shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/utils.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 shipyard_googlesheets-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 19:00:30.088676 shipyard_googlesheets-0.2.0a1/README.md
+-rw-r--r--   0        0        0      621 2024-04-18 15:52:18.859561 shipyard_googlesheets-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-12 18:48:21.832867 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436611 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/__init__.py
+-rw-r--r--   0        0        0      619 2024-04-17 14:16:05.060075 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/authtest.py
+-rw-r--r--   0        0        0     3702 2024-04-18 15:52:06.157346 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/clear_data.py
+-rw-r--r--   0        0        0     4814 2024-04-18 15:32:57.785255 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/download.py
+-rw-r--r--   0        0        0     5715 2024-04-18 15:52:06.173180 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/upload.py
+-rw-r--r--   0        0        0      538 2024-04-17 22:49:13.749017 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/exceptions.py
+-rw-r--r--   0        0        0     1238 2024-04-17 14:16:05.061443 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/googlesheets.py
+-rw-r--r--   0        0        0     5076 2024-04-18 15:52:06.167455 shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/utils.py
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 shipyard_googlesheets-0.2.0a1/PKG-INFO
```

### Comparing `shipyard_googlesheets-0.2.0a0/pyproject.toml` & `shipyard_googlesheets-0.2.0a1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-googlesheets"
-version = "0.2.0a0"
+version = "0.2.0a1"
 description = "A local client for connecting and working with Google Sheets"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_googlesheets"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/authtest.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/clear_data.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/clear_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 import json
 import os
 import socket
+import sys
 
 from shipyard_bp_utils import files as shipyard
-from shipyard_templates import ShipyardLogger
-
+from shipyard_templates import ShipyardLogger, ExitCodeException, Spreadsheets
+from shipyard_googlesheets import exceptions
 from shipyard_googlesheets import utils
 
 logger = ShipyardLogger.get_logger()
 
 socket.setdefaulttimeout(600)
 
 
@@ -61,54 +62,60 @@
     except Exception as e:
         if hasattr(e, "content"):
             err_msg = json.loads(e.content)
             logger.error(
                 f"Failed to clear spreadsheet. Response from Google {file_name}: {err_msg}"
             )
         else:
-            logger.errpr(f"Failed to clear spreadsheet {file_name}")
+            logger.error(f"Failed to clear spreadsheet {file_name}")
         raise e
 
     logger.info(f"{file_name} successfully cleared between range {cell_range}.")
 
 
 def main():
-    args = get_args()
-    tmp_file = utils.set_environment_variables(args)
-    file_name = shipyard.clean_folder_name(args.file_name)
-    tab_name = args.tab_name
-    cell_range = args.cell_range or "A1:ZZZ5000000"
-    drive = args.drive
-
-    if tmp_file:
-        service, drive_service = utils.get_service(credentials=tmp_file)
-    else:
-        service, drive_service = utils.get_service(
-            credentials=args.gcp_application_credentials
-        )
+    try:
+        args = get_args()
+        tmp_file = utils.set_environment_variables(args)
+        file_name = shipyard.clean_folder_name(args.file_name)
+        tab_name = args.tab_name
+        cell_range = args.cell_range or "A1:ZZZ5000000"
+        drive = args.drive
 
-    spreadsheet_id = utils.get_spreadsheet_id_by_name(
-        drive_service=drive_service, file_name=file_name, drive=drive
-    )
-    if not spreadsheet_id:
-        if len(file_name) >= 44:
-            spreadsheet_id = file_name
+        if tmp_file:
+            service, drive_service = utils.get_service(credentials=tmp_file)
         else:
-            logger.error(f"The spreadsheet {file_name} does not exist")
-            raise SystemExit(1)
+            service, drive_service = utils.get_service(
+                credentials=args.gcp_application_credentials
+            )
 
-    # check if workbook exists in the spreadsheet
-    clear_google_sheet(
-        service=service,
-        file_name=file_name,
-        spreadsheet_id=spreadsheet_id,
-        tab_name=tab_name,
-        cell_range=cell_range,
-    )
+        spreadsheet_id = utils.get_spreadsheet_id_by_name(
+            drive_service=drive_service, file_name=file_name, drive=drive
+        )
+        if not spreadsheet_id:
+            if len(file_name) >= 44:
+                spreadsheet_id = file_name
+            else:
+                raise exceptions.InvalidSheetError(file_name)
+
+        # check if workbook exists in the spreadsheet
+        clear_google_sheet(
+            service=service,
+            file_name=file_name,
+            spreadsheet_id=spreadsheet_id,
+            tab_name=tab_name,
+            cell_range=cell_range,
+        )
 
-    if tmp_file:
-        logger.info(f"Removing temporary credentials file {tmp_file}")
-        os.remove(tmp_file)
+        if tmp_file:
+            logger.info(f"Removing temporary credentials file {tmp_file}")
+            os.remove(tmp_file)
+    except ExitCodeException as e:
+        logger.error(e)
+        sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(e)
+        sys.exit(Spreadsheets.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/download.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import csv
 import os
+import sys
 
 from shipyard_bp_utils import files as shipyard
-from shipyard_templates import ShipyardLogger
+from shipyard_templates import ShipyardLogger, Spreadsheets, ExitCodeException
 
+from shipyard_googlesheets import exceptions
 from shipyard_googlesheets import utils
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
@@ -38,30 +40,30 @@
         required=True,
     )
     parser.add_argument("--drive", dest="drive", default=None, required=False)
     return parser.parse_args()
 
 
 def download_google_sheet_file(
-    service, spreadsheet_id, file_name, tab_name, cell_range, destination_file_name=None
+        service, spreadsheet_id, file_name, tab_name, cell_range, destination_file_name=None
 ):
     """
     Download th contents of a spreadsheet from Google Sheets to local storage in
     the current working directory.
     """
     local_path = os.path.normpath(f"{os.getcwd()}/{destination_file_name}")
     try:
         if tab_name:
             if utils.check_workbook_exists(
-                service=service, spreadsheet_id=spreadsheet_id, tab_name=tab_name
+                    service=service, spreadsheet_id=spreadsheet_id, tab_name=tab_name
             ):
                 cell_range = f"{tab_name}!{cell_range}"
             else:
-                print(f"The tab {tab_name} could not be found")
-                raise SystemExit(1)
+                raise exceptions.TabNotFoundError(tab_name)
+
         sheet = (
             service.spreadsheets()
             .values()
             .get(spreadsheetId=spreadsheet_id, range=cell_range)
             .execute()
         )
 
@@ -76,63 +78,71 @@
         logger.info(f"Successfully downloaded {file_name} - {tab_name} to {local_path}")
     except Exception as e:
         logger.error(f"Failed to download {file_name} from Google Sheets")
         raise e
 
 
 def main():
-    args = get_args()
-    tmp_file = utils.set_environment_variables(args)
-    file_name = shipyard.clean_folder_name(args.file_name)
-    tab_name = args.tab_name
-    cell_range = args.cell_range or "A1:ZZZ5000000"
-    drive = args.drive
-
-    destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
-    if not os.path.exists(destination_folder_name) and (destination_folder_name != ""):
-        os.makedirs(destination_folder_name)
-
-    if tmp_file:
-        service, drive_service = utils.get_service(credentials=tmp_file)
-    else:
-        service, drive_service = utils.get_service(
-            credentials=args.gcp_application_credentials
-        )
+    try:
+        args = get_args()
+        tmp_file = utils.set_environment_variables(args)
+        file_name = shipyard.clean_folder_name(args.file_name)
+        tab_name = args.tab_name
+        cell_range = args.cell_range or "A1:ZZZ5000000"
+        drive = args.drive
+
+        destination_folder_name = shipyard.clean_folder_name(args.destination_folder_name)
+        if not os.path.exists(destination_folder_name) and (destination_folder_name != ""):
+            os.makedirs(destination_folder_name)
 
-    spreadsheet_id = utils.get_spreadsheet_id_by_name(
-        drive_service=drive_service, file_name=file_name, drive=drive
-    )
-    if not spreadsheet_id:
-        if len(file_name) >= 44:
-            spreadsheet_id = file_name
+        if tmp_file:
+            service, drive_service = utils.get_service(credentials=tmp_file)
         else:
-            logger.error(f"Sheet {file_name} does not exist")
-            raise SystemExit(1)
+            service, drive_service = utils.get_service(
+                credentials=args.gcp_application_credentials
+            )
 
-    if not args.destination_file_name:
-        args.destination_file_name = f"{file_name} - {tab_name}.csv"
+        spreadsheet_id = utils.get_spreadsheet_id_by_name(
+            drive_service=drive_service, file_name=file_name, drive=drive
+        )
+        if not spreadsheet_id:
+            if len(file_name) >= 44:
+                spreadsheet_id = file_name
+            else:
+                raise exceptions.InvalidSheetError(file_name)
 
-    destination_name = shipyard.combine_folder_and_file_name(
-        destination_folder_name, args.destination_file_name
-    )
+        if not args.destination_file_name:
+            args.destination_file_name = f"{file_name} - {tab_name}.csv"
 
-    if len(destination_name.rsplit("/", 1)) > 1:
-        path = destination_name.rsplit("/", 1)[0]
-        if not os.path.exists(path):
-            os.makedirs(path)
-
-    download_google_sheet_file(
-        service=service,
-        tab_name=tab_name,
-        spreadsheet_id=spreadsheet_id,
-        file_name=file_name,
-        cell_range=cell_range,
-        destination_file_name=destination_name,
-    )
+        destination_name = shipyard.combine_folder_and_file_name(
+            destination_folder_name, args.destination_file_name
+        )
 
-    if tmp_file:
-        logger.info(f"Removing temporary credentials file {tmp_file}")
-        os.remove(tmp_file)
+        if len(destination_name.rsplit("/", 1)) > 1:
+            path = destination_name.rsplit("/", 1)[0]
+            if not os.path.exists(path):
+                os.makedirs(path)
+
+        download_google_sheet_file(
+            service=service,
+            tab_name=tab_name,
+            spreadsheet_id=spreadsheet_id,
+            file_name=file_name,
+            cell_range=cell_range,
+            destination_file_name=destination_name,
+        )
+        if tmp_file:
+            logger.info(f"Removing temporary credentials file {tmp_file}")
+            os.remove(tmp_file)
+    except FileNotFoundError as e:
+        logger.error(e)
+        sys.exit(Spreadsheets.EXIT_CODE_FILE_NOT_FOUND)
+    except ExitCodeException as e:
+        logger.error(e)
+        sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(e)
+        sys.exit(Spreadsheets.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/cli/upload.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/cli/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import argparse
 import csv
 import json
 import os
 import socket
+import sys
 
 from shipyard_bp_utils import files as shipyard
-from shipyard_templates import ShipyardLogger
+from shipyard_templates import ShipyardLogger, Spreadsheets, ExitCodeException
 
-from shipyard_googlesheets import utils
+from shipyard_googlesheets import utils, exceptions
 
 logger = ShipyardLogger.get_logger()
 
 socket.setdefaulttimeout(600)
 
 
 def get_args():
@@ -34,15 +35,15 @@
         required=True,
     )
     parser.add_argument("--drive", dest="drive", default=None, required=False)
     return parser.parse_args()
 
 
 def upload_google_sheets_file(
-    service, file_name, source_full_path, starting_cell, spreadsheet_id, tab_name
+        service, file_name, source_full_path, starting_cell, spreadsheet_id, tab_name
 ):
     """
     Uploads a single file to Google Sheets.
     """
     try:
         if not spreadsheet_id:
             file_metadata = {
@@ -63,15 +64,15 @@
         if not workbook_exists:
             utils.add_workbook(
                 service=service, spreadsheet_id=spreadsheet_id, tab_name=tab_name
             )
 
         data = []
         with open(
-            source_full_path, encoding="utf-8", newline=""
+                source_full_path, encoding="utf-8", newline=""
         ) as f:  # adding unicode encoding
             reader = csv.reader((line.replace("\0", "") for line in f), delimiter=",")
             data.extend(row for row in reader if set(row) != {""})
         _range = f"{starting_cell}:ZZZ5000000" if starting_cell else "A1:ZZZ5000000"
         if tab_name:
             _range = f"{tab_name}!{_range}"
 
@@ -101,57 +102,64 @@
             )
         raise e
 
     logger.info(f"{source_full_path} successfully uploaded to {file_name}")
 
 
 def main():
-    args = get_args()
-    tmp_file = utils.set_environment_variables(args)
-    source_file_name = args.source_file_name
-    source_folder_name = args.source_folder_name
-    source_full_path = shipyard.combine_folder_and_file_name(
-        folder_name=f"{os.getcwd()}/{source_folder_name}", file_name=source_file_name
-    )
-    file_name = shipyard.clean_folder_name(args.file_name)
-    tab_name = args.tab_name
-    starting_cell = args.starting_cell or "A1"
-    drive = args.drive
-
-    if not os.path.isfile(source_full_path):
-        logger.error(f"{source_full_path} does not exist")
-        raise SystemExit(1)
-
-    if tmp_file:
-        service, drive_service = utils.get_service(credentials=tmp_file)
-    else:
-        service, drive_service = utils.get_service(
-            credentials=args.gcp_application_credentials
+    try:
+        args = get_args()
+        tmp_file = utils.set_environment_variables(args)
+        source_file_name = args.source_file_name
+        source_folder_name = args.source_folder_name
+        source_full_path = shipyard.combine_folder_and_file_name(
+            folder_name=f"{os.getcwd()}/{source_folder_name}", file_name=source_file_name
         )
+        file_name = shipyard.clean_folder_name(args.file_name)
+        tab_name = args.tab_name
+        starting_cell = args.starting_cell or "A1"
+        drive = args.drive
 
-    spreadsheet_id = utils.get_spreadsheet_id_by_name(
-        drive_service=drive_service, file_name=file_name, drive=drive
-    )
-    if not spreadsheet_id:
-        if len(file_name) >= 44:
-            spreadsheet_id = file_name
-        else:
-            logger.error(f"The spreadsheet {file_name} does not exist")
-            raise SystemExit(1)
+        if not os.path.isfile(source_full_path):
+            raise FileNotFoundError(f"{source_full_path} does not exist")
 
-    # check if workbook exists in the spreadsheet
-    upload_google_sheets_file(
-        service=service,
-        file_name=file_name,
-        source_full_path=source_full_path,
-        spreadsheet_id=spreadsheet_id,
-        tab_name=tab_name,
-        starting_cell=starting_cell,
-    )
+        if tmp_file:
+            service, drive_service = utils.get_service(credentials=tmp_file)
+        else:
+            service, drive_service = utils.get_service(
+                credentials=args.gcp_application_credentials
+            )
 
-    if tmp_file:
-        logger.info(f"Removing temporary credentials file {tmp_file}")
-        os.remove(tmp_file)
+        spreadsheet_id = utils.get_spreadsheet_id_by_name(
+            drive_service=drive_service, file_name=file_name, drive=drive
+        )
+        if not spreadsheet_id:
+            if len(file_name) >= 44:
+                spreadsheet_id = file_name
+            else:
+                raise exceptions.InvalidSheetError(file_name)
+
+        # check if workbook exists in the spreadsheet
+        upload_google_sheets_file(
+            service=service,
+            file_name=file_name,
+            source_full_path=source_full_path,
+            spreadsheet_id=spreadsheet_id,
+            tab_name=tab_name,
+            starting_cell=starting_cell,
+        )
+        if tmp_file:
+            logger.info(f"Removing temporary credentials file {tmp_file}")
+            os.remove(tmp_file)
+    except FileNotFoundError as e:
+        logger.error(e)
+        sys.exit(Spreadsheets.EXIT_CODE_FILE_NOT_FOUND)
+    except ExitCodeException as e:
+        logger.error(e)
+        sys.exit(e.exit_code)
+    except Exception as e:
+        logger.error(f"An unexpected error occurred\n{e}")
+        sys.exit(Spreadsheets.EXIT_CODE_UNKNOWN_ERROR)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/googlesheets.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/googlesheets.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlesheets-0.2.0a0/shipyard_googlesheets/utils.py` & `shipyard_googlesheets-0.2.0a1/shipyard_googlesheets/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     try:
         spreadsheet = service.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
         sheets = spreadsheet["sheets"]
         exists = [True for sheet in sheets if sheet["properties"]["title"] == tab_name]
         logger.debug(f"exists: {exists}")
         return bool(exists)
     except Exception as e:
+
         logger.error(
             f"Failed to check workbook {tab_name} for spreadsheet " f"{spreadsheet_id}"
         )
         raise e
 
 
 def get_spreadsheet_id_by_name(drive_service, file_name, drive):
```

### Comparing `shipyard_googlesheets-0.2.0a0/PKG-INFO` & `shipyard_googlesheets-0.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-googlesheets
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: A local client for connecting and working with Google Sheets
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

