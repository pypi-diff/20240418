# Comparing `tmp/mvt-2.5.1.tar.gz` & `tmp/mvt-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.5.1.tar", last modified: Thu Apr 11 09:21:30 2024, max compression
+gzip compressed data, was "mvt-2.5.2.tar", last modified: Thu Apr 18 14:56:20 2024, max compression
```

## Comparing `mvt-2.5.1.tar` & `mvt-2.5.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-11 09:21:26.000000 mvt-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-11 09:21:30.102443 mvt-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-11 09:21:26.000000 mvt-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.062443 mvt-2.5.1/mvt/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.062443 mvt-2.5.1/mvt/android/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.066443 mvt-2.5.1/mvt/android/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_package_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/artifacts/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.066443 mvt-2.5.1/mvt/android/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.070443 mvt-2.5.1/mvt/android/modules/adb/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.074443 mvt-2.5.1/mvt/android/modules/androidqf/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.074443 mvt-2.5.1/mvt/android/modules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.078443 mvt-2.5.1/mvt/android/modules/bugreport/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.078443 mvt-2.5.1/mvt/android/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/parsers/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/android/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/common/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    22957 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/common/virustotal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/cmd_check_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/data/ios_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/data/ios_versions.json
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/decrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.082443 mvt-2.5.1/mvt/ios/modules/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.086443 mvt-2.5.1/mvt/ios/modules/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.090443 mvt-2.5.1/mvt/ios/modules/mixed/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/global_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/modules/net_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-11 09:21:26.000000 mvt-2.5.1/mvt/ios/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/mvt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:21:30.000000 mvt-2.5.1/mvt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-11 09:21:30.106443 mvt-2.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-04-11 09:21:26.000000 mvt-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.094443 mvt-2.5.1/tests/android/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_appops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_package_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_dumpsys_receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_artifact_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_backup_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android/test_backup_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.094443 mvt-2.5.1/tests/android_adb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_adb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/android_androidqf/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsys_dbinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/android_bugreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_bugreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/android_bugreport/test_bugreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.098443 mvt-2.5.1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/common/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/ios_backup/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_datausage.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_global_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_tcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:21:30.102443 mvt-2.5.1/tests/ios_fs/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_androidqf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_android_bugreport.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_check_ios_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/test_ios_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-11 09:21:26.000000 mvt-2.5.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.015806 mvt-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-18 14:56:14.000000 mvt-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-18 14:56:20.015806 mvt-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-18 14:56:14.000000 mvt-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.975806 mvt-2.5.2/mvt/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.979806 mvt-2.5.2/mvt/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.979806 mvt-2.5.2/mvt/android/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_package_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/artifacts/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.979806 mvt-2.5.2/mvt/android/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.983806 mvt-2.5.2/mvt/android/modules/adb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.987806 mvt-2.5.2/mvt/android/modules/androidqf/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.987806 mvt-2.5.2/mvt/android/modules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/backup/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/backup/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.991806 mvt-2.5.2/mvt/android/modules/bugreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.991806 mvt-2.5.2/mvt/android/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/parsers/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/android/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.995806 mvt-2.5.2/mvt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22957 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/common/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.995806 mvt-2.5.2/mvt/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/cmd_check_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.995806 mvt-2.5.2/mvt/ios/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/data/ios_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/data/ios_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.995806 mvt-2.5.2/mvt/ios/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.995806 mvt-2.5.2/mvt/ios/modules/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:19.999806 mvt-2.5.2/mvt/ios/modules/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.003806 mvt-2.5.2/mvt/ios/modules/mixed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/global_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/modules/net_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-18 14:56:14.000000 mvt-2.5.2/mvt/ios/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.015806 mvt-2.5.2/mvt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 14:56:19.000000 mvt-2.5.2/mvt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-18 14:56:20.015806 mvt-2.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-04-18 14:56:14.000000 mvt-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.015806 mvt-2.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.007806 mvt-2.5.2/tests/android/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_appops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_package_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_dumpsys_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_artifact_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_backup_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android/test_backup_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.007806 mvt-2.5.2/tests/android_adb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_adb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.011806 mvt-2.5.2/tests/android_androidqf/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsys_battery_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsys_battery_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsys_dbinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.011806 mvt-2.5.2/tests/android_bugreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_bugreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/android_bugreport/test_bugreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.011806 mvt-2.5.2/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/common/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/common/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.015806 mvt-2.5.2/tests/ios_backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_global_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:56:20.015806 mvt-2.5.2/tests/ios_fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/test_check_android_androidqf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/test_check_android_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/test_check_android_bugreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/test_check_ios_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/test_ios_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 14:56:14.000000 mvt-2.5.2/tests/utils.py
```

### Comparing `mvt-2.5.1/LICENSE` & `mvt-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/PKG-INFO` & `mvt-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.5.1
+Version: 2.5.2
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Requires-Dist: requests>=2.28.1
 Requires-Dist: simplejson>=3.17.6
 Requires-Dist: packaging>=21.3
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: iOSbackup>=0.9.923
 Requires-Dist: adb-shell>=0.4.3
 Requires-Dist: libusb1>=3.0.0
-Requires-Dist: cryptography>=38.0.1
+Requires-Dist: cryptography>=42.0.5
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pyahocorasick>=2.0.0
 
 <p align="center">
      <img src="https://docs.mvt.re/en/latest/mvt.png" width="200" />
 </p>
```

### Comparing `mvt-2.5.1/README.md` & `mvt-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/artifact.py` & `mvt-2.5.2/mvt/android/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_accessibility.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_appops.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_daily.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_battery_history.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_dbinfo.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_package_activities.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_package_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_packages.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/dumpsys_receivers.py` & `mvt-2.5.2/mvt/android/artifacts/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/getprop.py` & `mvt-2.5.2/mvt/android/artifacts/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/processes.py` & `mvt-2.5.2/mvt/android/artifacts/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/artifacts/settings.py` & `mvt-2.5.2/mvt/android/artifacts/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cli.py` & `mvt-2.5.2/mvt/android/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cmd_check_adb.py` & `mvt-2.5.2/mvt/android/cmd_check_adb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cmd_check_androidqf.py` & `mvt-2.5.2/mvt/android/cmd_check_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cmd_check_backup.py` & `mvt-2.5.2/mvt/android/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cmd_check_bugreport.py` & `mvt-2.5.2/mvt/android/cmd_check_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/cmd_download_apks.py` & `mvt-2.5.2/mvt/android/cmd_download_apks.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/__init__.py` & `mvt-2.5.2/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/base.py` & `mvt-2.5.2/mvt/android/modules/adb/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/chrome_history.py` & `mvt-2.5.2/mvt/android/modules/adb/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_full.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.5.2/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/files.py` & `mvt-2.5.2/mvt/android/modules/adb/files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/getprop.py` & `mvt-2.5.2/mvt/android/modules/adb/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/logcat.py` & `mvt-2.5.2/mvt/android/modules/adb/logcat.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/packages.py` & `mvt-2.5.2/mvt/android/modules/adb/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/processes.py` & `mvt-2.5.2/mvt/android/modules/adb/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/root_binaries.py` & `mvt-2.5.2/mvt/android/modules/adb/root_binaries.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/selinux_status.py` & `mvt-2.5.2/mvt/android/modules/adb/selinux_status.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/settings.py` & `mvt-2.5.2/mvt/android/modules/adb/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/sms.py` & `mvt-2.5.2/mvt/android/modules/adb/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/adb/whatsapp.py` & `mvt-2.5.2/mvt/android/modules/adb/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/__init__.py` & `mvt-2.5.2/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/base.py` & `mvt-2.5.2/mvt/android/modules/androidqf/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_daily.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_battery_history.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_dbinfo.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.5.2/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/getprop.py` & `mvt-2.5.2/mvt/android/modules/androidqf/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/processes.py` & `mvt-2.5.2/mvt/android/modules/androidqf/processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/settings.py` & `mvt-2.5.2/mvt/android/modules/androidqf/settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/androidqf/sms.py` & `mvt-2.5.2/mvt/android/modules/androidqf/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/backup/base.py` & `mvt-2.5.2/mvt/android/modules/backup/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/backup/helpers.py` & `mvt-2.5.2/mvt/android/modules/backup/helpers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/backup/sms.py` & `mvt-2.5.2/mvt/android/modules/backup/sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/__init__.py` & `mvt-2.5.2/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.5.2/mvt/android/modules/bugreport/accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/activities.py` & `mvt-2.5.2/mvt/android/modules/bugreport/activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/appops.py` & `mvt-2.5.2/mvt/android/modules/bugreport/appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/base.py` & `mvt-2.5.2/mvt/android/modules/bugreport/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.5.2/mvt/android/modules/bugreport/battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/battery_history.py` & `mvt-2.5.2/mvt/android/modules/bugreport/battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.5.2/mvt/android/modules/bugreport/dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/getprop.py` & `mvt-2.5.2/mvt/android/modules/bugreport/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/packages.py` & `mvt-2.5.2/mvt/android/modules/bugreport/packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/modules/bugreport/receivers.py` & `mvt-2.5.2/mvt/android/modules/bugreport/receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/parsers/backup.py` & `mvt-2.5.2/mvt/android/parsers/backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/android/utils.py` & `mvt-2.5.2/mvt/android/utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/artifact.py` & `mvt-2.5.2/mvt/common/artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/cmd_check_iocs.py` & `mvt-2.5.2/mvt/common/cmd_check_iocs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/command.py` & `mvt-2.5.2/mvt/common/command.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/help.py` & `mvt-2.5.2/mvt/common/help.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/indicators.py` & `mvt-2.5.2/mvt/common/indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/logo.py` & `mvt-2.5.2/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/module.py` & `mvt-2.5.2/mvt/common/module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/options.py` & `mvt-2.5.2/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/updates.py` & `mvt-2.5.2/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/url.py` & `mvt-2.5.2/mvt/common/url.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/common/utils.py` & `mvt-2.5.2/mvt/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,28 +49,31 @@
     delta = datetime.timedelta(microseconds=timestamp)
     return epoch_start + delta
 
 
 def convert_datetime_to_iso(date_time: datetime.datetime) -> str:
     """Converts datetime to ISO string.
 
-    :param datetime: datetime.
+    :param datetime: datetime, naive or timezone aware
     :type datetime: datetime.datetime
     :returns: ISO datetime string in YYYY-mm-dd HH:MM:SS.ms format.
     :rtype: str
 
     """
     try:
+        if date_time.tzinfo:
+            # Timezone aware object - convert to UTC
+            date_time = date_time.astimezone(tz=datetime.UTC)
         return date_time.strftime("%Y-%m-%d %H:%M:%S.%f")
     except Exception:
         return ""
 
 
 def convert_unix_to_utc_datetime(
-    timestamp: Union[int, float, str]
+    timestamp: Union[int, float, str],
 ) -> datetime.datetime:
     """Converts a unix epoch timestamp to UTC datetime.
 
     :param timestamp: Epoc timestamp to convert.
     :type timestamp: int
     :returns: datetime.
```

### Comparing `mvt-2.5.1/mvt/common/virustotal.py` & `mvt-2.5.2/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/cli.py` & `mvt-2.5.2/mvt/ios/cli.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/cmd_check_backup.py` & `mvt-2.5.2/mvt/ios/cmd_check_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/cmd_check_fs.py` & `mvt-2.5.2/mvt/ios/cmd_check_fs.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/data/ios_models.json` & `mvt-2.5.2/mvt/ios/data/ios_models.json`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/data/ios_versions.json` & `mvt-2.5.2/mvt/ios/data/ios_versions.json`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/decrypt.py` & `mvt-2.5.2/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/backup/backup_info.py` & `mvt-2.5.2/mvt/ios/modules/backup/backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.5.2/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/backup/manifest.py` & `mvt-2.5.2/mvt/ios/modules/backup/manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/backup/profile_events.py` & `mvt-2.5.2/mvt/ios/modules/backup/profile_events.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/base.py` & `mvt-2.5.2/mvt/ios/modules/base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/__init__.py` & `mvt-2.5.2/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/analytics.py` & `mvt-2.5.2/mvt/ios/modules/fs/analytics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.5.2/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/cache_files.py` & `mvt-2.5.2/mvt/ios/modules/fs/cache_files.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/filesystem.py` & `mvt-2.5.2/mvt/ios/modules/fs/filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.5.2/mvt/ios/modules/fs/net_netusage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.5.2/mvt/ios/modules/fs/safari_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.5.2/mvt/ios/modules/fs/shutdownlog.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/version_history.py` & `mvt-2.5.2/mvt/ios/modules/fs/version_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.5.2/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.5.2/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.5.2/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.5.2/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/__init__.py` & `mvt-2.5.2/mvt/ios/modules/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/applications.py` & `mvt-2.5.2/mvt/ios/modules/mixed/applications.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/calendar.py` & `mvt-2.5.2/mvt/ios/modules/mixed/calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/calls.py` & `mvt-2.5.2/mvt/ios/modules/mixed/calls.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.5.2/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.5.2/mvt/ios/modules/mixed/chrome_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/contacts.py` & `mvt-2.5.2/mvt/ios/modules/mixed/contacts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.5.2/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.5.2/mvt/ios/modules/mixed/firefox_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/global_preferences.py` & `mvt-2.5.2/mvt/ios/modules/mixed/global_preferences.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.5.2/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.5.2/mvt/ios/modules/mixed/interactionc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/locationd.py` & `mvt-2.5.2/mvt/ios/modules/mixed/locationd.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.5.2/mvt/ios/modules/mixed/net_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.5.2/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.5.2/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.5.2/mvt/ios/modules/mixed/safari_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.5.2/mvt/ios/modules/mixed/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/sms.py` & `mvt-2.5.2/mvt/ios/modules/mixed/sms.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,16 +62,19 @@
                     "data": sms_data,
                 }
             )
         return records
 
     def check_indicators(self) -> None:
         for message in self.results:
-            alert = "ALERT: State-sponsored attackers may be targeting your iPhone"
-            if message.get("text", "").startswith(alert):
+            alert_old = "ALERT: State-sponsored attackers may be targeting your iPhone"
+            alert_new = "ALERT: Apple detected a targeted mercenary spyware attack against your iPhone"
+            if message.get("text", "").startswith(alert_old) or message.get(
+                "text", ""
+            ).startswith(alert_new):
                 self.log.warning(
                     "Apple warning about state-sponsored attack received on the %s",
                     message["isodate"],
                 )
 
         if not self.indicators:
             return
```

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.5.2/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/tcc.py` & `mvt-2.5.2/mvt/ios/modules/mixed/tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.5.2/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.5.2/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.5.2/mvt/ios/modules/mixed/whatsapp.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/modules/net_base.py` & `mvt-2.5.2/mvt/ios/modules/net_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt/ios/versions.py` & `mvt-2.5.2/mvt/ios/versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/mvt.egg-info/PKG-INFO` & `mvt-2.5.2/mvt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.5.1
+Version: 2.5.2
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Requires-Dist: requests>=2.28.1
 Requires-Dist: simplejson>=3.17.6
 Requires-Dist: packaging>=21.3
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: iOSbackup>=0.9.923
 Requires-Dist: adb-shell>=0.4.3
 Requires-Dist: libusb1>=3.0.0
-Requires-Dist: cryptography>=38.0.1
+Requires-Dist: cryptography>=42.0.5
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pyahocorasick>=2.0.0
 
 <p align="center">
      <img src="https://docs.mvt.re/en/latest/mvt.png" width="200" />
 </p>
```

### Comparing `mvt-2.5.1/mvt.egg-info/SOURCES.txt` & `mvt-2.5.2/mvt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/setup.cfg` & `mvt-2.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	requests >=2.28.1
 	simplejson >=3.17.6
 	packaging >=21.3
 	appdirs >=1.4.4
 	iOSbackup >=0.9.923
 	adb-shell >=0.4.3
 	libusb1 >=3.0.0
-	cryptography >=38.0.1
+	cryptography >=42.0.5
 	pyyaml >=6.0
 	pyahocorasick >= 2.0.0
 
 [options.packages.find]
 where = ./
 
 [options.entry_points]
```

### Comparing `mvt-2.5.1/tests/android/test_artifact.py` & `mvt-2.5.2/tests/android/test_artifact.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_accessibility.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_accessibility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_appops.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_appops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_daily.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_battery_history.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_dbinfo.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_package_activities.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_package_activities.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_packages.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_packages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_dumpsys_receivers.py` & `mvt-2.5.2/tests/android/test_artifact_dumpsys_receivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_getprop.py` & `mvt-2.5.2/tests/android/test_artifact_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_artifact_processes.py` & `mvt-2.5.2/tests/android/test_artifact_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_backup_module.py` & `mvt-2.5.2/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android/test_backup_parser.py` & `mvt-2.5.2/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_daily.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsys_battery_daily.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsys_battery_history.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsys_battery_history.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsys_dbinfo.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsys_dbinfo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.5.2/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_getprop.py` & `mvt-2.5.2/tests/android_androidqf/test_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_processes.py` & `mvt-2.5.2/tests/android_androidqf/test_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_settings.py` & `mvt-2.5.2/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_androidqf/test_sms.py` & `mvt-2.5.2/tests/android_androidqf/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/android_bugreport/test_bugreport.py` & `mvt-2.5.2/tests/android_bugreport/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/common/test_indicators.py` & `mvt-2.5.2/tests/common/test_indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/common/test_utils.py` & `mvt-2.5.2/tests/common/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,22 @@
         assert converted.month == 7
         assert converted.day == 18
 
     def test_convert_datetime_to_iso(self):
         converted = convert_unix_to_utc_datetime(TEST_DATE_EPOCH)
         assert convert_datetime_to_iso(converted) == TEST_DATE_ISO
 
+    def test_convert_timezone_aware_to_iso(self):
+        assert (
+            convert_datetime_to_iso(
+                datetime.strptime("2024-09-30 11:21:20+0200", "%Y-%m-%d %H:%M:%S%z")
+            )
+            == "2024-09-30 09:21:20.000000"
+        )
+
 
 class TestHashes:
     def test_hash_from_file(self):
         path = os.path.join(get_artifact_folder(), "androidqf", "backup.ab")
         sha256 = get_sha256_from_file_path(path)
         assert (
             sha256 == "f0e32fe8a7fd5ac0e2de19636d123c0072e979396986139ba2bc49ec385dc325"
```

### Comparing `mvt-2.5.1/tests/conftest.py` & `mvt-2.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_backup_info.py` & `mvt-2.5.2/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_calendar.py` & `mvt-2.5.2/tests/ios_backup/test_calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_datausage.py` & `mvt-2.5.2/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_global_preferences.py` & `mvt-2.5.2/tests/ios_backup/test_global_preferences.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_manifest.py` & `mvt-2.5.2/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.5.2/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_sms.py` & `mvt-2.5.2/tests/ios_backup/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_tcc.py` & `mvt-2.5.2/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.5.2/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/ios_fs/test_filesystem.py` & `mvt-2.5.2/tests/ios_fs/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/test_check_android_androidqf.py` & `mvt-2.5.2/tests/test_check_android_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/test_check_android_backup.py` & `mvt-2.5.2/tests/test_check_android_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/test_check_android_bugreport.py` & `mvt-2.5.2/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/test_check_ios_backup.py` & `mvt-2.5.2/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.5.1/tests/utils.py` & `mvt-2.5.2/tests/utils.py`

 * *Files identical despite different names*

