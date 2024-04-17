# Comparing `tmp/django_azure_auth-1.1.0.tar.gz` & `tmp/django_azure_auth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.1.0.tar", max compression
+gzip compressed data, was "django_azure_auth-1.2.0.tar", max compression
```

## Comparing `django_azure_auth-1.1.0.tar` & `django_azure_auth-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/LICENSE
--rw-r--r--   0        0        0     3627 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/backends.py
--rw-r--r--   0        0        0      529 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/exceptions.py
--rw-r--r--   0        0        0     5491 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/handlers.py
--rw-r--r--   0        0        0     1148 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     1937 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3797 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1329 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     1805 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    10151 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/urls.py
--rw-r--r--   0        0        0      732 2023-03-19 13:26:46.388903 django_azure_auth-1.1.0/azure_auth/views.py
--rw-r--r--   0        0        0     1439 2023-03-19 13:26:46.392903 django_azure_auth-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4536 1970-01-01 00:00:00.000000 django_azure_auth-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4897 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/backends.py
+-rw-r--r--   0        0        0      529 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     6434 2024-04-17 22:31:40.077509 django_azure_auth-1.2.0/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1148 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1329 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     1805 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    11068 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/urls.py
+-rw-r--r--   0        0        0      732 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/azure_auth/views.py
+-rw-r--r--   0        0        0     1439 2024-04-17 22:31:40.081509 django_azure_auth-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 django_azure_auth-1.2.0/PKG-INFO
```

### Comparing `django_azure_auth-1.1.0/LICENSE` & `django_azure_auth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/decorators.py` & `django_azure_auth-1.2.0/azure_auth/decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/handlers.py` & `django_azure_auth-1.2.0/azure_auth/handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from http import HTTPStatus
 
 import msal
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group
 
 from azure_auth.exceptions import DjangoAzureAuthException, TokenError
 
 UserModel = get_user_model()
 
 
 class AuthHandler:
@@ -93,15 +94,31 @@
             user = UserModel._default_manager.get_by_natural_key(email)
         except UserModel.DoesNotExist:
             user = UserModel._default_manager.create_user(username=email, email=email)
             user.first_name = attr if (attr := azure_user["givenName"]) else ""
             user.last_name = attr if (attr := azure_user["surname"]) else ""
             user.save()
 
-        # TODO: Handle groups
+        # Syncing azure token claim roles with django user groups
+        # A role mapping in the AZURE_AUTH settings is expected.
+        role_mappings = settings.AZURE_AUTH.get("ROLES")
+        azure_token_roles = token.get("id_token_claims", {}).get("roles", None)
+        if role_mappings and azure_token_roles:
+            for role, group_name in role_mappings.items():
+                # all groups are created by default if they not exist
+                django_group = Group.objects.get_or_create(name=group_name)[0]
+
+                if role in azure_token_roles:
+                    # Add user with permissions to the corresponding django group
+                    user.groups.add(django_group)
+                else:
+                    # No permission so check if user is in group and remove
+                    if user.groups.filter(name=group_name).exists():
+                        user.groups.remove(django_group)
+
         return user
 
     @staticmethod
     def get_logout_uri() -> str:
         """
         Forms the URI to log the user out in the Active Directory app and
         redirect to the webapp logout page.
```

### Comparing `django_azure_auth-1.1.0/azure_auth/middleware.py` & `django_azure_auth-1.2.0/azure_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/conftest.py` & `django_azure_auth-1.2.0/azure_auth/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,13 +53,14 @@
             "oid": "dummy_id_token_claims_oid",
             "preferred_username": "dummy_id_token_claims_preferred_username",
             "rh": "dummy_id_token_claims_rh",
             "sub": "dummy_id_token_claims_sub",
             "tid": "dummy_id_token_claims_tid",
             "uti": "dummy_id_token_claims_uti",
             "ver": "2.0",
+            "roles": ["95170e67-2bbf-4e3e-a4d7-e7e5829fe7a7"],
         },
     }
 
     if request.cls:
         request.cls.token = _token
     return _token
```

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/settings.py` & `django_azure_auth-1.2.0/azure_auth/tests/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,10 +132,14 @@
     "CLIENT_SECRET": "dummy_client_secret",
     "REDIRECT_URI": "http://mydomain/azure_auth/callback",
     "SCOPES": ["User.Read"],
     "AUTHORITY": "https://login.microsoftonline.com/dummy_tenant_id",
     "LOGOUT_URI": "http://mydomain/logout",
     "PUBLIC_URLS": ["public", "decorator_protected"],
     "PUBLIC_PATHS": ["/public_external"],
+    "ROLES": {
+        "95170e67-2bbf-4e3e-a4d7-e7e5829fe7a7": "GroupName1",
+        "3dc6539e-0589-4663-b782-fef100d839aa": "GroupName2",
+    },
 }
 LOGIN_URL = "/azure_auth/login"
 LOGIN_REDIRECT_URL = "/"
```

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.2.0/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.2.0/azure_auth/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/test_views.py` & `django_azure_auth-1.2.0/azure_auth/tests/test_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from http import HTTPStatus
 from unittest.mock import patch
 
 import msal
 import pytest
 from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group
 from django.test import TestCase, TransactionTestCase, override_settings
 from django.urls import reverse
 from mixer.backend.django import Mixer
 
 from azure_auth.exceptions import TokenError
 from azure_auth.handlers import AuthHandler
 
@@ -57,14 +58,19 @@
         super().setUp()
         # Store in variable first
         # https://docs.djangoproject.com/en/4.0/topics/testing/tools/
         session = self.client.session
         session["auth_flow"] = self.auth_flow
         session.save()
 
+        # Adds a group to existing user that is not part of the token.
+        # Should be removed automatically during authentication.
+        dummy_group = Group.objects.get_or_create(name="GroupName2")[0]
+        self.user.groups.add(dummy_group)
+
     def _mocked_response(self, code, json):
         class MockResponse:
             def __init__(self, status_code, data):
                 self.status_code = status_code
                 self.data = data
                 self.ok = True if self.status_code == 200 else False
 
@@ -121,14 +127,20 @@
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FOUND
         assert resp.url == settings.LOGIN_REDIRECT_URL
         assert "id_token_claims" in self.client.session
 
+        # Group creation checks in existing user
+        assert Group.objects.filter(name="GroupName1").exists()
+        assert Group.objects.filter(name="GroupName2").exists()
+        assert self.user.groups.filter(name="GroupName1").exists()
+        assert not self.user.groups.filter(name="GroupName2").exists()
+
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
 
     def test_callback_new_user(self, mocked_msal_app, mocked_requests, mocked_cache):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
             self.token
         )
@@ -156,14 +168,20 @@
 
         # User creation checks
         created_user = UserModel.objects.get(email=new_user.email)
         assert created_user.username == new_user.email
         assert created_user.first_name == new_user.first_name
         assert created_user.last_name == new_user.last_name
 
+        # Group creation checks
+        assert Group.objects.filter(name="GroupName1").exists()
+        assert Group.objects.filter(name="GroupName2").exists()
+        assert created_user.groups.filter(name="GroupName1").exists()
+        assert not created_user.groups.filter(name="GroupName2").exists()
+
     def test_callback_acquire_token_error(self, mocked_msal_app, *args):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = {
             "error": "dummy_error",
             "error_description": "dummy_error_description",
         }
 
         with pytest.raises(TokenError) as exc:
```

### Comparing `django_azure_auth-1.1.0/azure_auth/tests/urls.py` & `django_azure_auth-1.2.0/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/azure_auth/views.py` & `django_azure_auth-1.2.0/azure_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.1.0/pyproject.toml` & `django_azure_auth-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.1.0"
+version = "1.2.0"
 description = "A simple Django app for user authentication with Azure Active Directory."
 authors = ["AgileTek Engineering <london@agiletek.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/AgileTek/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft']
 classifiers = [
```

### Comparing `django_azure_auth-1.1.0/PKG-INFO` & `django_azure_auth-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: django-azure-auth
-Version: 1.1.0
-Summary: A simple Django app for user authentication with Azure Active Directory.
-Home-page: https://github.com/AgileTek/django-azure-auth
-License: MIT
-Keywords: django,azure,authentication,microsoft
-Author: AgileTek Engineering
-Author-email: london@agiletek.co.uk
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=3.2)
-Requires-Dist: msal (>=1.18.0,<2.0.0)
-Description-Content-Type: text/markdown
-
 ![Build](https://github.com/AgileTek/django-azure-auth/actions/workflows/push-actions.yml/badge.svg)
 
 # Django Azure Auth
 
 A simple Django app for user authentication with Azure Active Directory.
 
 ## Description
@@ -65,14 +42,18 @@
     "CLIENT_SECRET": "<client secret>",
     "REDIRECT_URI": "https://<domain>/azure_auth/callback",
     "SCOPES": ["User.Read"],
     "AUTHORITY": "https://login.microsoftonline.com/<tenant id>",   # Or https://login.microsoftonline.com/common if multi-tenant
     "LOGOUT_URI": "https://<domain>/logout",    # Optional
     "PUBLIC_URLS": ["<public:view_name>",]  # Optional, public views accessible by non-authenticated users
     "PUBLIC_PATHS": ['/go/',],  # Optional, public paths accessible by non-authenticated users
+    "ROLES": {
+        "95170e67-2bbf-4e3e-a4d7-e7e5829fe7a7": "GroupName1",
+        "3dc6539e-0589-4663-b782-fef100d839aa": "GroupName2"
+    }  # Optional, will add user to django group if user is in EntraID group
 }
 LOGIN_URL = "/azure_auth/login"
 LOGIN_REDIRECT_URL = "/"    # Or any other endpoint
 ```
 
 #### Note: You should obfuscate the credentials by using environment variables.
 
@@ -138,22 +119,36 @@
 ```
 
 Make sure you add the middleware after Django's `session` and `authentication` middlewares so
 that the request includes the session and user objects. Public URLs which need to be accessed by
 non-authenticated users should be specified in the `settings.AZURE_AUTH["PUBLIC_URLS"]`, as
 shown above.
 
-## Planned development
-
-- Groups management
+## Groups Management
+Adding a group to the Azure Enterprise application will pass the group id down to the application via the token.
+This happens only, if the user is part of the group. In this case the group will be listed in the `token`.
+
+On how to configure this in Azure see here: https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/how-to-connect-fed-group-claims
+
+Groups available in the token are synced with the corresponding django groups. Therfor the group id's from Azure need to be mapped in the 
+settings with the Django groups by adding the following to `AZURE_AUTH` in `settings`.
+```
+"ROLES": {
+        "95170e67-2bbf-4e3e-a4d7-e7e5829fe7a7": "GroupName1",
+        "3dc6539e-0589-4663-b782-fef100d839aa": "GroupName2"
+    }
+```
+If a user is assigned to one or more of this groups listed in the configuration, the user will be added
+automatically to the respective Django group. The group will be created if it does not exist. 
+If a user is not part of a group (revoke permissions case), but is still in the Django group, the user
+will be removed from the Django group. 
 
 ## Credits
 
 This app is heavily inspired by and builds on functionality in
 https://github.com/shubhamdipt/django-microsoft-authentication, with both feature
 improvements and code assurance through testing.
 
 Credit also to:
 
 - https://github.com/Azure-Samples/ms-identity-python-webapp
 - https://github.com/AzMoo/django-okta-auth
-
```

