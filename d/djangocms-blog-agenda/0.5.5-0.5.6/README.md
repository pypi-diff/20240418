# Comparing `tmp/djangocms-blog-agenda-0.5.5.tar.gz` & `tmp/djangocms_blog_agenda-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-blog-agenda-0.5.5.tar", last modified: Tue Feb  6 10:03:51 2024, max compression
+gzip compressed data, was "djangocms_blog_agenda-0.5.6.tar", last modified: Thu Apr 18 15:59:53 2024, max compression
```

## Comparing `djangocms-blog-agenda-0.5.5.tar` & `djangocms_blog_agenda-0.5.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.991132 djangocms-blog-agenda-0.5.5/
--rw-r--r--   0 kapt       (501) kapt        (20)       45 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/AUTHORS.md
--rw-r--r--   0 kapt       (501) kapt        (20)     1318 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501) kapt        (20)    35149 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/LICENSE
--rw-r--r--   0 kapt       (501) kapt        (20)      159 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/MANIFEST.in
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-02-06 10:03:51.991132 djangocms-blog-agenda-0.5.5/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     2682 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/README.md
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.988132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)     4389 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1746 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/apps.py
--rw-r--r--   0 kapt       (501) kapt        (20)     3921 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/cms_plugins.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.986132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.986132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.989132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501) kapt        (20)     2095 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501) kapt        (20)     4357 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.990132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501) kapt        (20)     1076 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1139 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501) kapt        (20)      746 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)      651 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
--rw-r--r--   0 kapt       (501) kapt        (20)        0 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501) kapt        (20)      765 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1273 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-02-06 09:38:41.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.986132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.991132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501) kapt        (20)     1341 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1742 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1361 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501) kapt        (20)     1889 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-02-06 09:38:41.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-02-06 10:03:51.991132 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-02-06 10:03:51.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501) kapt        (20)     1222 2024-02-06 10:03:51.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-02-06 10:03:51.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-02-06 10:03:51.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-02-06 10:03:51.000000 djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-02-06 10:03:51.991132 djangocms-blog-agenda-0.5.5/setup.cfg
--rw-r--r--   0 kapt       (501) kapt        (20)       53 2024-02-06 09:21:08.000000 djangocms-blog-agenda-0.5.5/setup.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/
+-rw-r--r--   0 kapt       (501) kapt        (20)       45 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/AUTHORS.md
+-rw-r--r--   0 kapt       (501) kapt        (20)     1318 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501) kapt        (20)    35149 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/LICENSE
+-rw-r--r--   0 kapt       (501) kapt        (20)      159 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/MANIFEST.in
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     2682 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/README.md
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.630004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     4389 2023-05-25 06:47:09.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1746 2023-03-31 09:10:44.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/apps.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     3921 2023-12-12 08:25:46.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/cms_plugins.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.622004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.622004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.633004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501) kapt        (20)     2095 2023-11-27 13:10:23.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501) kapt        (20)     4357 2023-11-27 13:10:10.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.638004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1076 2023-03-30 10:38:48.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1139 2023-03-30 14:50:16.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      746 2023-11-13 16:05:40.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      651 2023-12-12 08:49:47.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py
+-rw-r--r--   0 kapt       (501) kapt        (20)        0 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501) kapt        (20)      951 2024-04-18 15:57:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1273 2023-11-27 13:02:24.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501) kapt        (20)     1117 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.623004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.640004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501) kapt        (20)     1341 2023-03-30 10:37:22.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1742 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1361 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     1889 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501) kapt        (20)     2549 2024-04-18 15:56:11.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501) kapt        (20)        0 2024-04-18 15:59:53.641004 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501) kapt        (20)     3465 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501) kapt        (20)     1222 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)        1 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       15 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)       22 2024-04-18 15:59:53.000000 djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501) kapt        (20)      786 2024-04-18 15:59:53.642004 djangocms_blog_agenda-0.5.6/setup.cfg
+-rw-r--r--   0 kapt       (501) kapt        (20)       53 2023-03-30 09:34:19.000000 djangocms_blog_agenda-0.5.6/setup.py
```

### Comparing `djangocms-blog-agenda-0.5.5/CONTRIBUTING.md` & `djangocms_blog_agenda-0.5.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/LICENSE` & `djangocms_blog_agenda-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/PKG-INFO` & `djangocms_blog_agenda-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.5.5
+Version: 0.5.6
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.5.5/README.md` & `djangocms_blog_agenda-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/admin.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/apps.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/cms_plugins.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0003_upcomingeventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/migrations/0004_pasteventsplugin.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/misc.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/misc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 def get_inline_instances(self, request, obj=None):
     from json import loads
 
     from djangocms_blog.admin import PostAdmin
     from djangocms_blog.cms_appconfig import BlogConfig
 
+    from .admin import PostExtensionInline
+
     inline_instances = super(PostAdmin, self).get_inline_instances(request, obj)
 
     if "app_config" in request.GET:
         # get blog config instance from request
         blog_config = BlogConfig.objects.filter(pk=request.GET["app_config"])
         # get config from saved json
         config = loads(blog_config.values()[0]["app_data"])
         # get template_prefix from config
 
         if config:
             template_prefix = config["config"]["template_prefix"]
             if template_prefix == "djangocms_blog_agenda":
                 return inline_instances
-    return []
+
+    return list(
+        filter(
+            lambda instance: not isinstance(instance, PostExtensionInline),
+            inline_instances,
+        )
+    )
```

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/models.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/patched_urls.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/patched_urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda/views.py` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.5.5
+Version: 0.5.6
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.5.5/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms_blog_agenda-0.5.6/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.5.5/setup.cfg` & `djangocms_blog_agenda-0.5.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.5.5
+version = 0.5.6
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

