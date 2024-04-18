# Comparing `tmp/djangoldp_esa-2.0.0.tar.gz` & `tmp/djangoldp_esa-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_esa-2.0.0.tar", last modified: Tue Oct 17 18:08:28 2023, max compression
+gzip compressed data, was "djangoldp_esa-2.0.1.tar", last modified: Thu Apr 18 15:01:40 2024, max compression
```

## Comparing `djangoldp_esa-2.0.0.tar` & `djangoldp_esa-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      275 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.958560 djangoldp_esa-2.0.0/djangoldp_esa/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-10-17 18:08:25.000000 djangoldp_esa-2.0.0/djangoldp_esa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    11189 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/migrations/0002_auto_20220623_1611.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/migrations/0003_auto_20220627_1354.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 18:08:06.000000 djangoldp_esa-2.0.0/djangoldp_esa/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6127 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/admin/login.html
--rw-rw-rw-   0 root         (0) root         (0)    10587 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     2617 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)    11036 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/password/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)     2728 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)    10225 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 18:08:28.958560 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2023-10-17 18:08:28.000000 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1029 2023-10-17 18:08:28.000000 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 18:08:28.000000 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-10-17 18:08:28.000000 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-17 18:08:28.000000 djangoldp_esa-2.0.0/djangoldp_esa.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-10-17 18:08:28.962561 djangoldp_esa-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-10-17 18:08:05.000000 djangoldp_esa-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.133991 djangoldp_esa-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 15:01:40.133991 djangoldp_esa-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-18 15:01:37.000000 djangoldp_esa-2.0.1/djangoldp_esa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    10770 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/migrations/0002_auto_20220623_1611.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/migrations/0003_auto_20220627_1354.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6128 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/admin/login.html
+-rw-rw-rw-   0 root         (0) root         (0)    10587 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.133991 djangoldp_esa-2.0.1/djangoldp_esa/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/password/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.133991 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)    10225 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:01:40.129991 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-18 15:01:40.000000 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1000 2024-04-18 15:01:40.000000 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 15:01:40.000000 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-18 15:01:40.000000 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 15:01:40.000000 djangoldp_esa-2.0.1/djangoldp_esa.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-18 15:01:40.133991 djangoldp_esa-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-18 15:01:19.000000 djangoldp_esa-2.0.1/setup.py
```

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/admin.py` & `djangoldp_esa-2.0.1/djangoldp_esa/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/migrations/0001_initial.py` & `djangoldp_esa-2.0.1/djangoldp_esa/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaBicLocation',
                 'container_path': 'esa-locations/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaBicPosition',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -52,15 +51,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaBicPosition',
                 'container_path': 'esa-positions/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaCommunity',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -83,17 +81,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:CommunityEsaProfile',
                 'container_path': '/esaprofiles/',
                 'permission_classes': [djangoldp_esa.permissions.EsaCommunityProfilePermissions],
                 'serializer_fields': ['@id', 'company_name', 'main_contact_first_name', 'main_contact_last_name', 'company_description', 'tags', 'role', 'sectors', 'spaces', 'status', 'graduation_year', 'esa_bic_position', 'location_esa_bic'],
                 'depth': 1,
-                'anonymous_perms': ['view'],
-                'authenticated_perms': ['inherit', 'add'],
-                'superuser_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaCommunityRole',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -107,15 +102,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaRole',
                 'container_path': 'esa-roles/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaCommunityTag',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -130,15 +124,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaTag',
                 'container_path': 'esa-tags/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaCommunitySpace',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -153,15 +146,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaSpace',
                 'container_path': 'esa-spaces/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.CreateModel(
             name='EsaCommunitySector',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('urlid', djangoldp.fields.LDPUrlField(blank=True, null=True, unique=True)),
@@ -176,15 +168,14 @@
                 'abstract': False,
                 'default_permissions': ['add', 'change', 'delete', 'view', 'control'],
                 'rdf_type': 'sib:EsaSector',
                 'container_path': 'esa-sectors/',
                 'serializer_fields': ['@id', 'name'],
                 'nested_fields': [],
                 'depth': 0,
-                'anonymous_perms': ['view'],
             },
         ),
         migrations.AddField(
             model_name='esacommunity',
             name='role',
             field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='tags', to='djangoldp_esa.EsaCommunityRole'),
         ),
```

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/migrations/0002_auto_20220623_1611.py` & `djangoldp_esa-2.0.1/djangoldp_esa/migrations/0002_auto_20220623_1611.py`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/models.py` & `djangoldp_esa-2.0.1/djangoldp_esa/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from django.conf import settings
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
 
+from djangoldp.permissions import InheritPermissions, AnonymousReadOnly
 from djangoldp.models import Model
 from djangoldp_community.models import Community
-from djangoldp_esa.permissions import EsaCommunityProfilePermissions
 
 
 class EsaCommunityRole(Model):
     name = models.CharField(max_length=254, blank=True, null=True, default='')
 
     def __str__(self):
         try:
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA Role')
         verbose_name_plural = _("ESA Roles")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-roles/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaRole"
 
 
 class EsaBicPosition(Model):
@@ -36,15 +36,15 @@
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA-BIC Position')
         verbose_name_plural = _("ESA-BIC Positions")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-positions/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaBicPosition"
 
 
 class EsaBicLocation(Model):
@@ -55,15 +55,15 @@
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA-BIC Location')
         verbose_name_plural = _("ESA-BIC Locations")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-locations/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaBicLocation"
 
 
 STATUS_CHOICES = [
@@ -96,18 +96,17 @@
             return '{} ({})'.format(self.community.urlid, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA Profile')
         verbose_name_plural = _("ESA Profiles")
-        permission_classes = [EsaCommunityProfilePermissions]
-        anonymous_perms = ['view']
-        authenticated_perms = ['inherit', 'add']
-        superuser_perms = ['view']
+        permission_classes = [InheritPermissions]
+        inherit_permissions = ['community']
+
         ordering = ['community']
         container_path = "/esaprofiles/"
         serializer_fields = ['@id', 'main_contact_first_name', 'main_contact_last_name', 'tags',
                              'role', 'sectors', 'spaces', 'status', 'graduation_year', 'position_esa_bic', 'location_esa_bic']
         rdf_type = "sib:CommunityEsaProfile"
         depth = 1
 
@@ -122,15 +121,15 @@
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA Tag')
         verbose_name_plural = _("ESA Tags")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-tags/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaTag"
 
 
 class EsaCommunitySector(Model):
@@ -143,15 +142,15 @@
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA Sector')
         verbose_name_plural = _("ESA Sectors")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-sectors/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaSector"
 
 
 class EsaCommunitySpace(Model):
@@ -164,15 +163,15 @@
             return '{} ({})'.format(self.name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
         verbose_name = _('ESA Space')
         verbose_name_plural = _("ESA Spaces")
-        anonymous_perms = ['view']
+        permission_classes = [AnonymousReadOnly]
         container_path = "esa-spaces/"
         serializer_fields = ['@id', 'name']
         nested_fields = []
         rdf_type = "sib:EsaSpace"
 
 
 @receiver(post_save, sender=Community)
```

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/admin/login.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/email.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/oidc_provider/authorize.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/password/email.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/login.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_confirm.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_done.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_email.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa/templates/registration/password_reset_form.html` & `djangoldp_esa-2.0.1/djangoldp_esa/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_esa-2.0.0/djangoldp_esa.egg-info/SOURCES.txt` & `djangoldp_esa-2.0.1/djangoldp_esa.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 setup.cfg
 setup.py
 djangoldp_esa/__init__.py
 djangoldp_esa/admin.py
 djangoldp_esa/apps.py
 djangoldp_esa/models.py
-djangoldp_esa/permissions.py
 djangoldp_esa/settings.py
 djangoldp_esa.egg-info/PKG-INFO
 djangoldp_esa.egg-info/SOURCES.txt
 djangoldp_esa.egg-info/dependency_links.txt
 djangoldp_esa.egg-info/requires.txt
 djangoldp_esa.egg-info/top_level.txt
 djangoldp_esa/migrations/0001_initial.py
```

### Comparing `djangoldp_esa-2.0.0/setup.cfg` & `djangoldp_esa-2.0.1/setup.cfg`

 * *Files identical despite different names*

