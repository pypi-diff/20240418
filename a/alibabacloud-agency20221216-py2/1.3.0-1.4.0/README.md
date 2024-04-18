# Comparing `tmp/alibabacloud_agency20221216_py2-1.3.0.tar.gz` & `tmp/alibabacloud_agency20221216_py2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_agency20221216_py2-1.3.0.tar", last modified: Fri Mar  8 17:08:23 2024, max compression
+gzip compressed data, was "dist/alibabacloud_agency20221216_py2-1.4.0.tar", last modified: Thu Apr 18 07:05:30 2024, max compression
```

## Comparing `alibabacloud_agency20221216_py2-1.3.0.tar` & `alibabacloud_agency20221216_py2-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      459 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42480 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/client.py
--rw-r--r--   0 root         (0) root         (0)   150401 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-08 17:08:23.000000 alibabacloud_agency20221216_py2-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42591 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/client.py
+-rw-r--r--   0 root         (0) root         (0)   152008 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-18 07:05:30.000000 alibabacloud_agency20221216_py2-1.4.0/setup.py
```

### Comparing `alibabacloud_agency20221216_py2-1.3.0/LICENSE` & `alibabacloud_agency20221216_py2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216_py2-1.3.0/PKG-INFO` & `alibabacloud_agency20221216_py2-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_agency20221216_py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Agency (20221216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_agency20221216_py2-1.3.0/README-CN.md` & `alibabacloud_agency20221216_py2-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216_py2-1.3.0/README.md` & `alibabacloud_agency20221216_py2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/client.py` & `alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,14 +817,16 @@
         return self.resend_email_with_options(request, runtime)
 
     def set_account_info_with_options(self, request, runtime):
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

### Comparing `alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216/models.py` & `alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1170,30 +1170,35 @@
             self.uid = m.get('Uid')
         if m.get('UserType') is not None:
             self.user_type = m.get('UserType')
         return self
 
 
 class GetAccountInfoResponseBodyAccountInfoListAccountInfo(TeaModel):
-    def __init__(self, account_nickname=None, aliyun_id=None, association_success_time=None, cid=None, email=None,
-                 mobile=None, remark=None, sub_account_type=None, uid=None):
+    def __init__(self, account_nickname=None, aliyun_id=None, association_success_time=None, cid=None,
+                 customer_bd=None, delay_amount=None, delay_status=None, email=None, mobile=None, new_buy_status=None,
+                 remark=None, sub_account_type=None, uid=None):
         # The name of Sub Account:
         # 1.	Use the official name of Company, if Sub Account is an enterprise.
         # 2.	Use the official name of Partner, if Sub Account is a T2 reseller.
         self.account_nickname = account_nickname  # type: str
         # Alibaba Cloud Login name of Distribution Customer.
         self.aliyun_id = aliyun_id  # type: str
         # The time that Distribution Customer successfully associated with Distributor.
         self.association_success_time = association_success_time  # type: str
         # Account CID of Distribution Customer.
         self.cid = cid  # type: long
+        self.customer_bd = customer_bd  # type: str
+        self.delay_amount = delay_amount  # type: str
+        self.delay_status = delay_status  # type: str
         # The E-mail of Distribution Customer.
         self.email = email  # type: str
         # Valid mobile number of Distribution Customer.
         self.mobile = mobile  # type: str
+        self.new_buy_status = new_buy_status  # type: str
         # Description of Distribution Customer.
         self.remark = remark  # type: str
         # Account Type:
         # - 1 Agency\"s End User
         # - 2 Reseller\"s End User
         # - 3 Enterprise
         # - 4 T2 Agency Partner
@@ -1216,18 +1221,26 @@
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
@@ -1238,18 +1251,26 @@
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
@@ -2557,22 +2578,23 @@
         if m.get('body') is not None:
             temp_model = GetUnassociatedCustomerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class InviteSubAccountRequestAccountInfoList(TeaModel):
-    def __init__(self, account_nickname=None, credit_line=None, customer_id=None, email_address=None,
-                 new_buy_status=None, remark=None, sub_account_type=None, zero_credit_shutdown_policy=None):
+    def __init__(self, account_nickname=None, credit_line=None, customer_bd=None, customer_id=None,
+                 email_address=None, new_buy_status=None, remark=None, sub_account_type=None, zero_credit_shutdown_policy=None):
         # The name of Sub Account:</br>
         # 1. Use the official name of Company, if Sub Account is an enterprise.</br>
         # 2. Use the official name of Partner, if Sub Account is a T2 reseller.</br>
         self.account_nickname = account_nickname  # type: str
         # The total budget Credit of Sub Account that distributed by Partner.
         self.credit_line = credit_line  # type: str
+        self.customer_bd = customer_bd  # type: str
         # Customer ID, Returning ID from CreateCustomer API.
         self.customer_id = customer_id  # type: str
         # The email address of End User,  which will receive the invitation email.
         self.email_address = email_address  # type: str
         # Initial Order Status</br>
         # 1. ban：Ban the new purchase action--After End User finish registration and authorization, they can\"t issue Cloud Resource order immediately. Partner should manually update the "Order Control" settings as "Normal" to enable new order.</br>
         # 2. normal：Normal--After End User finished registration and authorization, they can issue Cloud Resource order immediately.</br>
@@ -2600,14 +2622,16 @@
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
@@ -2620,14 +2644,16 @@
 
     def from_map(self, m=None):
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
@@ -3514,19 +3540,20 @@
         if m.get('body') is not None:
             temp_model = ResendEmailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetAccountInfoRequest(TeaModel):
-    def __init__(self, account_nickname=None, remark=None, uid=None):
+    def __init__(self, account_nickname=None, customer_bd=None, remark=None, uid=None):
         # Sub Account Nickname. 
         # * Use the official name of Company, if Sub Account is an enterprise.
         # * Use the official name of Partner, if Sub Account is a T2 reseller.
         self.account_nickname = account_nickname  # type: str
+        self.customer_bd = customer_bd  # type: str
         # Description of Sub Account.
         self.remark = remark  # type: str
         # The UID of Sub Account.
         self.uid = uid  # type: long
 
     def validate(self):
         pass
@@ -3535,24 +3562,28 @@
         _map = super(SetAccountInfoRequest, self).to_map()
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
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_agency20221216_py2-1.3.0/alibabacloud_agency20221216_py2.egg-info/PKG-INFO` & `alibabacloud_agency20221216_py2-1.4.0/alibabacloud_agency20221216_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-agency20221216-py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Agency (20221216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_agency20221216_py2-1.3.0/setup.py` & `alibabacloud_agency20221216_py2-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_agency20221216_py2.
 
-Created on 08/03/2024
+Created on 18/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_agency20221216"
 NAME = "alibabacloud_agency20221216_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Agency (20221216) SDK Library for Python2"
```

