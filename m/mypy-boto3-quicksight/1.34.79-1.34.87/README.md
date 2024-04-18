# Comparing `tmp/mypy-boto3-quicksight-1.34.79.tar.gz` & `tmp/mypy_boto3_quicksight-1.34.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.34.79.tar", last modified: Fri Apr  5 19:20:34 2024, max compression
+gzip compressed data, was "mypy_boto3_quicksight-1.34.87.tar", last modified: Thu Apr 18 19:34:22 2024, max compression
```

## Comparing `mypy-boto3-quicksight-1.34.79.tar` & `mypy_boto3_quicksight-1.34.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.730695 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   135091 2024-04-05 19:20:11.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   135088 2024-04-05 19:20:08.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    39673 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    39673 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-04-05 19:20:12.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-05 19:20:11.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   381664 2024-04-05 19:20:19.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   381664 2024-04-05 19:20:17.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 19:20:34.000000 mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:20:34.734695 mypy-boto3-quicksight-1.34.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-05 19:20:07.000000 mypy-boto3-quicksight-1.34.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135105 2024-04-18 19:33:31.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135102 2024-04-18 19:33:31.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    39714 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39714 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   386207 2024-04-18 19:33:42.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   386207 2024-04-18 19:33:36.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/setup.py
```

### Comparing `mypy-boto3-quicksight-1.34.79/LICENSE` & `mypy_boto3_quicksight-1.34.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/PKG-INFO` & `mypy_boto3_quicksight-1.34.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.79
-Summary: Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.79/README.md` & `mypy_boto3_quicksight-1.34.87/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.py` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/__init__.pyi` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.py` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2082,15 +2082,15 @@
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
         SnapshotConfiguration: SnapshotConfigurationTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
-        Starts an asynchronous job that generates a dashboard snapshot.
+        Starts an asynchronous job that generates a snapshot of a dashboard's output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
 
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/client.pyi` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2079,15 +2079,15 @@
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
         SnapshotConfiguration: SnapshotConfigurationTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
-        Starts an asynchronous job that generates a dashboard snapshot.
+        Starts an asynchronous job that generates a snapshot of a dashboard's output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
 
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.py` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,15 @@
     "Domain",
     "Host",
     "InstanceId",
     "ManifestFileLocation",
     "Name",
     "Password",
     "Port",
+    "ProductType",
     "RoleArn",
     "SecretArn",
     "Username",
     "Warehouse",
     "WorkGroup",
 ]
 AssetBundleExportJobRefreshSchedulePropertyToOverrideType = Literal["StartAfterDateTime"]
@@ -954,14 +955,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/literals.pyi` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,15 @@
     "Domain",
     "Host",
     "InstanceId",
     "ManifestFileLocation",
     "Name",
     "Password",
     "Port",
+    "ProductType",
     "RoleArn",
     "SecretArn",
     "Username",
     "Warehouse",
     "WorkGroup",
 ]
 AssetBundleExportJobRefreshSchedulePropertyToOverrideType = Literal["StartAfterDateTime"]
@@ -954,14 +955,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.py` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/paginator.pyi` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.py` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
+    "AssetBundleImportJobWarningTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
     "AuthorizedTargetsByServiceTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
@@ -390,14 +391,15 @@
     "DataSourceSummaryTypeDef",
     "RollingDateConfigurationTypeDef",
     "MappedDataSetParameterTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterTypeDef",
+    "FilterSelectableValuesTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteDataSetRefreshPropertiesRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -473,15 +475,14 @@
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
-    "FilterSelectableValuesTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
@@ -840,15 +841,14 @@
     "DashboardVisualPublishOptionsTypeDef",
     "TableInlineVisualizationTypeDef",
     "DataLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
-    "TimeEqualityFilterTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterTypeDef",
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     "DescribeFolderResolvedPermissionsRequestDescribeFolderResolvedPermissionsPaginateTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
@@ -883,15 +883,14 @@
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
-    "RelativeDatesFilterTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "SearchFoldersRequestSearchFoldersPaginateTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
     "TypographyTypeDef",
@@ -965,15 +964,14 @@
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
     "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
     "AssetBundleImportJobOverrideTagsTypeDef",
     "NumericAxisOptionsTypeDef",
-    "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
     "UpdateDashboardPermissionsResponseTypeDef",
@@ -991,15 +989,14 @@
     "ForecastScenarioTypeDef",
     "CustomContentConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "DataPathColorTypeDef",
     "DataPathSortTypeDef",
     "PivotTableDataPathOptionTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
-    "TimeRangeFilterTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
@@ -1038,14 +1035,15 @@
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupTypeDef",
+    "FilterCrossSheetControlTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
@@ -1085,16 +1083,14 @@
     "SeriesItemTypeDef",
     "ThemeConfigurationTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
-    "NumericEqualityFilterTypeDef",
-    "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterTypeDef",
     "DataSourcePaginatorTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
     "DataSourceTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
@@ -1111,25 +1107,32 @@
     "DescribeDashboardResponseTypeDef",
     "TemplateTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "LogicalTableTypeDef",
     "ColumnHierarchyTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "AxisDisplayOptionsTypeDef",
+    "DefaultDateTimePickerControlOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "DefaultFilterDropDownControlOptionsTypeDef",
     "FilterDropDownControlTypeDef",
     "ParameterDropDownControlTypeDef",
+    "DefaultFilterListControlOptionsTypeDef",
     "FilterListControlTypeDef",
     "ParameterListControlTypeDef",
+    "DefaultRelativeDateTimeControlOptionsTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
+    "DefaultSliderControlOptionsTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
+    "DefaultTextAreaControlOptionsTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
+    "DefaultTextFieldControlOptionsTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
     "PivotTableOptionsTypeDef",
     "PivotTotalOptionsTypeDef",
     "SubtotalOptionsTypeDef",
@@ -1151,15 +1154,14 @@
     "ThemeVersionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
-    "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
     "DatasetMetadataTypeDef",
     "ListDataSourcesResponsePaginatorTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
@@ -1174,14 +1176,15 @@
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "CustomActionSetParametersOperationTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "DefaultFilterControlOptionsTypeDef",
     "FilterControlTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
     "PivotTableTotalOptionsTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
@@ -1194,15 +1197,14 @@
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
-    "FilterTypeDef",
     "BarChartSortConfigurationTypeDef",
     "BoxPlotSortConfigurationTypeDef",
     "ComboChartSortConfigurationTypeDef",
     "FilledMapSortConfigurationTypeDef",
     "FunnelChartSortConfigurationTypeDef",
     "HeatMapSortConfigurationTypeDef",
     "KPISortConfigurationTypeDef",
@@ -1223,36 +1225,43 @@
     "UpdateDataSourceRequestRequestTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "DefaultFilterControlConfigurationTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
-    "FilterGroupTypeDef",
     "PivotTableSortConfigurationTypeDef",
     "TooltipOptionsTypeDef",
     "CreateTopicRequestRequestTypeDef",
     "DescribeTopicResponseTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationTypeDef",
     "VisualCustomActionTypeDef",
+    "CategoryFilterTypeDef",
+    "NumericEqualityFilterTypeDef",
+    "NumericRangeFilterTypeDef",
+    "RelativeDatesFilterTypeDef",
+    "TimeEqualityFilterTypeDef",
+    "TimeRangeFilterTypeDef",
+    "TopBottomFilterTypeDef",
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
     "UniqueValuesComputationTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
@@ -1284,14 +1293,15 @@
     "TreeMapAggregatedFieldWellsTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
+    "FilterTypeDef",
     "BarChartFieldWellsTypeDef",
     "BoxPlotFieldWellsTypeDef",
     "ComboChartFieldWellsTypeDef",
     "FilledMapFieldWellsTypeDef",
     "FunnelChartFieldWellsTypeDef",
     "GaugeChartConfigurationTypeDef",
     "GeospatialMapFieldWellsTypeDef",
@@ -1306,14 +1316,15 @@
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
     "TreeMapFieldWellsTypeDef",
     "WaterfallChartFieldWellsTypeDef",
     "WordCloudFieldWellsTypeDef",
     "TableFieldWellsTypeDef",
     "LayoutConfigurationTypeDef",
+    "FilterGroupTypeDef",
     "BarChartConfigurationTypeDef",
     "BoxPlotChartConfigurationTypeDef",
     "ComboChartConfigurationTypeDef",
     "FilledMapConfigurationTypeDef",
     "FunnelChartConfigurationTypeDef",
     "GaugeChartVisualTypeDef",
     "GeospatialMapConfigurationTypeDef",
@@ -1738,14 +1749,21 @@
         "JobStatus": NotRequired[AssetBundleImportJobStatusType],
         "Arn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "AssetBundleImportJobId": NotRequired[str],
         "FailureAction": NotRequired[AssetBundleImportFailureActionType],
     },
 )
+AssetBundleImportJobWarningTypeDef = TypedDict(
+    "AssetBundleImportJobWarningTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "Message": NotRequired[str],
+    },
+)
 AssetBundleImportSourceDescriptionTypeDef = TypedDict(
     "AssetBundleImportSourceDescriptionTypeDef",
     {
         "Body": NotRequired[str],
         "S3Uri": NotRequired[str],
     },
 )
@@ -2632,14 +2650,20 @@
 DecimalParameterTypeDef = TypedDict(
     "DecimalParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[float],
     },
 )
+FilterSelectableValuesTypeDef = TypedDict(
+    "FilterSelectableValuesTypeDef",
+    {
+        "Values": NotRequired[Sequence[str]],
+    },
+)
 DeleteAccountCustomizationRequestRequestTypeDef = TypedDict(
     "DeleteAccountCustomizationRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "Namespace": NotRequired[str],
     },
 )
@@ -3281,20 +3305,14 @@
 )
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": NotRequired[BaseMapStyleTypeType],
     },
 )
-FilterSelectableValuesTypeDef = TypedDict(
-    "FilterSelectableValuesTypeDef",
-    {
-        "Values": NotRequired[Sequence[str]],
-    },
-)
 SameSheetTargetVisualConfigurationTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationTypeDef",
     {
         "TargetVisuals": NotRequired[Sequence[str]],
         "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
     },
 )
@@ -6457,25 +6475,14 @@
         "DataSourceSummaries": List[DataSourceSummaryTypeDef],
         "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TimeEqualityFilterTypeDef = TypedDict(
-    "TimeEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "Value": NotRequired[TimestampTypeDef],
-        "ParameterName": NotRequired[str],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
-    },
-)
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[TimestampTypeDef],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
         "Parameter": NotRequired[str],
     },
@@ -6830,29 +6837,14 @@
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": NotRequired[ArcOptionsTypeDef],
         "DonutCenterOptions": NotRequired[DonutCenterOptionsTypeDef],
     },
 )
-RelativeDatesFilterTypeDef = TypedDict(
-    "RelativeDatesFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "RelativeDateType": RelativeDateTypeType,
-        "NullOption": FilterNullOptionType,
-        "MinimumGranularity": NotRequired[TimeGranularityType],
-        "RelativeDateValue": NotRequired[int],
-        "ParameterName": NotRequired[str],
-        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
-    },
-)
 FilterOperationTargetVisualsConfigurationTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationTypeDef",
     {
         "SameSheetTargetVisualConfiguration": NotRequired[
             SameSheetTargetVisualConfigurationTypeDef
         ],
     },
@@ -7543,22 +7535,14 @@
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
     {
         "Scale": NotRequired[AxisScaleTypeDef],
         "Range": NotRequired[AxisDisplayRangeTypeDef],
     },
 )
-CategoryFilterTypeDef = TypedDict(
-    "CategoryFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "Configuration": CategoryFilterConfigurationTypeDef,
-    },
-)
 ClusterMarkerConfigurationTypeDef = TypedDict(
     "ClusterMarkerConfigurationTypeDef",
     {
         "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
     },
 )
 TopicCategoryFilterTypeDef = TypedDict(
@@ -7777,28 +7761,14 @@
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": NotRequired[str],
         "FieldDataPathValues": NotRequired[Sequence[DataPathValueTypeDef]],
     },
 )
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "NullOption": FilterNullOptionType,
-        "IncludeMinimum": NotRequired[bool],
-        "IncludeMaximum": NotRequired[bool],
-        "RangeMinimumValue": NotRequired[TimeRangeFilterValueTypeDef],
-        "RangeMaximumValue": NotRequired[TimeRangeFilterValueTypeDef],
-        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-    },
-)
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": NotRequired[DisplayFormatType],
         "DisplayFormatOptions": NotRequired[DisplayFormatOptionsTypeDef],
     },
 )
@@ -8224,14 +8194,22 @@
 )
 SnapshotFileGroupTypeDef = TypedDict(
     "SnapshotFileGroupTypeDef",
     {
         "Files": NotRequired[List[SnapshotFileTypeDef]],
     },
 )
+FilterCrossSheetControlTypeDef = TypedDict(
+    "FilterCrossSheetControlTypeDef",
+    {
+        "FilterControlId": str,
+        "SourceFilterId": str,
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
+    },
+)
 DateTimeParameterDeclarationTypeDef = TypedDict(
     "DateTimeParameterDeclarationTypeDef",
     {
         "Name": str,
         "DefaultValues": NotRequired[DateTimeDefaultValuesTypeDef],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationTypeDef],
@@ -8672,41 +8650,14 @@
         "Column": ColumnIdentifierTypeDef,
         "Label": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
         "Aggregation": NotRequired[AggregationFunctionTypeDef],
         "TooltipTarget": NotRequired[TooltipTargetType],
     },
 )
-NumericEqualityFilterTypeDef = TypedDict(
-    "NumericEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "MatchOperator": NumericEqualityMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-        "Value": NotRequired[float],
-        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
-        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
-        "ParameterName": NotRequired[str],
-    },
-)
-NumericRangeFilterTypeDef = TypedDict(
-    "NumericRangeFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "NullOption": FilterNullOptionType,
-        "IncludeMinimum": NotRequired[bool],
-        "IncludeMaximum": NotRequired[bool],
-        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
-        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
-        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
-        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
-    },
-)
 ReferenceLineDynamicDataConfigurationTypeDef = TypedDict(
     "ReferenceLineDynamicDataConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
         "MeasureAggregationFunction": NotRequired[AggregationFunctionTypeDef],
     },
@@ -8929,14 +8880,21 @@
         "AxisLineVisibility": NotRequired[VisibilityType],
         "GridLineVisibility": NotRequired[VisibilityType],
         "DataOptions": NotRequired[AxisDataOptionsTypeDef],
         "ScrollbarOptions": NotRequired[ScrollBarOptionsTypeDef],
         "AxisOffset": NotRequired[str],
     },
 )
+DefaultDateTimePickerControlOptionsTypeDef = TypedDict(
+    "DefaultDateTimePickerControlOptionsTypeDef",
+    {
+        "Type": NotRequired[SheetControlDateTimePickerTypeType],
+        "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
+    },
+)
 FilterDateTimePickerControlTypeDef = TypedDict(
     "FilterDateTimePickerControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
@@ -8948,14 +8906,22 @@
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
     },
 )
+DefaultFilterDropDownControlOptionsTypeDef = TypedDict(
+    "DefaultFilterDropDownControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
+    },
+)
 FilterDropDownControlTypeDef = TypedDict(
     "FilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
@@ -8972,14 +8938,22 @@
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultFilterListControlOptionsTypeDef = TypedDict(
+    "DefaultFilterListControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
+    },
+)
 FilterListControlTypeDef = TypedDict(
     "FilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
@@ -8996,23 +8970,39 @@
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultRelativeDateTimeControlOptionsTypeDef = TypedDict(
+    "DefaultRelativeDateTimeControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[RelativeDateTimeControlDisplayOptionsTypeDef],
+    },
+)
 FilterRelativeDateTimeControlTypeDef = TypedDict(
     "FilterRelativeDateTimeControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[RelativeDateTimeControlDisplayOptionsTypeDef],
     },
 )
+DefaultSliderControlOptionsTypeDef = TypedDict(
+    "DefaultSliderControlOptionsTypeDef",
+    {
+        "MaximumValue": float,
+        "MinimumValue": float,
+        "StepSize": float,
+        "DisplayOptions": NotRequired[SliderControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlSliderTypeType],
+    },
+)
 FilterSliderControlTypeDef = TypedDict(
     "FilterSliderControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "MaximumValue": float,
@@ -9030,14 +9020,21 @@
         "SourceParameterName": str,
         "MaximumValue": float,
         "MinimumValue": float,
         "StepSize": float,
         "DisplayOptions": NotRequired[SliderControlDisplayOptionsTypeDef],
     },
 )
+DefaultTextAreaControlOptionsTypeDef = TypedDict(
+    "DefaultTextAreaControlOptionsTypeDef",
+    {
+        "Delimiter": NotRequired[str],
+        "DisplayOptions": NotRequired[TextAreaControlDisplayOptionsTypeDef],
+    },
+)
 FilterTextAreaControlTypeDef = TypedDict(
     "FilterTextAreaControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "Delimiter": NotRequired[str],
@@ -9050,14 +9047,20 @@
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "Delimiter": NotRequired[str],
         "DisplayOptions": NotRequired[TextAreaControlDisplayOptionsTypeDef],
     },
 )
+DefaultTextFieldControlOptionsTypeDef = TypedDict(
+    "DefaultTextFieldControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[TextFieldControlDisplayOptionsTypeDef],
+    },
+)
 FilterTextFieldControlTypeDef = TypedDict(
     "FilterTextFieldControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[TextFieldControlDisplayOptionsTypeDef],
@@ -9305,25 +9308,14 @@
 StringFormatConfigurationTypeDef = TypedDict(
     "StringFormatConfigurationTypeDef",
     {
         "NullValueFormatConfiguration": NotRequired[NullValueFormatConfigurationTypeDef],
         "NumericFormatConfiguration": NotRequired[NumericFormatConfigurationTypeDef],
     },
 )
-TopBottomFilterTypeDef = TypedDict(
-    "TopBottomFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
-        "Limit": NotRequired[int],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-        "ParameterName": NotRequired[str],
-    },
-)
 FieldSortOptionsTypeDef = TypedDict(
     "FieldSortOptionsTypeDef",
     {
         "FieldSort": NotRequired[FieldSortTypeDef],
         "ColumnSort": NotRequired[ColumnSortTypeDef],
     },
 )
@@ -9560,24 +9552,37 @@
 LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsTypeDef",
     {
         "AxisOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "MissingDataConfigurations": NotRequired[Sequence[MissingDataConfigurationTypeDef]],
     },
 )
+DefaultFilterControlOptionsTypeDef = TypedDict(
+    "DefaultFilterControlOptionsTypeDef",
+    {
+        "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
+        "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsTypeDef],
+        "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsTypeDef],
+        "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
+        "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
+        "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
+        "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
+    },
+)
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
         "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
         "List": NotRequired[FilterListControlTypeDef],
         "Dropdown": NotRequired[FilterDropDownControlTypeDef],
         "TextField": NotRequired[FilterTextFieldControlTypeDef],
         "TextArea": NotRequired[FilterTextAreaControlTypeDef],
         "Slider": NotRequired[FilterSliderControlTypeDef],
         "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
+        "CrossSheet": NotRequired[FilterCrossSheetControlTypeDef],
     },
 )
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
         "List": NotRequired[ParameterListControlTypeDef],
@@ -9748,26 +9753,14 @@
     "FormatConfigurationTypeDef",
     {
         "StringFormatConfiguration": NotRequired[StringFormatConfigurationTypeDef],
         "NumberFormatConfiguration": NotRequired[NumberFormatConfigurationTypeDef],
         "DateTimeFormatConfiguration": NotRequired[DateTimeFormatConfigurationTypeDef],
     },
 )
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
-    {
-        "CategoryFilter": NotRequired[CategoryFilterTypeDef],
-        "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
-        "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
-        "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
-        "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
-        "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
-        "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
-    },
-)
 BarChartSortConfigurationTypeDef = TypedDict(
     "BarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
@@ -9921,14 +9914,15 @@
         "OverrideParameters": AssetBundleImportJobOverrideParametersTypeDef,
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
         "OverridePermissions": AssetBundleImportJobOverridePermissionsTypeDef,
         "OverrideTags": AssetBundleImportJobOverrideTagsTypeDef,
         "OverrideValidationStrategy": AssetBundleImportJobOverrideValidationStrategyTypeDef,
+        "Warnings": List[AssetBundleImportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
@@ -10013,14 +10007,21 @@
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DefaultFilterControlConfigurationTypeDef = TypedDict(
+    "DefaultFilterControlConfigurationTypeDef",
+    {
+        "Title": str,
+        "ControlOptions": DefaultFilterControlOptionsTypeDef,
+    },
+)
 TableFieldOptionTypeDef = TypedDict(
     "TableFieldOptionTypeDef",
     {
         "FieldId": str,
         "Width": NotRequired[str],
         "CustomLabel": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
@@ -10110,24 +10111,14 @@
     "UnaggregatedFieldTypeDef",
     {
         "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
     },
 )
-FilterGroupTypeDef = TypedDict(
-    "FilterGroupTypeDef",
-    {
-        "FilterGroupId": str,
-        "Filters": Sequence[FilterTypeDef],
-        "ScopeConfiguration": FilterScopeConfigurationTypeDef,
-        "CrossDataset": CrossDatasetTypesType,
-        "Status": NotRequired[WidgetStatusType],
-    },
-)
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": NotRequired[Sequence[PivotFieldSortOptionsTypeDef]],
     },
 )
 TooltipOptionsTypeDef = TypedDict(
@@ -10201,14 +10192,107 @@
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
         "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
         "Status": NotRequired[WidgetStatusType],
     },
 )
+CategoryFilterTypeDef = TypedDict(
+    "CategoryFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Configuration": CategoryFilterConfigurationTypeDef,
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+NumericEqualityFilterTypeDef = TypedDict(
+    "NumericEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "MatchOperator": NumericEqualityMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "Value": NotRequired[float],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+NumericRangeFilterTypeDef = TypedDict(
+    "NumericRangeFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
+        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+RelativeDatesFilterTypeDef = TypedDict(
+    "RelativeDatesFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "RelativeDateType": RelativeDateTypeType,
+        "NullOption": FilterNullOptionType,
+        "MinimumGranularity": NotRequired[TimeGranularityType],
+        "RelativeDateValue": NotRequired[int],
+        "ParameterName": NotRequired[str],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TimeEqualityFilterTypeDef = TypedDict(
+    "TimeEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Value": NotRequired[TimestampTypeDef],
+        "ParameterName": NotRequired[str],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimumValue": NotRequired[TimeRangeFilterValueTypeDef],
+        "RangeMaximumValue": NotRequired[TimeRangeFilterValueTypeDef],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TopBottomFilterTypeDef = TypedDict(
+    "TopBottomFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
+        "Limit": NotRequired[int],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[TableFieldOptionTypeDef]],
         "Order": NotRequired[Sequence[str]],
         "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsTypeDef],
     },
@@ -10537,14 +10621,26 @@
     "EmptyVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
+    {
+        "CategoryFilter": NotRequired[CategoryFilterTypeDef],
+        "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
+        "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
+        "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
+        "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
+        "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
+    },
+)
 BarChartFieldWellsTypeDef = TypedDict(
     "BarChartFieldWellsTypeDef",
     {
         "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsTypeDef],
     },
 )
 BoxPlotFieldWellsTypeDef = TypedDict(
@@ -10694,14 +10790,24 @@
     "LayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
         "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationTypeDef],
         "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationTypeDef],
     },
 )
+FilterGroupTypeDef = TypedDict(
+    "FilterGroupTypeDef",
+    {
+        "FilterGroupId": str,
+        "Filters": Sequence[FilterTypeDef],
+        "ScopeConfiguration": FilterScopeConfigurationTypeDef,
+        "CrossDataset": CrossDatasetTypesType,
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BarChartSortConfigurationTypeDef],
         "Orientation": NotRequired[BarChartOrientationType],
         "BarsArrangement": NotRequired[BarsArrangementType],
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight/type_defs.pyi` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
+    "AssetBundleImportJobWarningTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
     "AuthorizedTargetsByServiceTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
@@ -390,14 +391,15 @@
     "DataSourceSummaryTypeDef",
     "RollingDateConfigurationTypeDef",
     "MappedDataSetParameterTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterTypeDef",
+    "FilterSelectableValuesTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteDataSetRefreshPropertiesRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteDataSourceRequestRequestTypeDef",
@@ -473,15 +475,14 @@
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
-    "FilterSelectableValuesTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
@@ -840,15 +841,14 @@
     "DashboardVisualPublishOptionsTypeDef",
     "TableInlineVisualizationTypeDef",
     "DataLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
-    "TimeEqualityFilterTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterTypeDef",
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     "DescribeFolderResolvedPermissionsRequestDescribeFolderResolvedPermissionsPaginateTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
@@ -883,15 +883,14 @@
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
-    "RelativeDatesFilterTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "SearchFoldersRequestSearchFoldersPaginateTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
     "TypographyTypeDef",
@@ -965,15 +964,14 @@
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
     "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
     "AssetBundleImportJobOverrideTagsTypeDef",
     "NumericAxisOptionsTypeDef",
-    "CategoryFilterTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationTypeDef",
     "ConditionalFormattingIconTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
     "UpdateDashboardPermissionsResponseTypeDef",
@@ -991,15 +989,14 @@
     "ForecastScenarioTypeDef",
     "CustomContentConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "DataPathColorTypeDef",
     "DataPathSortTypeDef",
     "PivotTableDataPathOptionTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
-    "TimeRangeFilterTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
@@ -1038,14 +1035,15 @@
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupTypeDef",
+    "FilterCrossSheetControlTypeDef",
     "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
@@ -1085,16 +1083,14 @@
     "SeriesItemTypeDef",
     "ThemeConfigurationTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
-    "NumericEqualityFilterTypeDef",
-    "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterTypeDef",
     "DataSourcePaginatorTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
     "DataSourceTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
@@ -1111,25 +1107,32 @@
     "DescribeDashboardResponseTypeDef",
     "TemplateTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "LogicalTableTypeDef",
     "ColumnHierarchyTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "AxisDisplayOptionsTypeDef",
+    "DefaultDateTimePickerControlOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "DefaultFilterDropDownControlOptionsTypeDef",
     "FilterDropDownControlTypeDef",
     "ParameterDropDownControlTypeDef",
+    "DefaultFilterListControlOptionsTypeDef",
     "FilterListControlTypeDef",
     "ParameterListControlTypeDef",
+    "DefaultRelativeDateTimeControlOptionsTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
+    "DefaultSliderControlOptionsTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
+    "DefaultTextAreaControlOptionsTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
+    "DefaultTextFieldControlOptionsTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
     "PivotTableOptionsTypeDef",
     "PivotTotalOptionsTypeDef",
     "SubtotalOptionsTypeDef",
@@ -1151,15 +1154,14 @@
     "ThemeVersionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
-    "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
     "DatasetMetadataTypeDef",
     "ListDataSourcesResponsePaginatorTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
@@ -1174,14 +1176,15 @@
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "CustomActionSetParametersOperationTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "DefaultFilterControlOptionsTypeDef",
     "FilterControlTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
     "PivotTableTotalOptionsTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
@@ -1194,15 +1197,14 @@
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
-    "FilterTypeDef",
     "BarChartSortConfigurationTypeDef",
     "BoxPlotSortConfigurationTypeDef",
     "ComboChartSortConfigurationTypeDef",
     "FilledMapSortConfigurationTypeDef",
     "FunnelChartSortConfigurationTypeDef",
     "HeatMapSortConfigurationTypeDef",
     "KPISortConfigurationTypeDef",
@@ -1223,36 +1225,43 @@
     "UpdateDataSourceRequestRequestTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "DefaultFilterControlConfigurationTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
-    "FilterGroupTypeDef",
     "PivotTableSortConfigurationTypeDef",
     "TooltipOptionsTypeDef",
     "CreateTopicRequestRequestTypeDef",
     "DescribeTopicResponseTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationTypeDef",
     "VisualCustomActionTypeDef",
+    "CategoryFilterTypeDef",
+    "NumericEqualityFilterTypeDef",
+    "NumericRangeFilterTypeDef",
+    "RelativeDatesFilterTypeDef",
+    "TimeEqualityFilterTypeDef",
+    "TimeRangeFilterTypeDef",
+    "TopBottomFilterTypeDef",
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
     "UniqueValuesComputationTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
@@ -1284,14 +1293,15 @@
     "TreeMapAggregatedFieldWellsTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
+    "FilterTypeDef",
     "BarChartFieldWellsTypeDef",
     "BoxPlotFieldWellsTypeDef",
     "ComboChartFieldWellsTypeDef",
     "FilledMapFieldWellsTypeDef",
     "FunnelChartFieldWellsTypeDef",
     "GaugeChartConfigurationTypeDef",
     "GeospatialMapFieldWellsTypeDef",
@@ -1306,14 +1316,15 @@
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
     "TreeMapFieldWellsTypeDef",
     "WaterfallChartFieldWellsTypeDef",
     "WordCloudFieldWellsTypeDef",
     "TableFieldWellsTypeDef",
     "LayoutConfigurationTypeDef",
+    "FilterGroupTypeDef",
     "BarChartConfigurationTypeDef",
     "BoxPlotChartConfigurationTypeDef",
     "ComboChartConfigurationTypeDef",
     "FilledMapConfigurationTypeDef",
     "FunnelChartConfigurationTypeDef",
     "GaugeChartVisualTypeDef",
     "GeospatialMapConfigurationTypeDef",
@@ -1738,14 +1749,21 @@
         "JobStatus": NotRequired[AssetBundleImportJobStatusType],
         "Arn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "AssetBundleImportJobId": NotRequired[str],
         "FailureAction": NotRequired[AssetBundleImportFailureActionType],
     },
 )
+AssetBundleImportJobWarningTypeDef = TypedDict(
+    "AssetBundleImportJobWarningTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "Message": NotRequired[str],
+    },
+)
 AssetBundleImportSourceDescriptionTypeDef = TypedDict(
     "AssetBundleImportSourceDescriptionTypeDef",
     {
         "Body": NotRequired[str],
         "S3Uri": NotRequired[str],
     },
 )
@@ -2632,14 +2650,20 @@
 DecimalParameterTypeDef = TypedDict(
     "DecimalParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[float],
     },
 )
+FilterSelectableValuesTypeDef = TypedDict(
+    "FilterSelectableValuesTypeDef",
+    {
+        "Values": NotRequired[Sequence[str]],
+    },
+)
 DeleteAccountCustomizationRequestRequestTypeDef = TypedDict(
     "DeleteAccountCustomizationRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "Namespace": NotRequired[str],
     },
 )
@@ -3281,20 +3305,14 @@
 )
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": NotRequired[BaseMapStyleTypeType],
     },
 )
-FilterSelectableValuesTypeDef = TypedDict(
-    "FilterSelectableValuesTypeDef",
-    {
-        "Values": NotRequired[Sequence[str]],
-    },
-)
 SameSheetTargetVisualConfigurationTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationTypeDef",
     {
         "TargetVisuals": NotRequired[Sequence[str]],
         "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
     },
 )
@@ -6457,25 +6475,14 @@
         "DataSourceSummaries": List[DataSourceSummaryTypeDef],
         "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TimeEqualityFilterTypeDef = TypedDict(
-    "TimeEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "Value": NotRequired[TimestampTypeDef],
-        "ParameterName": NotRequired[str],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
-    },
-)
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[TimestampTypeDef],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
         "Parameter": NotRequired[str],
     },
@@ -6830,29 +6837,14 @@
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": NotRequired[ArcOptionsTypeDef],
         "DonutCenterOptions": NotRequired[DonutCenterOptionsTypeDef],
     },
 )
-RelativeDatesFilterTypeDef = TypedDict(
-    "RelativeDatesFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "RelativeDateType": RelativeDateTypeType,
-        "NullOption": FilterNullOptionType,
-        "MinimumGranularity": NotRequired[TimeGranularityType],
-        "RelativeDateValue": NotRequired[int],
-        "ParameterName": NotRequired[str],
-        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
-    },
-)
 FilterOperationTargetVisualsConfigurationTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationTypeDef",
     {
         "SameSheetTargetVisualConfiguration": NotRequired[
             SameSheetTargetVisualConfigurationTypeDef
         ],
     },
@@ -7543,22 +7535,14 @@
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
     {
         "Scale": NotRequired[AxisScaleTypeDef],
         "Range": NotRequired[AxisDisplayRangeTypeDef],
     },
 )
-CategoryFilterTypeDef = TypedDict(
-    "CategoryFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "Configuration": CategoryFilterConfigurationTypeDef,
-    },
-)
 ClusterMarkerConfigurationTypeDef = TypedDict(
     "ClusterMarkerConfigurationTypeDef",
     {
         "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
     },
 )
 TopicCategoryFilterTypeDef = TypedDict(
@@ -7777,28 +7761,14 @@
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": NotRequired[str],
         "FieldDataPathValues": NotRequired[Sequence[DataPathValueTypeDef]],
     },
 )
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "NullOption": FilterNullOptionType,
-        "IncludeMinimum": NotRequired[bool],
-        "IncludeMaximum": NotRequired[bool],
-        "RangeMinimumValue": NotRequired[TimeRangeFilterValueTypeDef],
-        "RangeMaximumValue": NotRequired[TimeRangeFilterValueTypeDef],
-        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-    },
-)
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": NotRequired[DisplayFormatType],
         "DisplayFormatOptions": NotRequired[DisplayFormatOptionsTypeDef],
     },
 )
@@ -8224,14 +8194,22 @@
 )
 SnapshotFileGroupTypeDef = TypedDict(
     "SnapshotFileGroupTypeDef",
     {
         "Files": NotRequired[List[SnapshotFileTypeDef]],
     },
 )
+FilterCrossSheetControlTypeDef = TypedDict(
+    "FilterCrossSheetControlTypeDef",
+    {
+        "FilterControlId": str,
+        "SourceFilterId": str,
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
+    },
+)
 DateTimeParameterDeclarationTypeDef = TypedDict(
     "DateTimeParameterDeclarationTypeDef",
     {
         "Name": str,
         "DefaultValues": NotRequired[DateTimeDefaultValuesTypeDef],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationTypeDef],
@@ -8672,41 +8650,14 @@
         "Column": ColumnIdentifierTypeDef,
         "Label": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
         "Aggregation": NotRequired[AggregationFunctionTypeDef],
         "TooltipTarget": NotRequired[TooltipTargetType],
     },
 )
-NumericEqualityFilterTypeDef = TypedDict(
-    "NumericEqualityFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "MatchOperator": NumericEqualityMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-        "Value": NotRequired[float],
-        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
-        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
-        "ParameterName": NotRequired[str],
-    },
-)
-NumericRangeFilterTypeDef = TypedDict(
-    "NumericRangeFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "NullOption": FilterNullOptionType,
-        "IncludeMinimum": NotRequired[bool],
-        "IncludeMaximum": NotRequired[bool],
-        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
-        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
-        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
-        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
-    },
-)
 ReferenceLineDynamicDataConfigurationTypeDef = TypedDict(
     "ReferenceLineDynamicDataConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
         "MeasureAggregationFunction": NotRequired[AggregationFunctionTypeDef],
     },
@@ -8929,14 +8880,21 @@
         "AxisLineVisibility": NotRequired[VisibilityType],
         "GridLineVisibility": NotRequired[VisibilityType],
         "DataOptions": NotRequired[AxisDataOptionsTypeDef],
         "ScrollbarOptions": NotRequired[ScrollBarOptionsTypeDef],
         "AxisOffset": NotRequired[str],
     },
 )
+DefaultDateTimePickerControlOptionsTypeDef = TypedDict(
+    "DefaultDateTimePickerControlOptionsTypeDef",
+    {
+        "Type": NotRequired[SheetControlDateTimePickerTypeType],
+        "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
+    },
+)
 FilterDateTimePickerControlTypeDef = TypedDict(
     "FilterDateTimePickerControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
@@ -8948,14 +8906,22 @@
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
     },
 )
+DefaultFilterDropDownControlOptionsTypeDef = TypedDict(
+    "DefaultFilterDropDownControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
+    },
+)
 FilterDropDownControlTypeDef = TypedDict(
     "FilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
@@ -8972,14 +8938,22 @@
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultFilterListControlOptionsTypeDef = TypedDict(
+    "DefaultFilterListControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
+    },
+)
 FilterListControlTypeDef = TypedDict(
     "FilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
@@ -8996,23 +8970,39 @@
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultRelativeDateTimeControlOptionsTypeDef = TypedDict(
+    "DefaultRelativeDateTimeControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[RelativeDateTimeControlDisplayOptionsTypeDef],
+    },
+)
 FilterRelativeDateTimeControlTypeDef = TypedDict(
     "FilterRelativeDateTimeControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[RelativeDateTimeControlDisplayOptionsTypeDef],
     },
 )
+DefaultSliderControlOptionsTypeDef = TypedDict(
+    "DefaultSliderControlOptionsTypeDef",
+    {
+        "MaximumValue": float,
+        "MinimumValue": float,
+        "StepSize": float,
+        "DisplayOptions": NotRequired[SliderControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlSliderTypeType],
+    },
+)
 FilterSliderControlTypeDef = TypedDict(
     "FilterSliderControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "MaximumValue": float,
@@ -9030,14 +9020,21 @@
         "SourceParameterName": str,
         "MaximumValue": float,
         "MinimumValue": float,
         "StepSize": float,
         "DisplayOptions": NotRequired[SliderControlDisplayOptionsTypeDef],
     },
 )
+DefaultTextAreaControlOptionsTypeDef = TypedDict(
+    "DefaultTextAreaControlOptionsTypeDef",
+    {
+        "Delimiter": NotRequired[str],
+        "DisplayOptions": NotRequired[TextAreaControlDisplayOptionsTypeDef],
+    },
+)
 FilterTextAreaControlTypeDef = TypedDict(
     "FilterTextAreaControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "Delimiter": NotRequired[str],
@@ -9050,14 +9047,20 @@
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "Delimiter": NotRequired[str],
         "DisplayOptions": NotRequired[TextAreaControlDisplayOptionsTypeDef],
     },
 )
+DefaultTextFieldControlOptionsTypeDef = TypedDict(
+    "DefaultTextFieldControlOptionsTypeDef",
+    {
+        "DisplayOptions": NotRequired[TextFieldControlDisplayOptionsTypeDef],
+    },
+)
 FilterTextFieldControlTypeDef = TypedDict(
     "FilterTextFieldControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[TextFieldControlDisplayOptionsTypeDef],
@@ -9305,25 +9308,14 @@
 StringFormatConfigurationTypeDef = TypedDict(
     "StringFormatConfigurationTypeDef",
     {
         "NullValueFormatConfiguration": NotRequired[NullValueFormatConfigurationTypeDef],
         "NumericFormatConfiguration": NotRequired[NumericFormatConfigurationTypeDef],
     },
 )
-TopBottomFilterTypeDef = TypedDict(
-    "TopBottomFilterTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierTypeDef,
-        "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
-        "Limit": NotRequired[int],
-        "TimeGranularity": NotRequired[TimeGranularityType],
-        "ParameterName": NotRequired[str],
-    },
-)
 FieldSortOptionsTypeDef = TypedDict(
     "FieldSortOptionsTypeDef",
     {
         "FieldSort": NotRequired[FieldSortTypeDef],
         "ColumnSort": NotRequired[ColumnSortTypeDef],
     },
 )
@@ -9560,24 +9552,37 @@
 LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsTypeDef",
     {
         "AxisOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "MissingDataConfigurations": NotRequired[Sequence[MissingDataConfigurationTypeDef]],
     },
 )
+DefaultFilterControlOptionsTypeDef = TypedDict(
+    "DefaultFilterControlOptionsTypeDef",
+    {
+        "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
+        "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsTypeDef],
+        "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsTypeDef],
+        "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
+        "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
+        "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
+        "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
+    },
+)
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
         "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
         "List": NotRequired[FilterListControlTypeDef],
         "Dropdown": NotRequired[FilterDropDownControlTypeDef],
         "TextField": NotRequired[FilterTextFieldControlTypeDef],
         "TextArea": NotRequired[FilterTextAreaControlTypeDef],
         "Slider": NotRequired[FilterSliderControlTypeDef],
         "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
+        "CrossSheet": NotRequired[FilterCrossSheetControlTypeDef],
     },
 )
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
         "List": NotRequired[ParameterListControlTypeDef],
@@ -9748,26 +9753,14 @@
     "FormatConfigurationTypeDef",
     {
         "StringFormatConfiguration": NotRequired[StringFormatConfigurationTypeDef],
         "NumberFormatConfiguration": NotRequired[NumberFormatConfigurationTypeDef],
         "DateTimeFormatConfiguration": NotRequired[DateTimeFormatConfigurationTypeDef],
     },
 )
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
-    {
-        "CategoryFilter": NotRequired[CategoryFilterTypeDef],
-        "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
-        "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
-        "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
-        "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
-        "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
-        "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
-    },
-)
 BarChartSortConfigurationTypeDef = TypedDict(
     "BarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
@@ -9921,14 +9914,15 @@
         "OverrideParameters": AssetBundleImportJobOverrideParametersTypeDef,
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
         "OverridePermissions": AssetBundleImportJobOverridePermissionsTypeDef,
         "OverrideTags": AssetBundleImportJobOverrideTagsTypeDef,
         "OverrideValidationStrategy": AssetBundleImportJobOverrideValidationStrategyTypeDef,
+        "Warnings": List[AssetBundleImportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
@@ -10013,14 +10007,21 @@
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DefaultFilterControlConfigurationTypeDef = TypedDict(
+    "DefaultFilterControlConfigurationTypeDef",
+    {
+        "Title": str,
+        "ControlOptions": DefaultFilterControlOptionsTypeDef,
+    },
+)
 TableFieldOptionTypeDef = TypedDict(
     "TableFieldOptionTypeDef",
     {
         "FieldId": str,
         "Width": NotRequired[str],
         "CustomLabel": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
@@ -10110,24 +10111,14 @@
     "UnaggregatedFieldTypeDef",
     {
         "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
     },
 )
-FilterGroupTypeDef = TypedDict(
-    "FilterGroupTypeDef",
-    {
-        "FilterGroupId": str,
-        "Filters": Sequence[FilterTypeDef],
-        "ScopeConfiguration": FilterScopeConfigurationTypeDef,
-        "CrossDataset": CrossDatasetTypesType,
-        "Status": NotRequired[WidgetStatusType],
-    },
-)
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": NotRequired[Sequence[PivotFieldSortOptionsTypeDef]],
     },
 )
 TooltipOptionsTypeDef = TypedDict(
@@ -10201,14 +10192,107 @@
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
         "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
         "Status": NotRequired[WidgetStatusType],
     },
 )
+CategoryFilterTypeDef = TypedDict(
+    "CategoryFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Configuration": CategoryFilterConfigurationTypeDef,
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+NumericEqualityFilterTypeDef = TypedDict(
+    "NumericEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "MatchOperator": NumericEqualityMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "Value": NotRequired[float],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+NumericRangeFilterTypeDef = TypedDict(
+    "NumericRangeFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
+        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+RelativeDatesFilterTypeDef = TypedDict(
+    "RelativeDatesFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "RelativeDateType": RelativeDateTypeType,
+        "NullOption": FilterNullOptionType,
+        "MinimumGranularity": NotRequired[TimeGranularityType],
+        "RelativeDateValue": NotRequired[int],
+        "ParameterName": NotRequired[str],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TimeEqualityFilterTypeDef = TypedDict(
+    "TimeEqualityFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Value": NotRequired[TimestampTypeDef],
+        "ParameterName": NotRequired[str],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimumValue": NotRequired[TimeRangeFilterValueTypeDef],
+        "RangeMaximumValue": NotRequired[TimeRangeFilterValueTypeDef],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
+TopBottomFilterTypeDef = TypedDict(
+    "TopBottomFilterTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
+        "Limit": NotRequired[int],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
+    },
+)
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[TableFieldOptionTypeDef]],
         "Order": NotRequired[Sequence[str]],
         "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsTypeDef],
     },
@@ -10537,14 +10621,26 @@
     "EmptyVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
+    {
+        "CategoryFilter": NotRequired[CategoryFilterTypeDef],
+        "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
+        "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
+        "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
+        "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
+        "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
+    },
+)
 BarChartFieldWellsTypeDef = TypedDict(
     "BarChartFieldWellsTypeDef",
     {
         "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsTypeDef],
     },
 )
 BoxPlotFieldWellsTypeDef = TypedDict(
@@ -10694,14 +10790,24 @@
     "LayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
         "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationTypeDef],
         "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationTypeDef],
     },
 )
+FilterGroupTypeDef = TypedDict(
+    "FilterGroupTypeDef",
+    {
+        "FilterGroupId": str,
+        "Filters": Sequence[FilterTypeDef],
+        "ScopeConfiguration": FilterScopeConfigurationTypeDef,
+        "CrossDataset": CrossDatasetTypesType,
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BarChartSortConfigurationTypeDef],
         "Orientation": NotRequired[BarChartOrientationType],
         "BarsArrangement": NotRequired[BarsArrangementType],
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.79
-Summary: Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.87
+Summary: Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-quicksight-1.34.79/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.34.79/setup.py` & `mypy_boto3_quicksight-1.34.87/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.34.79",
+    version="1.34.87",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.QuickSight 1.34.79 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

