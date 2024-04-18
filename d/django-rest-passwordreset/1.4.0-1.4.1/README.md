# Comparing `tmp/django-rest-passwordreset-1.4.0.tar.gz` & `tmp/django-rest-passwordreset-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-passwordreset-1.4.0.tar", last modified: Fri Feb  9 15:59:40 2024, max compression
+gzip compressed data, was "django-rest-passwordreset-1.4.1.tar", last modified: Thu Apr 18 20:17:23 2024, max compression
```

## Comparing `django-rest-passwordreset-1.4.0.tar` & `django-rest-passwordreset-1.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.178919 django-rest-passwordreset-1.4.0/django_rest_passwordreset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.178919 django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.178919 django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.178919 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0002_pk_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0004_alter_resetpasswordtoken_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.178919 django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-02-09 15:59:40.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-09 15:59:40.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 15:59:40.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-09 15:59:40.000000 django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    58293 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/docs/browsable_api_email_validation.png
--rw-r--r--   0 runner    (1001) docker     (127)    60179 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/docs/browsable_api_password_validation.png
--rw-r--r--   0 runner    (1001) docker     (127)    79223 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/docs/coreapi_docs.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/settings_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:40.182919 django-rest-passwordreset-1.4.0/tests/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22091 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/test/test_auth_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/test/test_token_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-09 15:59:31.000000 django-rest-passwordreset-1.4.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.363056 django-rest-passwordreset-1.4.1/django_rest_passwordreset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.363056 django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0002_pk_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0004_alter_resetpasswordtoken_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.363056 django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-18 20:17:23.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 20:17:23.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:17:23.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 20:17:23.000000 django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    58293 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/docs/browsable_api_email_validation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60179 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/docs/browsable_api_password_validation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79223 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/docs/coreapi_docs.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/settings_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:23.367056 django-rest-passwordreset-1.4.1/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/test/test_auth_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/test/test_token_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-18 20:17:14.000000 django-rest-passwordreset-1.4.1/tests/urls.py
```

### Comparing `django-rest-passwordreset-1.4.0/LICENSE` & `django-rest-passwordreset-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/PKG-INFO` & `django-rest-passwordreset-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-passwordreset
-Version: 1.4.0
+Version: 1.4.1
 Summary: An extension of django rest framework, providing a configurable password reset strategy
 Home-page: https://github.com/anexia-it/django-rest-passwordreset
 Author: Harald Nezbeda
 Author-email: HNezbeda@anexia-it.com
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-rest-passwordreset-1.4.0/README.md` & `django-rest-passwordreset-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0001_initial.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0002_pk_migration.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0002_pk_migration.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/models.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/models.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/serializers.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/tokens.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/tokens.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/urls.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/urls.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset/views.py` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,22 @@
     # to change their password (e.g., LDAP user)
     for user in users:
         if user.eligible_for_reset():
             active_user_found = True
             break
 
     # No active user found, raise a ValidationError
-    # but not if DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE == True
-    if not active_user_found and not getattr(settings, 'DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE', False):
-        raise exceptions.ValidationError({
-            'email': [_(
-                "We couldn't find an account associated with that email. Please try a different e-mail address.")],
-        })
+    # but not if DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE == True, in that case we return None
+    if not active_user_found:
+        if not getattr(settings, 'DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE', False):
+            raise exceptions.ValidationError({
+                'email': [_(
+                    "We couldn't find an account associated with that email. Please try a different e-mail address.")],
+            })
+        return None
 
     # last but not least: iterate over all users that are active and can change their password
     # and create a Reset Password Token and send a signal with the created token
     for user in users:
         if user.eligible_for_reset() and _unicode_ci_compare(email, getattr(user, get_password_reset_lookup_field())):
             password_reset_tokens = user.password_reset_tokens.all()
 
@@ -195,17 +197,21 @@
         clear_expired_tokens()
         token = generate_token_for_email(
             email=serializer.validated_data['email'],
             user_agent=request.META.get(HTTP_USER_AGENT_HEADER, ''),
             ip_address=request.META.get(HTTP_IP_ADDRESS_HEADER, ''),
         )
 
-        # send a signal that the password token was created
-        # let whoever receives this signal handle sending the email for the password reset
-        reset_password_token_created.send(sender=self.__class__, instance=self, reset_password_token=token)
+        if token:
+            # send a signal that the password token was created
+            # let whoever receives this signal handle sending the email for the password reset
+            reset_password_token_created.send(
+                sender=self.__class__,
+                instance=self, reset_password_token=token
+            )
 
         return Response({'status': 'OK'})
 
 
 class ResetPasswordValidateTokenViewSet(ResetPasswordValidateToken, GenericViewSet):
     """
     An Api ViewSet which provides a method to verify that a token is valid
```

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/PKG-INFO` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-passwordreset
-Version: 1.4.0
+Version: 1.4.1
 Summary: An extension of django rest framework, providing a configurable password reset strategy
 Home-page: https://github.com/anexia-it/django-rest-passwordreset
 Author: Harald Nezbeda
 Author-email: HNezbeda@anexia-it.com
 License: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-rest-passwordreset-1.4.0/django_rest_passwordreset.egg-info/SOURCES.txt` & `django-rest-passwordreset-1.4.1/django_rest_passwordreset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/docs/browsable_api_email_validation.png` & `django-rest-passwordreset-1.4.1/docs/browsable_api_email_validation.png`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/docs/browsable_api_password_validation.png` & `django-rest-passwordreset-1.4.1/docs/browsable_api_password_validation.png`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/docs/coreapi_docs.png` & `django-rest-passwordreset-1.4.1/docs/coreapi_docs.png`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/setup.py` & `django-rest-passwordreset-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/tests/manage.py` & `django-rest-passwordreset-1.4.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/tests/settings.py` & `django-rest-passwordreset-1.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/tests/test/helpers.py` & `django-rest-passwordreset-1.4.1/tests/test/helpers.py`

 * *Files identical despite different names*

### Comparing `django-rest-passwordreset-1.4.0/tests/test/test_auth_test_case.py` & `django-rest-passwordreset-1.4.1/tests/test/test_auth_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,21 +356,23 @@
         self.assertIn('reset_password_token', mock_post_password_reset.call_args[1])
         self.assertEqual(mock_post_password_reset.call_args[1]['reset_password_token'], token1)
         self.assertTrue(mock_pre_password_reset.called)
         self.assertIn('reset_password_token', mock_pre_password_reset.call_args[1])
         self.assertEqual(mock_pre_password_reset.call_args[1]['reset_password_token'], token1)
 
     @override_settings(DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE=True)
-    def test_try_reset_password_email_does_not_exist_no_leakage_enabled(self):
+    @patch('django_rest_passwordreset.signals.reset_password_token_created.send')
+    def test_try_reset_password_email_does_not_exist_no_leakage_enabled(self, mock_reset_signal):
         """
         Tests requesting a token for an email that does not exist when
         DJANGO_REST_PASSWORDRESET_NO_INFORMATION_LEAKAGE == True
         """
         response = self.rest_do_request_reset_token(email="foobar@doesnotexist.com")
         self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertFalse(mock_reset_signal.called)
 
     def test_user_without_password(self):
         """ Tests requesting a token for an email without a password doesn't work"""
         response = self.rest_do_request_reset_token(email="user4@mail.com")
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
         decoded_response = json.loads(response.content.decode())
         # response should have "email" in it
```

### Comparing `django-rest-passwordreset-1.4.0/tests/test/test_token_generators.py` & `django-rest-passwordreset-1.4.1/tests/test/test_token_generators.py`

 * *Files identical despite different names*

