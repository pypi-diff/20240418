# Comparing `tmp/netbox_software-0.2.5.tar.gz` & `tmp/netbox_software-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.2.5.tar", max compression
+gzip compressed data, was "netbox_software-0.2.6.tar", max compression
```

## Comparing `netbox_software-0.2.5.tar` & `netbox_software-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.5/LICENSE
--rw-r--r--   0        0        0     3420 2023-07-24 10:08:36.275629 netbox_software-0.2.5/README.md
--rw-r--r--   0        0        0      534 2023-07-24 10:08:36.287629 netbox_software-0.2.5/netbox_software/__init__.py
--rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.5/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.5/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.5/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.5/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1357 2023-07-13 10:00:09.172753 netbox_software-0.2.5/netbox_software/api/views.py
--rw-r--r--   0        0        0     4830 2023-07-24 09:37:34.463592 netbox_software-0.2.5/netbox_software/filtersets.py
--rw-r--r--   0        0        0     5962 2023-07-24 09:38:12.495597 netbox_software-0.2.5/netbox_software/forms.py
--rw-r--r--   0        0        0     6329 2023-12-19 15:36:58.535655 netbox_software-0.2.5/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.5/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     7032 2023-12-11 12:33:01.474472 netbox_software-0.2.5/netbox_software/models.py
--rw-r--r--   0        0        0     3445 2024-03-05 07:33:13.671697 netbox_software-0.2.5/netbox_software/navigation.py
--rw-r--r--   0        0        0     1148 2023-07-13 14:24:33.277294 netbox_software-0.2.5/netbox_software/search.py
--rw-r--r--   0        0        0     4452 2023-07-13 11:47:12.302581 netbox_software-0.2.5/netbox_software/tables.py
--rw-r--r--   0        0        0     5789 2023-07-24 09:51:25.461957 netbox_software-0.2.5/netbox_software/template_content.py
--rw-r--r--   0        0        0     1889 2023-07-24 11:23:15.074495 netbox_software-0.2.5/netbox_software/templates/netbox_software/application.html
--rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.5/netbox_software/templates/netbox_software/application_edit.html
--rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.5/netbox_software/templates/netbox_software/applicationversion.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.5/netbox_software/templates/netbox_software/applicationversion_edit.html
--rw-r--r--   0        0        0     1704 2023-07-13 10:48:52.323169 netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0     2108 2023-07-13 10:27:29.270544 netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     3413 2024-03-05 07:46:18.314014 netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.5/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0     1116 2023-07-13 11:11:57.226346 netbox_software-0.2.5/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.5/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1691 2023-07-13 11:40:24.952229 netbox_software-0.2.5/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.5/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     3525 2023-07-13 10:14:12.001988 netbox_software-0.2.5/netbox_software/urls.py
--rw-r--r--   0        0        0     5533 2024-03-05 07:33:13.679697 netbox_software-0.2.5/netbox_software/views.py
--rw-r--r--   0        0        0      318 2024-03-05 07:54:20.245561 netbox_software-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3420 2023-07-24 10:08:36.275629 netbox_software-0.2.6/README.md
+-rw-r--r--   0        0        0      534 2023-07-24 10:08:36.287629 netbox_software-0.2.6/netbox_software/__init__.py
+-rw-r--r--   0        0        0      699 2023-07-13 07:09:13.118198 netbox_software-0.2.6/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.2.6/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     4757 2023-07-13 08:04:55.519077 netbox_software-0.2.6/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      445 2023-07-13 08:04:55.499076 netbox_software-0.2.6/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1357 2023-07-13 10:00:09.172753 netbox_software-0.2.6/netbox_software/api/views.py
+-rw-r--r--   0        0        0     4830 2023-07-24 09:37:34.463592 netbox_software-0.2.6/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     5962 2023-07-24 09:38:12.495597 netbox_software-0.2.6/netbox_software/forms.py
+-rw-r--r--   0        0        0     7032 2023-12-11 12:33:01.474472 netbox_software-0.2.6/netbox_software/models.py
+-rw-r--r--   0        0        0     3467 2024-04-18 07:14:33.974014 netbox_software-0.2.6/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1148 2023-07-13 14:24:33.277294 netbox_software-0.2.6/netbox_software/search.py
+-rw-r--r--   0        0        0     4452 2023-07-13 11:47:12.302581 netbox_software-0.2.6/netbox_software/tables.py
+-rw-r--r--   0        0        0     5789 2023-07-24 09:51:25.461957 netbox_software-0.2.6/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1889 2023-07-24 11:23:15.074495 netbox_software-0.2.6/netbox_software/templates/netbox_software/application.html
+-rw-r--r--   0        0        0      613 2023-07-13 07:50:20.328737 netbox_software-0.2.6/netbox_software/templates/netbox_software/application_edit.html
+-rw-r--r--   0        0        0      669 2023-07-13 07:39:13.081944 netbox_software-0.2.6/netbox_software/templates/netbox_software/applicationversion.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.6/netbox_software/templates/netbox_software/applicationversion_edit.html
+-rw-r--r--   0        0        0     1704 2023-07-13 10:48:52.323169 netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0     2108 2023-07-13 10:27:29.270544 netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     3413 2024-03-05 07:46:18.314014 netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.2.6/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0     1116 2023-07-13 11:11:57.226346 netbox_software-0.2.6/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.6/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1691 2023-07-13 11:40:24.952229 netbox_software-0.2.6/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.2.6/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     3525 2023-07-13 10:14:12.001988 netbox_software-0.2.6/netbox_software/urls.py
+-rw-r--r--   0        0        0     5618 2024-04-18 07:10:53.398361 netbox_software-0.2.6/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2024-04-18 07:19:56.195707 netbox_software-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.2.6/PKG-INFO
```

### Comparing `netbox_software-0.2.5/LICENSE` & `netbox_software-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/README.md` & `netbox_software-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/__init__.py` & `netbox_software-0.2.6/netbox_software/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/admin.py` & `netbox_software-0.2.6/netbox_software/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/api/serializers.py` & `netbox_software-0.2.6/netbox_software/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/api/views.py` & `netbox_software-0.2.6/netbox_software/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/filtersets.py` & `netbox_software-0.2.6/netbox_software/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/forms.py` & `netbox_software-0.2.6/netbox_software/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/models.py` & `netbox_software-0.2.6/netbox_software/models.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/navigation.py` & `netbox_software-0.2.6/netbox_software/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,60 +24,60 @@
             PluginMenuItem(
                 link='plugins:netbox_software:devicesoftware_list',
                 link_text='ПО устройств',
                 buttons=[PluginMenuButton(
                     link='plugins:netbox_software:devicesoftware_add',
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
-                    permissions=['netbox_software.change_software'],
+                    permissions=['netbox_software.change_devicesoftware'],
                     color=ButtonColorChoices.GREEN
                 )],
-                permissions=['netbox_software.view_software']
+                permissions=['netbox_software.view_devicesoftware']
             )
         )
         menuitem.append(
             PluginMenuItem(
                 link='plugins:netbox_software:softwaretype_list',
                 link_text='Типы ПО',
                 buttons=[PluginMenuButton(
                     link='plugins:netbox_software:softwaretype_add',
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
-                    permissions=['netbox_software.change_software'],
+                    permissions=['netbox_software.change_softwaretype'],
                     color=ButtonColorChoices.GREEN
                 )],
-                permissions=['netbox_software.view_software']
+                permissions=['netbox_software.view_softwaretype']
             )
         )
         menuitem.append(
             PluginMenuItem(
                 link='plugins:netbox_software:vendor_list',
                 link_text='Вендоры',
                 buttons=[PluginMenuButton(
                     link='plugins:netbox_software:vendor_add',
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
-                    permissions=['netbox_software.change_software'],
+                    permissions=['netbox_software.change_vendor'],
                     color=ButtonColorChoices.GREEN
                 )],
-                permissions=['netbox_software.view_software']
+                permissions=['netbox_software.view_vendor']
             )
         )
         menuitem.append(
             PluginMenuItem(
                 link='plugins:netbox_software:application_list',
                 link_text='ПО',
                 buttons=[PluginMenuButton(
                     link='plugins:netbox_software:application_add',
                     title='Создать',
                     icon_class='mdi mdi-plus-thick',
-                    permissions=['netbox_software.change_software'],
+                    permissions=['netbox_software.change_application'],
                     color=ButtonColorChoices.GREEN
                 )],
-                permissions=['netbox_software.view_software']
+                permissions=['netbox_software.view_application']
             )
         )
 
     # If we are using NB 3.4.0+ display the new top level navigation option
     if settings.VERSION >= '3.4.0':
         menu = MyPluginMenu(
             name='SoftPl',
```

### Comparing `netbox_software-0.2.5/netbox_software/search.py` & `netbox_software-0.2.6/netbox_software/search.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/tables.py` & `netbox_software-0.2.6/netbox_software/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/template_content.py` & `netbox_software-0.2.6/netbox_software/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/application.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/application.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/application_edit.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/application_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/applicationversion.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/applicationversion.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.2.6/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/urls.py` & `netbox_software-0.2.6/netbox_software/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.2.5/netbox_software/views.py` & `netbox_software-0.2.6/netbox_software/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,142 +7,142 @@
 #from rest_framework import status, viewsets
 #from rest_framework.response import Response
 
 
 ### Vendor
 @register_model_view(models.Vendor)
 class VendorView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_vendor"
     queryset = models.Vendor.objects.all()
 
 
 class VendorListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_vendor"
     queryset = models.Vendor.objects.all()
     table = tables.VendorTable
     filterset = filtersets.VendorFilterSet
     filterset_form = forms.VendorFilterForm
 
 
 @register_model_view(models.Vendor, 'edit')
 class VendorEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = "netbox_software.change_software"
+    permission_required = "netbox_software.change_vendor"
     queryset = models.Vendor.objects.all()
     form = forms.VendorForm
 
     template_name = 'netbox_software/vendor_edit.html'
 
 
 @register_model_view(models.Vendor, 'delete')
 class VendorDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = "netbox_software.delete_software"
+    permission_required = "netbox_software.delete_vendor"
     queryset = models.Vendor.objects.all()
 
 
 ### SoftwareType
 @register_model_view(models.SoftwareType)
 class SoftwareTypeView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_softwaretype"
     queryset = models.SoftwareType.objects.all()
 
 
 class SoftwareTypeListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_softwaretype"
     queryset = models.SoftwareType.objects.all()
     table = tables.SoftwareTypeTable
     filterset = filtersets.SoftwareTypeFilterSet
     filterset_form = forms.SoftwareTypeFilterForm
 
 
 @register_model_view(models.SoftwareType, 'edit')
 class SoftwareTypeEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = "netbox_software.change_software"
+    permission_required = "netbox_software.change_softwaretype"
     queryset = models.SoftwareType.objects.all()
     form = forms.SoftwareTypeForm
     template_name = 'netbox_software/softwaretype_edit.html'
 
 
 @register_model_view(models.SoftwareType, 'delete')
 class SoftwareTypeDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = "netbox_software.delete_software"
+    permission_required = "netbox_software.delete_softwaretype"
     queryset = models.SoftwareType.objects.all()
 
 
 ### Application
 class ApplicationView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_application"
     queryset = models.Application.objects.all()
 
 
 class ApplicationListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view__application"
     queryset = models.Application.objects.all()
     table = tables.ApplicationTable
     filterset = filtersets.ApplicationFilterSet
     filterset_form = forms.ApplicationFilterForm
 
 
 class ApplicationEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = "netbox_software.change_software"
+    permission_required = "netbox_software.change_application"
     queryset = models.Application.objects.all()
     form = forms.ApplicationForm
 
     template_name = 'netbox_software/application_edit.html'
 
 
 class ApplicationDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = "netbox_software.delete_software"
+    permission_required = "netbox_software.delete_application"
     queryset = models.Application.objects.all()
 
 
 ### ApplicationVersion
 class ApplicationVersionView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_applicationversion"
     queryset = models.ApplicationVersion.objects.all()
 
 
 class ApplicationVersionListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_applicationversion"
     queryset = models.ApplicationVersion.objects.all()
     table = tables.ApplicationVersionTable
     filterset = filtersets.ApplicationVersionFilterSet
     filterset_form = forms.ApplicationVersionFilterForm
 
 
 class ApplicationVersionEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = "netbox_software.change_software"
+    permission_required = "netbox_software.change_applicationversion"
     queryset = models.ApplicationVersion.objects.all()
     form = forms.ApplicationVersionForm
 
     template_name = 'netbox_software/applicationversion_edit.html'
 
 
 class ApplicationVersionDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = "netbox_software.delete_software"
+    permission_required = "netbox_software.delete_applicationversion"
     queryset = models.ApplicationVersion.objects.all()
 
 
 ### DeviceSoftware
 class DeviceSoftwareView(PermissionRequiredMixin, generic.ObjectView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_devicesoftware"
     queryset = models.DeviceSoftware.objects.all()
 
 
 class DeviceSoftwareListView(PermissionRequiredMixin, generic.ObjectListView):
-    permission_required = "netbox_software.view_software"
+    permission_required = "netbox_software.view_devicesoftware"
     queryset = models.DeviceSoftware.objects.all()
     table = tables.DeviceSoftwareTable
     filterset = filtersets.DeviceSoftwareFilterSet
     filterset_form = forms.DeviceSoftwareFilterForm
 
 
 class DeviceSoftwareEditView(PermissionRequiredMixin, generic.ObjectEditView):
-    permission_required = "netbox_software.change_software"
+    permission_required = "netbox_software.change_devicesoftware"
     queryset = models.DeviceSoftware.objects.all()
     form = forms.DeviceSoftwareForm
 
     template_name = 'netbox_software/devicesoftware_edit.html'
 
 
 class DeviceSoftwareDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
-    permission_required = "netbox_software.delete_software"
+    permission_required = "netbox_software.delete_devicesoftware"
     queryset = models.DeviceSoftware.objects.all()
```

### Comparing `netbox_software-0.2.5/PKG-INFO` & `netbox_software-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

