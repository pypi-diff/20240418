# Comparing `tmp/python-amcards-1.2.9.tar.gz` & `tmp/python_amcards-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amcards-1.2.9.tar", last modified: Thu Nov 17 23:13:15 2022, max compression
+gzip compressed data, was "python_amcards-1.3.0.tar", last modified: Thu Apr 18 05:23:22 2024, max compression
```

## Comparing `python-amcards-1.2.9.tar` & `python_amcards-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.044571 python-amcards-1.2.9/
--rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python-amcards-1.2.9/LICENSE
--rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:13:15.044449 python-amcards-1.2.9/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)     2467 2022-11-05 09:50:39.000000 python-amcards-1.2.9/README.rst
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.042783 python-amcards-1.2.9/amcards/
--rw-r--r--   0 simonesestili   (501) staff       (20)     5106 2022-11-08 04:57:10.000000 python-amcards-1.2.9/amcards/__helpers.py
--rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python-amcards-1.2.9/amcards/__init__.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    52468 2022-11-17 07:32:01.000000 python-amcards-1.2.9/amcards/amcards.py
--rw-r--r--   0 simonesestili   (501) staff       (20)     1649 2022-11-12 20:48:33.000000 python-amcards-1.2.9/amcards/exceptions.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    25679 2022-11-17 23:12:45.000000 python-amcards-1.2.9/amcards/models.py
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.042927 python-amcards-1.2.9/images/
--rw-r--r--   0 simonesestili   (501) staff       (20)   537836 2022-11-05 09:15:52.000000 python-amcards-1.2.9/images/readthedocs.png
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2022-11-17 23:13:15.044273 python-amcards-1.2.9/python_amcards.egg-info/
--rw-r--r--   0 simonesestili   (501) staff       (20)     3050 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)      339 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/SOURCES.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        1 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/dependency_links.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       12 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/requires.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        8 2022-11-17 23:13:15.000000 python-amcards-1.2.9/python_amcards.egg-info/top_level.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       38 2022-11-17 23:13:15.044613 python-amcards-1.2.9/setup.cfg
--rw-r--r--   0 simonesestili   (501) staff       (20)      874 2022-11-17 23:12:23.000000 python-amcards-1.2.9/setup.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.586978 python_amcards-1.3.0/
+-rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python_amcards-1.3.0/LICENSE
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-18 05:23:22.586663 python_amcards-1.3.0/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)     2466 2023-05-19 17:59:31.000000 python_amcards-1.3.0/README.rst
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.585160 python_amcards-1.3.0/amcards/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     5466 2024-04-18 04:14:42.000000 python_amcards-1.3.0/amcards/__helpers.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python_amcards-1.3.0/amcards/__init__.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    61560 2024-04-18 05:21:04.000000 python_amcards-1.3.0/amcards/amcards.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)     1978 2024-04-18 05:21:12.000000 python_amcards-1.3.0/amcards/exceptions.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    30696 2024-04-18 05:05:32.000000 python_amcards-1.3.0/amcards/models.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.586335 python_amcards-1.3.0/python_amcards.egg-info/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)      316 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/SOURCES.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        1 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/dependency_links.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       12 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/requires.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        8 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/top_level.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       38 2024-04-18 05:23:22.587023 python_amcards-1.3.0/setup.cfg
+-rw-r--r--   0 simonesestili   (501) staff       (20)      874 2024-04-18 05:23:12.000000 python_amcards-1.3.0/setup.py
```

### Comparing `python-amcards-1.2.9/LICENSE` & `python_amcards-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amcards-1.2.9/PKG-INFO` & `python_amcards-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.2.9
+Version: 1.3.0
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: requests>=2
 
 Getting Started | See the full docs at `Read the Docs <https://python-amcards.readthedocs.io/en/latest/>`_
 ==========================================================================================================
 .. image:: https://i.ibb.co/tCrVfj6/readthedocs.png
     :target: https://python-amcards.readthedocs.io/en/latest/
 
 Installation
@@ -34,15 +35,15 @@
 First, create an `AMcardsClient <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_ as follows:
 
 .. code-block::
 
     >>> from amcards import AMcardsClient
     >>> client = AMcardsClient('youraccesstoken')
 
-Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/connected-applications/>`_.
+Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/generate-access-token/>`_.
 
 Now we can perform all operations supported by the `client <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_.
 
 Let's try using ``send_card`` to send a card to a single recipient:
 
 .. code-block::
```

### Comparing `python-amcards-1.2.9/README.rst` & `python_amcards-1.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 First, create an `AMcardsClient <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_ as follows:
 
 .. code-block::
 
     >>> from amcards import AMcardsClient
     >>> client = AMcardsClient('youraccesstoken')
 
-Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/connected-applications/>`_.
+Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/generate-access-token/>`_.
 
 Now we can perform all operations supported by the `client <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_.
 
 Let's try using ``send_card`` to send a card to a single recipient:
 
 .. code-block::
```

### Comparing `python-amcards-1.2.9/amcards/__helpers.py` & `python_amcards-1.3.0/amcards/__helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+import time
 from typing import Optional
 from datetime import datetime
 
 REQUIRED_SHIPPING_ADDRESS_FIELDS = {
     'first_name',
     'last_name',
     'address_line_1',
     'city',
     'state',
     'postal_code',
-    'country',
 }
 
 CARD_OPTIONAL_SHIPPING_ADDRESS_FIELDS = {
+    'country',
     'organization',
     'third_party_contact_id',
+    'address_line_2',
 }
 
 CAMPAIGN_OPTIONAL_SHIPPING_ADDRESS_FIELDS = {
+    'country',
     'organization',
     'phone_number',
     'birth_date',
     'anniversary_date',
     'third_party_contact_id',
+    'address_line_2',
 }
 
 OPTIONAL_RETURN_ADDRESS_FIELDS = {
     'first_name',
     'last_name',
     'address_line_1',
     'city',
     'state',
     'postal_code',
     'country',
 }
 
+def current_timestamp() -> int:
+    return int(time.time() * 1000)
+
 def today() -> str:
     today = datetime.today()
     yyyy = today.year
     mm, dd = map(lambda x: str(x).zfill(2), (today.month, today.day))
     return f'{yyyy}-{mm}-{dd}'
 
 def to_datetime(datetime_str: Optional[str]) -> Optional[datetime]:
@@ -62,15 +69,15 @@
     whole, fractional = map(str, divmod(price_in_cents, 100))
     fractional = fractional.zfill(2)
     return f'${whole}.{fractional}'
 
 def get_missing_required_shipping_address_fields(shipping_address: dict) -> list:
     missings = []
     for req in REQUIRED_SHIPPING_ADDRESS_FIELDS:
-        if shipping_address.get(req, '').strip(): continue
+        if (shipping_address.get(req, '') or '').strip(): continue
         missings.append(req)
     return missings
 
 def is_valid_date(date: str) -> bool:
     if not isinstance(date, str): return False
     if len(date) != 10: return False
     if date.count('-') != 2 or date[4] != '-' or date[7] != '-': return False
@@ -79,25 +86,29 @@
             return False
     return True
 
 def is_valid_phone(phone: str) -> bool:
     if not isinstance(phone, str): return False
     return len(phone) == 10 and phone.isdigit()
 
+def sanitize_extra_data(extra_data: dict) -> Optional[dict]:
+    if not isinstance(extra_data, dict): return None
+    return {k: v for k, v in extra_data.items() if isinstance(k, str) and isinstance(v, str)}
+
 def sanitize_shipping_address_for_card_send(shipping_address: dict) -> dict:
     sanitized_shipping_address = {field: shipping_address[field] for field in REQUIRED_SHIPPING_ADDRESS_FIELDS}
     for optional in CARD_OPTIONAL_SHIPPING_ADDRESS_FIELDS:
-        if optional not in shipping_address: continue
+        if not shipping_address.get(optional): continue
         sanitized_shipping_address[optional] = shipping_address[optional]
     return sanitized_shipping_address
 
 def sanitize_shipping_address_for_campaign_send(shipping_address: dict) -> dict:
     sanitized_shipping_address = {field: shipping_address[field] for field in REQUIRED_SHIPPING_ADDRESS_FIELDS}
     for optional in CAMPAIGN_OPTIONAL_SHIPPING_ADDRESS_FIELDS:
-        if optional not in shipping_address: continue
+        if not shipping_address.get(optional): continue
         sanitized_shipping_address[optional] = shipping_address[optional]
     return sanitized_shipping_address
 
 def sanitize_return_address(return_address: dict) -> dict:
     sanitized_return_address = {}
     for optional in OPTIONAL_RETURN_ADDRESS_FIELDS:
         if optional not in return_address: continue
```

### Comparing `python-amcards-1.2.9/amcards/amcards.py` & `python_amcards-1.3.0/amcards/amcards.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
-from typing import List, Optional
+from typing import List, Optional, Callable, Any
 
 
-from .models import User, Template, Gift, Campaign, CardResponse, CardsResponse, CampaignResponse, Card, Contact
+from .models import User, Template, Gift, Campaign, CardResponse, CardsResponse, CampaignResponse, Card, Contact, Mailing, CreditTransaction
 from . import exceptions
 from . import __helpers as helpers
 
 
 DOMAIN = 'https://amcards.com'
 
 FIXED_COUNTRY = {
@@ -15,49 +15,155 @@
     # GB fixes
     'ENGLAND': 'GB',
 }
 
 
 class AMcardsClient:
     """Client for AMcards API."""
-    def __init__(self, access_token: str) -> None:
+    def __init__(self, access_token: str, oauth_config: Optional[dict] = None, callback: Optional[Callable[[str, str, int], Any]] = None) -> None:
+        """Client for AMcards API.
+
+        :param str access_token: Your AMcards access token. Generate one `here <https://amcards.com/user/generate-access-token/>`_.
+        :param Optional[dict] oauth_config: Your OAuth configuration, this is optional, but if you choose to include it, it must include all of the following keys:
+
+            .. code-block::
+
+                {
+                    'refresh_token': 'yourrefreshtoken',
+                    'expiration': 1671692131130,                    # Note that expiration is specified as a unix timestamp in ms.
+                    'client_id': 'yourapplicationclientid',
+                    'client_secret': 'yourapplicationclientsecret'
+                }
+
+        :param Optional[Callable[[str, str, int], Any]] callback: This function will be called by the client when you have ``oauth_config`` defined, and the client refreshes the ``access_token`` before making a request. This can be useful when you need perform some logic when the client refreshes the specified ``access_token`` (like updating your database to reflect the new access_token and refresh_token). ``callback`` is optional, but if you choose to include it, it needs to accept the following keyword arguments: ``access_token`` ``refresh_token`` ``expiration``. ``callback`` will be called by the client as follows: ``callback(access_token='newaccesstoken', refresh_token='newrefreshtoken', expiration=1671692135130)``, note that ``expiration`` is specified as a unix timestamp in ms.
+
+        """
         self._access_token = access_token
-        self.HEADERS = {
-            'Authorization': f'Bearer {access_token}',
+        self._oauth_config = oauth_config
+        self._callback = callback
+
+    def _token_expired(self) -> bool:
+        return self._oauth_config is not None and helpers.current_timestamp() >= self._oauth_config['expiration']
+
+    def _refresh_token(self) -> None:
+        # Refresh the tokens
+        payload = {
+            'grant_type': 'refresh_token',
+            'refresh_token': self._oauth_config['refresh_token'],
+            'client_id': self._oauth_config['client_id'],
+            'client_secret': self._oauth_config['client_secret'],
+        }
+        res = requests.post(url=f'{DOMAIN}/oauth2/token/', data=payload)
+
+        # Make sure the refresh was successful
+        if not res.ok:
+            raise exceptions.OAuthTokenRefreshError('Something went wrong when attempting to refresh AMcards access_token')
+
+        # Update the access_token, refresh_token, and expiration
+        res_json = res.json()
+        self._access_token = res_json['access_token']
+        self._oauth_config['refresh_token'] = res_json['refresh_token']
+        self._oauth_config['expiration'] = helpers.current_timestamp() + res_json['expires_in'] * 1000
+
+        # If specified, call the callback
+        if self._callback is not None:
+            self._callback(
+                access_token=self._access_token,
+                refresh_token=self._oauth_config['refresh_token'],
+                expiration=self._oauth_config['expiration'],
+            )
+
+    @property
+    def _HEADERS(self) -> dict:
+        if self._token_expired():
+            self._refresh_token()
+
+        return {
+            'Authorization': f'Bearer {self._access_token}',
         }
 
     def user(self) -> User:
         """Fetches client's AMcards user.
 
         :return: The client's :py:class:`user <amcards.models.User>`.
         :rtype: :py:class:`User <amcards.models.User>`
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/user/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/user/', headers=self._HEADERS)
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         user_json = res.json().get('objects', [{}])[0]
         return User._from_json(user_json)
 
+    def credit_transactions(self, limit: int = 25, skip: int = 0, filters: dict = None) -> List[CreditTransaction]:
+        """Fetches client's AMcards credit transactions.
+
+        :param int limit: Defaults to ``25``. Max number of credit transactions to be fetched.
+        :param int skip: Defaults to ``0``. Number of credit transactions to be skipped.
+        :param Optional[dict] filters: Defaults to ``None``. Filters to be applied when fetching credit transactions.
+
+            A common use case is to use ``filter = {'amount_paid_int__gt': 0}``, this will count all credit transactions that have ``amount_paid > 0``.
+
+        :return: The client's :py:class:`credit transactions <amcards.models.CreditTransaction>`.
+        :rtype: List[:py:class:`CreditTransaction <amcards.models.CreditTransaction>`]
+
+        :raises AuthenticationError: When the client's ``access_token`` is invalid.
+
+        """
+        params = {
+            'limit': limit,
+            'offset': skip,
+        } | (filters or {})
+
+        res = requests.get(url=f'{DOMAIN}/.api/v1/credittransaction/', headers=self._HEADERS, params=params)
+        if not res.ok:
+            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+
+        credit_transactions_json = res.json().get('objects', [])
+        return [CreditTransaction._from_json(credit_transaction_json) for credit_transaction_json in credit_transactions_json]
+
+    def credit_transaction_count(self, filters: dict = None) -> int:
+        """Fetches count of client's AMcards credit transactions.
+
+        :param Optional[dict] filters: Defaults to ``None``. Filters to be applied when counting credit transactions.
+
+            A common use case is to use ``filter = {'amount_paid_int__gt': 0}``, this will count all credit transactions that have ``amount_paid > 0``.
+
+        :return: The count of client's credit transactions.
+        :rtype: int
+
+        :raises AuthenticationError: When the client's ``access_token`` is invalid.
+
+        """
+        params = {
+            'limit': 1,
+        } | (filters or {})
+
+        res = requests.get(url=f'{DOMAIN}/.api/v1/credittransaction/', headers=self._HEADERS, params=params)
+        if not res.ok:
+            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+
+        return res.json()['meta']['total_count']
+
     def templates(self, limit: int = 25, skip: int = 0) -> List[Template]:
         """Fetches client's AMcards templates.
 
         :param int limit: Defaults to ``25``. Max number of templates to be fetched.
         :param int skip: Defaults to ``0``. Number of templates to be skipped.
 
         :return: The client's :py:class:`templates <amcards.models.Template>`.
         :rtype: List[:py:class:`Template <amcards.models.Template>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/template/', headers=self.HEADERS, params={'limit': limit, 'offset': skip})
+        res = requests.get(url=f'{DOMAIN}/.api/v1/template/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         templates_json = res.json().get('objects', [])
         return [Template._from_json(template_json) for template_json in templates_json]
 
     def template(self, id: str | int) -> Template:
@@ -68,15 +174,15 @@
         :return: The client's :py:class:`template <amcards.models.Template>` with specified ``id``.
         :rtype: :py:class:`Template <amcards.models.Template>`
 
         :raises ForbiddenTemplateError: When the template for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/template/{id}/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/template/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenTemplateError('The template for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         template_json = res.json()
         return Template._from_json(template_json)
@@ -89,15 +195,15 @@
 
         :return: The client's :py:class:`quicksend templates <amcards.models.Template>`.
         :rtype: List[:py:class:`Template <amcards.models.Template>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/quicksendtemplate/', headers=self.HEADERS, params={'limit': limit, 'offset': skip})
+        res = requests.get(url=f'{DOMAIN}/.api/v1/quicksendtemplate/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         templates_json = res.json().get('objects', [])
         return [Template._from_json(template_json) for template_json in templates_json]
 
     def quicksend(self, id: str | int) -> Template:
@@ -108,15 +214,15 @@
         :return: The client's :py:class:`quicksend template <amcards.models.Template>` with specified ``id``.
         :rtype: :py:class:`Template <amcards.models.Template>`
 
         :raises ForbiddenTemplateError: When the quicksend template for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/quicksendtemplate/{id}/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/quicksendtemplate/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenTemplateError('The quicksend template for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         template_json = res.json()
         return Template._from_json(template_json)
@@ -129,15 +235,15 @@
 
         :return: The client's :py:class:`drip campaigns <amcards.models.Campaign>`.
         :rtype: List[:py:class:`Campaign <amcards.models.Campaign>`]
 
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/campaign/', headers=self.HEADERS, params={'limit': limit, 'offset': skip})
+        res = requests.get(url=f'{DOMAIN}/.api/v1/campaign/', headers=self._HEADERS, params={'limit': limit, 'offset': skip})
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         campaigns_json = res.json().get('objects', [])
         return [Campaign._from_json(campaign_json) for campaign_json in campaigns_json]
 
     def campaign(self, id: str | int) -> Campaign:
@@ -148,15 +254,15 @@
         :return: The client's :py:class:`drip campaign <amcards.models.Campaign>` with specified ``id``.
         :rtype: :py:class:`Campaign <amcards.models.Campaign>`
 
         :raises ForbiddenCampaignError: When the drip campaign for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/campaign/{id}/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/campaign/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenCampaignError('The drip campaign for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         campaign_json = res.json()
         return Campaign._from_json(campaign_json)
@@ -177,15 +283,15 @@
 
         """
         params = {
             'limit': limit,
             'offset': skip,
         } | (filters or {})
 
-        res = requests.get(url=f'{DOMAIN}/.api/v1/card/', headers=self.HEADERS, params=params)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/card/', headers=self._HEADERS, params=params)
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         cards_json = res.json().get('objects', [])
         return [Card._from_json(card_json) for card_json in cards_json]
 
     def card(self, id: str | int) -> Card:
@@ -196,23 +302,67 @@
         :return: The client's :py:class:`card <amcards.models.Card>` with specified ``id``.
         :rtype: :py:class:`Card <amcards.models.Card>`
 
         :raises ForbiddenCardError: When the card for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/card/{id}/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/card/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenCardError('The card for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         card_json = res.json()
         return Card._from_json(card_json)
 
+    def card_count(self, filters: dict = None) -> int:
+        """Fetches count of client's AMcards cards.
+
+        :param Optional[dict] filters: Defaults to ``None``. Filters to be applied when counting cards.
+
+            A common use case is to use ``filter = {'third_party_contact_id': 'some_target_id'}``, this will fetch all cards that were shipped to a recipient with a ``third_party_contact_id == 'some_target_id'``.
+
+        :return: The count of client's cards.
+        :rtype: int
+
+        :raises AuthenticationError: When the client's ``access_token`` is invalid.
+
+        """
+        params = {
+            'limit': 1,
+        } | (filters or {})
+
+        res = requests.get(url=f'{DOMAIN}/.api/v1/card/', headers=self._HEADERS, params=params)
+        if not res.ok:
+            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+
+        return res.json()['meta']['total_count']
+
+    def mailing(self, id: str | int) -> Mailing:
+        """Fetches client's AMcards mailing with a specified id.
+
+        :param str or int id: Unique id for the :py:class:`mailing <amcards.models.Mailing>` you are fetching.
+
+        :return: The client's :py:class:`mailing <amcards.models.Mailing>` with specified ``id``.
+        :rtype: :py:class:`Mailing <amcards.models.Mailing>`
+
+        :raises ForbiddenMailingError: When the mailing for the specified ``id`` either does not exist or is not owned by the client's user.
+        :raises AuthenticationError: When the client's ``access_token`` is invalid.
+
+        """
+        res = requests.get(url=f'{DOMAIN}/.api/v1/mailing/{id}/', headers=self._HEADERS)
+        if not res.ok:
+            if res.status_code in (403, 404):
+                raise exceptions.ForbiddenMailingError('The mailing for the specified id either does not exist or is not owned by the client\'s user')
+            raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
+
+        mailing_json = res.json()
+        return Mailing._from_json(mailing_json)
+
     def contacts(self, limit: int = 25, skip: int = 0, filters: dict = None) -> List[Contact]:
         """Fetches client's AMcards contacts.
 
         :param int limit: Defaults to ``25``. Max number of contacts to be fetched.
         :param int skip: Defaults to ``0``. Number of contacts to be skipped.
         :param Optional[dict] filters: Defaults to ``None``. Filters to be applied when fetching contacts.
 
@@ -225,15 +375,15 @@
 
         """
         params = {
             'limit': limit,
             'offset': skip,
         } | (filters or {})
 
-        res = requests.get(url=f'{DOMAIN}/.api/v1/contact/', headers=self.HEADERS, params=params)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/contact/', headers=self._HEADERS, params=params)
         if not res.ok:
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         contacts_json = res.json().get('objects', [])
         return [Contact._from_json(contact_json) for contact_json in contacts_json]
 
     def contact(self, id: str | int) -> Contact:
@@ -244,15 +394,15 @@
         :return: The client's :py:class:`contact <amcards.models.Contact>` with specified ``id``.
         :rtype: :py:class:`Contact <amcards.models.Contact>`
 
         :raises ForbiddenContactError: When the contact for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.get(url=f'{DOMAIN}/.api/v1/contact/{id}/', headers=self.HEADERS)
+        res = requests.get(url=f'{DOMAIN}/.api/v1/contact/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenContactError('The contact for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
         contact_json = res.json()
         return Contact._from_json(contact_json)
@@ -322,30 +472,30 @@
         if birth_year is not None: body |= {'birth_year': birth_year}
         if birth_month is not None: body |= {'birth_month': birth_month}
         if birth_day is not None: body |= {'birth_day': birth_day}
         if anniversary_year is not None: body |= {'anniversary_year': anniversary_year}
         if anniversary_month is not None: body |= {'anniversary_month': anniversary_month}
         if anniversary_day is not None: body |= {'anniversary_day': anniversary_day}
 
-        res = requests.post(url=f'{DOMAIN}/.api/v1/contact/', json=body, headers=self.HEADERS)
+        res = requests.post(url=f'{DOMAIN}/.api/v1/contact/', json=body, headers=self._HEADERS)
         if not res.ok:
             if res.status_code == 401:
                 raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
             raise exceptions.AMcardsException('Something went wrong when trying to create a contact')
 
     def delete_contact(self, id: str | int) -> None:
         """Deletes client's AMcards contact with a specified id.
 
         :param str or int id: Unique id for the :py:class:`contact <amcards.models.Contact>` you are deleting.
 
         :raises ForbiddenContactError: When the contact for the specified ``id`` either does not exist or is not owned by the client's user.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
 
         """
-        res = requests.delete(url=f'{DOMAIN}/.api/v1/contact/{id}/', headers=self.HEADERS)
+        res = requests.delete(url=f'{DOMAIN}/.api/v1/contact/{id}/', headers=self._HEADERS)
         if not res.ok:
             if res.status_code in (403, 404):
                 raise exceptions.ForbiddenContactError('The contact for the specified id either does not exist or is not owned by the client\'s user')
             raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
 
     def send_card_cost(
         self,
@@ -451,14 +601,15 @@
         self,
         template_id: str | int,
         initiator: str,
         shipping_address: dict,
         return_address: dict = None,
         send_date: str = None,
         message: str = None,
+        extra_data: dict = None,
     ) -> CardResponse:
         """Attempt to send a card.
 
             .. code-block::
 
                 >>> from amcards import AMcardsClient
                 >>> client = AMcardsClient('youraccesstoken')
@@ -497,15 +648,16 @@
                     'last_name': 'Mullins',
                     'address_line_1': '2285 Reppert Road',
                     'city': 'Southfield',
                     'state': 'MI',
                     'postal_code': '48075',
                     'country': 'US',
                     'organization': 'Google',                # OPTIONAL
-                    'third_party_contact_id': 'crmid1453131' # OPTIONAL
+                    'third_party_contact_id': 'crmid1453131',# OPTIONAL
+                    'address_line_2': 'Apt 2'                # OPTIONAL
                 }
 
         :param Optional[dict] return_address: Dict of return details that will override the client's AMcards user default return details. Here's an example how the dict might look, all of the keys are optional:
 
             .. code-block::
 
                 {
@@ -516,14 +668,21 @@
                     'state': 'MI',                           # OPTIONAL
                     'postal_code': '48075',                  # OPTIONAL
                     'country': 'US',                         # OPTIONAL
                 }
 
         :param Optional[str] send_date: The date the card should be sent. If not specified, the card will be scheduled for the following day. The format should be: ``"YYYY-MM-DD"``.
         :param Optional[str] message: A message to add to the card. This will be added to the inside bottom or inside right panel on the card and will not replace any message that is currently on the template.
+        :param Optional[dict] extra_data: Extra data for merge fields. This is useful when you want to dynamically pass custom data to your templates. For example, if you pass in the example JSON, you would want to have your template contain a merge field in the form of *|data.carMake|*
+
+            .. code-block::
+
+                {
+                    'carMake': 'Honda',                      # OPTIONAL
+                }
 
         :return: AMcards' :py:class:`response <amcards.models.CardResponse>` for sending a single card.
         :rtype: :py:class:`CardResponse <amcards.models.CardResponse>`
 
         :raises CardSendError: When something goes wrong when attempting to send a card.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
         :raises ForbiddenTemplateError: When the client does not own the :py:class:`template <amcards.models.Template>` specified by ``template_id``.
@@ -546,14 +705,17 @@
         # Sanitize shipping address and return address
         shipping_address = helpers.sanitize_shipping_address_for_card_send(shipping_address)
         if return_address is not None:
             return_address = helpers.sanitize_return_address(return_address)
             # prefix return address fields with return_
             return_address = {f'return_{key}': value for key, value in return_address.items()}
 
+        # Sanitize extra_data
+        extra_data = helpers.sanitize_extra_data(extra_data)
+
         # Build request json payload
         body = {
             'template_id': template_id,
             'initiator': initiator,
         } | shipping_address
 
         if return_address is not None:
@@ -561,15 +723,18 @@
 
         if send_date is not None:
             body |= {'send_date': send_date}
 
         if message is not None:
             body |= {'message': message}
 
-        res = requests.post(f'{DOMAIN}/cards/open-card-form-oa/', json=body, headers=self.HEADERS)
+        if extra_data is not None:
+            body |= {'extra_data': extra_data}
+
+        res = requests.post(f'{DOMAIN}/cards/open-card-form-oa/', json=body, headers=self._HEADERS)
 
         # Check for errors
         match res.status_code:
             case 400:
                 raise exceptions.CardSendError('Something went wrong when attempting to send a card')
             case 401:
                 raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
@@ -700,15 +865,15 @@
         if send_date is not None:
             body |= {'send_date': send_date}
 
         if 'birth_date' in shipping_address:
             body['recipients'][0]['birth_day'] = shipping_address['birth_date'][-2:]
             body['recipients'][0]['birth_month'] = shipping_address['birth_date'][-5:-3]
 
-        res = requests.post(f'{DOMAIN}/campaigns/calculate-campaign-price/', json=body, headers=self.HEADERS)
+        res = requests.post(f'{DOMAIN}/campaigns/calculate-campaign-price/', json=body, headers=self._HEADERS)
 
         # Check for errors
         match res.status_code:
             case 401:
                 raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
             case 403:
                 raise exceptions.ForbiddenCampaignError(f'Clients\' user does not own given campaign with id of {campaign_id}')
@@ -718,14 +883,15 @@
     def send_campaign(
         self,
         campaign_id: str | int,
         initiator: str,
         shipping_address: dict,
         return_address: dict = None,
         send_date: str = None,
+        extra_data: dict = None,
     ) -> CampaignResponse:
         """Attempt to send a drip campaign.
 
             .. code-block::
 
                 >>> from amcards import AMcardsClient
                 >>> client = AMcardsClient('youraccesstoken')
@@ -767,15 +933,16 @@
                     'state': 'MI',
                     'postal_code': '48075',
                     'country': 'US',
                     'organization': 'Google',                # OPTIONAL
                     'phone_number': '15556667777',           # OPTIONAL
                     'birth_date': '2003-12-25',              # OPTIONAL
                     'anniversary_date': '2022-10-31',        # OPTIONAL
-                    'third_party_contact_id': 'crmid1453131' # OPTIONAL
+                    'third_party_contact_id': 'crmid1453131',# OPTIONAL
+                    'address_line_2': 'Apt 2'                # OPTIONAL
                 }
 
         :param Optional[dict] return_address: Dict of return details that will override the client's AMcards user default return details. Here's an example how the dict might look, all of the keys are optional:
 
             .. code-block::
 
                 {
@@ -785,14 +952,21 @@
                     'city': 'Southfield',                    # OPTIONAL
                     'state': 'MI',                           # OPTIONAL
                     'postal_code': '48075',                  # OPTIONAL
                     'country': 'US',                         # OPTIONAL
                 }
 
         :param Optional[str] send_date: The date the drip campaign should be sent, in ``"YYYY-MM-DD"`` format. If not specified, the drip campaign will be scheduled for the following day.
+        :param Optional[dict] extra_data: Extra data for merge fields. This is useful when you want to dynamically pass custom data to your templates. For example, if you pass in the example JSON, you would want to have your template contain a merge field in the form of *|data.carMake|*
+
+            .. code-block::
+
+                {
+                    'carMake': 'Honda',                      # OPTIONAL
+                }
 
         :return: AMcards' :py:class:`response <amcards.models.CampaignResponse>` for sending a single drip campaign.
         :rtype: :py:class:`CampaignResponse <amcards.models.CampaignResponse>`
 
         :raises CampaignSendError: When something goes wrong when attempting to send a drip campaign.
         :raises AuthenticationError: When the client's ``access_token`` is invalid.
         :raises ForbiddenCampaignError: When the client does not own the :py:class:`campaign <amcards.models.Campaign>` specified by ``campaign_id``.
@@ -829,28 +1003,33 @@
         if 'anniversary_date' in shipping_address and not helpers.is_valid_date(shipping_address['anniversary_date']):
             error_message = 'Invalid anniversary_date format, please specify date as "YYYY-MM-DD", or omit it'
             raise exceptions.DateFormatError(error_message)
         # Validate phone_number
         if 'phone_number' in shipping_address and not helpers.is_valid_phone(shipping_address['phone_number']):
             error_message = 'Invalid phone_number format, please specify phone as a 10 number string with no special formatting (ex. 15556667777), or omit it'
             raise exceptions.PhoneFormatError(error_message)
+        # Sanitize extra_data
+        extra_data = helpers.sanitize_extra_data(extra_data)
 
         # Build request json payload
         body = {
             'campaign_id': campaign_id,
             'initiator': initiator,
         } | shipping_address
 
         if return_address is not None:
             body |= return_address
 
         if send_date is not None:
             body |= {'send_date': send_date}
 
-        res = requests.post(f'{DOMAIN}/campaigns/open-campaign-form/', json=body, headers=self.HEADERS)
+        if extra_data is not None:
+            body |= {'extra_data': extra_data}
+
+        res = requests.post(f'{DOMAIN}/campaigns/open-campaign-form/', json=body, headers=self._HEADERS)
 
         # Check for errors
         match res.status_code:
             case 400:
                 raise exceptions.CampaignSendError('Something went wrong when attempting to send a drip campaign')
             case 401:
                 raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
@@ -1007,15 +1186,15 @@
 
         if return_address is not None:
             body |= return_address
 
         if send_date is not None:
             body |= {'send_type': 'specific_date', 'send_date': send_date}
 
-        res = requests.post(f'{DOMAIN}/cards/open-mailing-form/', json=body, headers=self.HEADERS)
+        res = requests.post(f'{DOMAIN}/cards/open-mailing-form/', json=body, headers=self._HEADERS)
 
         # Check for errors
         match res.status_code:
             case 400:
                 raise exceptions.CardsSendError('Something went wrong when attempting to send cards')
             case 401:
                 raise exceptions.AuthenticationError('Access token provided to client is unauthorized')
```

### Comparing `python-amcards-1.2.9/amcards/exceptions.py` & `python_amcards-1.3.0/amcards/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 class ForbiddenCampaignError(ForbiddenResourceError):
     """Campaign is not owned by clients' user"""
 
 class ForbiddenCardError(ForbiddenResourceError):
     """Card is not owned by clients' user"""
 
+class ForbiddenMailingError(ForbiddenResourceError):
+    """Mailing is not owned by clients' user"""
+
 class ForbiddenContactError(ForbiddenResourceError):
     """Contact is not owned by clients' user"""
 
 class ShippingAddressError(AMcardsException, ValueError):
     """Some shipping address fields are missing or invalid"""
 
 class AuthenticationError(AMcardsException):
@@ -29,18 +32,24 @@
 
 class DateFormatError(AMcardsException, ValueError):
     """Invalid format for date"""
 
 class PhoneFormatError(AMcardsException, ValueError):
     """Invalid format for phone number"""
 
+class ExtraDataFormatError(AMcardsException, ValueError):
+    """Invalid format for extra data"""
+
 class DuplicateCampaignError(AMcardsException):
     """Duplicate campaign detected"""
 
 class CardSendError(AMcardsException):
     """Something went wrong when attempting to send a card"""
 
 class CardsSendError(AMcardsException):
     """Something went wrong when attempting to send cards"""
 
 class CampaignSendError(AMcardsException):
     """Something went wrong when attempting to send a drip campaign"""
+
+class OAuthTokenRefreshError(AMcardsException):
+    """Something went wrong when attempting to refresh AMcards access_token"""
```

### Comparing `python-amcards-1.2.9/amcards/models.py` & `python_amcards-1.3.0/amcards/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     def __init__(
         self,
         id: int,
         first_name: str,
         last_name: str,
         credits: int,
         email: str,
+        phone: str,
         date_joined: datetime,
         address_line_1: str,
         city: str,
         state: str,
         postal_code: str,
         country: str,
         domestic_postage_cost: int,
@@ -27,14 +28,15 @@
         greeting_card_cost: int,
     ) -> None:
         self._id = id
         self._first_name = first_name
         self._last_name = last_name
         self._credits = credits
         self._email = email
+        self._phone = phone
         self._date_joined = date_joined
         self._address_line_1 = address_line_1
         self._city = city
         self._state = state
         self._postal_code = postal_code
         self._country = country
         self._domestic_postage_cost = domestic_postage_cost
@@ -66,14 +68,19 @@
 
     @property
     def email(self) -> str:
         """User's email address."""
         return self._email
 
     @property
+    def phone(self) -> str:
+        """User's phone number."""
+        return self._phone
+
+    @property
     def date_joined(self) -> datetime:
         """Date and time when user created their AMcards account."""
         return self._date_joined
 
     @property
     def address_line_1(self) -> str:
         """User's primary address line (street)."""
@@ -127,14 +134,15 @@
         if not user_id[-1].isdigit(): user_id = user_id[:-1]
         return cls(
             id=int(user_id),
             first_name=json['first_name'],
             last_name=json['last_name'],
             credits=json['credits'],
             email=json['email'],
+            phone=json['phone'],
             date_joined=helpers.to_datetime(json['date_joined']),
             address_line_1=json['address_line_1'],
             city=json['city'],
             state=json['state'],
             postal_code=json['postal'],
             country=json['country'],
             domestic_postage_cost=json['postage']['domestic_cost'],
@@ -195,19 +203,21 @@
 
 class Template:
     """Represents an AMcards template."""
     def __init__(
         self,
         id: int,
         name: str,
+        message: str,
         thumbnail: str,
         gifts: List[Gift],
     ) -> None:
         self._id = id
         self._name = name
+        self._message = None if message == 'False' else message
         self._thumbnail = thumbnail
         self._gifts = gifts
         self._gifts_total = sum(gift.total_cost for gift in gifts)
 
     __repr__ = helpers.repr
 
     @property
@@ -217,14 +227,19 @@
 
     @property
     def name(self) -> str:
         """Template's name."""
         return self._name
 
     @property
+    def message(self) -> str:
+        """Template's message on default panel."""
+        return self._message
+
+    @property
     def thumbnail(self) -> str:
         """Template's image thumbnail."""
         return self._thumbnail
 
     @property
     def gifts(self) -> List[Gift]:
         """List of template's :py:class:`gifts <amcards.models.Gift>` (could be an empty list)."""
@@ -236,53 +251,78 @@
         return self._gifts_total
 
     @classmethod
     def _from_json(cls, json: dict):
         return cls(
             id=json['id'],
             name=json['name'],
+            message=json['has_message_on_default_panel'],
             thumbnail=json['thumbnail'],
             gifts=[Gift._from_json(gift_json) for gift_json in json['gifts']],
         )
 
 class Campaign:
     """Represents an AMcards drip campaign."""
     def __init__(
         self,
         id: int,
         name: str,
+        drip_count: int,
         send_if_duplicate: bool,
+        has_anniversary_drip: bool = False,
+        has_birthday_drip: bool = False,
     ) -> None:
         self._id = id
         self._name = name
+        self._drip_count = drip_count
         self._send_if_duplicate = send_if_duplicate
+        self._has_anniversary_drip = has_anniversary_drip
+        self._has_birthday_drip = has_birthday_drip
 
     __repr__ = helpers.repr
 
     @property
     def id(self) -> int:
         """Drip campaign's unique identifier."""
         return self._id
 
     @property
     def name(self) -> str:
         """Drip campaign's name."""
         return self._name
 
     @property
+    def drip_count(self) -> int:
+        """Drip campaign's drip count."""
+        return self._drip_count
+
+    @property
     def send_if_duplicate(self) -> bool:
         """If True, AMcards will not attempt to detect and prevent duplicates. Otherwise, if this campaign has been previously sent to a contact, further campaign send attempts to the same contact will be prevented."""
         return self._send_if_duplicate
 
+    @property
+    def has_anniversary_drip(self) -> bool:
+        """True if one of more drips in this campaign are anniversary drips. False otherwise."""
+        return self._has_anniversary_drip
+
+    @property
+    def has_birthday_drip(self) -> bool:
+        """True if one of more drips in this campaign are birthday drips. False otherwise."""
+        return self._has_birthday_drip
+
     @classmethod
     def _from_json(cls, json: dict):
         return cls(
             id=json['id'],
             name=json['title'],
+            drip_count=json['drip_count'],
             send_if_duplicate=json['send_even_if_duplicate'],
+            has_anniversary_drip=json['has_anniversary_drip'],
+            has_birthday_drip=json['has_birthday_drip'],
         )
 
 class CardStatus(Enum):
     """Represents the status of an AMcards card."""
     EDITABLE = 0
     VERIFYING_ADDRESS = 1
     IN_THE_MAIL = 2
@@ -303,30 +343,36 @@
         status: CardStatus,
         initiator: str,
         send_date: str,
         date_created: datetime,
         date_last_modified: datetime,
         date_fulfilled: datetime,
         is_international: bool,
+        template_name: str,
+        thumbnail: str,
         campaign_id: Optional[int],
         shipping_address: dict,
         return_address: dict,
+        gifts: List[Gift],
     ) -> None:
         self._id = id
         self._amount_charged = amount_charged
         self._status = status
         self._initiator = initiator
         self._send_date = send_date
         self._date_created = date_created
         self._date_last_modified = date_last_modified
         self._date_fulfilled = date_fulfilled
         self._is_international = is_international
+        self._template_name = template_name
+        self._thumbnail = thumbnail
         self._campaign_id = campaign_id
         self._shipping_address = shipping_address
         self._return_address = return_address
+        self._gifts = gifts
 
     __repr__ = helpers.repr
 
     @property
     def id(self) -> int:
         """Card's unique identifier."""
         return self._id
@@ -344,18 +390,28 @@
     @property
     def initiator(self) -> str:
         """Unique identifier of client's user so if multiple users use a single AMcards.com account, a card can be identified per person."""
         return self._initiator
 
     @property
     def send_date(self) -> str:
-        """The date the card is sent. If not specified, the card is scheduled for the day after it was created and the value will be ``None``. The format should be: ``"YYYY-MM-DD"``."""
+        """The date the card is sent. The format should be: ``"YYYY-MM-DD"``."""
         return self._send_date
 
     @property
+    def edit_link(self) -> str:
+        """This is the link to edit the card inside of AMcards.com."""
+        return f'https://amcards.com/cards/edit/{self._id}/'
+
+    @property
+    def cancel_link(self) -> str:
+        """This is the link to cancel the card inside of AMcards.com."""
+        return f'https://amcards.com/cards/cancel/{self._id}/'
+
+    @property
     def date_created(self) -> datetime:
         """Date and time card was created."""
         return self._date_created
 
     @property
     def date_last_modified(self) -> Optional[datetime]:
         """Date and time card was last modified. ``None`` if not modified yet."""
@@ -368,14 +424,24 @@
 
     @property
     def is_international(self) -> bool:
         """If True, card was shipped international. If False, card was shipped domestic."""
         return self._is_international
 
     @property
+    def template_name(self) -> str:
+        """Name of template for this card."""
+        return self._template_name
+
+    @property
+    def thumbnail(self) -> str:
+        """Url of thumbnail for this card."""
+        return self._thumbnail
+
+    @property
     def campaign_id(self) -> Optional[int]:
         """Unique identifier for drip campaign associated with this card. If this card is not a part of a drip campaign, this value will be ``None``."""
         return self._campaign_id
 
     @property
     def shipping_address(self) -> dict:
         """Shipping address for the card.
@@ -414,88 +480,74 @@
                     'postal_code': '48075',                  # OPTIONAL
                     'country': 'US',                         # OPTIONAL
                 }
 
         """
         return self._return_address
 
+    @property
+    def gifts(self) -> List[Gift]:
+        """Gifts attached to this card."""
+        return self._gifts
+
     @classmethod
     def _from_json(cls, json: dict):
         return cls(
             id=json['id'],
             amount_charged=int(json['amount_charged'] * 100),
             status=CardStatus(json['status']),
             initiator=json['initiator'],
             send_date=json['send_date'],
             date_created=helpers.to_datetime(json['created']),
             date_last_modified=helpers.to_datetime(json['last_modified']),
             date_fulfilled=helpers.to_datetime(json['fulfilled']),
             is_international=json['is_international'],
+            template_name=json['template_name'],
+            thumbnail=json['thumbnail'],
             campaign_id=json['campaign_pk'],
             shipping_address=helpers.parse_shipping_address(json),
             return_address=helpers.parse_return_address(json),
+            gifts=[Gift(
+                name=gift['name'],
+                thumbnail='',
+                base_cost=gift['price'],
+                shipping_and_handling_cost=gift['shipping_and_handling'],
+            ) for gift in json['gifts']],
         )
 
 class MailingStatus(Enum):
     """Represents the status of an AMcards mailing."""
     COMPLETE = 0
     PROCESSING = 1
 
 class Mailing:
     """Represents an AMcards mailing."""
     def __init__(
         self,
         id: int,
-        amount_charged: int,
-        cards: List[Card],
-        status: MailingStatus,
-        date_created: datetime,
     ) -> None:
         self._id = id
-        self._amount_charged = amount_charged
-        self._cards = cards
-        self._status = status
-        self._date_created = date_created
 
     __repr__ = helpers.repr
 
     @property
     def id(self) -> int:
         """Mailing's unique identifier."""
         return self._id
 
     @property
-    def amount_charged(self) -> int:
-        """Total amount charged to client's user in `cents`."""
-        return self._amount_charged
+    def mailing_link(self) -> str:
+        """This is the link to the mailing list inside of AMcards.com."""
+        return f'https://amcards.com/cards/history/?mailing={self._id}'
 
-    @property
-    def cards(self) -> List[Card]:
-        """All cards that are a part of this mailing."""
-        return self._cards
-
-    @property
-    def status(self) -> MailingStatus:
-        """Current status of mailing."""
-        return self._status
-
-    @property
-    def date_created(self) -> datetime:
-        """Date and time mailing was created."""
-        return self._date_created
-
-    # @classmethod
-    # def _from_json(cls, json: dict):
-    #     recipients = json['report']['recipients']
-    #     return cls(
-    #         id=json['id'],
-    #         amount_charged=int(json['amount_charged']),
-    #         status=CardStatus(json['status']),
-    #         date_created=helpers.to_datetime(json['created']),
-    #     )
+    @classmethod
+    def _from_json(cls, json: dict):
+        return cls(
+            id=json['id'],
+        )
 
 class Contact:
     """Represents an AMcards contact."""
     def __init__(
         self,
         id: int,
         date_created: datetime,
@@ -694,14 +746,24 @@
 
     @property
     def card_id(self) -> int:
         """Unique id for the :py:class:`card <amcards.models.Card>` created."""
         return self._card_id
 
     @property
+    def edit_link(self) -> str:
+        """This is the link to edit the card inside of AMcards.com."""
+        return f'https://amcards.com/cards/edit/{self._card_id}/'
+
+    @property
+    def cancel_link(self) -> str:
+        """This is the link to cancel the card inside of AMcards.com."""
+        return f'https://amcards.com/cards/cancel/{self._card_id}/'
+
+    @property
     def total_cost(self) -> int:
         """Total cost the client's user was charged in `cents`."""
         return self._total_cost
 
     @property
     def user_email(self) -> str:
         """Client's user email."""
@@ -747,14 +809,19 @@
 
     @property
     def mailing_id(self) -> int:
         """Unique id for the :py:class:`mailing <amcards.models.Mailing>` created."""
         return self._mailing_id
 
     @property
+    def mailing_link(self) -> str:
+        """This is the link to the mailing list inside of AMcards.com."""
+        return f'https://amcards.com/cards/history/?mailing={self._mailing_id}'
+
+    @property
     def card_ids(self) -> List[int]:
         """List of unique ids for the :py:class:`cards <amcards.models.Card>` created."""
         return self._card_ids
 
     @property
     def user_email(self) -> str:
         """Client's user email."""
@@ -819,8 +886,101 @@
     @classmethod
     def _from_json(cls, json: dict):
         return cls(
             mailing_id=int(json['mailing_uri'][17:-1]),
             user_email=json['user'],
             message=json['message'],
             shipping_addresses=json['shipping_addresses'],
-        )
+        )
+
+class CreditTransaction:
+    """Represents an AMcards CreditTransaction."""
+    def __init__(
+        self,
+        id: int,
+        wallet_id: str,
+        amount_granted: int,
+        amount_before: int,
+        amount_after: int,
+        amount_paid: int,
+        amount: int,
+        description: str,
+        credit_card_details: str,
+        date_created: datetime,
+    ) -> None:
+        self._id = id
+        self._wallet_id = wallet_id
+        self._amount_granted = amount_granted
+        self._amount_before = amount_before
+        self._amount_after = amount_after
+        self._amount_paid = amount_paid
+        self._amount = amount
+        self._description = description
+        self._credit_card_details = credit_card_details
+        self._date_created = date_created
+
+    __repr__ = helpers.repr
+
+    @property
+    def id(self) -> int:
+        """CreditTransaction's unique identifier."""
+        return self._id
+
+    @property
+    def wallet_id(self) -> str:
+        """CreditTransaction's wallet id."""
+        return self._wallet_id
+
+    @property
+    def amount_granted(self) -> int:
+        """CreditTransaction's amount granted in `cents`."""
+        return self._amount_granted
+
+    @property
+    def amount_before(self) -> int:
+        """CreditTransaction's amount before in `cents`."""
+        return self._amount_before
+
+    @property
+    def amount_after(self) -> int:
+        """CreditTransaction's amount after in `cents`."""
+        return self._amount_after
+
+    @property
+    def amount_paid(self) -> int:
+        """CreditTransaction's amount paid in `cents`."""
+        return self._amount_paid
+
+    @property
+    def amount(self) -> int:
+        """CreditTransaction's amount in `cents`."""
+        return self._amount
+
+    @property
+    def description(self) -> str:
+        """CreditTransaction's description."""
+        return self._description
+
+    @property
+    def credit_card_details(self) -> str:
+        """CreditTransaction's credit card details."""
+        return self._credit_card_details
+
+    @property
+    def date_created(self) -> datetime:
+        """Date and time CreditTransaction was created."""
+        return self._date_created
+
+    @classmethod
+    def _from_json(cls, json: dict):
+        return cls(
+            id=int(json['id']),
+            wallet_id=json['wallet_id'],
+            amount_granted=json['grant_volume'],
+            amount_before=json['before_int'],
+            amount_after=json['after_int'],
+            amount_paid=json['amount_paid_int'],
+            amount=json['amount_int'],
+            description=json['description'],
+            credit_card_details=json['credit_card_details'],
+            date_created=helpers.to_datetime(json['date_time']),
+        )
```

### Comparing `python-amcards-1.2.9/python_amcards.egg-info/PKG-INFO` & `python_amcards-1.3.0/python_amcards.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.2.9
+Version: 1.3.0
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: requests>=2
 
 Getting Started | See the full docs at `Read the Docs <https://python-amcards.readthedocs.io/en/latest/>`_
 ==========================================================================================================
 .. image:: https://i.ibb.co/tCrVfj6/readthedocs.png
     :target: https://python-amcards.readthedocs.io/en/latest/
 
 Installation
@@ -34,15 +35,15 @@
 First, create an `AMcardsClient <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_ as follows:
 
 .. code-block::
 
     >>> from amcards import AMcardsClient
     >>> client = AMcardsClient('youraccesstoken')
 
-Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/connected-applications/>`_.
+Here ``'youraccesstoken'`` will be replaced with a string containing your AMcards access token. You can generate one `here <https://amcards.com/user/generate-access-token/>`_.
 
 Now we can perform all operations supported by the `client <https://python-amcards.readthedocs.io/en/latest/amcards.html#amcards.amcards.AMcardsClient>`_.
 
 Let's try using ``send_card`` to send a card to a single recipient:
 
 .. code-block::
```

### Comparing `python-amcards-1.2.9/setup.py` & `python_amcards-1.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def README():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='python-amcards',
-    version='1.2.9',
+    version='1.3.0',
     description='A wrapper for the AMcards API.',
     long_description=README(),
     long_description_content_type='text/x-rst',
     author='Simone Sestili',
     author_email='simone.sestili@amcards.com',
     url='https://github.com/simonesestili/python-amcards',
     packages=['amcards'],
```

