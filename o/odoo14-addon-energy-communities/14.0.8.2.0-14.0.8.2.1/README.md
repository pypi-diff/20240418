# Comparing `tmp/odoo14_addon_energy_communities-14.0.8.2.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_energy_communities-14.0.8.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 278721 bytes, number of entries: 118
+Zip file size: 278718 bytes, number of entries: 118
 -rw-rw-r--  2.0 unx      146 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/__init__.py
--rw-rw-r--  2.0 unx     3001 b- defN 24-Apr-12 08:27 odoo/addons/energy_communities/__manifest__.py
+-rw-rw-r--  2.0 unx     3001 b- defN 24-Apr-18 08:42 odoo/addons/energy_communities/__manifest__.py
 -rw-rw-r--  2.0 unx      514 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/hooks.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/client_map/__init__.py
 -rw-rw-r--  2.0 unx     2556 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/client_map/config.py
 -rw-rw-r--  2.0 unx    18690 b- defN 24-Mar-05 11:47 odoo/addons/energy_communities/client_map/resources/landing_cmplace.py
 -rw-rw-r--  2.0 unx      154 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/controllers/__init__.py
 -rw-rw-r--  2.0 unx      188 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/controllers/controllers.py
 -rw-rw-r--  2.0 unx    25576 b- defN 24-Mar-05 11:47 odoo/addons/energy_communities/controllers/website_community_data.py
@@ -109,12 +109,12 @@
 -rw-rw-r--  2.0 unx      123 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/wizards/__init__.py
 -rw-rw-r--  2.0 unx     3044 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/wizards/assign_admin_wizard.py
 -rw-rw-r--  2.0 unx     1762 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/wizards/assign_admin_wizard.xml
 -rw-rw-r--  2.0 unx     3214 b- defN 24-Feb-27 11:59 odoo/addons/energy_communities/wizards/assign_crm_to_coordinator_company.py
 -rw-rw-r--  2.0 unx     1087 b- defN 23-Dec-12 09:45 odoo/addons/energy_communities/wizards/assign_crm_to_coordinator_company.xml
 -rw-rw-r--  2.0 unx    16813 b- defN 24-Apr-10 12:47 odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
 -rw-rw-r--  2.0 unx     4256 b- defN 24-Mar-05 11:47 odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
--rw-rw-r--  2.0 unx     1872 b- defN 24-Apr-12 08:32 odoo14_addon_energy_communities-14.0.8.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-12 08:32 odoo14_addon_energy_communities-14.0.8.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 24-Apr-12 08:32 odoo14_addon_energy_communities-14.0.8.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    13616 b- defN 24-Apr-12 08:32 odoo14_addon_energy_communities-14.0.8.2.0.dist-info/RECORD
-118 files, 1569488 bytes uncompressed, 255813 bytes compressed:  83.7%
+-rw-rw-r--  2.0 unx     1872 b- defN 24-Apr-18 08:49 odoo14_addon_energy_communities-14.0.8.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-18 08:49 odoo14_addon_energy_communities-14.0.8.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-Apr-18 08:49 odoo14_addon_energy_communities-14.0.8.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13616 b- defN 24-Apr-18 08:49 odoo14_addon_energy_communities-14.0.8.2.1.dist-info/RECORD
+118 files, 1569488 bytes uncompressed, 255810 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -336,20 +336,20 @@
 
 Filename: odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
 Comment: 
 
 Filename: odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
 Comment: 
 
-Filename: odoo14_addon_energy_communities-14.0.8.2.0.dist-info/METADATA
+Filename: odoo14_addon_energy_communities-14.0.8.2.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_energy_communities-14.0.8.2.0.dist-info/WHEEL
+Filename: odoo14_addon_energy_communities-14.0.8.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_energy_communities-14.0.8.2.0.dist-info/top_level.txt
+Filename: odoo14_addon_energy_communities-14.0.8.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_energy_communities-14.0.8.2.0.dist-info/RECORD
+Filename: odoo14_addon_energy_communities-14.0.8.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/energy_communities/__manifest__.py

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Energy Community",
-    "version": "14.0.8.2.0",
+    "version": "14.0.8.2.1",
     "depends": [
         "account",
         "cooperator_account_banking_mandate",
         "account_lock_date_update",
         "account_multicompany_easy_creation",
         "cooperator_account_payment",
         "account_payment_order",
```

## Comparing `odoo14_addon_energy_communities-14.0.8.2.0.dist-info/METADATA` & `odoo14_addon_energy_communities-14.0.8.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-energy-communities
-Version: 14.0.8.2.0
+Version: 14.0.8.2.1
 Summary: Energy Community
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL & Som Energia SCCL
 License: AGPL-3
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -23,15 +23,15 @@
 Requires-Dist: odoo14-addon-community-maps ==14.0.0.2.4
 Requires-Dist: odoo14-addon-cooperator
 Requires-Dist: odoo14-addon-cooperator-account-banking-mandate ==14.0.1.1.1
 Requires-Dist: odoo14-addon-cooperator-account-payment ==14.0.1.1.0
 Requires-Dist: odoo14-addon-crm-metadata-rest-api ==14.0.1.0.2
 Requires-Dist: odoo14-addon-crm-metadata ==14.0.1.0.0
 Requires-Dist: odoo14-addon-crm-rest-api ==14.0.1.0.2
-Requires-Dist: odoo14-addon-energy-selfconsumption ==14.0.4.0.0
+Requires-Dist: odoo14-addon-energy-selfconsumption ==14.0.4.0.1
 Requires-Dist: odoo14-addon-l10n-es-aeat-sii-oca ==14.0.2.8.1
 Requires-Dist: odoo14-addon-l10n-es-aeat
 Requires-Dist: odoo14-addon-l10n-es-cooperator
 Requires-Dist: odoo14-addon-mail-multicompany ==14.0.0.1.1.dev2
 Requires-Dist: odoo14-addon-metadata ==14.0.0.0.1
 Requires-Dist: odoo14-addon-partner-multi-company ==14.0.1.0.1.dev4
 Requires-Dist: odoo14-addon-queue-job ==14.0.3.1.5
```

## Comparing `odoo14_addon_energy_communities-14.0.8.2.0.dist-info/RECORD` & `odoo14_addon_energy_communities-14.0.8.2.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 odoo/addons/energy_communities/__init__.py,sha256=fD11ibF1SBSYjM0pQgicu5OLqwBEnAJvS2KUJMtdK18,146
-odoo/addons/energy_communities/__manifest__.py,sha256=8iP2zUobj9Bz6Imu0TW7l_v15xQ2LChC_fAozhyC9c8,3001
+odoo/addons/energy_communities/__manifest__.py,sha256=R883NvQotNd1VW0DBSGfa3y7WpFsTFP_1xnnNe28DF8,3001
 odoo/addons/energy_communities/hooks.py,sha256=3wGIOiUguugO48Ayr2JwgjRE6ONDngu68VTwyrtZRuE,514
 odoo/addons/energy_communities/client_map/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 odoo/addons/energy_communities/client_map/config.py,sha256=LCmpRrX_PmQLlX8Pl79H8JWddQyfoKAUcSIwk6GtmMA,2556
 odoo/addons/energy_communities/client_map/resources/landing_cmplace.py,sha256=Uofl65LC_Axx6UoyJ_5ZJ7BDL-ENfAWbik_udVSVReE,18690
 odoo/addons/energy_communities/controllers/__init__.py,sha256=ZrGfeG_LxxVrbLo_NYvcMuLtVpFjSj2TwSeJsYz-T70,154
 odoo/addons/energy_communities/controllers/controllers.py,sha256=Ze-pphuFFssMsru5-9F-R-P1r8Q9jdIa4MSKJwYu0s0,188
 odoo/addons/energy_communities/controllers/website_community_data.py,sha256=5lcxESATlGDHKKaEBbgJtkiqOoyFeq1AA0mTBKgMioA,25576
@@ -108,11 +108,11 @@
 odoo/addons/energy_communities/wizards/__init__.py,sha256=cO-T8mEYDrjW6Hf6S1qpUHIZYuM4xmYLr-3aT8ULdy4,123
 odoo/addons/energy_communities/wizards/assign_admin_wizard.py,sha256=vO6jzJnFdHxefMkGXgg4fJ6EfVf3m_fbiufD5nTnQwM,3044
 odoo/addons/energy_communities/wizards/assign_admin_wizard.xml,sha256=Y7lHFLiAudjh_zAop6it7dypXZnE6tzKiYg9EJ64vgI,1762
 odoo/addons/energy_communities/wizards/assign_crm_to_coordinator_company.py,sha256=EVUF6Fieu2bwVb854JU6jrGL7-6vamNxMtmYtNFkQP8,3214
 odoo/addons/energy_communities/wizards/assign_crm_to_coordinator_company.xml,sha256=tiudcVV7R5njiCrn-hLBRkKtL_yh9KQNYxqh-FjvtVM,1087
 odoo/addons/energy_communities/wizards/multicompany_easy_creation.py,sha256=uhYq2Vr8CH2KuPQIXJCC8aak8pDTzHbfeyNyQHWd9k4,16813
 odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml,sha256=B1ofUkQHcuXzWH9OP34IPH6sfTR2rFQRkxNyMfcAIsM,4256
-odoo14_addon_energy_communities-14.0.8.2.0.dist-info/METADATA,sha256=vxctN0DuqwtYms7cUXhpq_NGAP_upUorkJmMOAs7uuQ,1872
-odoo14_addon_energy_communities-14.0.8.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-odoo14_addon_energy_communities-14.0.8.2.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_energy_communities-14.0.8.2.0.dist-info/RECORD,,
+odoo14_addon_energy_communities-14.0.8.2.1.dist-info/METADATA,sha256=NlHSF1b8kYmm8c8-x-uoEMn9Z4ETwbwE4g_npcyD7Oc,1872
+odoo14_addon_energy_communities-14.0.8.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+odoo14_addon_energy_communities-14.0.8.2.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_energy_communities-14.0.8.2.1.dist-info/RECORD,,
```

