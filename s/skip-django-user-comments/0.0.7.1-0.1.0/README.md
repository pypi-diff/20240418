# Comparing `tmp/skip-django-user-comments-0.0.7.1.tar.gz` & `tmp/skip_django_user_comments-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-user-comments-0.0.7.1.tar", last modified: Thu Jan 19 00:01:08 2023, max compression
+gzip compressed data, was "skip_django_user_comments-0.1.0.tar", last modified: Thu Apr 18 14:42:26 2024, max compression
```

## Comparing `skip-django-user-comments-0.0.7.1.tar` & `skip_django_user_comments-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 00:01:08.533990 skip-django-user-comments-0.0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-19 00:01:08.000000 skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/user_comments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/user_comments/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/user_comments/contrib/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/contrib/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/contrib/is_core/cores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.525990 skip-django-user-comments-0.0.7.1/user_comments/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.525990 skip-django-user-comments-0.0.7.1/user_comments/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/user_comments/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 00:01:08.529990 skip-django-user-comments-0.0.7.1/user_comments/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-19 00:00:58.000000 skip-django-user-comments-0.0.7.1/user_comments/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 14:42:26.000000 skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/user_comments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/user_comments/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/user_comments/contrib/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/contrib/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/contrib/is_core/cores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.644255 skip_django_user_comments-0.1.0/user_comments/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.644255 skip_django_user_comments-0.1.0/user_comments/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/user_comments/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:26.648254 skip_django_user_comments-0.1.0/user_comments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 14:42:23.000000 skip_django_user_comments-0.1.0/user_comments/models.py
```

### Comparing `skip-django-user-comments-0.0.7.1/README.md` & `skip_django_user_comments-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/skip_django_user_comments.egg-info/SOURCES.txt` & `skip_django_user_comments-0.1.0/skip_django_user_comments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/contrib/is_core/cores.py` & `skip_django_user_comments-0.1.0/user_comments/contrib/is_core/cores.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from django import forms
 from django.contrib.contenttypes.models import ContentType
-from django.utils.translation import ugettext_lazy
+from django.utils.translation import gettext_lazy
 
 from is_core.generic_views.inlines.inline_objects_views import TabularInlineObjectsView
 
 from user_comments.models import Comment
 
 from is_core.forms.models import SmartModelForm
 from is_core.generic_views.detail_views import DjangoDetailFormView
 
 
 class CommentUiForm(SmartModelForm):
 
-    comment = forms.CharField(label=ugettext_lazy('add comment'), required=False, widget=forms.Textarea())
+    comment = forms.CharField(label=gettext_lazy('add comment'), required=False, widget=forms.Textarea())
 
     def _post_save(self, obj):
         super()._post_save(obj)
         comment = self.cleaned_data.get('comment')
         if comment:
             Comment.objects.create(
                 content_object=obj,
@@ -25,17 +25,17 @@
             )
 
 
 class CommentObjectsView(TabularInlineObjectsView):
 
     model = Comment
     fields = (
-        ('author', ugettext_lazy('Author')),
-        ('created_at', ugettext_lazy('Created at')),
-        ('comment', ugettext_lazy('Comment')),
+        ('author', gettext_lazy('Author')),
+        ('created_at', gettext_lazy('Created at')),
+        ('comment', gettext_lazy('Comment')),
     )
 
     def get_objects(self):
         return self.model.objects.filter(
             content_type=ContentType.objects.get_for_model(self.parent_instance),
             object_pk=self.parent_instance.pk
         )
@@ -53,15 +53,15 @@
 
 class CommentCoreMixin:
 
     form_class = CommentUiForm
     ui_detail_view = DetailCommentFormView
 
     notes_fieldset = (
-        (ugettext_lazy('Comments'), {
+        (gettext_lazy('Comments'), {
             'fieldsets': (
                 (None, {'inline_view': CommentObjectsView}),
                 (None, {'fields': ('comment',)}),
             )
         }),
     )
```

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/locale/cs/LC_MESSAGES/django.mo` & `skip_django_user_comments-0.1.0/user_comments/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/locale/cs/LC_MESSAGES/django.po` & `skip_django_user_comments-0.1.0/user_comments/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/migrations/0001_initial.py` & `skip_django_user_comments-0.1.0/user_comments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/migrations/0002_migration.py` & `skip_django_user_comments-0.1.0/user_comments/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-user-comments-0.0.7.1/user_comments/models.py` & `skip_django_user_comments-0.1.0/user_comments/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
-from django.utils.translation import ugettext_lazy
+from django.utils.translation import gettext_lazy
 
 from chamber.models import SmartModel
 
 
 class CommentQuerySet(models.QuerySet):
 
     def filter_for_object(self, obj):
@@ -16,19 +16,19 @@
         )
 
 
 class Comment(SmartModel):
 
     objects = CommentQuerySet.as_manager()
 
-    author = models.ForeignKey(settings.AUTH_USER_MODEL, verbose_name=ugettext_lazy('author'), on_delete=models.CASCADE,
+    author = models.ForeignKey(settings.AUTH_USER_MODEL, verbose_name=gettext_lazy('author'), on_delete=models.CASCADE,
                                null=True, blank=True, db_index=True)
-    comment = models.TextField(verbose_name=ugettext_lazy('comment'), null=False, blank=False)
+    comment = models.TextField(verbose_name=gettext_lazy('comment'), null=False, blank=False)
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_pk = models.TextField(db_index=True)
     content_object = GenericForeignKey('content_type', 'object_pk')
-    content_object.verbose_name = ugettext_lazy('object')
+    content_object.verbose_name = gettext_lazy('object')
 
     class Meta:
-        verbose_name = ugettext_lazy('comment')
-        verbose_name_plural = ugettext_lazy('comments')
+        verbose_name = gettext_lazy('comment')
+        verbose_name_plural = gettext_lazy('comments')
         ordering = ('-created_at',)
```

