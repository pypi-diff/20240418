# Comparing `tmp/alibabacloud_dms-enterprise20181101-1.60.0.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101-1.60.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.60.0.tar", last modified: Tue Apr 16 17:16:42 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.60.1.tar", last modified: Thu Apr 18 04:31:55 2024, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101-1.60.0.tar` & `alibabacloud_dms-enterprise20181101-1.60.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/
--rw-r--r--   0 root         (0) root         (0)     8119 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2479 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1224 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   882271 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  2015708 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2479 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2668 2024-04-16 17:16:42.000000 alibabacloud_dms-enterprise20181101-1.60.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/
+-rw-r--r--   0 root         (0) root         (0)     8187 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1224 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   882527 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  2024361 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-18 04:31:55.000000 alibabacloud_dms-enterprise20181101-1.60.1/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/ChangeLog.md` & `alibabacloud_dms-enterprise20181101-1.60.1/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-16 Version: 1.60.0
+- Support API ListSensitiveColumnInfo.
+
+
 2024-03-27 Version: 1.59.1
 - Update API AddInstance: add param UseSsl.
 - Update API ModifyInstance: add param UseSsl.
 - Update API ModifyInstance: update param DatabasePassword.
 - Update API ModifyInstance: update param DatabaseUser.
 - Update API ModifyInstance: update param DbaId.
 - Update API ModifyInstance: update param EnvType.
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/LICENSE` & `alibabacloud_dms-enterprise20181101-1.60.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.60.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101
-Version: 1.60.0
+Version: 1.60.1
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/README-CN.md` & `alibabacloud_dms-enterprise20181101-1.60.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/README.md` & `alibabacloud_dms-enterprise20181101-1.60.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,14 +782,16 @@
             query['ApprovalNodePos'] = request.approval_node_pos
         if not UtilClient.is_unset(request.approval_type):
             query['ApprovalType'] = request.approval_type
         if not UtilClient.is_unset(request.comment):
             query['Comment'] = request.comment
         if not UtilClient.is_unset(request.new_approver):
             query['NewApprover'] = request.new_approver
+        if not UtilClient.is_unset(request.new_approver_list):
+            query['NewApproverList'] = request.new_approver_list
         if not UtilClient.is_unset(request.old_approver):
             query['OldApprover'] = request.old_approver
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         if not UtilClient.is_unset(request.workflow_instance_id):
             query['WorkflowInstanceId'] = request.workflow_instance_id
         req = open_api_models.OpenApiRequest(
@@ -824,14 +826,16 @@
             query['ApprovalNodePos'] = request.approval_node_pos
         if not UtilClient.is_unset(request.approval_type):
             query['ApprovalType'] = request.approval_type
         if not UtilClient.is_unset(request.comment):
             query['Comment'] = request.comment
         if not UtilClient.is_unset(request.new_approver):
             query['NewApprover'] = request.new_approver
+        if not UtilClient.is_unset(request.new_approver_list):
+            query['NewApproverList'] = request.new_approver_list
         if not UtilClient.is_unset(request.old_approver):
             query['OldApprover'] = request.old_approver
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         if not UtilClient.is_unset(request.workflow_instance_id):
             query['WorkflowInstanceId'] = request.workflow_instance_id
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2164,14 +2164,15 @@
     def __init__(
         self,
         approval_node_id: int = None,
         approval_node_pos: str = None,
         approval_type: str = None,
         comment: str = None,
         new_approver: int = None,
+        new_approver_list: str = None,
         old_approver: int = None,
         tid: int = None,
         workflow_instance_id: int = None,
     ):
         # If ApprovalType is set to ADD_APPROVAL_NODE, you need to specify this parameter. The ID of the user that is added as the new approval node. This node must be a user-defined approval node. You can call the ListUserDefineWorkFlowNodes operation to obtain the value of this parameter.
         self.approval_node_id = approval_node_id
         # If ApprovalType is set to ADD_APPROVAL_NODE, you need to specify this parameter. The position of the new approval node. Valid values:
@@ -2187,14 +2188,15 @@
         # *   **TRANSFER**\
         # *   **ADD_APPROVAL_NODE**\
         self.approval_type = approval_type
         # The description of the ticket.
         self.comment = comment
         # The ID of the user to which the ticket is transferred. If ApprovalType is set to TRANSFER, you need to specify this parameter.
         self.new_approver = new_approver
+        self.new_approver_list = new_approver_list
         # The ID of the user that transfers the ticket to another user. The default value is the ID of the current user. If the current user is an administrator or a database administrator (DBA), the user can change the value of this parameter to the ID of another user.
         self.old_approver = old_approver
         # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
         # The ID of the approval process. You can call the [GetOrderBaseInfo](~~144642~~) operation to obtain the ID of the approval process.
         self.workflow_instance_id = workflow_instance_id
 
@@ -2213,14 +2215,16 @@
             result['ApprovalNodePos'] = self.approval_node_pos
         if self.approval_type is not None:
             result['ApprovalType'] = self.approval_type
         if self.comment is not None:
             result['Comment'] = self.comment
         if self.new_approver is not None:
             result['NewApprover'] = self.new_approver
+        if self.new_approver_list is not None:
+            result['NewApproverList'] = self.new_approver_list
         if self.old_approver is not None:
             result['OldApprover'] = self.old_approver
         if self.tid is not None:
             result['Tid'] = self.tid
         if self.workflow_instance_id is not None:
             result['WorkflowInstanceId'] = self.workflow_instance_id
         return result
@@ -2233,14 +2237,16 @@
             self.approval_node_pos = m.get('ApprovalNodePos')
         if m.get('ApprovalType') is not None:
             self.approval_type = m.get('ApprovalType')
         if m.get('Comment') is not None:
             self.comment = m.get('Comment')
         if m.get('NewApprover') is not None:
             self.new_approver = m.get('NewApprover')
+        if m.get('NewApproverList') is not None:
+            self.new_approver_list = m.get('NewApproverList')
         if m.get('OldApprover') is not None:
             self.old_approver = m.get('OldApprover')
         if m.get('Tid') is not None:
             self.tid = m.get('Tid')
         if m.get('WorkflowInstanceId') is not None:
             self.workflow_instance_id = m.get('WorkflowInstanceId')
         return self
@@ -16622,14 +16628,202 @@
         if m.get('OrderId') is not None:
             self.order_id = m.get('OrderId')
         if m.get('Tid') is not None:
             self.tid = m.get('Tid')
         return self
 
 
+class GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailCronExtConfig(TeaModel):
+    def __init__(
+        self,
+        current_clear_task_count: int = None,
+        optimize_table_after_every_clear_times: int = None,
+    ):
+        self.current_clear_task_count = current_clear_task_count
+        self.optimize_table_after_every_clear_times = optimize_table_after_every_clear_times
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.current_clear_task_count is not None:
+            result['CurrentClearTaskCount'] = self.current_clear_task_count
+        if self.optimize_table_after_every_clear_times is not None:
+            result['OptimizeTableAfterEveryClearTimes'] = self.optimize_table_after_every_clear_times
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CurrentClearTaskCount') is not None:
+            self.current_clear_task_count = m.get('CurrentClearTaskCount')
+        if m.get('OptimizeTableAfterEveryClearTimes') is not None:
+            self.optimize_table_after_every_clear_times = m.get('OptimizeTableAfterEveryClearTimes')
+        return self
+
+
+class GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailImportExtConfig(TeaModel):
+    def __init__(
+        self,
+        csv_first_row_is_column_def: bool = None,
+        ignore_error: bool = None,
+        import_mode: str = None,
+        insert_type: str = None,
+    ):
+        self.csv_first_row_is_column_def = csv_first_row_is_column_def
+        self.ignore_error = ignore_error
+        self.import_mode = import_mode
+        self.insert_type = insert_type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.csv_first_row_is_column_def is not None:
+            result['CsvFirstRowIsColumnDef'] = self.csv_first_row_is_column_def
+        if self.ignore_error is not None:
+            result['IgnoreError'] = self.ignore_error
+        if self.import_mode is not None:
+            result['ImportMode'] = self.import_mode
+        if self.insert_type is not None:
+            result['InsertType'] = self.insert_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CsvFirstRowIsColumnDef') is not None:
+            self.csv_first_row_is_column_def = m.get('CsvFirstRowIsColumnDef')
+        if m.get('IgnoreError') is not None:
+            self.ignore_error = m.get('IgnoreError')
+        if m.get('ImportMode') is not None:
+            self.import_mode = m.get('ImportMode')
+        if m.get('InsertType') is not None:
+            self.insert_type = m.get('InsertType')
+        return self
+
+
+class GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetail(TeaModel):
+    def __init__(
+        self,
+        cron: bool = None,
+        cron_call_times: int = None,
+        cron_ext_config: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailCronExtConfig = None,
+        cron_format: str = None,
+        cron_last_call_start_time: str = None,
+        cron_next_call_time: str = None,
+        cron_status: str = None,
+        csv_table_name: str = None,
+        current_task_id: int = None,
+        detail_type: str = None,
+        duration: int = None,
+        file_encoding: str = None,
+        file_type: str = None,
+        import_ext_config: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailImportExtConfig = None,
+    ):
+        self.cron = cron
+        self.cron_call_times = cron_call_times
+        self.cron_ext_config = cron_ext_config
+        self.cron_format = cron_format
+        self.cron_last_call_start_time = cron_last_call_start_time
+        self.cron_next_call_time = cron_next_call_time
+        self.cron_status = cron_status
+        self.csv_table_name = csv_table_name
+        self.current_task_id = current_task_id
+        self.detail_type = detail_type
+        self.duration = duration
+        self.file_encoding = file_encoding
+        self.file_type = file_type
+        self.import_ext_config = import_ext_config
+
+    def validate(self):
+        if self.cron_ext_config:
+            self.cron_ext_config.validate()
+        if self.import_ext_config:
+            self.import_ext_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cron is not None:
+            result['Cron'] = self.cron
+        if self.cron_call_times is not None:
+            result['CronCallTimes'] = self.cron_call_times
+        if self.cron_ext_config is not None:
+            result['CronExtConfig'] = self.cron_ext_config.to_map()
+        if self.cron_format is not None:
+            result['CronFormat'] = self.cron_format
+        if self.cron_last_call_start_time is not None:
+            result['CronLastCallStartTime'] = self.cron_last_call_start_time
+        if self.cron_next_call_time is not None:
+            result['CronNextCallTime'] = self.cron_next_call_time
+        if self.cron_status is not None:
+            result['CronStatus'] = self.cron_status
+        if self.csv_table_name is not None:
+            result['CsvTableName'] = self.csv_table_name
+        if self.current_task_id is not None:
+            result['CurrentTaskId'] = self.current_task_id
+        if self.detail_type is not None:
+            result['DetailType'] = self.detail_type
+        if self.duration is not None:
+            result['Duration'] = self.duration
+        if self.file_encoding is not None:
+            result['FileEncoding'] = self.file_encoding
+        if self.file_type is not None:
+            result['FileType'] = self.file_type
+        if self.import_ext_config is not None:
+            result['ImportExtConfig'] = self.import_ext_config.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Cron') is not None:
+            self.cron = m.get('Cron')
+        if m.get('CronCallTimes') is not None:
+            self.cron_call_times = m.get('CronCallTimes')
+        if m.get('CronExtConfig') is not None:
+            temp_model = GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailCronExtConfig()
+            self.cron_ext_config = temp_model.from_map(m['CronExtConfig'])
+        if m.get('CronFormat') is not None:
+            self.cron_format = m.get('CronFormat')
+        if m.get('CronLastCallStartTime') is not None:
+            self.cron_last_call_start_time = m.get('CronLastCallStartTime')
+        if m.get('CronNextCallTime') is not None:
+            self.cron_next_call_time = m.get('CronNextCallTime')
+        if m.get('CronStatus') is not None:
+            self.cron_status = m.get('CronStatus')
+        if m.get('CsvTableName') is not None:
+            self.csv_table_name = m.get('CsvTableName')
+        if m.get('CurrentTaskId') is not None:
+            self.current_task_id = m.get('CurrentTaskId')
+        if m.get('DetailType') is not None:
+            self.detail_type = m.get('DetailType')
+        if m.get('Duration') is not None:
+            self.duration = m.get('Duration')
+        if m.get('FileEncoding') is not None:
+            self.file_encoding = m.get('FileEncoding')
+        if m.get('FileType') is not None:
+            self.file_type = m.get('FileType')
+        if m.get('ImportExtConfig') is not None:
+            temp_model = GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetailImportExtConfig()
+            self.import_ext_config = temp_model.from_map(m['ImportExtConfig'])
+        return self
+
+
 class GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailDatabaseListDatabase(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         db_type: str = None,
         env_type: str = None,
         logic: bool = None,
@@ -16922,20 +17116,22 @@
                 self.task_check_do.append(temp_model.from_map(k))
         return self
 
 
 class GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetail(TeaModel):
     def __init__(
         self,
+        config_detail: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetail = None,
         database_list: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailDatabaseList = None,
         exec_mode: str = None,
         order_detail: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailOrderDetail = None,
         pre_check_detail: GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailPreCheckDetail = None,
         status: str = None,
     ):
+        self.config_detail = config_detail
         # The information about the database in which data is changed.
         self.database_list = database_list
         # The execution mode of the ticket after the ticket is approved. Valid values:
         # 
         # - **COMMITOR**: The data change is performed by the user who submits the ticket.
         # - **AUTO**: The data change is automatically performed after the ticket is approved.
         # - **LAST_AUDITOR**: The data change is performed by the last approver of the ticket.
@@ -16956,41 +17152,48 @@
         # - **waiting**: The ticket is submitted and waits to be scheduled.
         # - **processing**: The ticket is being executed.
         # - **success**: The ticket is executed.
         # - **closed**: The ticket is closed.
         self.status = status
 
     def validate(self):
+        if self.config_detail:
+            self.config_detail.validate()
         if self.database_list:
             self.database_list.validate()
         if self.order_detail:
             self.order_detail.validate()
         if self.pre_check_detail:
             self.pre_check_detail.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.config_detail is not None:
+            result['ConfigDetail'] = self.config_detail.to_map()
         if self.database_list is not None:
             result['DatabaseList'] = self.database_list.to_map()
         if self.exec_mode is not None:
             result['ExecMode'] = self.exec_mode
         if self.order_detail is not None:
             result['OrderDetail'] = self.order_detail.to_map()
         if self.pre_check_detail is not None:
             result['PreCheckDetail'] = self.pre_check_detail.to_map()
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('ConfigDetail') is not None:
+            temp_model = GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailConfigDetail()
+            self.config_detail = temp_model.from_map(m['ConfigDetail'])
         if m.get('DatabaseList') is not None:
             temp_model = GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailDatabaseList()
             self.database_list = temp_model.from_map(m['DatabaseList'])
         if m.get('ExecMode') is not None:
             self.exec_mode = m.get('ExecMode')
         if m.get('OrderDetail') is not None:
             temp_model = GetDataCorrectOrderDetailResponseBodyDataCorrectOrderDetailOrderDetail()
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.60.1/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101
-Version: 1.60.0
+Version: 1.60.1
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.60.0/setup.py` & `alibabacloud_dms-enterprise20181101-1.60.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101.
 
-Created on 16/04/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python"
```

