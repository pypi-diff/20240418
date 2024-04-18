# Comparing `tmp/alibabacloud_agency20221216-1.3.0.tar.gz` & `tmp/alibabacloud_agency20221216-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_agency20221216-1.3.0.tar", last modified: Fri Mar  8 17:09:32 2024, max compression
+gzip compressed data, was "dist/alibabacloud_agency20221216-1.4.0.tar", last modified: Thu Apr 18 07:06:02 2024, max compression
```

## Comparing `alibabacloud_agency20221216-1.3.0.tar` & `alibabacloud_agency20221216-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      457 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1192 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94383 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/client.py
--rw-r--r--   0 root         (0) root         (0)   149775 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-08 17:09:32.000000 alibabacloud_agency20221216-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2626 2024-03-08 17:09:31.000000 alibabacloud_agency20221216-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94605 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/client.py
+-rw-r--r--   0 root         (0) root         (0)   151377 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-04-18 07:06:02.000000 alibabacloud_agency20221216-1.4.0/setup.py
```

### Comparing `alibabacloud_agency20221216-1.3.0/LICENSE` & `alibabacloud_agency20221216-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216-1.3.0/PKG-INFO` & `alibabacloud_agency20221216-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_agency20221216
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Agency (20221216) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_agency20221216-1.3.0/README-CN.md` & `alibabacloud_agency20221216-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216-1.3.0/README.md` & `alibabacloud_agency20221216-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/client.py` & `alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1730,14 +1730,16 @@
         request: agency_20221216_models.SetAccountInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> agency_20221216_models.SetAccountInfoResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_nickname):
             query['AccountNickname'] = request.account_nickname
+        if not UtilClient.is_unset(request.customer_bd):
+            query['CustomerBd'] = request.customer_bd
         if not UtilClient.is_unset(request.remark):
             query['Remark'] = request.remark
         if not UtilClient.is_unset(request.uid):
             query['Uid'] = request.uid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1762,14 +1764,16 @@
         request: agency_20221216_models.SetAccountInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> agency_20221216_models.SetAccountInfoResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_nickname):
             query['AccountNickname'] = request.account_nickname
+        if not UtilClient.is_unset(request.customer_bd):
+            query['CustomerBd'] = request.customer_bd
         if not UtilClient.is_unset(request.remark):
             query['Remark'] = request.remark
         if not UtilClient.is_unset(request.uid):
             query['Uid'] = request.uid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
```

### Comparing `alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216/models.py` & `alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1332,34 +1332,42 @@
 class GetAccountInfoResponseBodyAccountInfoListAccountInfo(TeaModel):
     def __init__(
         self,
         account_nickname: str = None,
         aliyun_id: str = None,
         association_success_time: str = None,
         cid: int = None,
+        customer_bd: str = None,
+        delay_amount: str = None,
+        delay_status: str = None,
         email: str = None,
         mobile: str = None,
+        new_buy_status: str = None,
         remark: str = None,
         sub_account_type: int = None,
         uid: int = None,
     ):
         # The name of Sub Account:
         # 1.	Use the official name of Company, if Sub Account is an enterprise.
         # 2.	Use the official name of Partner, if Sub Account is a T2 reseller.
         self.account_nickname = account_nickname
         # Alibaba Cloud Login name of Distribution Customer.
         self.aliyun_id = aliyun_id
         # The time that Distribution Customer successfully associated with Distributor.
         self.association_success_time = association_success_time
         # Account CID of Distribution Customer.
         self.cid = cid
+        self.customer_bd = customer_bd
+        self.delay_amount = delay_amount
+        self.delay_status = delay_status
         # The E-mail of Distribution Customer.
         self.email = email
         # Valid mobile number of Distribution Customer.
         self.mobile = mobile
+        self.new_buy_status = new_buy_status
         # Description of Distribution Customer.
         self.remark = remark
         # Account Type:
         # - 1 Agency\"s End User
         # - 2 Reseller\"s End User
         # - 3 Enterprise
         # - 4 T2 Agency Partner
@@ -1382,18 +1390,26 @@
             result['AccountNickname'] = self.account_nickname
         if self.aliyun_id is not None:
             result['AliyunId'] = self.aliyun_id
         if self.association_success_time is not None:
             result['AssociationSuccessTime'] = self.association_success_time
         if self.cid is not None:
             result['Cid'] = self.cid
+        if self.customer_bd is not None:
+            result['CustomerBd'] = self.customer_bd
+        if self.delay_amount is not None:
+            result['DelayAmount'] = self.delay_amount
+        if self.delay_status is not None:
+            result['DelayStatus'] = self.delay_status
         if self.email is not None:
             result['Email'] = self.email
         if self.mobile is not None:
             result['Mobile'] = self.mobile
+        if self.new_buy_status is not None:
+            result['NewBuyStatus'] = self.new_buy_status
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.sub_account_type is not None:
             result['SubAccountType'] = self.sub_account_type
         if self.uid is not None:
             result['Uid'] = self.uid
         return result
@@ -1404,18 +1420,26 @@
             self.account_nickname = m.get('AccountNickname')
         if m.get('AliyunId') is not None:
             self.aliyun_id = m.get('AliyunId')
         if m.get('AssociationSuccessTime') is not None:
             self.association_success_time = m.get('AssociationSuccessTime')
         if m.get('Cid') is not None:
             self.cid = m.get('Cid')
+        if m.get('CustomerBd') is not None:
+            self.customer_bd = m.get('CustomerBd')
+        if m.get('DelayAmount') is not None:
+            self.delay_amount = m.get('DelayAmount')
+        if m.get('DelayStatus') is not None:
+            self.delay_status = m.get('DelayStatus')
         if m.get('Email') is not None:
             self.email = m.get('Email')
         if m.get('Mobile') is not None:
             self.mobile = m.get('Mobile')
+        if m.get('NewBuyStatus') is not None:
+            self.new_buy_status = m.get('NewBuyStatus')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('SubAccountType') is not None:
             self.sub_account_type = m.get('SubAccountType')
         if m.get('Uid') is not None:
             self.uid = m.get('Uid')
         return self
@@ -2887,27 +2911,29 @@
 
 
 class InviteSubAccountRequestAccountInfoList(TeaModel):
     def __init__(
         self,
         account_nickname: str = None,
         credit_line: str = None,
+        customer_bd: str = None,
         customer_id: str = None,
         email_address: str = None,
         new_buy_status: str = None,
         remark: str = None,
         sub_account_type: str = None,
         zero_credit_shutdown_policy: str = None,
     ):
         # The name of Sub Account:</br>
         # 1. Use the official name of Company, if Sub Account is an enterprise.</br>
         # 2. Use the official name of Partner, if Sub Account is a T2 reseller.</br>
         self.account_nickname = account_nickname
         # The total budget Credit of Sub Account that distributed by Partner.
         self.credit_line = credit_line
+        self.customer_bd = customer_bd
         # Customer ID, Returning ID from CreateCustomer API.
         self.customer_id = customer_id
         # The email address of End User,  which will receive the invitation email.
         self.email_address = email_address
         # Initial Order Status</br>
         # 1. ban：Ban the new purchase action--After End User finish registration and authorization, they can\"t issue Cloud Resource order immediately. Partner should manually update the "Order Control" settings as "Normal" to enable new order.</br>
         # 2. normal：Normal--After End User finished registration and authorization, they can issue Cloud Resource order immediately.</br>
@@ -2935,14 +2961,16 @@
             return _map
 
         result = dict()
         if self.account_nickname is not None:
             result['AccountNickname'] = self.account_nickname
         if self.credit_line is not None:
             result['CreditLine'] = self.credit_line
+        if self.customer_bd is not None:
+            result['CustomerBd'] = self.customer_bd
         if self.customer_id is not None:
             result['CustomerId'] = self.customer_id
         if self.email_address is not None:
             result['EmailAddress'] = self.email_address
         if self.new_buy_status is not None:
             result['NewBuyStatus'] = self.new_buy_status
         if self.remark is not None:
@@ -2955,14 +2983,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AccountNickname') is not None:
             self.account_nickname = m.get('AccountNickname')
         if m.get('CreditLine') is not None:
             self.credit_line = m.get('CreditLine')
+        if m.get('CustomerBd') is not None:
+            self.customer_bd = m.get('CustomerBd')
         if m.get('CustomerId') is not None:
             self.customer_id = m.get('CustomerId')
         if m.get('EmailAddress') is not None:
             self.email_address = m.get('EmailAddress')
         if m.get('NewBuyStatus') is not None:
             self.new_buy_status = m.get('NewBuyStatus')
         if m.get('Remark') is not None:
@@ -3969,21 +3999,23 @@
         return self
 
 
 class SetAccountInfoRequest(TeaModel):
     def __init__(
         self,
         account_nickname: str = None,
+        customer_bd: str = None,
         remark: str = None,
         uid: int = None,
     ):
         # Sub Account Nickname. 
         # * Use the official name of Company, if Sub Account is an enterprise.
         # * Use the official name of Partner, if Sub Account is a T2 reseller.
         self.account_nickname = account_nickname
+        self.customer_bd = customer_bd
         # Description of Sub Account.
         self.remark = remark
         # The UID of Sub Account.
         self.uid = uid
 
     def validate(self):
         pass
@@ -3992,24 +4024,28 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.account_nickname is not None:
             result['AccountNickname'] = self.account_nickname
+        if self.customer_bd is not None:
+            result['CustomerBd'] = self.customer_bd
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.uid is not None:
             result['Uid'] = self.uid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AccountNickname') is not None:
             self.account_nickname = m.get('AccountNickname')
+        if m.get('CustomerBd') is not None:
+            self.customer_bd = m.get('CustomerBd')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('Uid') is not None:
             self.uid = m.get('Uid')
         return self
```

### Comparing `alibabacloud_agency20221216-1.3.0/alibabacloud_agency20221216.egg-info/PKG-INFO` & `alibabacloud_agency20221216-1.4.0/alibabacloud_agency20221216.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-agency20221216
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Agency (20221216) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_agency20221216-1.3.0/setup.py` & `alibabacloud_agency20221216-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_agency20221216.
 
-Created on 08/03/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_agency20221216"
 NAME = "alibabacloud_agency20221216" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Agency (20221216) SDK Library for Python"
```

