# Comparing `tmp/graphene_django_query_optimizer-0.5.1.tar.gz` & `tmp/graphene_django_query_optimizer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.5.1.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.5.2.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.5.1.tar` & `graphene_django_query_optimizer-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/LICENSE
--rw-r--r--   0        0        0     3151 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/README.md
--rw-r--r--   0        0        0     6905 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      496 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11596 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/ast.py
--rw-r--r--   0        0        0     8683 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/errors.py
--rw-r--r--   0        0        0    15513 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/filter.py
--rw-r--r--   0        0        0     5238 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    10870 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/py.typed
--rw-r--r--   0        0        0     2627 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/settings.py
--rw-r--r--   0        0        0     2996 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/types.py
--rw-r--r--   0        0        0     3639 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/typing.py
--rw-r--r--   0        0        0     6141 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/utils.py
--rw-r--r--   0        0        0     3840 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3151 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/README.md
+-rw-r--r--   0        0        0     6905 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8683 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/errors.py
+-rw-r--r--   0        0        0    15533 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5239 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    10870 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3529 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/settings.py
+-rw-r--r--   0        0        0     2996 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/types.py
+-rw-r--r--   0        0        0     3661 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6141 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3840 2024-04-18 09:38:52.432274 graphene_django_query_optimizer-0.5.2/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.2/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.5.1/LICENSE` & `graphene_django_query_optimizer-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/README.md` & `graphene_django_query_optimizer-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/pyproject.toml` & `graphene_django_query_optimizer-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.5.1"
+version = "0.5.2"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
@@ -62,17 +62,17 @@
 [tool.poetry.group.test.dependencies]
 pytest = "8.1.1"
 coverage = "7.4.4"
 pytest-django = "4.8.0"
 pre-commit = "3.7.0"
 tox = "4.14.2"
 tox-gh-actions = "3.2.0"
-faker = "24.4.0"
+faker = "24.9.0"
 factory-boy = "3.3.0"
-sqlparse = "0.4.4"
+sqlparse = "0.5.0"
 django-graphiql-debug-toolbar = "0.2.0"
 py-spy = "0.3.14"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
 pymdown-extensions = "10.7.1"
 mkdocs-mermaid2-plugin = "1.1.1"
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,40 +77,48 @@
 
     def handle_field_node(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         graphene_type: type[ObjectType] = field_type.graphene_type
 
         if self.info.parent_type == field_type:
             return self.handle_query_class(field_type, field_node)
 
-        if issubclass(graphene_type, DjangoObjectType):
-            return self.handle_object_type(field_type, field_node)
-
         if issubclass(graphene_type, Connection):
             return self.handle_connection(field_type, field_node)
 
+        if is_edge(field_type):
+            return self.handle_edge(field_type, field_node)
+
         if issubclass(graphene_type, PageInfo):  # pragma: no cover
             return self.handle_page_info(field_type, field_node)
 
-        if is_edge(field_type):
-            return self.handle_edge(field_type, field_node)
+        if issubclass(graphene_type, ObjectType):
+            return self.handle_object_type(field_type, field_node)
 
         msg = f"Unhandled graphene type: '{graphene_type}'"  # pragma: no cover
         raise OptimizerError(msg)  # pragma: no cover
 
     def handle_query_class(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         graphene_type = self.get_graphene_type(field_type, field_node)
         selections = get_selections(field_node)
         return self.handle_selections(graphene_type, selections)
 
     def handle_object_type(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         field_name = to_snake_case(field_node.name.value)
         if is_graphql_builtin(field_name):
-            return None
+            return self.handle_graphql_builtin(field_type, field_node)
+
+        graphene_type: type[ObjectType] = field_type.graphene_type
+
+        if issubclass(graphene_type, DjangoObjectType):
+            return self.handle_model_field(field_type, field_node, field_name)
+        return self.handle_plain_object_type(field_type, field_node)
+
+    def handle_graphql_builtin(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None: ...
 
-        return self.handle_model_field(field_type, field_node, field_name)
+    def handle_plain_object_type(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None: ...
 
     def handle_model_field(self, field_type: GrapheneObjectType, field_node: FieldNode, field_name: str) -> None:
         model: type[Model] = field_type.graphene_type._meta.model
         field = get_model_field(model, field_name)
 
         if field is None:
             with self.use_model(model):
@@ -129,19 +137,17 @@
             related_model = get_related_model(field, model)
             with self.use_model(model):
                 return self.handle_to_many_field(field_type, field_node, field, related_model)
 
         msg = f"Unhandled field: '{field.name}'"  # pragma: no cover
         raise OptimizerError(msg)  # pragma: no cover
 
-    def handle_custom_field(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
-        pass
+    def handle_custom_field(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None: ...
 
-    def handle_normal_field(self, field_type: GrapheneObjectType, field_node: FieldNode, field: Field) -> None:
-        pass
+    def handle_normal_field(self, field_type: GrapheneObjectType, field_node: FieldNode, field: Field) -> None: ...
 
     def handle_to_one_field(
         self,
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToOneField,
         related_model: type[Model],
@@ -172,19 +178,17 @@
         return self.handle_selections(graphene_type, selections)
 
     def handle_edge(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         graphene_type = self.get_graphene_type(field_type, field_node)
         selections = get_selections(field_node)
         return self.handle_selections(graphene_type, selections)
 
-    def handle_total_count(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
-        pass  # pragma: no cover
+    def handle_total_count(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None: ...
 
-    def handle_page_info(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
-        pass  # pragma: no cover
+    def handle_page_info(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None: ...
 
     def handle_fragment_spread(self, field_type: GrapheneObjectType, fragment_spread: FragmentSpreadNode) -> None:
         name = fragment_spread.name.value
         fragment_definition = self.info.fragments[name]
         selections = get_selections(fragment_definition)
         return self.handle_selections(field_type, selections)
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import contextlib
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING
 
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.db.models import ForeignKey, Manager, ManyToOneRel, Model, QuerySet
 from graphene.utils.str_converters import to_snake_case
 from graphene_django.utils import maybe_queryset
 
 from .ast import GraphQLASTWalker
@@ -17,15 +17,15 @@
 
 if TYPE_CHECKING:
     import graphene
     from django.db import models
     from graphene.types.definitions import GrapheneObjectType
     from graphql import FieldNode
 
-    from .typing import PK, GQLInfo, TModel, ToManyField, ToOneField
+    from .typing import PK, GQLInfo, Optional, TModel, ToManyField, ToOneField, Union
 
 
 __all__ = [
     "optimize",
     "optimize_single",
     "OptimizationCompiler",
 ]
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             return parent_resolver
         return self.related_resolver
 
     def related_resolver(self, root: models.Model, info: GQLInfo) -> Optional[models.Model]:
         field_name = self.field_name or to_snake_case(info.field_name)
         # Related object should be optimized to the root model.
         related_instance: Optional[models.Model] = getattr(root, field_name, None)
-        if related_instance is None:
+        if related_instance is None:  # pragma: no cover
             return None
         self.underlying_type.run_instance_checks(related_instance, info)
         return related_instance
 
     @cached_property
     def underlying_type(self) -> type[DjangoObjectType]:
         return get_underlying_type(self.type)
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/filter_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToManyField,
         related_model: type[Model],
     ) -> None:
         self.add_filter_info(field_type, field_node)
         with self.child_filter_info(field_node):
-            return super().handle_to_one_field(field_type, field_node, related_field, related_model)
+            return super().handle_to_many_field(field_type, field_node, related_field, related_model)
 
     @contextlib.contextmanager
     def child_filter_info(self, field_node: FieldNode) -> None:
         field_name = to_snake_case(field_node.name.value)
         arguments: dict[str, GraphQLFilterInfo] = {}
         orig_arguments = self.filter_info
         try:
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 ]
 
 
 SETTING_NAME: str = "GRAPHQL_QUERY_OPTIMIZER"
 
 
 class DefaultSettings(NamedTuple):
-    QUERY_CACHE_KEY: str = "_query_cache"
-    """Key to store fetched model instances under in the GraphQL schema extensions."""
-
     OPTIMIZER_MARK: str = "_optimized"
     """Key used mark if a queryset has been optimized by the query optimizer."""
 
     PREFETCH_COUNT_KEY: str = "_optimizer_count"
     """Name used for annotating the prefetched queryset total count."""
 
     PREFETCH_SLICE_START: str = "_optimizer_slice_start"
@@ -62,14 +59,15 @@
 
 
 DEFAULTS: dict[str, Any] = DefaultSettings()._asdict()
 IMPORT_STRINGS: set[Union[bytes, str]] = set()
 REMOVED_SETTINGS: set[str] = {
     "PK_CACHE_KEY",
     "DONT_OPTIMIZE_ON_ERROR",
+    "QUERY_CACHE_KEY",
 }
 
 optimizer_settings = SettingsHolder(
     setting_name=SETTING_NAME,
     defaults=DEFAULTS,
     import_strings=IMPORT_STRINGS,
     removed_settings=REMOVED_SETTINGS,
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/types.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,11 +144,11 @@
 
 
 class ExpressionKind(Protocol):
     def resolve_expression(
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
-        reuse: Any,
+        reuse: set[str] | None,
         summarize: bool,  # noqa: FBT001
         for_save: bool,  # noqa: FBT001
-    ) -> Expr: ...
+    ) -> ExpressionKind: ...
```

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.5.2/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.1/PKG-INFO` & `graphene_django_query_optimizer-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.5.1
+Version: 0.5.2
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

