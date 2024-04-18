# Comparing `tmp/dicomtrolley-3.0.5.tar.gz` & `tmp/dicomtrolley-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomtrolley-3.0.5.tar", max compression
+gzip compressed data, was "dicomtrolley-3.1.0.tar", max compression
```

## Comparing `dicomtrolley-3.0.5.tar` & `dicomtrolley-3.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/LICENSE
--rw-r--r--   0        0        0     1821 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/README.md
--rw-r--r--   0        0        0       87 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/__init__.py
--rw-r--r--   0        0        0     3189 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/auth.py
--rw-r--r--   0        0        0    21394 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/core.py
--rw-r--r--   0        0        0     8033 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/dicom_qr.py
--rw-r--r--   0        0        0      277 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/exceptions.py
--rw-r--r--   0        0        0     4398 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/fields.py
--rw-r--r--   0        0        0     7620 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/http.py
--rw-r--r--   0        0        0      135 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/logs.py
--rw-r--r--   0        0        0    10027 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/mint.py
--rw-r--r--   0        0        0     9350 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/parsing.py
--rw-r--r--   0        0        0    15671 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/qido_rs.py
--rw-r--r--   0        0        0    13586 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/rad69.py
--rw-r--r--   0        0        0     5429 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/servers.py
--rw-r--r--   0        0        0     2361 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/storage.py
--rw-r--r--   0        0        0    14906 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/trolley.py
--rw-r--r--   0        0        0     6768 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/wado_rs.py
--rw-r--r--   0        0        0     4990 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/wado_uri.py
--rw-r--r--   0        0        0    12337 2023-11-13 15:24:33.781897 dicomtrolley-3.0.5/dicomtrolley/xml_templates.py
--rw-r--r--   0        0        0     1392 2023-11-13 15:24:33.785897 dicomtrolley-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 dicomtrolley-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1821 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/README.md
+-rw-r--r--   0        0        0       87 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/auth.py
+-rw-r--r--   0        0        0    10593 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/caching.py
+-rw-r--r--   0        0        0    24676 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/core.py
+-rw-r--r--   0        0        0    11793 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/datastructures.py
+-rw-r--r--   0        0        0     8033 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/dicom_qr.py
+-rw-r--r--   0        0        0      446 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/exceptions.py
+-rw-r--r--   0        0        0     4398 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/fields.py
+-rw-r--r--   0        0        0     7620 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/http.py
+-rw-r--r--   0        0        0      135 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/logs.py
+-rw-r--r--   0        0        0    10027 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/mint.py
+-rw-r--r--   0        0        0     8231 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/parsing.py
+-rw-r--r--   0        0        0    15569 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/qido_rs.py
+-rw-r--r--   0        0        0    13586 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/rad69.py
+-rw-r--r--   0        0        0     5429 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/servers.py
+-rw-r--r--   0        0        0     2361 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/storage.py
+-rw-r--r--   0        0        0     7231 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/trolley.py
+-rw-r--r--   0        0        0     6768 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/wado_rs.py
+-rw-r--r--   0        0        0     4990 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/wado_uri.py
+-rw-r--r--   0        0        0    12337 2024-04-18 20:26:52.595606 dicomtrolley-3.1.0/dicomtrolley/xml_templates.py
+-rw-r--r--   0        0        0     1392 2024-04-18 20:26:52.599606 dicomtrolley-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 dicomtrolley-3.1.0/PKG-INFO
```

### Comparing `dicomtrolley-3.0.5/LICENSE` & `dicomtrolley-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/README.md` & `dicomtrolley-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/auth.py` & `dicomtrolley-3.1.0/dicomtrolley/auth.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/core.py` & `dicomtrolley-3.1.0/dicomtrolley/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,139 @@
 """Provides common base classes that allow modules to talk to each other."""
 from dataclasses import dataclass
 from datetime import date, datetime
-from enum import Enum
+from enum import Enum, IntEnum
 from itertools import chain
-from typing import List, Optional, Sequence, Type, TypeVar, Union
+from typing import (
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+)
 
 from pydantic import Field, ValidationError
 from pydantic.class_validators import validator
 from pydantic.main import BaseModel
 from pydicom.datadict import tag_for_keyword
 from pydicom.dataset import Dataset
 
 from dicomtrolley.exceptions import (
     DICOMTrolleyError,
+    NoReferencesFoundError,
     UnSupportedParameterError,
 )
 
 
-class DICOMObjectLevels:
-    """DICOM uses a study->series->instance structure"""
+class DICOMObjectLevels(IntEnum):
+    """Represents DICOM study->series->instance structure
+
+    Level is ordered. Study is highest, instance the lowest level.
+
+    Notes
+    -----
+    Similar to core.QueryLevels, but different enough to warrant separate classes.
+    DICOMObjectLevel is a property of a DICOM object. QueryLevel is a property of
+    a Query.
+    """
 
-    STUDY = "Study"
-    SERIES = "Series"
-    INSTANCE = "Instance"
+    STUDY = 2
+    SERIES = 1
+    INSTANCE = 0
 
-    all = [STUDY, SERIES, INSTANCE]
+    @classmethod
+    def from_query_level(cls, level: "QueryLevels"):
+        if level == QueryLevels.STUDY:
+            return cls.STUDY
+        elif level == QueryLevels.SERIES:
+            return cls.SERIES
+        elif level == QueryLevels.INSTANCE:
+            return cls.INSTANCE
+        else:
+            raise ValueError(f"Unknown DICOMObjectLevels {level}")
 
 
 class DICOMDownloadable:
     """An object that can be downloaded by a Downloader"""
 
     def reference(self) -> "DICOMObjectReference":
-        raise NotImplementedError
+        raise NotImplementedError()
+
+    def contained_references(
+        self, max_level: DICOMObjectLevels
+    ) -> Tuple["DICOMObjectReference", ...]:
+        """DICOM object references contained in this object at the given level.
 
+        For example, a Study might contain information for all its Instances. In
+        this case sub_references(max_level=Instance) will return InstanceReferences
 
-@dataclass
+        Parameters
+        ----------
+        max_level:
+            The returned references will be this level or lower. For example, an
+            instance will return a reference to itself when max_level is Series:
+                >>> Instance.contained_references(max_level=Series)
+                (InstanceReference,)
+            A study will be broken up:
+                >>> Study.contained_references(max_level=Series)
+                (SeriesReference, SeriesReference, ...)
+
+        Returns
+        -------
+        Tuple of references. Of max_level or lower
+
+        Raises
+        ------
+        NoReferencesFoundError
+            If sub-references cannot be obtained from this downloadable.
+
+        """
+        raise NotImplementedError()
+
+
+@dataclass(frozen=True)  # make this hashable and non-modifyable
 class DICOMObjectReference(DICOMDownloadable):
     """Points to a study, series, or instance by uid
 
     Contrary to DICOMObjects, DICOMObjectReferences are shallow. They do
     not have parents or children and do not contain any additional information.
 
     They were created to use in object-level downloads (download study X)
     """
 
     study_uid: str
 
     @property
-    def level(self) -> str:
+    def level(self):
         """Does this reference point to Study, Series or Instance?
         Returns
         -------
         str
             One of the values in DICOMObjectLevels.all
         """
-        return ""
+        return NotImplementedError()
 
     def reference(self):
         return self
 
+    def contained_references(
+        self, max_level: DICOMObjectLevels
+    ) -> Tuple["DICOMObjectReference", ...]:
+        """DICOM object references either return themselves or an error"""
+        if max_level < self.level:
+            raise NoReferencesFoundError(
+                f"{self} does not contain references of {str(max_level)} or lower"
+            )
+        else:
+            return (self.reference(),)
+
 
-@dataclass
+@dataclass(frozen=True)
 class InstanceReference(DICOMObjectReference):
     """All information needed to download a single slice (SOPInstance)"""
 
     study_uid: str
     series_uid: str
     instance_uid: str
 
@@ -75,30 +144,30 @@
         )
 
     @property
     def level(self):
         return DICOMObjectLevels.INSTANCE
 
 
-@dataclass
+@dataclass(frozen=True)
 class SeriesReference(DICOMObjectReference):
     """Reference to a single Series, part of a study"""
 
     study_uid: str
     series_uid: str
 
     def __str__(self):
         return f"SeriesReference {self.study_uid} -> {self.series_uid} "
 
     @property
     def level(self):
         return DICOMObjectLevels.SERIES
 
 
-@dataclass
+@dataclass(frozen=True)
 class StudyReference(DICOMObjectReference):
     """Reference to a single study"""
 
     study_uid: str
 
     def __str__(self):
         return f"StudyReference {self.study_uid}"
@@ -163,14 +232,36 @@
         Returns
         -------
         List[Series]
             All Series contained in this object
         """
         raise NotImplementedError()
 
+    def max_object_depth(self) -> DICOMObjectLevels:
+        """What is the deepest object level? Does contain only Study or also Series,
+        Instances?
+        """
+        raise NotImplementedError()
+
+    @staticmethod
+    def extract_refs(
+        objects: Iterable["DICOMObject"],
+    ) -> Tuple[DICOMObjectReference, ...]:
+        """Extract reference from each object and put in a tuple, raise error for
+        empty objects. For cleaner code in DICOMObject.contained_references()
+
+        Raises
+        ------
+        NoReferencesFoundError
+            if objects is empty
+        """
+        if not objects:
+            raise NoReferencesFoundError()
+        return tuple(x.reference() for x in objects)
+
 
 class Instance(DICOMObject):
     parent: "Series"
 
     def all_instances(self):
         """A list containing this instance itself. To match other signatures"""
         return [self]
@@ -188,14 +279,25 @@
         """Return a Reference to this object using uids"""
         return InstanceReference(
             study_uid=self.parent.parent.uid,
             series_uid=self.parent.uid,
             instance_uid=self.uid,
         )
 
+    def contained_references(
+        self, max_level: DICOMObjectLevels
+    ) -> Tuple["DICOMObjectReference", ...]:
+        return (self.reference(),)  # instance is deepest level so always OK
+
+    def max_object_depth(self) -> DICOMObjectLevels:
+        """What is the deepest object level? Does contain only Study or also Series,
+        Instances?
+        """
+        return DICOMObjectLevels.INSTANCE
+
 
 class Series(DICOMObject):
     instances: Sequence[Instance]
     parent: "Study"
 
     def __getitem__(self, instance_uid):
         return self.get(instance_uid)
@@ -222,14 +324,36 @@
                 f'instance with uid "{instance_uid}" not found in series'
             ) from e
 
     def reference(self) -> SeriesReference:
         """Return a Reference to this object using uids"""
         return SeriesReference(study_uid=self.parent.uid, series_uid=self.uid)
 
+    def contained_references(
+        self, max_level: DICOMObjectLevels
+    ) -> Tuple["DICOMObjectReference", ...]:
+
+        if max_level == DICOMObjectLevels.STUDY:
+            return self.extract_refs([self])
+        elif max_level == DICOMObjectLevels.SERIES:
+            return self.extract_refs([self])
+        elif max_level == DICOMObjectLevels.INSTANCE:
+            return self.extract_refs(self.all_instances())
+        else:
+            raise ValueError(f'unknown DICOMObjectLevel "{str(max_level)}"')
+
+    def max_object_depth(self) -> DICOMObjectLevels:
+        """What is the deepest object level? Does contain only Study or also Series,
+        Instances?
+        """
+        if self.instances:
+            return DICOMObjectLevels.INSTANCE
+        else:
+            return DICOMObjectLevels.SERIES
+
 
 class Study(DICOMObject):
     series: Sequence[Series]
 
     def __getitem__(self, series_uid) -> Series:
         return self.get(series_uid)
 
@@ -255,14 +379,36 @@
                 f'series with uid "{series_uid}" not found in study'
             ) from e
 
     def reference(self) -> StudyReference:
         """Return a Reference to this object using uids"""
         return StudyReference(study_uid=self.uid)
 
+    def contained_references(
+        self, max_level: DICOMObjectLevels
+    ) -> Tuple["DICOMObjectReference", ...]:
+
+        if max_level == DICOMObjectLevels.STUDY:
+            return self.extract_refs([self])
+        elif max_level == DICOMObjectLevels.SERIES:
+            return self.extract_refs(self.all_series())
+        elif max_level == DICOMObjectLevels.INSTANCE:
+            return self.extract_refs(self.all_instances())
+        else:
+            raise ValueError(f'unknown DICOMObjectLevel "{str(max_level)}"')
+
+    def max_object_depth(self) -> DICOMObjectLevels:
+        """What is the deepest object level? Does contain only Study or also Series,
+        Instances?
+        """
+        if self.series:
+            return self.series[0].max_object_depth()
+        else:
+            return DICOMObjectLevels.STUDY
+
 
 class NonInstanceParameterError(DICOMTrolleyError):
     """A DICOMDownloadable could not be converted into its constituent instances.
 
     Trolley allows the downloading of higher-level DICOM objects like
     download(StudyInstanceUID='1234'). Some Downloader implementations can handle
     this out of the box. Others, like WADO-URI, cannot, and instead require the
@@ -278,114 +424,73 @@
 
 class NonSeriesParameterError(DICOMTrolleyError):
     """A DICOMDownloadable could not be converted into Series or Instance reference.
     Weaker version of NonInstanceParameterError
     """
 
 
-def to_instance_refs(
-    objects: Sequence[DICOMDownloadable],
-) -> List[InstanceReference]:
-    """Convert all input to instance references. Raise informative errors.
-
-    This is a common pre-processing step used by Downloader classes. Many cannot
-    download higher-level objects like 'study 123' directly, but instead require
-    you to query all instances contained in 'study 123' first and pass those to
-    the downloader.
-
-    Parameters
-    ----------
-    objects:
-        Convert these objects
-
-    Returns
-    -------
-    List[InstanceReference]
-        References to all instances contained in objects
-
-    Raises
-    ------
-    NonInstanceParameterError
-        If any input object could not be converted into instances. This is the
-        case for higher-level references like StudyReference, or for DICOMObjects
-        that do not contain any deeper-level information, such as a Study that
-        contains no Series (which is the correct result of Study-level queries).
-
-    """
-    output: List[InstanceReference] = []
-    for obj in objects:
-        if isinstance(obj, InstanceReference):
-            output.append(obj)  # Already an instance reference. Just add
-        elif isinstance(obj, DICOMObjectReference):
-            raise NonInstanceParameterError(
-                f"Cannot extract instances from '{obj}' "
-            )
-        elif isinstance(obj, DICOMObject):
-            instances = obj.all_instances()  # Extract instances
-            if instances:
-                output = output + [x.reference() for x in instances]
-            else:
-                raise NonInstanceParameterError(
-                    f"{obj} contains no instances. "
-                    f"Was this information queried for?"
-                )
-
-    return output
-
-
-def to_series_level_refs(
-    objects: Sequence[DICOMDownloadable],
-) -> List[Union[SeriesReference, InstanceReference]]:
-    """Make sure all input objects are Series or Instance references.
-    Convert if possible, raise exceptions if not.
-
-    Weaker version of to_instance_refs(). Weaker because series references without
-    instance info are also allowed here. See that function for more info
+def to_instance_refs(objects: Sequence[DICOMDownloadable]):
+    """Convert all to instance references. See to_refs()"""
+    try:
+        return to_references(objects, max_level=DICOMObjectLevels.INSTANCE)
+    except NoReferencesFoundError as e:
+        raise NonInstanceParameterError(
+            f"Cannot obtain instance references: {e}"
+        ) from e
+
+
+def to_series_level_refs(objects: Sequence[DICOMDownloadable]):
+    """Convert all to at least series references."""
+    try:
+        return to_references(objects, max_level=DICOMObjectLevels.SERIES)
+    except NoReferencesFoundError as e:
+        raise NonSeriesParameterError(
+            f"Cannot obtain series references: {e}"
+        ) from e
+
+
+def to_references(
+    objects: Sequence[DICOMDownloadable], max_level: DICOMObjectLevels
+) -> List[DICOMObjectReference]:
+    """Make sure all input objects are of max_level or lower. Extract lower level
+    references if possible. For example, if max_level is series, try to extract
+    series references from a study. Raise exceptions if not possible.
 
     Parameters
     ----------
     objects:
         Convert these objects
+    max_level:
+        Return references of this level or lower, otherwise raise exception.
 
     Returns
     -------
     List[Union[SeriesReference, InstanceReference]]
         References to series and instances contained in input objects
 
+    Notes
+    -----
+    This is a common pre-processing step used by Downloader classes. Many cannot
+    download higher-level objects like 'study 123' directly, but instead require
+    you to query all instances contained in 'study 123' first and pass those to
+    the downloader.
+
     Raises
     ------
-    NonSeriesParameterError
+    NoReferencesFoundError
         If any input object could not be converted into instances. This is the
         case for higher-level references like StudyReference, or for DICOMObjects
         that do not contain any deeper-level information, such as a Study that
-        contains no Series (which is the correct result of Study-level queries).
+        contains no Series (which is a correct result for Study-level queries).
 
     """
-    output: List[Union[InstanceReference, SeriesReference]] = []
+    refs: List[DICOMObjectReference] = []
     for obj in objects:
-        if isinstance(
-            obj, (InstanceReference, SeriesReference, Instance, Series)
-        ):
-            # already OK, just add
-            output.append(obj.reference())
-        elif isinstance(obj, StudyReference):
-            # no series in here, I don't have enough info
-            raise NonSeriesParameterError(
-                f"Cannot extract series from '{obj}' "
-            )
-        elif isinstance(obj, Study):
-            if obj.series:
-                for series in obj.series:
-                    output.append(series.reference())
-            else:
-                raise NonSeriesParameterError(
-                    f"Cannot extract series from '{obj}'"
-                    f". It contains no series "
-                )
-    return output
+        refs.extend(obj.contained_references(max_level=max_level))
+    return refs
 
 
 class Downloader:
     """Something that can download DICOM images. Base class"""
 
     def get_dataset(self, instance: InstanceReference):
         """Get DICOM dataset for the given instance (slice)
@@ -412,15 +517,15 @@
         Raises
         ------
         NonInstanceParameterError
             If objects contain non-instance targets like a StudyInstanceUID and
             download can only process Instance targets. See Exception docstring
             for rationale
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def datasets_async(
         self, instances: Sequence[InstanceReference], max_workers=None
     ):
         """Retrieve each instance in multiple threads
 
         Parameters
@@ -436,24 +541,36 @@
         DICOMTrolleyError
             When a server response cannot be parsed as DICOM
 
         Returns
         -------
         Iterator[Dataset, None, None]
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 class QueryLevels(str, Enum):
     """Used in dicom queries to indicate how rich the search should be"""
 
     STUDY = "STUDY"
     SERIES = "SERIES"
     INSTANCE = "INSTANCE"
 
+    @classmethod
+    def from_object_level(cls, level: DICOMObjectLevels):
+        """Convert from DICOMObjectLevel enum. See docstring there for reason"""
+        if level == DICOMObjectLevels.STUDY:
+            return cls.STUDY
+        elif level == DICOMObjectLevels.SERIES:
+            return cls.SERIES
+        elif level == DICOMObjectLevels.INSTANCE:
+            return cls.INSTANCE
+        else:
+            raise ValueError(f"Unknown DICOMObjectLevels {level}")
+
 
 # Used in Query.init_from_query() type annotation
 QuerySubType = TypeVar("QuerySubType", bound="Query")
 
 
 class Query(BaseModel):
     """A simple DICOM query that is acceptable to all Searcher classes
@@ -615,81 +732,42 @@
         if len(results) == 0 or len(results) > 1:
             raise DICOMTrolleyError(
                 f"Expected exactly one study for query '{query.to_short_string()}',"
                 f" but found {len(results)}"
             )
         return results[0]
 
-    def find_full_study_by_id(self, study_uid: str) -> Study:
-        """Find a single study at image level
+    def find_study_by_id(
+        self, study_uid: str, query_level: QueryLevels = QueryLevels.STUDY
+    ) -> Study:
+        """Find a single study at the given depth
 
         Useful for automatically finding all instances for a study. Meant to be
         implemented in child classes
 
         Parameters
         ----------
         study_uid: str
             Study to search for
+        query_level: QueryLevels
+            Depth of search. Whether to find only study level info or go deeper into
+            series or instances. Deeper levels will result in slower, more extensive
+            searches
 
         Returns
         -------
         Study
+            Potentially containing series or instances, dependent on query_level
 
-        Raises
-        ------
-        DICOMTrolleyError
-            If no results or more than one result is returned by query
-        """
-        raise NotImplementedError()
-
-    def find_study_at_instance_level(self, study_uid: str) -> Study:
-        """Find a single study at image level
-
-        Useful for automatically finding all instances for a study.
-
-        Parameters
-        ----------
-        study_uid: str
-            Study to search for
-
-        Returns
-        -------
-        Study
-            Containing full DICOM object information, series and instances
-
-        Raises
-        ------
-        DICOMTrolleyError
-            If no results or more than one result is returned by query
-        """
-        return self.find_study(
-            Query(StudyInstanceUID=study_uid, query_level=QueryLevels.INSTANCE)
-        )
-
-    def find_study_at_series_level(self, study_uid: str) -> Study:
-        """Find a single study at series level
-
-        Meant to be
-        implemented in child classes
-
-        Parameters
-        ----------
-        study_uid: str
-            Study to search for
-
-        Returns
-        -------
-        Study
-            Containing series, but not instances
 
         Raises
         ------
         DICOMTrolleyError
             If no results or more than one result is returned by query
         """
         return self.find_study(
-            Query(StudyInstanceUID=study_uid, query_level=QueryLevels.SERIES)
+            Query(StudyInstanceUID=study_uid, query_level=query_level)
         )
 
 
 Instance.update_forward_refs()  # enables pydantic validation
 Series.update_forward_refs()
```

### Comparing `dicomtrolley-3.0.5/dicomtrolley/dicom_qr.py` & `dicomtrolley-3.1.0/dicomtrolley/dicom_qr.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/fields.py` & `dicomtrolley-3.1.0/dicomtrolley/fields.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/http.py` & `dicomtrolley-3.1.0/dicomtrolley/http.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/mint.py` & `dicomtrolley-3.1.0/dicomtrolley/mint.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/parsing.py` & `dicomtrolley-3.1.0/dicomtrolley/parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,34 @@
 """Models parsing things into study/series/instance structure"""
-from typing import Any, DefaultDict, Dict, List, Sequence
+from typing import Dict, List, Sequence
 
 from pydicom.dataset import Dataset
 
 from dicomtrolley.core import (
     DICOMObject,
     DICOMObjectReference,
     Instance,
     InstanceReference,
     Series,
     SeriesReference,
     Study,
     StudyReference,
 )
+from dicomtrolley.datastructures import TreeNode
 from dicomtrolley.exceptions import DICOMTrolleyError
 
 
 def flatten(dicom_object) -> List[DICOMObject]:
     """All nodes and as a flat list, study, series"""
     nodes = [dicom_object]
     for child in dicom_object.children():
         nodes = nodes + flatten(child)
     return nodes
 
 
-class TreeNode(DefaultDict[Any, "TreeNode"]):
-    """Recursive defaultdict with a 'data' property. Helps parse to tree structures.
-
-    Examples
-    --------
-    >>> root = TreeNode()
-    >>> root['study1']['series1']['instance1'].data = 'some instance info'
-    >>> 'study1' in root
-    True
-    >>> root['study1']['series2'].data = 'some series data'
-    >>> list(root['study1'].keys)
-    ['series1', 'series2']
-    """
-
-    def __init__(self, data=None, allow_overwrite=True):
-        """
-
-        Parameters
-        ----------
-        data:
-            Optional data to associate with this node
-        allow_overwrite: bool, optional
-            If False, will raise exception when overwriting data attribute
-        """
-        super().__init__(lambda: TreeNode(allow_overwrite=allow_overwrite))
-        self._data = data
-        self.allow_overwrite = allow_overwrite
-
-    @property
-    def data(self):
-        return self._data
-
-    @data.setter
-    def data(self, value):
-        if self.allow_overwrite or not self.data:
-            self._data = value
-        else:
-            raise ValueError("Overwriting data is not allowed")
-
-
 class DICOMParseTree:
     """Models study/series/instance as a tree. Allows arbitrary branch insertions"""
 
     def __init__(self, root=None, allow_overwrite=False):
         """
 
         Parameters
@@ -83,15 +44,15 @@
 
     @classmethod
     def init_from_objects(cls, objects: Sequence[DICOMObject]):
         """Create a tree from given objects. Useful for augmenting query results
 
         Notes
         -----
-        Parent objects for instances and series will be created to maintain to
+        Parent objects for instances and series will be created to
         ensure all nodes are connected to the tree root. For example, running this
         method with only a single instance as input will result in a regular
         root->study->series->instance tree. This is possible because all DICOMObjects
         maintain links to their parent objects
 
         Returns
         -------
@@ -185,15 +146,15 @@
                 return val
             else:
                 return Dataset()
 
         study_instance_uid, study_node = study_node_in
 
         study = Study(
-            uid=study_instance_uid,
+            uid=str(study_instance_uid),
             data=value_or_dataset(study_node.data),
             series=tuple(),
         )
         all_series = []
         for series_instance_uid, series_node in study_node.items():
             series = Series(
                 uid=series_instance_uid,
@@ -259,15 +220,14 @@
         """Retrieve data for the given study, series or instance from tree
 
         Raises
         ------
         DICOMObjectNotFound
             If data for the given parameters does not exist in tree
         """
-
         try:
             if isinstance(reference, StudyReference):
                 return self[reference.study_uid]
             elif isinstance(reference, SeriesReference):
                 return self[reference.study_uid].get(reference.series_uid)
             elif isinstance(reference, InstanceReference):
                 return (
```

### Comparing `dicomtrolley-3.0.5/dicomtrolley/qido_rs.py` & `dicomtrolley-3.1.0/dicomtrolley/qido_rs.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     def uri_base(self) -> str:
         """WADO-RS url to call when performing this query. Full URI also needs
         uri_search_params()
 
         The non-query part of the URI as defined in
         DICOM PS3.18 section 10.6 table 10.6.1-2
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def uri_search_params(self) -> Dict[str, Union[str, List[str]]]:
         """The search parameter part of the URI as defined in
         DICOM PS3.18 section 10.6 table 10.6.1-2
 
         Returns
         -------
@@ -297,49 +297,41 @@
     @root_validator()  # type: ignore
     def query_level_should_be_series_or_instance(
         cls, values  # noqa: B902, N805
     ):
         """A relational query only makes sense for the instance and series levels.
         If you want to look for studies, us a hierarchical query
         """
-        if values["query_level"] == QueryLevels.STUDY:
+        if values.get("query_level") == QueryLevels.STUDY:
             raise ValueError(STUDY_VALUE_ERROR_TEXT)
 
         return values
 
     def uri_base(self) -> str:
         """WADO-RS url to call when performing this query. Full URI also needs
         uri_search_params()
 
         The non-query part of the URI as defined in
         DICOM PS3.18 section 10.6 table 10.6.1-2
-
-        Raises
-        ------
-        ValueError
-            if query_level is STUDY. This makes no sense for a relational query
         """
 
-        if self.query_level == QueryLevels.STUDY:
-            raise ValueError(STUDY_VALUE_ERROR_TEXT)
-        elif self.query_level == QueryLevels.SERIES:
+        # QueryLevels.Study is checked in query_level_should_be_series_or_instance()
+        if self.query_level == QueryLevels.SERIES:
             return "/series"
         elif self.query_level == QueryLevels.INSTANCE:
             if self.StudyInstanceUID:
                 # all instances for this study
                 return f"/studies/{self.StudyInstanceUID}/instances"
             else:
-                # all instances on the intire server (might be slow)
+                # all instances on the entire server (might be slow)
                 return "/instances"
-
         else:
-            raise ValueError(
-                f'Unknown querylevel "{self.query_level}". '
-                f'Should be one of "{QueryLevels}"'
-            )
+            # Unreachable due to pydantic validation and root validator. But I
+            # get uncomfortable from open elifs.
+            raise ValueError(f"Unknown query level {self.query_level}")
 
 
 class QidoRS(Searcher):
     """A connection to a QIDO-RS server"""
 
     def __init__(self, session, url):
         """
```

### Comparing `dicomtrolley-3.0.5/dicomtrolley/rad69.py` & `dicomtrolley-3.1.0/dicomtrolley/rad69.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/servers.py` & `dicomtrolley-3.1.0/dicomtrolley/servers.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/storage.py` & `dicomtrolley-3.1.0/dicomtrolley/storage.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/wado_rs.py` & `dicomtrolley-3.1.0/dicomtrolley/wado_rs.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/wado_uri.py` & `dicomtrolley-3.1.0/dicomtrolley/wado_uri.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/dicomtrolley/xml_templates.py` & `dicomtrolley-3.1.0/dicomtrolley/xml_templates.py`

 * *Files identical despite different names*

### Comparing `dicomtrolley-3.0.5/pyproject.toml` & `dicomtrolley-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicomtrolley"
-version = "3.0.5"
+version = "3.1.0"
 description = "Retrieve medical images via WADO-URI, WADO-RS, QIDO-RS, MINT, RAD69 and DICOM-QR"
 authors = ["sjoerdk <sjoerd.kerkstra@radboudumc.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/sjoerdk/dicomtrolley"
 
 [tool.black]
```

### Comparing `dicomtrolley-3.0.5/PKG-INFO` & `dicomtrolley-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomtrolley
-Version: 3.0.5
+Version: 3.1.0
 Summary: Retrieve medical images via WADO-URI, WADO-RS, QIDO-RS, MINT, RAD69 and DICOM-QR
 Home-page: https://github.com/sjoerdk/dicomtrolley
 License: Apache-2.0
 Author: sjoerdk
 Author-email: sjoerd.kerkstra@radboudumc.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

