# Comparing `tmp/lazy_type_hint-2.0.8.tar.gz` & `tmp/lazy_type_hint-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.8.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.9.tar", max compression
```

## Comparing `lazy_type_hint-2.0.8.tar` & `lazy_type_hint-2.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.8/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0    10091 2024-04-16 13:16:36.800734 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     6810 2024-04-16 12:36:20.103593 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      969 2024-04-15 15:41:02.051201 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0      772 2024-04-15 15:41:02.056201 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
--rw-r--r--   0        0        0     1091 2024-04-15 15:41:02.061200 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4803 2024-04-15 15:41:02.067200 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     5806 2024-04-15 15:41:02.072465 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      719 2024-04-15 15:41:02.076615 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6665 2024-04-16 13:10:09.301241 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1486 2024-04-15 15:41:02.081610 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2098 2024-04-16 12:24:06.022499 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2832 2024-04-15 15:41:02.092078 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      365 2024-04-15 15:41:02.101065 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
--rw-r--r--   0        0        0      401 2024-04-15 15:41:02.105064 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.8/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.8/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.8/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-16 12:08:47.077767 lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9756 2024-04-16 12:16:29.926108 lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.8/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1809 2024-04-16 12:04:50.028546 lazy_type_hint-2.0.8/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.8/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.8/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.0.8/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.8/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.8/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.8/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.8/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2468 2024-04-16 13:17:05.982823 lazy_type_hint-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     7007 2024-04-16 12:16:29.914611 lazy_type_hint-2.0.8/README.md
--rw-r--r--   0        0        0     7392 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.9/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    10586 2024-04-18 12:50:55.117818 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     7262 2024-04-18 12:50:55.128183 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0     1118 2024-04-18 12:50:55.134208 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    17314 2024-04-18 12:50:55.137251 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-17 13:44:57.982002 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      775 2024-04-18 12:50:55.144203 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1094 2024-04-18 12:50:55.145202 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4816 2024-04-18 12:50:55.146209 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      601 2024-04-18 12:50:55.151203 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     5809 2024-04-18 12:50:55.160218 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      719 2024-04-17 14:44:54.567291 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6506 2024-04-18 12:50:55.165811 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1486 2024-04-17 10:55:20.513506 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2101 2024-04-18 12:50:55.165811 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     3013 2024-04-18 12:50:55.166804 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      368 2024-04-18 12:50:55.171934 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      404 2024-04-18 12:50:55.176929 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      439 2024-04-18 12:50:55.178906 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      755 2024-04-18 12:50:55.184933 lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-16 12:08:47.077767 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9756 2024-04-16 12:16:29.926108 lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.9/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     2222 2024-04-18 12:50:55.191932 lazy_type_hint-2.0.9/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      732 2024-04-18 12:50:55.192858 lazy_type_hint-2.0.9/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.9/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.0.9/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.9/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.9/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.9/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3783 2024-04-18 12:50:55.193858 lazy_type_hint-2.0.9/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2600 2024-04-18 12:50:55.195064 lazy_type_hint-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7007 2024-04-16 12:16:29.914611 lazy_type_hint-2.0.9/README.md
+-rw-r--r--   0        0        0     7392 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.9/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     FrozenSet,
     Hashable,
-    Iterable,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     final,
 )
 
 from lazy_type_hint.strategies import ParsingStrategies
 from lazy_type_hint.utils import (
     ImportManager,
     OrderedSet,
-    cache_returned_value,
+    cache_returned_value_per_instance,
     is_string_python_keyword_compatible,
 )
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
@@ -67,15 +66,15 @@
     holding_type: Type[object]
     """Type of input data given."""
     strategies: ParsingStrategies
     """Strategies to follow when parsing the data."""
 
     subclasses: ClassVar[Mapping[Type[object], Type[DataTypeTree]]] = {}
     """Available subclasses according to the type they are able to parse."""
-    wraps: ClassVar[Union[Type[object], Sequence[Type[object]]]] = object
+    wraps: ClassVar[Sequence[Type[object]]] = (object,)
     """Object type that the tree is able to parse."""
 
     @final
     def __init__(
         self,
         data: object,
         name: str,
@@ -93,32 +92,32 @@
         self.name = name
         self.holding_type = type(data)
         self.strategies = strategies
         self.depth = depth
         self.imports = ImportManager() if imports is None else imports
         self.parent = parent
         self.__pre_child_instantiation__()
-        self.children = self._instantiate_children(data)
+        self.children = self._instantiate_children(self.data)
         self.height = self._get_height()
         self.__post_child_instantiation__()
 
     @classmethod
     def get_subclass(cls, data: object) -> Type[DataTypeTree]:
+        if type(data) in DataTypeTree.subclasses:
+            return DataTypeTree.subclasses[type(data)]
+
         for subclass in DataTypeTree.subclasses.values():
-            wraps = [subclass.wraps] if not isinstance(subclass.wraps, Iterable) else subclass.wraps
-            for wrap in wraps:
+            for wrap in subclass.wraps:
                 if isinstance(data, wrap):
                     return subclass
         return DataTypeTree.subclasses[int]  # For instances created from any custom class.
 
     def _check_tree_is_correct_one(self, data: object) -> None:
-        wraps = self.wraps if isinstance(self.wraps, Iterable) else [self.wraps]
-        if not any(isinstance(data, wraps_) for wraps_ in wraps):
-            # if type(data) not in wraps:
-            wraps_str = [element.__name__ for element in wraps]
+        if not any(isinstance(data, wraps_) for wraps_ in self.wraps):
+            wraps_str = [element.__name__ for element in self.wraps]
             raise DataTypeTreeError(
                 f"The given parser ({type(self).__name__}) is meant to parse `{', '.join(wraps_str)}` data type but "
                 f"{type(data).__name__} was given"
             )
 
     def __pre_child_instantiation__(self) -> None:
         ...
@@ -146,26 +145,26 @@
         This one will depend on how each subclass manage the child structure.
         """
 
     @final
     def __init_subclass__(cls, **kwargs: Any) -> None:
         """Populate `subclasses` with all subclasses of this same class."""
         super().__init_subclass__(**kwargs)
-        wraps = cls.wraps if isinstance(cls.wraps, Iterable) else [cls.wraps]
-        for type_ in wraps:
+        for type_ in cls.wraps:
             if type_ != object:
                 if type_ in cls.subclasses:
                     raise DataTypeTreeError(f"A parser for {type_.__name__} was already found")
                 cls.subclasses[type_] = cls  # type: ignore
 
     @abstractmethod
     def _get_hash(self) -> Hashable:
         """Get a unique hash that identifies the current data type."""
 
     @final
+    @cache_returned_value_per_instance
     def __hash__(self) -> int:
         """Unique hash that identifies whether the current tree is considered to be unique."""
         return hash(self._get_hash())
 
     @abstractmethod
     def _get_str_top_node(self) -> str:
         """Get the type alias or the representation only for the current self.
@@ -194,15 +193,15 @@
 
     @final
     def get_str_all_nodes(self, include_imports: bool = True) -> str:
         """String that represents the .py file created from the tree."""
         return self._format_node_strings(self.get_strs_all_nodes_unformatted(include_imports=include_imports))
 
     @final
-    @cache_returned_value
+    @cache_returned_value_per_instance
     def get_strs_all_nodes_unformatted(self, *, include_imports: bool = True) -> Tuple[str, ...]:
         """Get, ordered by dependencies, all strings representing the whole tree."""
         strings: OrderedSet[str] = OrderedSet()
         self._get_strs_all_nodes_unformatted(types=strings)
         strings_lst = strings.as_list()
         if include_imports:
             strings_lst.insert(0, self.imports.format())
@@ -277,7 +276,23 @@
         print(repr(self))
 
     @final
     def __eq__(self, other_object: object) -> bool:
         if type(self) is type(other_object):
             return hash(self) == hash(other_object)
         return False
+
+    @final
+    def rename(self, new_name: str) -> None:
+        """Rename the current node and all its subsequent children."""
+        self._rename(new_name, len_old_name=len(self.name))
+
+    @final
+    def _rename(self, new_name: str, *, len_old_name: int) -> None:
+        """Rename the current node and all its subsequent children."""
+        if self.children:
+            for child in self:
+                child._rename(new_name=new_name, len_old_name=len_old_name)
+        if self.parent is not None:
+            self.name = new_name + self.name[len_old_name:]
+        else:
+            self.name = new_name
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     import pandas as pd
 
     from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import IteratorDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
+    from lazy_type_hint.data_type_tree.generic_type.mapping_proxy_data_type_tree import MappingProxyDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import PandasDataFrameDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import TupleDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.io_data_type_tree import IoDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.module_data_type_tree import ModuleTypeDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
@@ -37,14 +38,27 @@
     )
     from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
     from lazy_type_hint.utils import ImportManager
 
 
 @overload
 def data_type_tree_factory(  # type: ignore[overload-overlap]
+    data: "MappingProxyType[Any, Any]",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "MappingProxyDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[overload-overlap]
     data: "Iterator[Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
@@ -180,15 +194,15 @@
     parent: "Optional[DataTypeTree]" = None,
 ) -> "SequenceDataTypeTree":
     ...
 
 
 @overload
 def data_type_tree_factory(  # type: ignore[misc]
-    data: "Union[Mapping[Any, Any], MappingProxyType[Any, Any]]",
+    data: "Mapping[Any, Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "MappingDataTypeTree":
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,11 +9,14 @@
 with suppress(ImportError):
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import (
         PandasDataFrameDataTypeTree as PandasDataFrameDataTypeTree,
     )
 from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import (
     IteratorDataTypeTree as IteratorDataTypeTree,
 )
+from lazy_type_hint.data_type_tree.generic_type.mapping_proxy_data_type_tree import (
+    MappingProxyDataTypeTree as MappingProxyDataTypeTree,
+)
 from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree as SetDataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import (
     TupleDataTypeTree as TupleDataTypeTree,
 )
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import keyword
 from collections import defaultdict
 from dataclasses import dataclass, field
+from itertools import islice
 from typing import (
     Any,
     Dict,
     Hashable,
     Iterable,
     KeysView,
     List,
@@ -18,15 +19,20 @@
 )
 
 from typing_extensions import Self, TypeGuard, override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
 from lazy_type_hint.strategies import ParsingStrategies
-from lazy_type_hint.utils import TAB, format_string_as_docstring, is_string_python_keyword_compatible
+from lazy_type_hint.utils import (
+    TAB,
+    cache_returned_value_per_instance,
+    format_string_as_docstring,
+    is_string_python_keyword_compatible,
+)
 
 ValueT = TypeVar("ValueT")
 
 
 @dataclass(frozen=True)
 class DictMetadataComparison:
     common_keys: Set[Hashable] = field(default_factory=set)
@@ -105,23 +111,25 @@
     @property
     def is_typed_dict(self) -> bool:
         if self._all_keys_are_string(self._data) and self._strategies.dict_strategy == "TypedDict":
             return True
         return False
 
     @property
+    @cache_returned_value_per_instance
     def is_functional_syntax(self) -> bool:
         if self._all_keys_are_string(self._data) and self._all_keys_are_parsable():
             return False
         return True
 
     @staticmethod
     def _all_keys_are_string(dct: Mapping[Hashable, ValueT]) -> "TypeGuard[Mapping[str, ValueT]]":
         return all(isinstance(key, str) for key in dct)
 
+    @cache_returned_value_per_instance
     def _all_keys_are_parsable(self) -> bool:
         if self._all_keys_are_string(self._data) and all(key not in keyword.kwlist for key in self._data):
             return all(is_string_python_keyword_compatible(key) for key in self._data)
         return False
 
     def update(self, other: "DictMetadata") -> Mapping[Hashable, object]:
         """Update the wrapped dictionary and its metadata by including a new metadata object."""
@@ -194,15 +202,15 @@
                         dct[key] = formated_docstring
                     else:
                         dct[key] = unformatted_docstring
         return dct
 
 
 class DictDataTypeTree(MappingDataTypeTree):
-    wraps = dict  # type: ignore
+    wraps = (dict,)
     data: Dict[Hashable, object]
     dict_metadata: DictMetadata
 
     @staticmethod
     @override
     def _validate_name(name: str) -> None:
         """Removed name validation as the TypedDict can type any name."""
@@ -213,14 +221,17 @@
     def permission_to_be_created_as_type_alias(self) -> bool:
         if self.dict_metadata.is_typed_dict:
             return True
         return super().permission_to_be_created_as_type_alias
 
     @override
     def __pre_child_instantiation__(self) -> None:
+        check_n_max = self.strategies.check_max_n_elements_within_container
+        if self.strategies.dict_strategy != "TypedDict" and check_n_max:
+            self.data = dict(islice(self.data.items(), check_n_max))
         self.dict_metadata = DictMetadata(
             self.data, hidden_key_prefix=self.hidden_keys_prefix, strategies=self.strategies
         )
 
     @override
     def _get_str_top_node(self) -> str:
         if self.dict_metadata.is_typed_dict:
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import (
     SequenceDataTypeTree,
 )
 
 
 class IteratorDataTypeTree(SequenceDataTypeTree):
-    wraps = Iterator
+    wraps = (Iterator,)
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree, DataTypeTreeError
 from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import (
     SequenceDataTypeTree,
 )
 
 
 class ListDataTypeTree(SequenceDataTypeTree):
-    wraps = list
+    wraps = (list,)
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 import re
-from types import MappingProxyType
 from typing import Dict, Final, Hashable, Iterator, List, Literal, Mapping, Set
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.factory import data_type_tree_factory
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import GenericDataTypeTree
 from lazy_type_hint.file_modifiers.yaml_file_modifier import YamlFileModifier
 
 
 class MappingDataTypeTree(GenericDataTypeTree):
     children: Mapping[Hashable, DataTypeTree]
-    wraps = MappingProxyType
     hidden_keys_prefix: Final = YamlFileModifier.prefix
 
     # Iterable-protocol related
     _keys: Iterator[Hashable]
 
     @override
     def _instantiate_children(self, data: Mapping[Hashable, object]) -> Mapping[Hashable, DataTypeTree]:  # type: ignore
         children: Dict[Hashable, DataTypeTree] = {}
+
         for key, value in data.items():
             suffix = type(key).__name__ if not isinstance(key, str) else self._to_camel_case(key)
             if isinstance(key, str) and key.startswith(self.hidden_keys_prefix):
                 continue
             child = data_type_tree_factory(
                 data=value,
                 name=f"{self.name}{suffix}",
                 imports=self.imports,
                 depth=self.depth + 1,
                 strategies=self.strategies,
                 parent=self,
             )
             if child in children.values():
-                self._replace_old_childs_by_new_one(child, children)
+                self._replace_old_children_by_new_one(child, children)
                 children[key] = child
             else:
                 children[key] = child
         return children
 
-    def _replace_old_childs_by_new_one(self, child: DataTypeTree, children: Dict[Hashable, DataTypeTree]) -> None:
+    def _replace_old_children_by_new_one(self, child: DataTypeTree, children: Dict[Hashable, DataTypeTree]) -> None:
         """
         Replaces old child nodes with a new one in the given dictionary of children.
 
         Only replaced those children that are equal to the given child. In addition, naming is updated to
         make them match.
         """
         name = f"{self.name}{type(child.data).__name__.capitalize()}"
@@ -104,15 +103,18 @@
                     new_string[idx] = string[idx].upper()
                     removed = False
                 else:
                     new_string[idx] = string[idx]
             else:
                 removed = True
 
-        new_string[0] = new_string[0].upper()
+        try:
+            new_string[0] = new_string[0].upper()
+        except IndexError:
+            return string
         return "".join(new_string)
 
     @override
     def _get_hash(self) -> Hashable:
         hashes: List[object] = []
         for name, child in self.children.items():
             hashes.append(("mapping", hash(type(name)), child._get_hash()))
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             List[Union[Scalar, Tuple[Hashable, ...]]],
         ],
     ) -> Union[pd.Series, pd.DataFrame]:
         return super().__getitem__(key)"""
 
 
 class PandasDataFrameDataTypeTree(MappingDataTypeTree):
-    wraps = pd.DataFrame
+    wraps = (pd.DataFrame,)
     data: pd.DataFrame
     children: Mapping[str, DataTypeTree]  # type: ignore[assignment]
 
     @override
     @property
     def permission_to_be_created_as_type_alias(self) -> bool:
         return bool(len(self) >= 1 and self.are_columns_either_all_str_or_all_tuple)
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         if allow_repeated_children:
             children: Union[Set[DataTypeTree], List[DataTypeTree]] = []
         else:
             children = set()
         names_added: Dict[DataTypeTree, str] = {}  # Used to generate new and unique cnames in a quicker way.
 
         child: DataTypeTree
-        for element in data:
+        n_elements_to_check = self.data_type_tree.strategies.check_max_n_elements_within_container
+        for idx, element in enumerate(data):
+            if n_elements_to_check and idx >= n_elements_to_check:
+                break
             name = f"{self.data_type_tree.name}{type(element).__name__.capitalize()}"
             # Generate new name in case this one was already added
             if name in names_added.values():
                 modified_name = name
                 count = 2
                 while modified_name in names_added.values():
                     modified_name = f"{name}{count}"
@@ -58,28 +61,22 @@
                 name=name,
                 imports=self.data_type_tree.imports,
                 depth=self.data_type_tree.depth + 1,
                 parent=self.data_type_tree,
                 strategies=self.data_type_tree.strategies,
             )
             if allow_repeated_children:
+                # Tuple case
                 children = cast("List[DataTypeTree]", children)
                 if child in names_added:
-                    # Rebuild the tree with the name that is already defined
-                    child = data_type_tree_factory(
-                        data=element,
-                        name=names_added[child],
-                        imports=self.data_type_tree.imports,
-                        depth=self.data_type_tree.depth + 1,
-                        parent=self.data_type_tree,
-                        strategies=self.data_type_tree.strategies,
-                    )
+                    child.rename(names_added[child])
                 children.append(child)
                 names_added[child] = child.name
             else:
+                # List and Set cases
                 children = cast("Set[DataTypeTree]", children)
                 if child in children and isinstance(child, DictDataTypeTree) and child.dict_metadata.is_typed_dict:
                     self._update_existing_typed_dict_child_from_another_equal_child(children, child)
                 if child not in children:
                     children.add(child)
                     names_added[child] = name
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
 
 
 class TupleDataTypeTree(SequenceDataTypeTree):
-    wraps = tuple
+    wraps = (tuple,)
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         if self.strategies.tuple_size_strategy == "fixed":
             return self.operations.instantiate_children(data, allow_repeated_children=True)
         else:
             return self.operations.instantiate_children(data, allow_repeated_children=False)
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,22 +56,26 @@
 
     def get_func_params(self) -> MappingProxyType[str, Parameter]:
         signature = inspect.signature(self.data)
         return signature.parameters
 
     def _get_lambda_str(self) -> str:
         self.imports.add("Callable").add("Any")
-        return f"{self.name} = Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]"
+        if self.can_be_inspected:
+            return f"{self.name} = Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]"
+        return f"{self.name} = Callable"
 
     @override
     def _get_hash(self) -> Hashable:
-        if self.is_lambda:
+        if self.is_lambda and self.can_be_inspected:
             return str(f"Callable[[{', '.join(['Any']*len(self.get_func_params().values()))}], Any]")
         else:
-            return str(inspect.signature(self.data))
+            if self.can_be_inspected:
+                return str(inspect.signature(self.data))
+            return "Callable"
 
     def _has_return(self) -> Optional[bool]:
         code = textwrap.dedent(inspect.getsource(self.data))
         try:
             tree = ast.parse(code)
         except:  # noqa: E722
             return None
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.9/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
 
 
 class TypeDataTypeTree(SimpleDataTypeTree):
-    wraps = type
+    wraps = (type,)
     data: Type[object]
 
     @override
     def _get_str_top_node(self) -> str:
         self.imports.add("type")
         if self.is_builtin_class():
             return f"{self.name} = Type[{self.data.__name__}]"
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.9/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.9/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from lazy_type_hint.utils.import_manager import ImportManager as ImportManager
 from lazy_type_hint.utils.mypy import Mypy as Mypy
 from lazy_type_hint.utils.ordered_set import OrderedSet as OrderedSet
 from lazy_type_hint.utils.utils import (
     TAB as TAB,
 )
 from lazy_type_hint.utils.utils import (
-    cache_returned_value as cache_returned_value,
+    cache_returned_value_per_instance as cache_returned_value_per_instance,
 )
 from lazy_type_hint.utils.utils import (
     check_if_command_available as check_if_command_available,
 )
 from lazy_type_hint.utils.utils import (
     is_string_python_keyword_compatible as is_string_python_keyword_compatible,
 )
```

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.9/lazy_type_hint/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def __call__(*args: Any, **kwargs: Any) -> Any:
         ...
 
 
 _AnyMethodT = TypeVar("_AnyMethodT", bound=_AnyMethodProtocol)
 
 
-def cache_returned_value(method: _AnyMethodT) -> _AnyMethodT:
+def cache_returned_value_per_instance(method: _AnyMethodT) -> _AnyMethodT:
     """
     A decorator that caches the returned value of a method.
 
     This decorator can be used to cache the returned value of a method
     to improve performance by avoiding redundant computations.
 
     Args:
```

### Comparing `lazy_type_hint-2.0.8/pyproject.toml` & `lazy_type_hint-2.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.8"
+version = "2.0.9"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
@@ -20,14 +20,16 @@
 black = "23.12.1"  # Autoformatter
 pytest-clarity = "^1.0.1"
 pyyaml = "*"  # Used by the `check_code.py` script
 types-pyyaml = "*"
 filelock = "*"
 pytest_xdist = "*"  # Parallel execution tests
 pandas = "*"
+pyinstrument = "^4.6.2"
+pytest-benchmark = "^4.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Config for developer tools
@@ -64,11 +66,15 @@
 "tests/**/test_func_data_type_tree.py" = ["ARG005", "ARG001"]
 "lazy_type_hint/**/lazy_type_hint*.py" = ["ARG002"]
 
 [tool.codespell]
 ignore-words-list = "bu"  # Comma separated
 
 [tool.pytest.ini_options]
+markers = "integration"
 # addopts = "-vv"
 # addopts = ["-n", "auto", "-m", "not integration"]
 addopts = ["-n", "auto"]  # All tests
-testpaths = ["tests"]
+testpaths = ["tests"]
+
+# Commands:
+# poetry run pytest --benchmark-only
```

### Comparing `lazy_type_hint-2.0.8/README.md` & `lazy_type_hint-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.8/PKG-INFO` & `lazy_type_hint-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.8
+Version: 2.0.9
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

