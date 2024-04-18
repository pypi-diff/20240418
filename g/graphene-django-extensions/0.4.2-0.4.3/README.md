# Comparing `tmp/graphene_django_extensions-0.4.2.tar.gz` & `tmp/graphene_django_extensions-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_extensions-0.4.2.tar", max compression
+gzip compressed data, was "graphene_django_extensions-0.4.3.tar", max compression
```

## Comparing `graphene_django_extensions-0.4.2.tar` & `graphene_django_extensions-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1064 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/LICENSE
--rw-r--r--   0        0        0     4375 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/gdx_pytest/__init__.py
--rw-r--r--   0        0        0      632 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/gdx_pytest/fixtures.py
--rw-r--r--   0        0        0      383 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/__init__.py
--rw-r--r--   0        0        0    32115 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/bases.py
--rw-r--r--   0        0        0      524 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/connections.py
--rw-r--r--   0        0        0      635 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/constants.py
--rw-r--r--   0        0        0    10013 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/converters.py
--rw-r--r--   0        0        0     7331 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/errors.py
--rw-r--r--   0        0        0      923 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/__init__.py
--rw-r--r--   0        0        0     2765 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/form.py
--rw-r--r--   0        0        0     6997 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/graphql.py
--rw-r--r--   0        0        0     2760 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/model.py
--rw-r--r--   0        0        0     3343 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/fields/serializer.py
--rw-r--r--   0        0        0     3882 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/files.py
--rw-r--r--   0        0        0    13174 2024-04-03 17:09:02.642790 graphene_django_extensions-0.4.2/graphene_django_extensions/filters.py
--rw-r--r--   0        0        0     3356 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/model_operations.py
--rw-r--r--   0        0        0     1745 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/options.py
--rw-r--r--   0        0        0     3694 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/permissions.py
--rw-r--r--   0        0        0        0 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/py.typed
--rw-r--r--   0        0        0    11264 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/serializers.py
--rw-r--r--   0        0        0     2722 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/settings.py
--rw-r--r--   0        0        0      367 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/__init__.py
--rw-r--r--   0        0        0     8466 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/builders.py
--rw-r--r--   0        0        0    14361 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/client.py
--rw-r--r--   0        0        0     7286 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/testing/utils.py
--rw-r--r--   0        0        0     4660 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/typing.py
--rw-r--r--   0        0        0     5845 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/utils.py
--rw-r--r--   0        0        0     2924 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/graphene_django_extensions/views.py
--rw-r--r--   0        0        0     6817 2024-04-03 17:09:02.646790 graphene_django_extensions-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 graphene_django_extensions-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-18 05:05:40.213966 graphene_django_extensions-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4375 2024-04-18 05:05:40.213966 graphene_django_extensions-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/gdx_pytest/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/gdx_pytest/fixtures.py
+-rw-r--r--   0        0        0      383 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/__init__.py
+-rw-r--r--   0        0        0    31530 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/bases.py
+-rw-r--r--   0        0        0      524 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/connections.py
+-rw-r--r--   0        0        0      635 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/constants.py
+-rw-r--r--   0        0        0    10013 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/converters.py
+-rw-r--r--   0        0        0     9406 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/errors.py
+-rw-r--r--   0        0        0      923 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/fields/__init__.py
+-rw-r--r--   0        0        0     2765 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/fields/form.py
+-rw-r--r--   0        0        0     6997 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/fields/graphql.py
+-rw-r--r--   0        0        0     2760 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/fields/model.py
+-rw-r--r--   0        0        0     3343 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/fields/serializer.py
+-rw-r--r--   0        0        0     3882 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/files.py
+-rw-r--r--   0        0        0    13174 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/filters.py
+-rw-r--r--   0        0        0     3281 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/model_operations.py
+-rw-r--r--   0        0        0     1745 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/options.py
+-rw-r--r--   0        0        0     3708 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/permissions.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/py.typed
+-rw-r--r--   0        0        0     2758 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/selections.py
+-rw-r--r--   0        0        0    11259 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/serializers.py
+-rw-r--r--   0        0        0     2722 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/settings.py
+-rw-r--r--   0        0        0      367 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/testing/__init__.py
+-rw-r--r--   0        0        0     8466 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/testing/builders.py
+-rw-r--r--   0        0        0    14361 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/testing/client.py
+-rw-r--r--   0        0        0     7286 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/testing/utils.py
+-rw-r--r--   0        0        0     4499 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/typing.py
+-rw-r--r--   0        0        0     2787 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/utils.py
+-rw-r--r--   0        0        0     2924 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/graphene_django_extensions/views.py
+-rw-r--r--   0        0        0     6817 2024-04-18 05:05:40.217966 graphene_django_extensions-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6112 1970-01-01 00:00:00.000000 graphene_django_extensions-0.4.3/PKG-INFO
```

### Comparing `graphene_django_extensions-0.4.2/LICENSE` & `graphene_django_extensions-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/README.md` & `graphene_django_extensions-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/gdx_pytest/fixtures.py` & `graphene_django_extensions-0.4.3/gdx_pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/bases.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/bases.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,38 @@
 from graphene_django.forms.mutation import fields_for_form
 from graphene_django.registry import get_global_registry
 from graphene_django.rest_framework.mutation import fields_for_serializer
 from graphene_django.types import ALL_FIELDS
 from graphene_django.utils import is_valid_django_model
 from graphql_relay import to_global_id
 from query_optimizer import DjangoConnectionField, DjangoListField, DjangoObjectType
+from query_optimizer.filter_info import get_filter_info
 from rest_framework.exceptions import ValidationError as SerializerValidationError
 from rest_framework.fields import SerializerMethodField, get_attribute
 from rest_framework.serializers import ListSerializer, ModelSerializer, Serializer
 
 from .connections import Connection
 from .converters import convert_form_fields_to_not_required, convert_serializer_fields_to_not_required
-from .errors import GDXWarning, GQLPermissionDeniedError, validation_errors_to_graphql_errors
+from .errors import (
+    GDXWarning,
+    GQLCreatePermissionDeniedError,
+    GQLDeletePermissionDeniedError,
+    GQLFilterPermissionDeniedError,
+    GQLMutationPermissionDeniedError,
+    GQLNodePermissionDeniedError,
+    GQLUpdatePermissionDeniedError,
+    validation_errors_to_graphql_errors,
+)
 from .fields import RelatedField
 from .model_operations import get_model_lookup_field, get_object_or_404
 from .options import DjangoMutationOptions, DjangoNodeOptions
 from .permissions import AllowAny, BasePermission, restricted_field
 from .settings import gdx_settings
 from .typing import Fields, GQLFields, Sequence
-from .utils import add_translatable_fields, get_filter_info
+from .utils import add_translatable_fields
 
 if TYPE_CHECKING:
     from django.db import models
     from graphene.relay.node import NodeField
 
     from .typing import Any, AnyUser, FieldNameStr, GQLInfo, Literal, PermCheck, Self
 
@@ -46,15 +56,15 @@
     "UpdateMutation",
     "DeleteMutation",
 ]
 
 
 class DjangoNode(DjangoObjectType):
     """
-    Custom base class for GraphQL-types that are backed by a Django model.
+    Custom base class for GraphQL types that are backed by a Django model.
     Adds the following features to all types that inherit it:
 
     - Makes the `graphene.relay.Node` interface the default interface for the type.
 
     - Adds the `totalCount` field the default Connection field for the type.
 
     - Adds the `filter_queryset` method that can be overridden to add additional filtering for both
@@ -173,45 +183,39 @@
 
             setattr(cls, f"resolve_{field_name}", restricted_field(check)(resolver))
 
     @classmethod
     def get_queryset(cls, queryset: models.QuerySet, info: GQLInfo) -> models.QuerySet:
         """Override `filter_queryset` instead of this method to add filtering of possible rows."""
         if not cls.has_filter_permissions(info):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.FILTER_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.FILTER_PERMISSION_ERROR_CODE,
-            )
+            raise GQLFilterPermissionDeniedError
         return queryset
 
     @classmethod
     def run_instance_checks(cls, instance: models.Model, info: GQLInfo) -> None:
         if not cls.has_node_permissions(info, instance):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.QUERY_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.QUERY_PERMISSION_ERROR_CODE,
-            )
+            raise GQLNodePermissionDeniedError
 
     @classmethod
     def has_node_permissions(cls, info: GQLInfo, instance: models.Model) -> bool:
         """Check which permissions are required to access single items of this type."""
-        filters = get_filter_info(info)
+        filters = get_filter_info(info, cls._meta.model)
         return all(
             perm.has_node_permission(
                 instance=instance,
                 user=info.context.user,
                 filters=filters,
             )
             for perm in cls._meta.permission_classes
         )
 
     @classmethod
     def has_filter_permissions(cls, info: GQLInfo) -> bool:
         """Check which permissions are required to access lists of this type."""
-        filters = get_filter_info(info)
+        filters = get_filter_info(info, cls._meta.model)
         return all(
             perm.has_filter_permission(
                 user=info.context.user,
                 filters=filters,
             )
             for perm in cls._meta.permission_classes
         )
@@ -220,18 +224,18 @@
     def get_global_id(cls, pk: Any) -> str:
         """Get id used for `node` queries."""
         return to_global_id(cls.__name__, pk)
 
 
 class DjangoMutation(Mutation):
     """
-    Custom base class for GraphQL-mutations that are backed by a Django model.
+    Custom base class for GraphQL mutations that are backed by a Django model.
     Adds the following features to all types that inherit it:
 
-    - For updates, converts all fields to optional fields, enabling partial updates.
+    - For updates, convert all fields to optional fields, enabling partial updates.
 
     - Checks for missing object types for nested model serializer fields to avoid nebulous import order errors.
 
     - Can add permission checks via permission classes.
 
     - Converts raise serializer validation errors to GraphQL validation errors.
 
@@ -541,23 +545,17 @@
         return cls.custom_mutation(info, validated_data)
 
     @classmethod
     def update_or_create(cls, info: GQLInfo, input_data: dict[str, Any]) -> Self:
         maybe_instance = cls.get_instance(input_data)
 
         if cls._meta.model_operation == "create" and not cls.has_create_permissions(info, input_data):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.CREATE_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.CREATE_PERMISSION_ERROR_CODE,
-            )
+            raise GQLCreatePermissionDeniedError
         if cls._meta.model_operation == "update" and not cls.has_update_permissions(maybe_instance, info, input_data):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.UPDATE_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.UPDATE_PERMISSION_ERROR_CODE,
-            )
+            raise GQLUpdatePermissionDeniedError
 
         validator = cls.run_validation(input_data, info, maybe_instance)
         instance = validator.save()
 
         if cls._meta.serializer_class is not None:
             output = cls.get_serializer_output(instance)
         else:
@@ -565,35 +563,29 @@
 
         return cls(**output)  # type: ignore[arg-type]
 
     @classmethod
     def delete(cls, info: GQLInfo, input_data: dict[str, Any]) -> Self:
         instance = cls.get_instance(input_data)
         if not cls.has_delete_permissions(instance, info, input_data):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.DELETE_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.DELETE_PERMISSION_ERROR_CODE,
-            )
+            raise GQLDeletePermissionDeniedError
 
         cls.validate_deletion(instance, info.context.user)
         count, _ = instance.delete()
         return cls(deleted=bool(count))  # type: ignore[arg-type]
 
     @classmethod
     def custom_mutation(cls, info: GQLInfo, input_data: dict[str, Any]) -> Self:  # pragma: no cover
         """Override this method to perform custom mutations instead of the regular create, update or delete."""
         raise NotImplementedError(f"Custom model operation not defined for '{cls.__name__}'")  # noqa: EM102
 
     @classmethod
     def validate_custom_mutation_input_data(cls, info: GQLInfo, input_data: dict[str, Any]) -> dict[str, Any]:
         if not cls.has_mutation_permission(info, input_data):
-            raise GQLPermissionDeniedError(
-                message=gdx_settings.MUTATION_PERMISSION_ERROR_MESSAGE,
-                code=gdx_settings.MUTATION_PERMISSION_ERROR_CODE,
-            )
+            raise GQLMutationPermissionDeniedError
 
         validator = cls.run_validation(input_data, info)
         if isinstance(validator, Serializer):
             return validator.validated_data
         return validator.cleaned_data
 
     @classmethod
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/connections.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/connections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/constants.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/constants.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/converters.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/errors.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,46 +23,104 @@
 
     T = TypeVar("T")
     P = ParamSpec("P")
 
 
 __all__ = [
     "GDXWarning",
-    "get_constraint_message",
+    "GQLCodeError",
+    "GQLCreatePermissionDeniedError",
+    "GQLDeletePermissionDeniedError",
+    "GQLFieldPermissionDeniedError",
+    "GQLFilterPermissionDeniedError",
+    "GQLMutationPermissionDeniedError",
+    "GQLNodePermissionDeniedError",
     "GQLNotFoundError",
-    "GQLPermissionDeniedError",
+    "GQLUpdatePermissionDeniedError",
     "GQLValidationError",
+    "get_constraint_message",
 ]
 
 
-class GQLPermissionDeniedError(GraphQLError):
-    """Exception raised when the user has insufficient permissions to access a resource."""
+class GQLCodeError(GraphQLError):
+    """Exception raised with a custom error code."""
+
+    code: str = "ERROR_CODE"
+    message: str = "Error message."
+
+    def __init__(self, message: str | None = None, code: str | None = None) -> None:
+        super().__init__(message=message or self.message, extensions={"code": code or self.code})
+
+
+class GQLNodePermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to access a single resource."""
+
+    code = gdx_settings.QUERY_PERMISSION_ERROR_CODE
+    message = gdx_settings.QUERY_PERMISSION_ERROR_MESSAGE
+
+
+class GQLFilterPermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to access multiple resources."""
+
+    code = gdx_settings.FILTER_PERMISSION_ERROR_CODE
+    message = gdx_settings.FILTER_PERMISSION_ERROR_MESSAGE
+
+
+class GQLCreatePermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to create a resource."""
+
+    code = gdx_settings.CREATE_PERMISSION_ERROR_CODE
+    message = gdx_settings.CREATE_PERMISSION_ERROR_MESSAGE
+
+
+class GQLUpdatePermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to update a resource."""
+
+    code = gdx_settings.UPDATE_PERMISSION_ERROR_CODE
+    message = gdx_settings.UPDATE_PERMISSION_ERROR_MESSAGE
+
+
+class GQLDeletePermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to delete a resource."""
+
+    code = gdx_settings.DELETE_PERMISSION_ERROR_CODE
+    message = gdx_settings.DELETE_PERMISSION_ERROR_MESSAGE
+
+
+class GQLMutationPermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to mutate a resource."""
+
+    code = gdx_settings.MUTATION_PERMISSION_ERROR_CODE
+    message = gdx_settings.MUTATION_PERMISSION_ERROR_MESSAGE
+
+
+class GQLFieldPermissionDeniedError(GQLCodeError):
+    """Exception raised when the user has insufficient permissions to access a field from a resource."""
 
-    def __init__(self, message: str, code: str) -> None:
-        super().__init__(message, extensions={"code": code})
+    code = gdx_settings.FIELD_PERMISSION_ERROR_CODE
+    message = gdx_settings.FIELD_PERMISSION_ERROR_MESSAGE
 
 
-class GQLNotFoundError(GraphQLError):
-    """Exception raised when the user has insufficient permissions to access a resource."""
+class GQLNotFoundError(GQLCodeError):
+    """Exception raised when a resource does not exist."""
 
-    def __init__(self, message: str, code: str) -> None:
-        super().__init__(message, extensions={"code": code})
+    code = gdx_settings.NOT_FOUND_ERROR_CODE
 
 
 class GQLValidationError(GraphQLError):
     """Exception raised when mutation validation fails."""
 
     def __init__(self, error: ValidationErrorType) -> None:
         detail = as_serializer_error(error)
         if graphene_settings.CAMELCASE_ERRORS:
             detail = camelize(detail)
         detail = flatten_errors(detail)
         errors = to_field_errors(detail)
         super().__init__(
-            gdx_settings.MUTATION_VALIDATION_ERROR_MESSAGE,
+            message=gdx_settings.MUTATION_VALIDATION_ERROR_MESSAGE,
             extensions={"code": gdx_settings.MUTATION_VALIDATION_ERROR_CODE, "errors": errors},
         )
 
 
 class GDXWarning(UserWarning):
     """Base warning class for graphene-django-extensions."""
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/__init__.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/form.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/fields/form.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/graphql.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/fields/graphql.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/model.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/fields/model.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/fields/serializer.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/fields/serializer.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/files.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/files.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/filters.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/filters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/model_operations.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/model_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from django.db import models
 
 from .errors import GQLNotFoundError
-from .settings import gdx_settings
 
 if TYPE_CHECKING:
     from django.db.models import ForeignObjectRel
     from django.db.models.fields.related import RelatedField
 
     from .typing import Any, RelationType
 
@@ -23,15 +22,15 @@
 
 
 def get_object_or_404(model_class: type[models.Model], **kwargs: Any) -> models.Model:
     try:
         return model_class._default_manager.get(**kwargs)
     except model_class.DoesNotExist as error:
         msg = f"`{model_class.__name__}` object matching query `{kwargs}` does not exist."
-        raise GQLNotFoundError(msg, code=gdx_settings.NOT_FOUND_ERROR_CODE) from error
+        raise GQLNotFoundError(msg) from error
 
 
 def get_model_lookup_field(model_class: type[models.Model], lookup_field: str | None = None) -> str:
     if lookup_field is None:
         # Use model primary key as lookup field.
         # This is usually the 'id' field, in which case we use 'pk' instead
         # to avoid collision with the 'id' field in GraphQL Relay nodes.
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/options.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/options.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/permissions.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 from functools import wraps
 from typing import TYPE_CHECKING
 
-from .errors import GQLPermissionDeniedError
+from .errors import GQLFieldPermissionDeniedError
 from .settings import gdx_settings
 from .typing import ParamSpec, TypeVar
 
 if TYPE_CHECKING:
     from django.db.models import Model
+    from query_optimizer.typing import GraphQLFilterInfo
 
-    from .typing import Any, AnyUser, Callable, GraphQLFilterInfo, PermCheck
+    from .typing import Any, AnyUser, Callable, PermCheck
 
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 __all__ = [
@@ -103,12 +104,12 @@
             except TypeError:
                 result = check(args[1].context.user)
 
             if result is None:  # pragma: no cover
                 return None
             if result:  # pragma: no cover
                 return func(*args, **kwargs)
-            raise GQLPermissionDeniedError(message, gdx_settings.FIELD_PERMISSION_ERROR_CODE)
+            raise GQLFieldPermissionDeniedError(message=message)
 
         return wrapper
 
     return decorator
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/serializers.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         instance.save()
         return instance
 
     def _pre_save(self, validated_data: dict[str, Any]) -> list[PreSaveInfo]:
         """
         Prepare related models defined using BaseModelSerializers.
         Forward 'one-to-one' and 'many-to-one' related entities will be fetched, updated, or created.
-        Other related entities will be saved to be handled after the main model is saved using '_handle_to_many'.
+        Other related entities will be saved to be handled after the main model is saved using '_post_save'.
         """
         pre_save_infos: list[PreSaveInfo] = []
         related_info = get_related_field_info(self.Meta.model)
 
         for name in list(validated_data):  # Copy keys so that we can pop from the original dict in the loop
             field: Field | None = self.fields.get(name, None)
             if field is None:
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/settings.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/builders.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/testing/builders.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/client.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/testing/client.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/testing/utils.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/testing/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/typing.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "FieldError",
     "FieldNameStr",
     "FilterOverride",
     "FilterSetMeta",
     "GQLFields",
     "GQLInfo",
     "Generic",
-    "GraphQLFilterInfo",
     "Iterable",
     "Literal",
     "Mapping",
     "NamedTuple",
     "NodeConnectionType",
     "ParamSpec",
     "PermCheck",
@@ -170,13 +169,7 @@
     ordering: list[str]
 
 
 class FieldError(TypedDict):
     field: str
     message: str
     code: str
-
-
-class GraphQLFilterInfo(TypedDict, total=False):
-    name: str
-    filters: dict[str, Any]
-    children: dict[str, GraphQLFilterInfo]
```

### Comparing `graphene_django_extensions-0.4.2/graphene_django_extensions/views.py` & `graphene_django_extensions-0.4.3/graphene_django_extensions/views.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extensions-0.4.2/pyproject.toml` & `graphene_django_extensions-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-extensions"
-version = "0.4.2"
+version = "0.4.3"
 description = "Extensions for graphene-django"
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "graphene_django_extensions" },
     { include = "gdx_pytest" },
@@ -54,15 +54,15 @@
 graphene_django_extensions = "gdx_pytest.fixtures"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 Django = ">=4.2"
 djangorestframework = ">=3.14.0"
 graphene-django = ">=3.0.0"
-graphene-django-query-optimizer = ">=0.5.0"
+graphene-django-query-optimizer = ">=0.5.1"
 django-settings-holder = ">=0.1.2"
 django-filter = ">=23.5"
 typing-extensions = { version = ">=4.4.0", python = "<3.11" }
 django-modeltranslation = { version = ">=0.18.11", optional = true }
 pillow = { version = ">=10.2.0", optional = true }
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `graphene_django_extensions-0.4.2/PKG-INFO` & `graphene_django_extensions-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-extensions
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extensions for graphene-django
 Home-page: https://mrthearman.github.io/graphene-django-extensions
 License: MIT
 Keywords: django,graphene,extensions,graphql,graphene-django,mutations,queries,object_types,fields
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.10,<4
@@ -26,15 +26,15 @@
 Provides-Extra: translation
 Requires-Dist: Django (>=4.2)
 Requires-Dist: django-filter (>=23.5)
 Requires-Dist: django-modeltranslation (>=0.18.11) ; extra == "translation"
 Requires-Dist: django-settings-holder (>=0.1.2)
 Requires-Dist: djangorestframework (>=3.14.0)
 Requires-Dist: graphene-django (>=3.0.0)
-Requires-Dist: graphene-django-query-optimizer (>=0.5.0)
+Requires-Dist: graphene-django-query-optimizer (>=0.5.1)
 Requires-Dist: pillow (>=10.2.0) ; extra == "files"
 Requires-Dist: typing-extensions (>=4.4.0) ; python_version < "3.11"
 Project-URL: Bug Tracker, https://github.com/MrThearMan/graphene-django-extensions/issues
 Project-URL: Repository, https://github.com/MrThearMan/graphene-django-extensions
 Description-Content-Type: text/markdown
 
 # Graphene Django Extensions
```

