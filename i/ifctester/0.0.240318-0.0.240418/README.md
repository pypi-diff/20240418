# Comparing `tmp/ifctester-0.0.240318.tar.gz` & `tmp/ifctester-0.0.240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.240318.tar", last modified: Mon Mar 18 01:13:14 2024, max compression
+gzip compressed data, was "ifctester-0.0.240418.tar", last modified: Thu Apr 18 01:14:03 2024, max compression
```

## Comparing `ifctester-0.0.240318.tar` & `ifctester-0.0.240418.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:13:14.371914 ifctester-0.0.240318/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-18 01:13:14.371914 ifctester-0.0.240318/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-18 01:13:10.000000 ifctester-0.0.240318/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:13:14.371914 ifctester-0.0.240318/ifctester/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49559 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/ids.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:13:14.371914 ifctester-0.0.240318/ifctester/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-03-18 01:13:10.000000 ifctester-0.0.240318/ifctester/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:13:14.371914 ifctester-0.0.240318/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-18 01:13:14.000000 ifctester-0.0.240318/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-18 01:13:14.000000 ifctester-0.0.240318/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 01:13:14.000000 ifctester-0.0.240318/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-18 01:13:14.000000 ifctester-0.0.240318/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-18 01:13:14.000000 ifctester-0.0.240318/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-18 01:13:12.000000 ifctester-0.0.240318/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 01:13:14.371914 ifctester-0.0.240318/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 01:13:14.371914 ifctester-0.0.240318/test/
--rw-r--r--   0 runner    (1001) docker     (127)    88893 2024-03-18 01:13:10.000000 ifctester-0.0.240318/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-03-18 01:13:10.000000 ifctester-0.0.240318/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.941325 ifctester-0.0.240418/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-18 01:14:03.941325 ifctester-0.0.240418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-18 01:14:00.000000 ifctester-0.0.240418/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49995 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/ids.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/ifctester/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.941325 ifctester-0.0.240418/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-18 01:14:02.000000 ifctester-0.0.240418/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:14:03.941325 ifctester-0.0.240418/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    89195 2024-04-18 01:14:00.000000 ifctester-0.0.240418/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-04-18 01:14:00.000000 ifctester-0.0.240418/test/test_ids.py
```

### Comparing `ifctester-0.0.240318/PKG-INFO` & `ifctester-0.0.240418/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 2.1
-Name: ifctester
-Version: 0.0.240318
-Summary: IFC model auditing tool with support for IDS
-Author-email: Dion Moult <dion@thinkmoult.com>
-Project-URL: Homepage, http://ifcopenshell.org
-Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
-Keywords: IFC,IDS,BIM
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Description-Content-Type: text/markdown
-Requires-Dist: ifcopenshell
-
 # ifctester
 
 With **IfcTester**, you can author and read **Information Delivery Specification** - **IDS** - files and validate your IFC models against IDS to see if your model is compliant. After the audit, you can generate reports in console, as a web page, JSON or BCF file. It works from the command line, as a web app, or as a library.
 
 ## How to use it
 
+### Command line use
+
+.. code-block:: bash
+
+    # run console reporter
+    python -m ifctester example.ids example.ifc
+    python -m ifctester example.ids example.ifc -r Html -o report.html
+
+Available flags:
+
+- ``-r`` / ``--reporter``: The reporting method to view audit results. Availabe reporters: Console, Txt, Json, Html, Ods, Bcf
+- ``--no-color``: Disable colour output (supported by Console reporting).
+- ``--excel-safe``: Make sure exported ODS is safely exported for Excel.
+- ``-o`` / ``--output``: Output file (supported for all types of reporting except Console).
+
+### Code example
+
 ```python
 import ifcopenshell
 from ifctester import ids, reporter
 
 
 # create new IDS
 my_ids = ids.Ids(title="My IDS")
 
 # add specification to it
 my_spec = ids.Specification(name="My first specification")
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
-    name="IsExternal", 
+    baseName="IsExternal",
     value="TRUE", 
     propertySet="Pset_WallCommon", 
-    datatype="IfcBoolean",
+    dataType="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
     instructions="Walls need to be load bearing.",
-    minOccurs=1,
-    maxOccurs="unbounded")
+    cardinality="required")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
 
 # Save such IDS to file
 result = my_ids.to_xml("SampleIDS.xml")
 
 # open  IFC file:
```

### Comparing `ifctester-0.0.240318/ifctester/__init__.py` & `ifctester-0.0.240418/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240318/ifctester/__main__.py` & `ifctester-0.0.240418/ifctester/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,18 +27,21 @@
 parser = argparse.ArgumentParser(description="Uses an IDS to audit an IFC")
 parser.add_argument("ids", type=str, help="Path to an IDS")
 parser.add_argument("ifc", type=str, help="Path to an IFC")
 parser.add_argument(
     "-r", "--reporter", type=str, help="The reporting method to view audit results", default="Console"
 )
 parser.add_argument(
-    "--no-color", help="Disable colour output supported by Console reporting", action="store_true"
+    "--no-color", help="Disable colour output (supported by Console reporting)", action="store_true"
 )
 parser.add_argument(
-    "-o", "--output", help="Output file supported by Json reporting"
+    "--excel-safe", help="Make sure exported ODS is safely exported for Excel", action="store_true"
+)
+parser.add_argument(
+    "-o", "--output", help="Output file (supported for all types of reporting except Console)"
 )
 args = parser.parse_args()
 
 start = time.time()
 specs = ids.open(args.ids)
 ifc = ifcopenshell.open(args.ifc)
 print("Finished loading:", time.time() - start)
@@ -52,15 +55,15 @@
 elif args.reporter == "Txt":
     engine = reporter.Txt(specs)
 elif args.reporter == "Json":
     engine = reporter.Json(specs)
 elif args.reporter == "Html":
     engine = reporter.Html(specs)
 elif args.reporter == "Ods":
-    engine = reporter.Ods(specs)
+    engine = reporter.Ods(specs, excel_safe=args.excel_safe)
 elif args.reporter == "Bcf":
     engine = reporter.Bcf(specs)
 
 engine.report()
 
 if args.output:
     engine.to_file(args.output)
```

### Comparing `ifctester-0.0.240318/ifctester/facet.py` & `ifctester-0.0.240418/ifctester/facet.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcTester.  If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 import re
 import builtins
 import ifcopenshell.util.unit
 import ifcopenshell.util.element
 import ifcopenshell.util.classification
 from functools import lru_cache
 from xmlschema.validators import identities
-from typing import List, Union
+from typing import Union, Optional, Any, Literal, TYPE_CHECKING, TypedDict
+from logging import Logger
+
+if TYPE_CHECKING:
+    from .ids import Specification
 
 
 def cast_to_value(from_value, to_value):
     try:
         target_type = type(to_value).__name__
         if target_type == "int":
             # Casting str -> float means that notation like '1e3' is preserved
@@ -49,60 +54,74 @@
 
 
 @lru_cache
 def get_psets(element):
     return ifcopenshell.util.element.get_psets(element)
 
 
+Cardinality = Literal["required", "optional", "prohibited"]
+
+
+class FacetFailure(TypedDict):
+    element: ifcopenshell.entity_instance
+    reason: str
+
+
 class Facet:
+    cardinality: Cardinality
+
     def __init__(self, *parameters):
         self.status = None
-        self.failed_entities: List[Facet] = []
-        self.failed_reasons: List[str] = []
+        self.failures: list[FacetFailure] = []
         for i, name in enumerate(self.parameters):
             setattr(self, name.replace("@", ""), parameters[i])
 
-    def asdict(self, clause_type):
+    def asdict(self, clause_type: str) -> dict[str, Any]:
         results = {}
         for name in self.parameters:
             value = getattr(self, name.replace("@", ""))
             if value is not None:
+                if name == "@dataType":
+                    value = value.upper()
                 results[name] = value if "@" in name else self.to_ids_value(value)
         if clause_type == "applicability":
-            for key in ["@uri", "@instructions", "@minOccurs", "@maxOccurs"]:
+            for key in ["@uri", "@instructions", "@cardinality"]:
                 results.pop(key, None)
         return results
 
     def parse(self, xml):
-        setattr(self, "minOccurs", 1)
-        setattr(self, "maxOccurs", 1)
+        setattr(self, "cardinality", "required")
         for name, value in xml.items():
             name = name.replace("@", "")
             if isinstance(value, dict) and "simpleValue" in value.keys():
                 setattr(self, name, value["simpleValue"])
             elif isinstance(value, dict) and "restriction" in value.keys():
-                setattr(self, name, Restriction().parse(value["restriction"][0]))
-                # TODO handle more than one restriction: return [restriction(r) for r in v["restriction"]]
+                setattr(self, name, Restriction().parse(value["restriction"]))
             else:
                 setattr(self, name, value)
         return self
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: List[ifcopenshell.entity_instance]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: list[ifcopenshell.entity_instance]
+    ) -> list[ifcopenshell.entity_instance]:
         return [e for e in elements if self(e)]
 
-    def to_string(self, clause_type, specification=None, requirement=None):
+    def to_string(
+        self,
+        clause_type: str,
+        specification: Optional[Specification] = None,
+        requirement: Optional[Facet] = None,
+    ) -> str:
         if clause_type == "applicability":
             templates = self.applicability_templates
         elif clause_type == "requirement":
             is_prohibited = False
             if specification.maxOccurs == 0:
                 is_prohibited = not is_prohibited
-            if requirement.maxOccurs == 0:
+            if requirement.cardinality == "prohibited":
                 is_prohibited = not is_prohibited
             templates = self.prohibited_templates if is_prohibited else self.requirement_templates
 
         for template in templates:
             total_variables = len(template) - len(template.replace("{", ""))
             total_replacements = 0
             for key in self.parameters:
@@ -111,36 +130,34 @@
                 key_variable = "{" + key + "}"
                 if value is not None and key_variable in template:
                     template = template.replace(key_variable, str(value))
                     total_replacements += 1
                 if total_replacements == total_variables:
                     return template
 
-    def to_ids_value(self, parameter):
+    def to_ids_value(self, parameter: Union[str, Restriction, list]) -> dict[str, Any]:
         if isinstance(parameter, str):
             parameter_dict = {"simpleValue": parameter}
         elif isinstance(parameter, Restriction):
             parameter_dict = {"xs:restriction": [parameter.asdict()]}
         elif isinstance(parameter, list):
             restrictions = {"@base": "xs:" + parameter[0].base}
             for p in parameter:
                 x = p.asdict()
                 restrictions[list(x)[1]] = x[list(x)[1]]
             parameter_dict = {"xs:restriction": [restrictions]}
         else:
             raise Exception(str(parameter) + " was not able to be converted into 'Parameter_dict'")
         return parameter_dict
 
-    def get_usage(self):
-        if self.minOccurs != 0:
-            return "required"
-        elif self.minOccurs == 0 and self.maxOccurs != 0:
-            return "optional"
-        elif self.maxOccurs == 0:
-            return "prohibited"
+    def get_usage(self) -> Cardinality:
+        return self.cardinality
+
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> Result:
+        raise NotImplementedError
 
 
 class Entity(Facet):
     def __init__(self, name="IFCWALL", predefinedType=None, instructions=None):
         self.parameters = ["name", "predefinedType", "@instructions"]
         self.applicability_templates = [
             "All {name} data of type {predefinedType}",
@@ -152,15 +169,17 @@
         ]
         self.prohibited_templates = [
             "Shall not be {name} data of type {predefinedType}",
             "Shall not be {name} data",
         ]
         super().__init__(name, predefinedType, instructions)
 
-    def filter(self, ifc_file, elements):
+    def filter(
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]] = None
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
 
         if isinstance(self.name, str):
             try:
                 results = ifc_file.by_type(self.name, include_subtypes=False)
             except:
@@ -175,15 +194,15 @@
                 except:
                     # If the user has specified a class that doesn't exist in the version
                     continue
         if self.predefinedType:
             return [r for r in results if self(r)]
         return results
 
-    def __call__(self, inst, logger=None):
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> EntityResult:
         is_pass = inst.is_a().upper() == self.name
         reason = None
 
         if not is_pass:
             reason = {"type": "NAME", "actual": inst.is_a().upper()}
 
         if is_pass and self.predefinedType:
@@ -193,33 +212,33 @@
             if not is_pass:
                 reason = {"type": "PREDEFINEDTYPE", "actual": predefined_type}
 
         return EntityResult(is_pass, reason)
 
 
 class Attribute(Facet):
-    def __init__(self, name="Name", value=None, minOccurs=None, maxOccurs=None, instructions=None):
-        self.parameters = ["name", "value", "@minOccurs", "@maxOccurs", "@instructions"]
+    def __init__(self, name="Name", value=None, cardinality: Cardinality = "required", instructions=None):
+        self.parameters = ["name", "value", "@cardinality", "@instructions"]
         self.applicability_templates = [
             "Data where the {name} is {value}",
             "Data where the {name} is provided",
         ]
         self.requirement_templates = [
             "The {name} shall be {value}",
             "The {name} shall be provided",
         ]
         self.prohibited_templates = [
             "The {name} shall not be {value}",
             "The {name} shall not be provided",
         ]
-        super().__init__(name, value, minOccurs, maxOccurs, instructions)
+        super().__init__(name, value, cardinality, instructions)
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: Union[ifcopenshell.entity_instance, None]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
 
         results = []
         schema = ifcopenshell.ifcopenshell_wrapper.schema_by_name(ifc_file.schema)
         entities = {entity.name(): entity for entity in schema.entities()}
 
@@ -237,16 +256,16 @@
                     # e.g. if IfcRoot already has .Name, it's safe not to check all it's subtypes attributes
                     ignore_subtypes(entity)
 
         # TODO: perhaps we should consider value in the filter
 
         return results
 
-    def __call__(self, inst, logger=None):
-        if self.minOccurs == 0 and self.maxOccurs != 0:
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> AttributeResult:
+        if self.cardinality == "optional":
             return AttributeResult(True)
 
         if isinstance(self.name, str):
             names = [self.name]
             attribute_type = inst.wrapped_data.get_attribute_category(self.name)
             if attribute_type == 1:  # Forward attribute
                 values = [getattr(inst, self.name, None)]
@@ -319,53 +338,50 @@
                         reason = {"type": "VALUE", "actual": value}
                         break
                 elif value != self.value:
                     is_pass = False
                     reason = {"type": "VALUE", "actual": value}
                     break
 
-        if self.maxOccurs == 0:
+        if self.cardinality == "prohibited":
             return AttributeResult(not is_pass, {"type": "PROHIBITED"})
         return AttributeResult(is_pass, reason)
 
 
 class Classification(Facet):
-    def __init__(self, value=None, system=None, uri=None, minOccurs=None, maxOccurs="unbounded", instructions=None):
-        self.parameters = ["value", "system", "@uri", "@minOccurs", "@maxOccurs", "@instructions"]
+    def __init__(self, value=None, system=None, uri=None, cardinality: Cardinality = "required", instructions=None):
+        self.parameters = ["value", "system", "@uri", "@cardinality", "@instructions"]
         self.applicability_templates = [
             "Data having a {system} reference of {value}",
             "Data classified using {system}",
             "Data classified as {value}",
-            "Classified data",
         ]
         self.requirement_templates = [
             "Shall have a {system} reference of {value}",
             "Shall be classified using {system}",
             "Shall be classified as {value}",
-            "Shall be classified",
         ]
         self.prohibited_templates = [
             "Shall not have a {system} reference of {value}",
             "Shall not be classified using {system}",
             "Shall not be classified as {value}",
-            "Shall not be classified",
         ]
 
-        super().__init__(value, system, uri, minOccurs, maxOccurs, instructions)
+        super().__init__(value, system, uri, cardinality, instructions)
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: Union[ifcopenshell.entity_instance, None]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
         return ifc_file.by_type("IfcObjectDefinition")
 
-    def __call__(self, inst, logger=None):
-        if self.minOccurs == 0 and self.maxOccurs != 0:
-            return ClassificationResult(True)
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> ClassificationResult:
+        if self.cardinality == "optional":
+            return ClassificationResult(True)  # Is this really the correct behaviour?
 
         leaf_references = ifcopenshell.util.classification.get_references(inst)
 
         references = leaf_references.copy()
         for leaf_reference in leaf_references:
             references.update(ifcopenshell.util.classification.get_inherited_references(leaf_reference))
 
@@ -377,58 +393,57 @@
 
         if is_pass and self.value:
             values = [getattr(r, "Identification", getattr(r, "ItemReference", None)) for r in references]
             is_pass = any([self.value == v for v in values])
             if not is_pass:
                 reason = {"type": "VALUE", "actual": values}
 
-        if is_pass and self.system:
+        if is_pass:
             systems = [ifcopenshell.util.classification.get_classification(r).Name for r in references]
             is_pass = any([self.system == s for s in systems])
             if not is_pass:
                 reason = {"type": "SYSTEM", "actual": systems}
 
-        if self.maxOccurs == 0:
+        if self.cardinality == "prohibited":
             return ClassificationResult(not is_pass, {"type": "PROHIBITED"})
         return ClassificationResult(is_pass, reason)
 
 
 class PartOf(Facet):
     def __init__(
         self,
         name="IFCWALL",
         predefinedType=None,
         relation=None,
-        minOccurs=None,
-        maxOccurs="unbounded",
+        cardinality: Cardinality = "required",
         instructions=None,
     ):
-        self.parameters = ["name", "predefinedType", "@relation", "@minOccurs", "@maxOccurs", "@instructions"]
+        self.parameters = ["name", "predefinedType", "@relation", "@cardinality", "@instructions"]
         self.applicability_templates = [
             "An element with an {relation} relationship with an {name}",
             "An element with an {relation} relationship",
         ]
         self.requirement_templates = [
             "An element must have an {relation} relationship with an {name}",
             "An element must have an {relation} relationship",
         ]
         self.prohibited_templates = [
             "An element must not have an {relation} relationship with an {name}",
             "An element must not have an {relation} relationship",
         ]
-        super().__init__(name, predefinedType, relation, minOccurs, maxOccurs, instructions)
+        super().__init__(name, predefinedType, relation, cardinality, instructions)
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: Union[ifcopenshell.entity_instance, None]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
         return list(ifc_file)  # Lazy
 
-    def asdict(self, clause_type):
+    def asdict(self, clause_type: str) -> dict[str, Any]:
         results = super().asdict(clause_type)
         entity = {}
         if "name" in results:
             entity["name"] = results["name"]
             del results["name"]
         if "predefinedType" in results:
             entity["predefinedType"] = results["predefinedType"]
@@ -439,18 +454,15 @@
 
     def parse(self, xml):
         if "entity" in xml:
             super().parse(xml["entity"])
             del xml["entity"]
         return super().parse(xml)
 
-    def __call__(self, inst, logger=None):
-        if self.minOccurs == 0 and self.maxOccurs != 0:
-            return PartOfResult(True)
-
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> PartOfResult:
         reason = None
         if not self.relation:
             is_pass = False
             ancestors = []
             parent = self.get_parent(inst)
             while parent:
                 ancestors.append(parent.is_a())
@@ -532,46 +544,37 @@
                                 is_pass = True
                         else:
                             is_pass = True
                         break
                     nest = self.get_nested_whole(nest)
                 if not is_pass:
                     reason = {"type": "ENTITY", "actual": ancestors}
-        elif self.relation == "IFCRELVOIDSELEMENT":
-            building_element = self.get_voided_element(inst)
+        elif self.relation == "IFCRELVOIDSELEMENT IFCRELFILLSELEMENT":
+            if inst.is_a("IfcOpeningElement"):
+                building_element = self.get_voided_element(inst)
+            else:
+                building_element = None
+                opening = self.get_filled_opening(inst)
+                if opening:
+                    building_element = self.get_voided_element(opening)
             is_pass = building_element is not None
             if not is_pass:
                 reason = {"type": "NOVALUE"}
             if is_pass and self.name:
                 is_pass = False
                 if building_element.is_a().upper() == self.name:
                     if self.predefinedType:
                         if ifcopenshell.util.element.get_predefined_type(building_element) == self.predefinedType:
                             is_pass = True
                     else:
                         is_pass = True
                 if not is_pass:
                     reason = {"type": "ENTITY", "actual": building_element}
-        elif self.relation == "IFCRELFILLSELEMENT":
-            opening = self.filled_opening(inst)
-            is_pass = opening is not None
-            if not is_pass:
-                reason = {"type": "NOVALUE"}
-            if is_pass and self.name:
-                is_pass = False
-                if opening.is_a().upper() == self.name:
-                    if self.predefinedType:
-                        if ifcopenshell.util.element.get_predefined_type(opening) == self.predefinedType:
-                            is_pass = True
-                    else:
-                        is_pass = True
-                if not is_pass:
-                    reason = {"type": "ENTITY", "actual": opening}
 
-        if self.maxOccurs == 0:
+        if self.cardinality == "prohibited":
             return PartOfResult(not is_pass, {"type": "PROHIBITED"})
         return PartOfResult(is_pass, reason)
 
     def get_nested_whole(self, element):
         for rel in getattr(element, "Nests", []) or []:
             return rel.RelatingObject
 
@@ -601,61 +604,59 @@
         return parent
 
 
 class Property(Facet):
     def __init__(
         self,
         propertySet="Property_Set",
-        name="PropertyName",
+        baseName="PropertyName",
         value=None,
-        datatype=None,
+        dataType=None,
         uri=None,
-        minOccurs=None,
-        maxOccurs="unbounded",
+        cardinality: Cardinality = "required",
         instructions=None,
     ):
         self.parameters = [
             "propertySet",
-            "name",
+            "baseName",
             "value",
-            "@datatype",
+            "@dataType",
             "@uri",
-            "@minOccurs",
-            "@maxOccurs",
+            "@cardinality",
             "@instructions",
         ]
         self.applicability_templates = [
-            "Elements with {name} data of {value} in the dataset {propertySet}",
-            "Elements with {name} data in the dataset {propertySet}",
+            "Elements with {baseName} data of {value} in the dataset {propertySet}",
+            "Elements with {baseName} data in the dataset {propertySet}",
         ]
         self.requirement_templates = [
-            "{name} data shall be {value} and in the dataset {propertySet}",
-            "{name} data shall be provided in the dataset {propertySet}",
+            "{baseName} data shall be {value} and in the dataset {propertySet}",
+            "{baseName} data shall be provided in the dataset {propertySet}",
         ]
         self.prohibited_templates = [
-            "{name} data shall not be {value} and in the dataset {propertySet}",
-            "{name} data shall not be provided in the dataset {propertySet}",
+            "{baseName} data shall not be {value} and in the dataset {propertySet}",
+            "{baseName} data shall not be provided in the dataset {propertySet}",
         ]
-        super().__init__(propertySet, name, value, datatype, uri, minOccurs, maxOccurs, instructions)
+        super().__init__(propertySet, baseName, value, dataType, uri, cardinality, instructions)
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: Union[ifcopenshell.entity_instance, None]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
         if ifc_file.schema == "IFC2X3":
             return ifc_file.by_type("IfcObjectDefinition")
         return (
             ifc_file.by_type("IfcObjectDefinition")
             + ifc_file.by_type("IfcMaterialDefinition")
             + ifc_file.by_type("IfcProfileDef")
         )
 
-    def __call__(self, inst, logger=None):
-        if self.minOccurs == 0 and self.maxOccurs != 0:
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> PropertyResult:
+        if self.cardinality == "optional":
             return PropertyResult(True)
 
         if isinstance(self.propertySet, str):
             pset = get_pset(inst, self.propertySet)
             psets = {self.propertySet: pset} if pset else {}
         else:
             all_psets = get_psets(inst)
@@ -667,26 +668,26 @@
         if not is_pass:
             reason = {"type": "NOPSET"}
 
         if is_pass:
             props = {}
             for pset_name, pset_props in psets.items():
                 props[pset_name] = {}
-                if isinstance(self.name, str):
-                    prop = pset_props.get(self.name)
+                if isinstance(self.baseName, str):
+                    prop = pset_props.get(self.baseName)
                     if prop == "UNKNOWN" and [
                         p
                         for p in self.get_properties(inst.wrapped_data.file.by_id(pset_props["id"]))
-                        if p.Name == self.name
+                        if p.Name == self.baseName
                     ][0].NominalValue.is_a("IfcLogical"):
                         pass
                     elif prop is not None and prop != "":
-                        props[pset_name][self.name] = prop
+                        props[pset_name][self.baseName] = prop
                 else:
-                    props[pset_name] = {k: v for k, v in pset_props.items() if k == self.name}
+                    props[pset_name] = {k: v for k, v in pset_props.items() if k == self.baseName}
 
                 if not bool(props[pset_name]):
                     is_pass = False
                     reason = {"type": "NOVALUE"}
                     break
 
                 pset_entity = inst.wrapped_data.file.by_id(pset_props["id"])
@@ -697,17 +698,17 @@
                         continue
                     if not isinstance(prop_entity, ifcopenshell.entity_instance):
                         # Predefined properties are special :(
                         pass
                     elif prop_entity.is_a("IfcPropertySingleValue"):
                         data_type = prop_entity.NominalValue.is_a()
 
-                        if data_type.lower() != self.datatype.lower():
+                        if self.dataType and data_type.lower() != self.dataType.lower():
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
 
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit and getattr(unit, "Name", None):
                             # TODO support unnamed derived units
                             props[pset_name][prop_entity.Name] = ifcopenshell.util.unit.convert(
                                 prop_entity.NominalValue.wrappedValue,
@@ -716,17 +717,17 @@
                                 None,
                                 ifcopenshell.util.unit.si_type_names[unit.UnitType],
                             )
                     elif prop_entity.is_a("IfcPhysicalSimpleQuantity"):
                         prop_schema = prop_entity.wrapped_data.declaration().as_entity()
                         data_type = prop_schema.attribute_by_index(3).type_of_attribute().declared_type().name()
 
-                        if data_type.lower() != self.datatype.lower():
+                        if self.dataType and data_type.lower() != self.dataType.lower():
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
 
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             props[pset_name][prop_entity.Name] = ifcopenshell.util.unit.convert(
                                 prop_entity[3],
                                 getattr(unit, "Prefix", None),
@@ -736,27 +737,27 @@
                             )
                     elif prop_entity.is_a("IfcPropertyEnumeratedValue"):
                         if not prop_entity.EnumerationValues:
                             is_pass = False
                             reason = {"type": "NOVALUE"}
                             break
                         data_type = prop_entity.EnumerationValues[0].is_a()
-                        if data_type.lower() != self.datatype.lower():
+                        if self.dataType and data_type.lower() != self.dataType.lower():
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
                     elif prop_entity.is_a("IfcPropertyListValue"):
                         if not prop_entity.ListValues:
                             is_pass = False
                             reason = {"type": "NOVALUE"}
                             break
                         data_type = prop_entity.ListValues[0].is_a()
-                        if data_type.lower() != self.datatype.lower():
+                        if self.dataType and data_type.lower() != self.dataType.lower():
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             props[pset_name][prop_entity.Name] = [
                                 ifcopenshell.util.unit.convert(
                                     v,
                                     getattr(unit, "Prefix", None),
@@ -769,17 +770,17 @@
                     elif prop_entity.is_a("IfcPropertyBoundedValue"):
                         values = []
                         for attribute in ["UpperBoundValue", "LowerBoundValue", "SetPointValue"]:
                             value = getattr(prop_entity, attribute)
                             if value is not None:
                                 data_type = value.is_a()
                                 values.append(value.wrappedValue)
-                        if data_type.lower() != self.datatype.lower():
+                        if self.dataType and data_type.lower() != self.dataType.lower():
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
                         unit = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         if unit:
                             values = [
                                 ifcopenshell.util.unit.convert(
                                     v,
                                     getattr(unit, "Prefix", None),
@@ -794,15 +795,15 @@
                         values = []
                         units = ifcopenshell.util.unit.get_property_unit(prop_entity, inst.wrapped_data.file)
                         for attribute in ["Defining", "Defined"]:
                             column_values = props[pset_name][prop_entity.Name][f"{attribute}Values"]
                             if not column_values:
                                 continue
                             data_type = column_values[0].is_a()
-                            if data_type.lower() == self.datatype.lower():
+                            if self.dataType and data_type.lower() == self.dataType.lower():
                                 column_values = [v.wrappedValue for v in column_values]
                                 unit = units[f"{attribute}Unit"]
                                 if unit:
                                     column_values = [
                                         ifcopenshell.util.unit.convert(
                                             v,
                                             getattr(unit, "Prefix", None),
@@ -811,15 +812,15 @@
                                             ifcopenshell.util.unit.si_type_names[unit.UnitType],
                                         )
                                         for v in column_values
                                     ]
                                 values.extend(column_values)
                         if not values:
                             is_pass = False
-                            reason = {"type": "DATATYPE", "actual": data_type, "datatype": self.datatype}
+                            reason = {"type": "DATATYPE", "actual": data_type, "dataType": self.dataType}
                             break
                         props[pset_name][prop_entity.Name] = values
                     else:
                         is_property_supported_class = False
 
                 if not is_property_supported_class:
                     is_pass = False
@@ -864,15 +865,15 @@
                                 break
                         elif value != self.value:
                             # XSD restriction = whatever
                             is_pass = False
                             reason = {"type": "VALUE", "actual": value}
                             break
 
-        if self.maxOccurs == 0:
+        if self.cardinality == "prohibited":
             return PropertyResult(not is_pass, {"type": "PROHIBITED"})
         return PropertyResult(is_pass, reason)
 
     def get_properties(self, pset):
         if pset.is_a("IfcPropertySet"):
             return pset.HasProperties
         elif pset.is_a("IfcElementQuantity"):
@@ -884,39 +885,39 @@
                 type("", (object,), {"Name": k, "Value": v})()
                 for k, v in pset.get_info().items()
                 if not isinstance(v, ifcopenshell.entity_instance)
             ]
 
 
 class Material(Facet):
-    def __init__(self, value=None, uri=None, minOccurs=None, maxOccurs="unbounded", instructions=None):
-        self.parameters = ["value", "@uri", "@minOccurs", "@maxOccurs", "@instructions"]
+    def __init__(self, value=None, uri=None, cardinality: Cardinality = "required", instructions=None):
+        self.parameters = ["value", "@uri", "@cardinality", "@instructions"]
         self.applicability_templates = [
             "All data with a {value} material",
             "All data with a material",
         ]
         self.requirement_templates = [
             "Shall have a material of {value}",
             "Shall have a material",
         ]
         self.prohibited_templates = [
             "Shall not have a material of {value}",
             "Shall not have a material",
         ]
-        super().__init__(value, uri, minOccurs, maxOccurs, instructions)
+        super().__init__(value, uri, cardinality, instructions)
 
     def filter(
-        self, ifc_file: ifcopenshell.file, elements: Union[ifcopenshell.entity_instance, None]
-    ) -> List[ifcopenshell.entity_instance]:
+        self, ifc_file: ifcopenshell.file, elements: Optional[list[ifcopenshell.entity_instance]]
+    ) -> list[ifcopenshell.entity_instance]:
         if isinstance(elements, list):
             return super().filter(ifc_file, elements)
         return ifc_file.by_type("IfcObjectDefinition")
 
-    def __call__(self, inst, logger=None):
-        if self.minOccurs == 0 and self.maxOccurs != 0:
+    def __call__(self, inst: ifcopenshell.entity_instance, logger: Optional[Logger] = None) -> MaterialResult:
+        if self.cardinality == "optional":
             return MaterialResult(True)
 
         material = ifcopenshell.util.element.get_material(inst, should_skip_usage=True)
 
         is_pass = material is not None
         reason = None
 
@@ -959,15 +960,15 @@
                 if value == self.value:
                     is_pass = True
                     break
 
             if not is_pass:
                 reason = {"type": "VALUE", "actual": values}
 
-        if self.maxOccurs == 0:
+        if self.cardinality == "prohibited":
             return MaterialResult(not is_pass, {"type": "PROHIBITED"})
         return MaterialResult(is_pass, reason)
 
 
 class Restriction:
     def __init__(self, options=None, base="string"):
         self.base = base
@@ -985,15 +986,15 @@
                 self.options[key] = [value["@value"]]  # A single enumeration value which is pretty meaningless
             elif isinstance(value, dict):
                 self.options[key] = value["@value"]
             else:
                 self.options[key] = [v["@value"] for v in value]
         return self
 
-    def asdict(self):
+    def asdict(self) -> dict[str, Any]:
         result = {"@base": "xs:" + self.base}
         for constraint, value in self.options.items():
             value = [value] if not isinstance(value, list) else value
             for v in value:
                 if constraint in ["length", "minLength", "maxLength"]:
                     value_dict = {"@value": v}
                 else:
@@ -1104,15 +1105,15 @@
 class PropertyResult(Result):
     def to_string(self):
         if self.reason["type"] == "NOPSET":
             return "The required property set does not exist"
         elif self.reason["type"] == "NOVALUE":
             return "The property set does not contain the required property"
         elif self.reason["type"] == "DATATYPE":
-            return f"The property's data type \"{str(self.reason['actual'])}\" does not match the required data type of \"{str(self.reason['datatype'])}\""
+            return f"The property's data type \"{str(self.reason['actual'])}\" does not match the required data type of \"{str(self.reason['dataType'])}\""
         elif self.reason["type"] == "VALUE":
             if isinstance(self.reason["actual"], list):
                 if len(self.reason["actual"]) == 1:
                     return f"The property value \"{str(self.reason['actual'][0])}\" does not match the requirements"
                 else:
                     return f"The property values \"{str(self.reason['actual'])}\" do not match the requirements"
             else:
```

### Comparing `ifctester-0.0.240318/ifctester/ids.py` & `ifctester-0.0.240418/ifctester/ids.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,27 +12,46 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcTester.  If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 import os
 import datetime
+import ifcopenshell
 from xmlschema import XMLSchema
 from xmlschema import etree_tostring
 from xml.etree import ElementTree as ET
-from .facet import Facet, Entity, Attribute, Classification, Property, PartOf, Material, Restriction, get_pset, get_psets
-from typing import List, Set
+from .facet import (
+    Facet,
+    Entity,
+    Attribute,
+    Classification,
+    Property,
+    PartOf,
+    Material,
+    Restriction,
+    get_pset,
+    get_psets,
+    Cardinality,
+    FacetFailure,
+)
+from typing import List, Optional, Union, overload, Literal
 
 cwd = os.path.dirname(os.path.realpath(__file__))
 schema = None
 
 
-def open(filepath, validate=False):
+@overload
+def open(filepath: str, validate: Literal[False] = False) -> Ids: ...
+@overload
+def open(filepath: str, validate: Literal[True]) -> None: ...
+def open(filepath: str, validate=False) -> Union[Ids, None]:
     if validate:
         get_schema().validate(filepath)
     return Ids().parse(
         get_schema().decode(filepath, strip_namespaces=True, namespaces={"": "http://standards.buildingsmart.org/IDS"})
     )
 
 
@@ -42,15 +61,15 @@
         schema = XMLSchema(os.path.join(cwd, "ids.xsd"))
     return schema
 
 
 class Ids:
     def __init__(
         self,
-        title="Untitled",
+        title: Optional[str] = "Untitled",
         copyright=None,
         version=None,
         description=None,
         author=None,
         date=None,
         purpose=None,
         milestone=None,
@@ -85,15 +104,15 @@
         for attr in ["title", "copyright", "version", "description", "author", "date", "purpose", "milestone"]:
             if attr in self.info:
                 info[attr] = self.info[attr]
         ids_dict = {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.6/ids.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.7/ids.xsd",
             "info": info,
             "specifications": {"specification": []},
         }
         for spec in self.specifications:
             ids_dict["specifications"]["specification"].append(spec.asdict())
         return ids_dict
 
@@ -116,15 +135,15 @@
         return etree_tostring(get_schema().encode(self.asdict()), namespaces=ns)
 
     def to_xml(self, filepath="output.xml"):
         ET.register_namespace("", "http://standards.buildingsmart.org/IDS")
         ET.ElementTree(get_schema().encode(self.asdict())).write(filepath, encoding="utf-8", xml_declaration=True)
         return get_schema().is_valid(filepath)
 
-    def validate(self, ifc_file, filter_version=False, filepath=None):
+    def validate(self, ifc_file: ifcopenshell.file, filter_version=False, filepath: Optional[str] = None) -> None:
         if filepath:
             self.filepath = filepath
             self.filename = os.path.basename(filepath)
         else:
             self.filepath = self.filename = None
         get_pset.cache_clear()
         get_psets.cache_clear()
@@ -143,32 +162,32 @@
         identifier=None,
         description=None,
         instructions=None,
     ):
         self.name = name or "Unnamed"
         self.applicability: List[Facet] = []
         self.requirements: List[Facet] = []
-        self.minOccurs = minOccurs
-        self.maxOccurs = maxOccurs
+        self.minOccurs: Union[int, str] = minOccurs
+        self.maxOccurs: Union[int, str] = maxOccurs
         self.ifcVersion = ifcVersion
         self.identifier = identifier
         self.description = description
         self.instructions = instructions
 
-        self.applicable_entities: List[Entity] = []
+        self.applicable_entities: list[ifcopenshell.entity_instance] = []
         self.status = None
 
     def asdict(self):
         results = {
             "@name": self.name,
             "@ifcVersion": self.ifcVersion,
             "applicability": {},
             "requirements": {},
         }
-        for attribute in ["identifier", "description", "instructions", "minOccurs", "maxOccurs"]:
+        for attribute in ["identifier", "description", "instructions"]:
             value = getattr(self, attribute)
             if value is not None:
                 results[f"@{attribute}"] = value
         for clause_type in ["applicability", "requirements"]:
             clause = getattr(self, clause_type)
             if not clause:
                 continue
@@ -177,28 +196,33 @@
                 facet_type = type(facet).__name__
                 facet_type = facet_type[0].lower() + facet_type[1:]
                 facets.setdefault(facet_type, []).append(facet.asdict(clause_type))
             # Canonicalise ordering as per XSD requirements
             for facet_type in ("entity", "partOf", "classification", "attribute", "property", "material"):
                 if facet_type in facets:
                     results[clause_type][facet_type] = facets[facet_type]
+            if clause_type == "applicability":
+                for attribute in ["minOccurs", "maxOccurs"]:
+                    value = getattr(self, attribute)
+                    if value is not None:
+                        results[clause_type][f"@{attribute}"] = value
         return results
 
     def parse(self, ids_dict):
         self.name = ids_dict.get("@name", "")
         self.description = ids_dict.get("@description", "")
         self.instructions = ids_dict.get("@instructions", "")
-        self.minOccurs = ids_dict["@minOccurs"]
-        self.maxOccurs = ids_dict["@maxOccurs"]
+        self.minOccurs = ids_dict.get("applicability", {}).get("@minOccurs", 0)
+        self.maxOccurs = ids_dict.get("applicability", {}).get("@maxOccurs", "unbounded")
         self.ifcVersion = ids_dict["@ifcVersion"]
         self.applicability = (
-            self.parse_clause(ids_dict["applicability"]) if ids_dict.get("applicability") is not None else []
+            self.parse_clause(ids_dict["applicability"]) if ids_dict.get("applicability", None) is not None else []
         )
         self.requirements = (
-            self.parse_clause(ids_dict["requirements"]) if ids_dict.get("requirements") is not None else []
+            self.parse_clause(ids_dict["requirements"]) if ids_dict.get("requirements", None) is not None else []
         )
         return self
 
     def parse_clause(self, clause):
         results = []
         for name, facets in clause.items():
             if name not in ["entity", "attribute", "classification", "partOf", "property", "material"]:
@@ -209,21 +233,21 @@
                 name_capitalised = name[0].upper() + name[1:]
                 facet = globals()[name_capitalised]().parse(facet_xml)
                 results.append(facet)
         return results
 
     def reset_status(self):
         self.applicable_entities.clear()
-        self.failed_entities: Set[Entity] = set()
+        self.failed_entities: set[ifcopenshell.entity_instance] = set()
         for facet in self.requirements:
             facet.status = None
-            facet.failed_entities.clear()
+            facet.failures.clear()
         self.status = None
 
-    def validate(self, ifc_file, filter_version=False):
+    def validate(self, ifc_file: ifcopenshell.file, filter_version=False) -> None:
         if filter_version and ifc_file.schema not in self.ifcVersion:
             return
 
         elements = None
 
         # This is a broadphase filter of applicability. We almost never want to
         # test every single class in an IFC model.
@@ -239,46 +263,50 @@
                     is_applicable = False
                     break
             if not is_applicable:
                 continue
             self.applicable_entities.append(element)
             for facet in self.requirements:
                 result = facet(element)
-                if self.maxOccurs == 0:
-                    prohibited = bool(result)
-                else:
-                    prohibited = not bool(result)
-                if prohibited:
-                    self.failed_entities.add(element)
-                    facet.failed_entities.append(element)
-                    facet.failed_reasons.append(str(result))
+                is_pass = bool(result)
+                if self.maxOccurs != 0:  # This is a required or optional specification
+                    if not is_pass:
+                        self.failed_entities.add(element)
+                        facet.failures.append(FacetFailure(element=element, reason=str(result)))
+                else:  # This is a prohibited specification
+                    if is_pass:
+                        self.failed_entities.add(element)
+                        facet.failures.append(FacetFailure(element=element, reason=str(result)))
 
+        self.status = True
         for facet in self.requirements:
-            if facet.minOccurs != 0:
-                facet.status = not bool(facet.failed_entities)
-            elif facet.minOccurs == 0 and facet.maxOccurs != 0:
-                facet.status = True
-            elif facet.maxOccurs == 0:
-                facet.status = bool(facet.failed_entities)
+            facet.status = not bool(facet.failures)
+            if not facet.status:
+                self.status = False
 
-        self.status = True
-        if self.minOccurs != 0:
+        if self.minOccurs != 0:  # Required specification
             if not self.applicable_entities:
                 self.status = False
                 for facet in self.requirements:
                     facet.status = False
-            elif self.failed_entities:
-                self.status = False
-        elif self.minOccurs == 0 and self.maxOccurs != 0:
-            if self.failed_entities:
-                self.status = False
-        elif self.maxOccurs == 0:
-            if (len(self.applicable_entities)) > 0:
+        elif self.maxOccurs == 0:  # Prohibited specification
+            if self.applicable_entities and not self.requirements:
                 self.status = False
 
-    def get_usage(self):
+    def get_usage(self) -> Cardinality:
         if self.minOccurs != 0:
             return "required"
         elif self.minOccurs == 0 and self.maxOccurs != 0:
             return "optional"
         elif self.maxOccurs == 0:
             return "prohibited"
+
+    def set_usage(self, usage: Cardinality) -> None:
+        if usage == "optional":
+            self.minOccurs = 0
+            self.maxOccurs = "unbounded"
+        elif usage == "prohibited":
+            self.minOccurs = 0
+            self.maxOccurs = 0
+        else:  # required
+            self.minOccurs = 1
+            self.maxOccurs = "unbounded"
```

### Comparing `ifctester-0.0.240318/ifctester/ids.xsd` & `ifctester-0.0.240418/ifctester/ids.xsd`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!-- June 20, 2023 - DRAFT  -->
-<xs:schema xmlns:ids="http://standards.buildingsmart.org/IDS" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:altova="http://www.altova.com/xml-schema-extensions" targetNamespace="http://standards.buildingsmart.org/IDS" elementFormDefault="qualified" attributeFormDefault="unqualified" version="0.9.6">
+<!-- Draft - Do not use in production -->
+<xs:schema xmlns:ids="http://standards.buildingsmart.org/IDS" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:altova="http://www.altova.com/xml-schema-extensions" targetNamespace="http://standards.buildingsmart.org/IDS" elementFormDefault="qualified" attributeFormDefault="unqualified" version="0.9.7">
 	<xs:import namespace="http://www.w3.org/XML/1998/namespace" schemaLocation="http://www.w3.org/2001/xml.xsd"/>
 	<xs:import namespace="http://www.w3.org/2001/XMLSchema" schemaLocation="http://www.w3.org/2001/XMLSchema.xsd"/>
 	<xs:import namespace="http://www.w3.org/2001/XMLSchema-instance" schemaLocation="http://www.w3.org/2001/XMLSchema-instance"/>
 	<xs:element name="ids">
 		<xs:complexType>
 			<xs:sequence>
 				<xs:element name="info">
@@ -36,56 +36,83 @@
 			<xs:element name="predefinedType" type="ids:idsValue" minOccurs="0"/>
 		</xs:sequence>
 	</xs:complexType>
 	<xs:complexType name="idsValue">
 		<xs:choice minOccurs="1">
 			<!-- place for potential additional rules for idsValue -->
 			<xs:element name="simpleValue" type="xs:string" minOccurs="1" maxOccurs="1"/>
-			<xs:element ref="xs:restriction" minOccurs="1" maxOccurs="unbounded"/>
+			<xs:element ref="xs:restriction" minOccurs="1" maxOccurs="1"/>
 		</xs:choice>
 	</xs:complexType>
 	<xs:complexType name="classificationType">
 		<xs:sequence>
 			<xs:element name="value" type="ids:idsValue" minOccurs="0"/>
-			<xs:element name="system" type="ids:idsValue" minOccurs="0"/>
+			<xs:element name="system" type="ids:idsValue" minOccurs="1"/>
 		</xs:sequence>
 	</xs:complexType>
 	<xs:complexType name="partOfType">
 		<xs:sequence>
 			<xs:element name="entity" type="ids:entityType" minOccurs="1"/>
 		</xs:sequence>
-		<xs:attribute name="relation" type="ids:relations"/>
+		<xs:attribute name="relation" type="ids:relations" use="optional" />
 	</xs:complexType>
 	<xs:complexType name="applicabilityType">
 		<xs:sequence>
 			<xs:element name="entity" type="ids:entityType" minOccurs="0"/>
 			<xs:element name="partOf" type="ids:partOfType" minOccurs="0" maxOccurs="unbounded"/>
 			<xs:element name="classification" type="ids:classificationType" minOccurs="0" maxOccurs="unbounded"/>
 			<xs:element name="attribute" type="ids:attributeType" minOccurs="0" maxOccurs="unbounded"/>
 			<xs:element name="property" type="ids:propertyType" minOccurs="0" maxOccurs="unbounded"/>
-			<xs:element name="material" type="ids:materialType" minOccurs="0"/>
+			<xs:element name="material" type="ids:materialType" minOccurs="0" maxOccurs="unbounded"/>
 		</xs:sequence>
+		<!-- Please note there is an implementation agreement on the use of minOccurs and maxOccurs.
+			Valid values are: 
+			a. 0 to unbounded, meaning Optional
+			b. 1 to unbounded, meaning Required
+			c. 0 to 0, meaning Prohibited
+		 -->
+		<xs:attributeGroup ref="xs:occurs"/>
 	</xs:complexType>
 	<xs:complexType name="propertyType">
 		<xs:sequence>
 			<xs:element name="propertySet" type="ids:idsValue"/>
-			<xs:element name="name" type="ids:idsValue"/>
-			<xs:element name="value" type="ids:idsValue" minOccurs="0"/>
+			<xs:element name="baseName" type="ids:idsValue">
+				<xs:annotation>
+					<xs:documentation>
+						the moniker 'baseName' is chosen to clarify that the data needs to reference the property name as stored in the IFC file, 
+						which might differ from the multiple language-dependent presentations (e.g. 'FireRating' vs. 'Fire rating').
+					</xs:documentation>
+				</xs:annotation>
+			</xs:element>
+			<xs:element name="value" type="ids:idsValue" minOccurs="0">
+				<xs:annotation>
+					<xs:documentation>
+						Depending on the dataType attribute, values are expressed in the default unit documented at 
+						https://github.com/buildingSMART/IDS/blob/master/Documentation/units.md, and unit conversion might be required.
+					</xs:documentation>
+				</xs:annotation>
+			</xs:element>
 		</xs:sequence>
-		<xs:attribute name="datatype" use="required">
+		<xs:attribute name="dataType" type="ids:upperCaseName" use="optional">
 			<xs:annotation>
-				<xs:documentation>This is the name of an IFC Defined Type. See the full list for IFC 4 on https://standards.buildingsmart.org/IFC/RELEASE/IFC4/ADD2_TC1/HTML/link/alphabeticalorder-defined-types.htm  Documentation and default units on https://github.com/buildingSMART/IDS/blob/master/Documentation/units.md</xs:documentation>
+				<xs:documentation>This is the name of an IFC Defined Type, all uppercase.</xs:documentation>
 			</xs:annotation>
-			<!-- renamed 'measure' to data type to better represent reality -->
 		</xs:attribute>
 	</xs:complexType>
 	<xs:complexType name="attributeType">
 		<xs:sequence>
 			<xs:element name="name" type="ids:idsValue"/>
-			<xs:element name="value" type="ids:idsValue" minOccurs="0"/>
+			<xs:element name="value" type="ids:idsValue" minOccurs="0">
+				<xs:annotation>
+					<xs:documentation>
+						Depending on the IFC type of the attribute, values are expressed in the default unit documented at 
+						https://github.com/buildingSMART/IDS/blob/master/Documentation/units.md, and unit conversion might be required.
+					</xs:documentation>
+				</xs:annotation>
+			</xs:element>
 		</xs:sequence>
 	</xs:complexType>
 	<xs:complexType name="materialType">
 		<xs:sequence>
 			<xs:element name="value" type="ids:idsValue" minOccurs="0"/>
 		</xs:sequence>
 	</xs:complexType>
@@ -94,86 +121,94 @@
 			<xs:element name="entity" minOccurs="0">
 				<xs:annotation>
 					<xs:documentation>Make sure 'Name' value of requirements entity is the same as the 'applicability' node, or a wildcard (inclusive pattern).</xs:documentation>
 				</xs:annotation>
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:entityType">
+							<!-- 
+								Contrary to other requirements facet extensions, cardinality is not available in the entityType facet when used for requirements.
+								Its cardinality state is always considered to be "required".
+								Constraining the acceptable values is achieved by specifying criteria via with xs:Enumeration and xs:Pattern, rather than the negative form.
+								This is possible because the list of options is finite and mandated by the IFC schema, so prohibited constraints are superfluous.
+								This choice allows for improved user experience in the editors.
+							-->
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
 			<xs:element name="partOf" minOccurs="0" maxOccurs="unbounded">
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:partOfType">
-							<xs:attributeGroup ref="xs:occurs"/>
+							<xs:attribute name="cardinality" type="ids:simpleCardinality" use="optional" default="required"/>
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
 			<xs:element name="classification" minOccurs="0" maxOccurs="unbounded">
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:classificationType">
 							<xs:attribute name="uri" type="xs:anyURI" use="optional"/>
-							<xs:attributeGroup ref="xs:occurs"/>
+							<xs:attribute name="cardinality" type="ids:conditionalCardinality" use="optional" default="required"/>
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
 			<xs:element name="attribute" minOccurs="0" maxOccurs="unbounded">
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:attributeType">
+							<xs:attribute name="cardinality" type="ids:conditionalCardinality" use="optional" default="required"/>
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
 			<xs:element name="property" minOccurs="0" maxOccurs="unbounded">
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:propertyType">
 							<xs:attribute name="uri" type="xs:anyURI" use="optional"/>
-							<xs:attributeGroup ref="xs:occurs"/>
+							<xs:attribute name="cardinality" type="ids:conditionalCardinality" use="optional" default="required"/>
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
-			<xs:element name="material" minOccurs="0">
+			<xs:element name="material" minOccurs="0" maxOccurs="unbounded">
 				<xs:complexType>
 					<xs:complexContent>
 						<xs:extension base="ids:materialType">
 							<xs:attribute name="uri" type="xs:anyURI" use="optional"/>
-							<xs:attributeGroup ref="xs:occurs"/>
+							<xs:attribute name="cardinality" type="ids:conditionalCardinality" use="optional" default="required"/>
 							<xs:attribute name="instructions" type="xs:string" use="optional">
 								<xs:annotation>
 									<xs:documentation>Author of the IDS can leave instructions for the authors of the IFC. This text could/should be displayed in the BIM/IFC authoring tool.</xs:documentation>
 								</xs:annotation>
 							</xs:attribute>
 						</xs:extension>
 					</xs:complexContent>
@@ -191,30 +226,29 @@
 							<xs:attribute name="description" type="xs:string" use="optional"/>
 						</xs:extension>
 					</xs:complexContent>
 				</xs:complexType>
 			</xs:element>
 		</xs:sequence>
 		<xs:attribute name="name" type="xs:string" use="required"/>
-		<xs:attributeGroup ref="xs:occurs"/>
 		<xs:attribute name="ifcVersion" use="required">
 			<xs:simpleType>
 				<xs:list>
 					<xs:simpleType>
 						<xs:restriction base="xs:string">
 							<xs:minLength value="1"/>
 							<xs:enumeration value="IFC2X3"/>
 							<xs:enumeration value="IFC4"/>
 							<xs:enumeration value="IFC4X3"/>
 						</xs:restriction>
 					</xs:simpleType>
 				</xs:list>
 			</xs:simpleType>
 		</xs:attribute>
-		<xs:attribute name="identifier" type="xs:string">
+		<xs:attribute name="identifier" type="xs:string" use="optional">
 			<xs:annotation>
 				<xs:documentation>Author of the IDS can provide an identifier to the specification. This is intended to be a machine readable identifier. Beware: because of the possibility to combine different 'specification' elements from several ids files this cannot be enforced/assumed as (global) unique.</xs:documentation>
 			</xs:annotation>
 		</xs:attribute>
 		<xs:attribute name="description" type="xs:string" use="optional"/>
 		<xs:attribute name="instructions" type="xs:string" use="optional">
 			<xs:annotation>
@@ -225,16 +259,34 @@
 	<xs:complexType name="specificationsType">
 		<xs:sequence>
 			<xs:element name="specification" type="ids:specificationType" minOccurs="1" maxOccurs="unbounded"/>
 		</xs:sequence>
 	</xs:complexType>
 	<xs:simpleType name="relations">
 		<xs:restriction base="xs:string">
-			<xs:enumeration value="IFCRELAGGREGATES"/>
-			<xs:enumeration value="IFCRELASSIGNSTOGROUP"/>
-			<xs:enumeration value="IFCRELCONTAINEDINSPATIALSTRUCTURE"/>
-			<xs:enumeration value="IFCRELNESTS"/>
-			<xs:enumeration value="IFCRELVOIDSELEMENT"/>
-			<xs:enumeration value="IFCRELFILLSELEMENT"/>
+			<xs:enumeration value="IFCRELAGGREGATES"/>  
+			<xs:enumeration value="IFCRELASSIGNSTOGROUP"/> 
+			<xs:enumeration value="IFCRELCONTAINEDINSPATIALSTRUCTURE"/> 
+			<xs:enumeration value="IFCRELNESTS"/> 
+			<xs:enumeration value="IFCRELVOIDSELEMENT IFCRELFILLSELEMENT"/> 
+		</xs:restriction>
+	</xs:simpleType>
+	<xs:simpleType name="upperCaseName">
+		<xs:restriction base="xs:normalizedString">
+			<xs:pattern value="[A-Z]+"/>
+		</xs:restriction>
+	</xs:simpleType>
+	<xs:simpleType name="simpleCardinality">
+		<xs:restriction base="xs:string">
+			<xs:enumeration value="required"/>
+			<xs:enumeration value="prohibited"/>
+		</xs:restriction>
+	</xs:simpleType>
+	<xs:simpleType name="conditionalCardinality">
+		<xs:restriction base="xs:string">
+			<xs:enumeration value="required"/>
+			<xs:enumeration value="prohibited"/>
+			<xs:enumeration value="optional"/>
 		</xs:restriction>
 	</xs:simpleType>
-</xs:schema>
+	
+</xs:schema>
```

### Comparing `ifctester-0.0.240318/ifctester/reporter.py` & `ifctester-0.0.240418/ifctester/reporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,44 +12,118 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with IfcTester.  If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
 import os
+import re
 import sys
 import math
 import logging
 import datetime
-import numpy as np
 import ifcopenshell
 import ifcopenshell.util.unit
 import ifcopenshell.util.element
-import ifcopenshell.util.placement
+from .ids import Specification, Ids
+from .facet import Facet, FacetFailure
+from typing import TypedDict, Union, Literal, Optional
 
 cwd = os.path.dirname(os.path.realpath(__file__))
 
 
 class Reporter:
-    def __init__(self, ids):
+    def __init__(self, ids: Ids):
         self.ids = ids
 
     def report(self, ids):
         pass
 
     def to_string(self):
         return ""
 
     def write(self, filepath):
         pass
 
 
+ResultsPercent = Union[int, Literal["N/A"]]
+
+
+class Results(TypedDict):
+    title: str
+    date: str
+    filepath: str
+    filename: str
+    specifications: list[ResultsSpecification]
+    status: bool
+    total_specifications: int
+    total_specifications: int
+    total_specifications_pass: int
+    total_specifications_fail: int
+    percent_specifications_pass: ResultsPercent
+    total_requirements: int
+    total_requirements_pass: int
+    total_requirements_fail: int
+    percent_requirements_pass: ResultsPercent
+    total_checks: int
+    total_checks_pass: int
+    total_checks_fail: int
+    percent_checks_pass: ResultsPercent
+
+
+class ResultsSpecification(TypedDict):
+    name: str
+    description: str
+    instructions: str
+    status: bool
+    total_applicable: int
+    total_applicable_pass: int
+    total_applicable_fail: int
+    percent_applicable_pass: ResultsPercent
+    total_checks: int
+    total_checks_pass: int
+    total_checks_fail: int
+    percent_checks_pass: ResultsPercent
+    required: bool
+    applicability: list[str]
+    requirements: list[ResultsRequirement]
+
+
+class ResultsRequirement(TypedDict):
+    description: str
+    status: bool
+    failed_entities: list[ResultsFailedEntity]
+    total_applicable: int
+    total_pass: int
+    total_fail: int
+    percent_pass: ResultsPercent
+
+
+# use different syntax because of the "class" key
+ResultsFailedEntity = TypedDict(
+    "ResultsFailedEntity",
+    {
+        "reason": str,
+        "element": str,
+        "element_type": str,
+        "class": str,
+        "predefined_type": str,
+        "name": Union[str, None],
+        "description": Union[str, None],
+        "id": int,
+        "global_id": Union[str, None],
+        "tag": Union[str, None],
+    },
+)
+
+
 class Console(Reporter):
-    def __init__(self, ids, use_colour=True):
+    def __init__(self, ids: Ids, use_colour=True):
         super().__init__(ids)
         self.use_colour = use_colour
         self.colours = {
             "red": "\033[1;31m",
             "blue": "\033[1;34m",
             "cyan": "\033[1;36m",
             "green": "\033[0;32m",
@@ -57,22 +131,22 @@
             "purple": "\033[0;95m",
             "grey": "\033[0;90m",
             "reset": "\033[0;0m",
             "bold": "\033[;1m",
             "reverse": "\033[;7m",
         }
 
-    def report(self):
+    def report(self) -> None:
         self.set_style("bold", "blue")
         self.print(self.ids.info.get("title", "Untitled IDS"))
         for specification in self.ids.specifications:
             self.report_specification(specification)
         self.set_style("reset")
 
-    def report_specification(self, specification):
+    def report_specification(self, specification: Specification) -> None:
         if specification.status is True:
             self.set_style("bold", "green")
             self.print("[PASS] ", end="")
         elif specification.status is False:
             self.set_style("bold", "red")
             self.print("[FAIL] ", end="")
         elif specification.status is None:
@@ -101,70 +175,70 @@
 
         self.set_style("cyan")
         self.print(" " * 4 + "Requirements:")
         self.set_style("reset")
 
         for requirement in specification.requirements:
             self.set_style("reset")
-            self.set_style("red") if requirement.failed_entities else self.set_style("green")
+            self.set_style("red") if requirement.failures else self.set_style("green")
             self.print(" " * 8 + requirement.to_string("requirement", specification, requirement))
             self.set_style("reset")
-            for i, element in enumerate(requirement.failed_entities[0:10]):
+            for failure in requirement.failures[0:10]:
                 self.print(" " * 12, end="")
-                self.report_reason(requirement.failed_reasons[i], element)
-            if len(requirement.failed_entities) > 10:
-                self.print(" " * 12 + f"... {len(requirement.failed_entities)} in total ...")
+                self.report_reason(failure)
+            if len(requirement.failures) > 10:
+                self.print(" " * 12 + f"... {len(requirement.failures)} in total ...")
         self.set_style("reset")
 
-    def report_reason(self, reason, element):
+    def report_reason(self, failure: FacetFailure) -> None:
         is_bold = False
-        for substring in reason.split('"'):
+        for substring in failure["reason"].split('"'):
             if is_bold:
                 self.set_style("purple")
             else:
                 self.set_style("reset")
             self.print(substring, end="")
             is_bold = not is_bold
         self.set_style("grey")
-        self.print(" - " + str(element))
+        self.print(" - " + str(failure["element"]))
         self.set_style("reset")
 
-    def set_style(self, *colours):
+    def set_style(self, *colours: str):
         if self.use_colour:
             sys.stdout.write("".join([self.colours[c] for c in colours]))
 
-    def print(self, txt, end=None):
+    def print(self, txt: str, end: Optional[str] = None):
         if end is not None:
             print(txt, end=end)
         else:
             print(txt)
 
 
 class Txt(Console):
-    def __init__(self, ids):
+    def __init__(self, ids: Ids):
         super().__init__(ids, use_colour=False)
         self.text = ""
 
-    def print(self, txt, end=None):
-        self.text += txt + "\n" if end is None else txt
+    def print(self, txt: str, end: Optional[str] = None):
+        self.text += txt + "\n" if end is None else end
 
-    def to_string(self):
+    def to_string(self) -> None:
         print(self.text)
 
     def to_file(self, filepath: str) -> None:
         with open(filepath, "w", encoding="utf-8") as outfile:
             return outfile.write(self.text)
 
 
 class Json(Reporter):
-    def __init__(self, ids):
+    def __init__(self, ids: Ids):
         super().__init__(ids)
-        self.results = {}
+        self.results = Results()
 
-    def report(self):
+    def report(self) -> Results:
         self.results["title"] = self.ids.info.get("title", "Untitled IDS")
         self.results["date"] = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.results["filepath"] = self.ids.filepath
         self.results["filename"] = self.ids.filename
         total_specifications = 0
         total_specifications_pass = 0
         total_requirements = 0
@@ -201,129 +275,158 @@
         self.results["total_checks_pass"] = total_checks_pass
         self.results["total_checks_fail"] = total_checks - total_checks_pass
         self.results["percent_checks_pass"] = (
             math.floor((total_checks_pass / total_checks) * 100) if total_checks else "N/A"
         )
         return self.results
 
-    def report_specification(self, specification):
+    def report_specification(self, specification: Specification) -> ResultsSpecification:
         applicability = [a.to_string("applicability") for a in specification.applicability]
         total_applicable = len(specification.applicable_entities)
         total_checks = 0
         total_checks_pass = 0
         requirements = []
         for requirement in specification.requirements:
-            total_fail = len(requirement.failed_entities)
+            total_fail = len(requirement.failures)
             total_pass = total_applicable - total_fail
             percent_pass = math.floor((total_pass / total_applicable) * 100) if total_applicable else "N/A"
             total_checks += total_applicable
             total_checks_pass += total_pass
             requirements.append(
-                {
-                    "description": requirement.to_string("requirement", specification, requirement),
-                    "status": requirement.status,
-                    "failed_entities": self.report_failed_entities(requirement),
-                    "total_applicable": total_applicable,
-                    "total_pass": total_pass,
-                    "total_fail": total_fail,
-                    "percent_pass": percent_pass,
-                }
+                ResultsRequirement(
+                    description=requirement.to_string("requirement", specification, requirement),
+                    status=requirement.status,
+                    failed_entities=self.report_failed_entities(requirement),
+                    total_applicable=total_applicable,
+                    total_pass=total_pass,
+                    total_fail=total_fail,
+                    percent_pass=percent_pass,
+                )
             )
         total_applicable_pass = total_applicable - len(specification.failed_entities)
         percent_applicable_pass = (
             math.floor((total_applicable_pass / total_applicable) * 100) if total_applicable else "N/A"
         )
         percent_checks_pass = math.floor((total_checks_pass / total_checks) * 100) if total_checks else "N/A"
-        return {
-            "name": specification.name,
-            "description": specification.description,
-            "instructions": specification.instructions,
-            "status": specification.status,
-            "total_applicable": total_applicable,
-            "total_applicable_pass": total_applicable_pass,
-            "total_applicable_fail": total_applicable - total_applicable_pass,
-            "percent_applicable_pass": percent_applicable_pass,
-            "total_checks": total_checks,
-            "total_checks_pass": total_checks_pass,
-            "total_checks_fail": total_checks - total_checks_pass,
-            "percent_checks_pass": percent_checks_pass,
-            "required": specification.minOccurs != 0,
-            "applicability": applicability,
-            "requirements": requirements,
-        }
 
-    def report_failed_entities(self, requirement):
+        return ResultsSpecification(
+            name=specification.name,
+            description=specification.description,
+            instructions=specification.instructions,
+            status=specification.status,
+            total_applicable=total_applicable,
+            total_applicable_pass=total_applicable_pass,
+            total_applicable_fail=total_applicable - total_applicable_pass,
+            percent_applicable_pass=percent_applicable_pass,
+            total_checks=total_checks,
+            total_checks_pass=total_checks_pass,
+            total_checks_fail=total_checks - total_checks_pass,
+            percent_checks_pass=percent_checks_pass,
+            required=specification.minOccurs != 0,
+            applicability=applicability,
+            requirements=requirements,
+        )
+
+    def report_failed_entities(self, requirement: Facet) -> list[ResultsFailedEntity]:
         return [
-            {
-                "reason": requirement.failed_reasons[i],
-                "element": str(e),
-                "element_type": str(ifcopenshell.util.element.get_type(e)),
-                "class": e.is_a(),
-                "predefined_type": ifcopenshell.util.element.get_predefined_type(e),
-                "name": getattr(e, "Name", None),
-                "description": getattr(e, "Description", None),
-                "id": e.id(),
-                "global_id": getattr(e, "GlobalId", None),
-                "tag": getattr(e, "Tag", None),
-            }
-            for i, e in enumerate(requirement.failed_entities)
+            ResultsFailedEntity(
+                {
+                    "reason": f["reason"],
+                    "element": str(f["element"]),
+                    "element_type": str(ifcopenshell.util.element.get_type(f["element"])),
+                    "class": f["element"].is_a(),
+                    "predefined_type": ifcopenshell.util.element.get_predefined_type(f["element"]),
+                    "name": getattr(f["element"], "Name", None),
+                    "description": getattr(f["element"], "Description", None),
+                    "id": f["element"].id(),
+                    "global_id": getattr(f["element"], "GlobalId", None),
+                    "tag": getattr(f["element"], "Tag", None),
+                }
+            )
+            for f in requirement.failures
         ]
 
-    def to_string(self):
+    def to_string(self) -> str:
         import json
 
         return json.dumps(self.results)
 
     def to_file(self, filepath: str) -> None:
         import json
 
         with open(filepath, "w", encoding="utf-8") as outfile:
             return json.dump(self.results, outfile, ensure_ascii=False)
 
 
 class Html(Json):
-    def __init__(self, ids):
+    def __init__(self, ids: Ids):
         super().__init__(ids)
-        self.results = {}
 
-    def report(self):
+    def report(self) -> None:
         super().report()
         entity_limit = 100
         for spec in self.results["specifications"]:
             for requirement in spec["requirements"]:
                 total = len(requirement["failed_entities"])
                 requirement["failed_entities"] = requirement["failed_entities"][0:entity_limit]
                 requirement["has_omitted"] = total > entity_limit
                 requirement["total_entities"] = total
                 requirement["total_omitted"] = total - entity_limit
 
-    def to_string(self):
+    def to_string(self) -> str:
         import pystache
 
         with open(os.path.join(cwd, "templates", "report.html"), "r") as file:
             return pystache.render(file.read(), self.results)
 
     def to_file(self, filepath: str) -> None:
         import pystache
 
         with open(os.path.join(cwd, "templates", "report.html"), "r") as file:
             with open(filepath, "w", encoding="utf-8") as outfile:
                 return outfile.write(pystache.render(file.read(), self.results))
 
 
 class Ods(Json):
-    def __init__(self, ids):
+    def __init__(self, ids: Ids, excel_safe=False):
         super().__init__(ids)
+        self.excel_safe = excel_safe
         self.colours = {
             "h": "cccccc",  # Header
             "p": "97cc64",  # Pass
             "f": "fb5a3e",  # Fail
             "t": "ffffff",  # Regular text
         }
-        self.results = {}
+
+    def excel_safe_spreadsheet_name(self, name: str) -> str:
+        if not self.excel_safe:
+            return name
+
+        warning = (
+            f'WARNING. Sheet name "{name}" is not valid for Excel and will be changed. '
+            "See: https://support.microsoft.com/en-us/office/rename-a-worksheet-3f1f7148-ee83-404d-8ef0-9ff99fbad1f9"
+        )
+
+        if not name or name == "History":
+            print(warning)
+            return "placeholder spreadsheet name"
+
+        if name.startswith("'") or name.endswith("'"):
+            print(warning)
+            name = name.strip("'")
+
+        pattern = r"[\\\/\?\*\:\[\]]"
+        if re.search(pattern, name):
+            name = re.sub(pattern, "", name)
+            print(warning)
+
+        if len(name) > 31:
+            name = name[:31]
+            print(warning)
+        return name
 
     def to_file(self, filepath: str) -> None:
         from odf.opendocument import OpenDocumentSpreadsheet
         from odf.style import Style, TableCellProperties
         from odf.table import Table, TableRow, TableCell
         from odf.text import P
 
@@ -332,15 +435,15 @@
         self.cell_formats = {}
         for key, value in self.colours.items():
             style = Style(name=key, family="table-cell")
             style.addElement(TableCellProperties(backgroundcolor="#" + value))
             self.doc.automaticstyles.addElement(style)
             self.cell_formats[key] = style
 
-        table = Table(name=self.results["title"])
+        table = Table(name=self.excel_safe_spreadsheet_name(self.results["title"]))
         tr = TableRow()
         for header in ["Specification", "Status", "Total Pass", "Total Checks", "Percentage Pass"]:
             tc = TableCell(valuetype="string", stylename="h")
             tc.addElement(P(text=header))
             tr.addElement(tc)
         table.addElement(tr)
 
@@ -369,15 +472,15 @@
                 c += 1
             table.addElement(tr)
         self.doc.spreadsheet.addElement(table)
 
         for specification in self.results["specifications"]:
             if specification["status"]:
                 continue
-            table = Table(name=specification["name"])
+            table = Table(name=self.excel_safe_spreadsheet_name(specification["name"]))
             tr = TableRow()
             for header in [
                 "Requirement",
                 "Problem",
                 "Class",
                 "PredefinedType",
                 "Name",
@@ -417,24 +520,24 @@
                             col = "NULL"
                         tc.addElement(P(text=col))
                         tr.addElement(tc)
                         c += 1
                     table.addElement(tr)
             self.doc.spreadsheet.addElement(table)
 
-        self.doc.save(filepath, addsuffix=filepath.lower().endswith(".ods"))
+        self.doc.save(filepath, addsuffix=not filepath.lower().endswith(".ods"))
 
 
 class Bcf(Json):
-    def report_failed_entities(self, requirement):
-        return [
-            {"reason": requirement.failed_reasons[i], "element": e} for i, e in enumerate(requirement.failed_entities)
-        ]
+    def report_failed_entities(self, requirement: Facet) -> list[FacetFailure]:
+        return [FacetFailure(f) for f in requirement.failures]
 
     def to_file(self, filepath: str) -> None:
+        import numpy as np
+        import ifcopenshell.util.placement
         from bcf.v2.bcfxml import BcfXml
 
         unit_scale = None
         bcfxml = BcfXml.create_new(self.results["title"])
         for specification in self.results["specifications"]:
             if specification["status"]:
                 continue
```

### Comparing `ifctester-0.0.240318/ifctester/templates/report.html` & `ifctester-0.0.240418/ifctester/templates/report.html`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240318/test/test_facet.py` & `ifctester-0.0.240418/test/test_facet.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     ifctester.facet.get_psets.cache_clear()
     assert bool(facet(inst)) is expected
 
 
 class TestEntity:
     def test_creating_an_entity_facet(self):
         facet = Entity(name="IfcName")
-        assert facet.asdict() == {"name": {"simpleValue": "IfcName"}}
+        assert facet.asdict("applicability") == {"name": {"simpleValue": "IfcName"}}
         facet = Entity(name="IfcName", predefinedType="predefinedType", instructions="instructions")
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {
             "name": {"simpleValue": "IfcName"},
             "predefinedType": {"simpleValue": "predefinedType"},
             "@instructions": "instructions",
         }
 
     def test_filtering_using_an_entity_facet(self):
         set_facet("entity")
@@ -164,24 +164,24 @@
             inst=ifc.createIfcWall(PredefinedType="USERDEFINED", ObjectType="WALDO"),
             expected=False,
         )
 
         ifc = ifcopenshell.file()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType", predefined_type="X")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         facet = Entity(name="IFCWALL", predefinedType="X")
         run("Inherited predefined types should pass", facet=facet, inst=wall, expected=True)
 
         ifc = ifcopenshell.file()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall", predefined_type="X")
         wall_type = ifcopenshell.api.run(
             "root.create_entity", ifc, ifc_class="IfcWallType", predefined_type="NOTDEFINED"
         )
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         facet = Entity(name="IFCWALL", predefinedType="X")
         run("Overridden predefined types should pass", facet=facet, inst=wall, expected=True)
 
         restriction = Restriction(options={"enumeration": ["IFCWALL", "IFCSLAB"]})
         facet = Entity(name=restriction)
         ifc = ifcopenshell.file()
         run("Entities can be specified as an enumeration 1/3", facet=facet, inst=ifc.createIfcWall(), expected=True)
@@ -219,25 +219,22 @@
         wall3 = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall", predefined_type="BAZFOO")
         run("Restrictions an be specified for the predefined type 3/3", facet=facet, inst=wall3, expected=False)
 
 
 class TestAttribute:
     def test_creating_an_attribute_facet(self):
         attribute = Attribute(name="name")
-        assert attribute.asdict() == {"name": {"simpleValue": "name"}}
+        assert attribute.asdict("applicability") == {"name": {"simpleValue": "name"}}
         attribute = Attribute(name="name", value="value")
-        assert attribute.asdict() == {"name": {"simpleValue": "name"}, "value": {"simpleValue": "value"}}
-        attribute = Attribute(
-            name="name", value="value", minOccurs="0", maxOccurs="unbounded", instructions="instructions"
-        )
-        assert attribute.asdict() == {
+        assert attribute.asdict("applicability") == {"name": {"simpleValue": "name"}, "value": {"simpleValue": "value"}}
+        attribute = Attribute(name="name", value="value", cardinality="required", instructions="instructions")
+        assert attribute.asdict("requirement") == {
             "name": {"simpleValue": "name"},
             "value": {"simpleValue": "value"},
-            "@minOccurs": "0",
-            "@maxOccurs": "unbounded",
+            "@cardinality": "required",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_an_attribute_facet(self):
         set_facet("attribute")
 
         ifc = ifcopenshell.file()
@@ -254,20 +251,20 @@
         )
 
         ifc = ifcopenshell.file()
         facet = Attribute(name="Name")
         element = ifc.createIfcWall(Name="Foobar")
         run("A required facet checks all parameters as normal", facet=facet, inst=element, expected=True)
 
-        # facet = Attribute(name="Name", minOccurs=0, maxOccurs=0)
-        # run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
-        # facet = Attribute(name="Name", minOccurs=0)
-        # run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        # facet = Attribute(name="Rabbit", minOccurs=0)
-        # run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
+        facet = Attribute(name="Name", cardinality="prohibited")
+        run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
+        facet = Attribute(name="Name", cardinality="optional")
+        run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
+        facet = Attribute(name="Rabbit", cardinality="optional")
+        run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Attribute(name="Name")
         run("Attributes with null values always fail", facet=facet, inst=ifc.createIfcWall(), expected=False)
         # The logic is that unfortunately most BIM users cannot differentiate between the two.
         ifc = ifcopenshell.file()
         run("Attributes with empty strings always fail", facet=facet, inst=ifc.createIfcWall(Name=""), expected=False)
@@ -636,15 +633,15 @@
         run("Value restrictions may be used 2/3", facet=facet, inst=ifc.createIfcWall(Name="Bar"), expected=True)
         ifc = ifcopenshell.file()
         run("Value restrictions may be used 3/3", facet=facet, inst=ifc.createIfcWall(Name="Foobar"), expected=False)
 
         ifc = ifcopenshell.file()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         wall_type.Description = "Foobar"
         facet = Attribute(name="Description", value="Foobar")
         run("Attributes are not inherited by the occurrence", facet=facet, inst=wall, expected=False)
 
         restriction = Restriction(options={"enumeration": ["42", "43"]})
         facet = Attribute(name="RefractionIndex", value=restriction)
         ifc = ifcopenshell.file()
@@ -664,34 +661,34 @@
             inst=ifc.createIfcSurfaceStyleRefraction(RefractionIndex=42),
             expected=True,
         )
 
 
 class TestClassification:
     def test_creating_a_classification_facet(self):
-        facet = Classification()
-        assert facet.asdict() == {
-            "@maxOccurs": "unbounded"
-        }
+        facet = Classification(system="system")
+        assert facet.asdict("requirement") == {"system": {"simpleValue": "system"}, "@cardinality": "required"}
         facet = Classification(value="value", system="system")
-        assert facet.asdict() == {"value": {"simpleValue": "value"}, "system": {"simpleValue": "system"}, "@maxOccurs": "unbounded" }
+        assert facet.asdict("requirement") == {
+            "value": {"simpleValue": "value"},
+            "system": {"simpleValue": "system"},
+            "@cardinality": "required",
+        }
         facet = Classification(
             value="value",
             system="system",
             uri="https://test.com",
-            minOccurs="0",
-            maxOccurs="unbounded",
+            cardinality="required",
             instructions="instructions",
         )
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {
             "value": {"simpleValue": "value"},
             "system": {"simpleValue": "system"},
             "@uri": "https://test.com",
-            "@minOccurs": "0",
-            "@maxOccurs": "unbounded",
+            "@cardinality": "required",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_classification_facet(self):
         set_facet("classification")
 
         library = ifcopenshell.file()
@@ -705,73 +702,73 @@
 
         ifc = ifcopenshell.file()
         project = ifc.createIfcProject()
         system_a = ifcopenshell.api.run("classification.add_classification", ifc, classification=system_a)
         element0 = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         element1 = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=element1, reference=ref1, classification=system_a
+            "classification.add_reference", ifc, products=[element1], reference=ref1, classification=system_a
         )
         element11 = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcColumn")
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=element11, reference=ref11, classification=system_a
+            "classification.add_reference", ifc, products=[element11], reference=ref11, classification=system_a
         )
         element22 = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
         ifcopenshell.api.run(
             "classification.add_reference",
             ifc,
-            product=element22,
+            products=[element22],
             reference=ref22,
             classification=system_a,
             is_lightweight=False,
         )
         material = ifc.createIfcMaterial(Name="Material")
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=material, reference=ref1, classification=system_a
+            "classification.add_reference", ifc, products=[material], reference=ref1, classification=system_a
         )
 
-        facet = Classification()
+        facet = Classification(system="Foobar")
         run(
-            "A classification facet with no data matches any classification 1/2",
+            "A classification facet with no value matches any classification 1/2",
             facet=facet,
             inst=element0,
             expected=False,
         )
         run(
-            "A classification facet with no data matches any classification 2/2",
+            "A classification facet with no value matches any classification 2/2",
             facet=facet,
             inst=element1,
             expected=True,
         )
 
         run("A required facet checks all parameters as normal", facet=facet, inst=element1, expected=True)
-        facet = Classification(minOccurs=0, maxOccurs=0)
+        facet = Classification(system="Foobar", cardinality="prohibited")
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element1, expected=False)
-        facet = Classification(minOccurs=0)
+        facet = Classification(system="Foobar", cardinality="optional")
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element0, expected=True)
-        facet = Classification(minOccurs=0)
+        facet = Classification(system="Foobar", cardinality="optional")
         run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element1, expected=True)
 
-        facet = Classification(value="1")
+        facet = Classification(system="Foobar", value="1")
         run(
             "Values should match exactly if lightweight classifications are used",
             facet=facet,
             inst=element1,
             expected=True,
         )
 
-        facet = Classification(value="2")
+        facet = Classification(system="Foobar", value="2")
         run(
             "Values match subreferences if full classifications are used (e.g. EF_25_10 should match EF_25_10_25, EF_25_10_30, etc)",
             facet=facet,
             inst=element22,
             expected=True,
         )
 
-        facet = Classification(value="1")
+        facet = Classification(system="Foobar", value="1")
         run(
             "Non-rooted resources that have external classification references should also pass",
             facet=facet,
             inst=material,
             expected=True,
         )
 
@@ -779,15 +776,15 @@
         run("Systems should match exactly 1/5", facet=facet, inst=project, expected=True)
         run("Systems should match exactly 2/5", facet=facet, inst=element0, expected=False)
         run("Systems should match exactly 3/5", facet=facet, inst=element1, expected=True)
         run("Systems should match exactly 4/5", facet=facet, inst=element11, expected=True)
         run("Systems should match exactly 5/5", facet=facet, inst=element22, expected=True)
 
         restriction = Restriction(options={"pattern": "1.*"})
-        facet = Classification(value=restriction)
+        facet = Classification(system="Foobar", value=restriction)
         run("Restrictions can be used for values 1/3", facet=facet, inst=element1, expected=True)
         run("Restrictions can be used for values 2/3", facet=facet, inst=element11, expected=True)
         run("Restrictions can be used for values 3/3", facet=facet, inst=element22, expected=False)
 
         restriction = Restriction(options={"pattern": "Foo.*"})
         facet = Classification(system=restriction)
         run("Restrictions can be used for systems 1/2", facet=facet, inst=element0, expected=False)
@@ -807,172 +804,170 @@
             expected=False,
         )
 
         # IFC doesn't yet formally specify how inheritance and overrides work here. We follow these rules:
         # https://github.com/buildingSMART/IFC4.3.x-development/issues/475
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=wall, reference=ref11, classification=system_a
+            "classification.add_reference", ifc, products=[wall], reference=ref11, classification=system_a
         )
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=wall_type, reference=ref22, classification=system_a
+            "classification.add_reference", ifc, products=[wall_type], reference=ref22, classification=system_a
         )
 
         system_b = ifcopenshell.api.run("classification.add_classification", ifc, classification=system_b)
         ifcopenshell.api.run(
-            "classification.add_reference", ifc, product=wall_type, reference=refx, classification=system_b
+            "classification.add_reference", ifc, products=[wall_type], reference=refx, classification=system_b
         )
 
-        facet = Classification(value="11")
+        facet = Classification(system="Foobar", value="11")
         run("Occurrences override the type classification per system 1/3", facet=facet, inst=wall, expected=True)
-        facet = Classification(value="22")
+        facet = Classification(system="Foobar", value="22")
         run("Occurrences override the type classification per system 2/3", facet=facet, inst=wall, expected=False)
-        facet = Classification(value="X")
+        facet = Classification(system="Foobaz", value="X")
         run("Occurrences override the type classification per system 3/3", facet=facet, inst=wall, expected=True)
 
 
 class TestProperty:
     def test_creating_a_property_facet(self):
         facet = Property()
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {
             "propertySet": {"simpleValue": "Property_Set"},
-            "name": {"simpleValue": "PropertyName"},
-            "@maxOccurs": "unbounded"
+            "baseName": {"simpleValue": "PropertyName"},
+            "@cardinality": "required",
         }
         facet = Property(
             propertySet="propertySet",
-            name="name",
+            baseName="baseName",
             value="value",
-            datatype="datatype",
+            dataType="dataType",
             uri="https://test.com",
-            minOccurs="0",
-            maxOccurs="unbounded",
+            cardinality="required",
             instructions="instructions",
         )
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {
             "propertySet": {"simpleValue": "propertySet"},
-            "name": {"simpleValue": "name"},
+            "baseName": {"simpleValue": "baseName"},
             "value": {"simpleValue": "value"},
-            "@datatype": "datatype",
+            "@dataType": "DATATYPE",
             "@uri": "https://test.com",
-            "@minOccurs": "0",
-            "@maxOccurs": "unbounded",
+            "@cardinality": "required",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_property_facet(self):
         set_facet("property")
 
         ifc = self.setup_ifc()
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         run("Elements with no properties always fail", facet=facet, inst=element, expected=False)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": "AnotherValue"})
         run("Elements with a matching pset but no property also fail", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": None})
         run("Properties with a null value fail", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("A name check will match any property with any string value", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("A required facet checks all parameters as normal", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL", minOccurs=0, maxOccurs=0)
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL", cardinality="prohibited")
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL", minOccurs=0)
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL", cardinality="optional")
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Bar", datatype="IFCLABEL", minOccurs=0)
+        facet = Property(propertySet="Foo_Bar", baseName="Bar", dataType="IFCLABEL", cardinality="optional")
         run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=element, expected=True)
 
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ""})
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLOGICAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLOGICAL")
         run("An empty string is considered falsey and will not pass", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcLogical("UNKNOWN")})
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCDURATION")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCDURATION")
         run("A logical unknown is considered falsey and will not pass", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("P0D")})
         run("A zero duration will pass", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCBOOLEAN")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCBOOLEAN")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcBoolean(True)})
         run("A property set to true will pass a name check", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": False})
         run(
             "A property set to false is still considered a value and will pass a name check",
             facet=facet,
             inst=element,
             expected=True,
         )
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="Bar", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("Specifying a value performs a case-sensitive match 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "bar"})
         run("Specifying a value performs a case-sensitive match 2/2", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Baz"})
         run("Specifying a value fails against different values", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="♫Don'tÄrgerhôtelЊет", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="♫Don'tÄrgerhôtelЊет", dataType="IFCLABEL")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "♫Don'tÄrgerhôtelЊет"})
         run("Non-ascii characters are treated without encoding", facet=facet, inst=element, expected=True)
 
         identifier = "123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345678901234567890123456789012345"
         facet = Property(
-            propertySet="Foo_Bar", name="Foo", value=identifier + "_extra_characters", datatype="IFCIDENTIFIER"
+            propertySet="Foo_Bar", baseName="Foo", value=identifier + "_extra_characters", dataType="IFCIDENTIFIER"
         )
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcIdentifier(identifier)})
         run("IDS does not handle string truncation such as for identifiers", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="1", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "1"})
         run("A number specified as a string is treated as a string", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", datatype="IFCINTEGER")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42", dataType="IFCINTEGER")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcInteger(42)})
         run("Integer values are checked using type casting 1/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", datatype="IFCINTEGER")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.", dataType="IFCINTEGER")
         run("Integer values are checked using type casting 2/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", datatype="IFCINTEGER")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.0", dataType="IFCINTEGER")
         run("Integer values are checked using type casting 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", datatype="IFCINTEGER")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.3", dataType="IFCINTEGER")
         run("Integer values are checked using type casting 4/4", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42", dataType="IFCREAL")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0)})
         run("Real values are checked using type casting 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.0", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.0", dataType="IFCREAL")
         run("Real values are checked using type casting 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.3", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.3", dataType="IFCREAL")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.3)})
         run("Real values are checked using type casting 3/3", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42,3", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42,3", dataType="IFCREAL")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.3)})
         run("Only specifically formatted numbers are allowed 1/4", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="123,4.5", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="123,4.5", dataType="IFCREAL")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(1234.5)})
         run("Only specifically formatted numbers are allowed 2/4", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345e3", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="1.2345e3", dataType="IFCREAL")
         run("Only specifically formatted numbers are allowed 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1.2345E3", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="1.2345E3", dataType="IFCREAL")
         run("Only specifically formatted numbers are allowed 4/4", facet=facet, inst=element, expected=True)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="42.", datatype="IFCREAL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="42.", dataType="IFCREAL")
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 + 1e-6))}
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 1/4", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 - 1e-6))}
         )
@@ -982,31 +977,31 @@
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 3/4", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcReal(42.0 * (1.0 - 2e-6))}
         )
         run("Floating point numbers are compared with a 1e-6 tolerance 4/4", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="TRUE", datatype="IFCBOOLEAN")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="TRUE", dataType="IFCBOOLEAN")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcBoolean(False)})
         run("Booleans must be specified as uppercase strings 1/3", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="FALSE", datatype="IFCBOOLEAN")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="FALSE", dataType="IFCBOOLEAN")
         run("Booleans must be specified as uppercase strings 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="False", datatype="IFCBOOLEAN")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="False", dataType="IFCBOOLEAN")
         run("Booleans must be specified as uppercase strings 3/3", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2022-01-01", datatype="IFCDATE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="2022-01-01", dataType="IFCDATE")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDate("2022-01-01")})
         run("Dates are treated as strings 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run(
             "pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDate("2022-01-01+00:00")}
         )
         run("Dates are treated as strings 2/2", facet=facet, inst=element, expected=False)
 
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="PT16H", datatype="IFCDURATION")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="PT16H", dataType="IFCDURATION")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("PT16H")})
         run("Durations are treated as strings 1/2", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcDuration("P2D")})
         run("Durations are treated as strings 1/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
@@ -1015,73 +1010,73 @@
         ifcopenshell.api.run(
             "pset.edit_pset",
             ifc,
             pset=pset,
             properties={"Status": ["EXISTING", "DEMOLISH"]},
             pset_template=pset_template,
         )
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="EXISTING", datatype="IFCLABEL")
+        facet = Property(propertySet="Pset_WallCommon", baseName="Status", value="EXISTING", dataType="IFCLABEL")
         run("Any matching value in an enumerated property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="DEMOLISH", datatype="IFCLABEL")
+        facet = Property(propertySet="Pset_WallCommon", baseName="Status", value="DEMOLISH", dataType="IFCLABEL")
         run("Any matching value in an enumerated property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Pset_WallCommon", name="Status", value="NEW", datatype="IFCLABEL")
+        facet = Property(propertySet="Pset_WallCommon", baseName="Status", value="NEW", dataType="IFCLABEL")
         run("Any matching value in an enumerated property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         list_property = ifc.createIfcPropertyListValue(
             Name="Foo", ListValues=[ifc.createIfcLabel("X"), ifc.createIfcLabel("Y")]
         )
         pset.HasProperties = [list_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="X", dataType="IFCLABEL")
         run("Any matching value in a list property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="Y", dataType="IFCLABEL")
         run("Any matching value in a list property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Z", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="Z", dataType="IFCLABEL")
         run("Any matching value in a list property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         bounded_property = ifc.createIfcPropertyBoundedValue(
             Name="Foo",
             UpperBoundValue=ifc.createIfcLengthMeasure(5000),
             LowerBoundValue=ifc.createIfcLengthMeasure(1000),
             SetPointValue=ifc.createIfcLengthMeasure(3000),
         )
         pset.HasProperties = [bounded_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="1", dataType="IFCLENGTHMEASURE")
         run("Any matching value in a bounded property will pass 1/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="5", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="5", dataType="IFCLENGTHMEASURE")
         run("Any matching value in a bounded property will pass 2/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="3", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="3", dataType="IFCLENGTHMEASURE")
         run("Any matching value in a bounded property will pass 3/4", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="2", dataType="IFCLENGTHMEASURE")
         run("Any matching value in a bounded property will pass 4/4", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         table_property = ifc.createIfcPropertyTableValue(
             Name="Foo", DefiningValues=[ifc.createIfcLabel("X")], DefinedValues=[ifc.createIfcLengthMeasure(1000)]
         )
         pset.HasProperties = [table_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="X", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="X", dataType="IFCLABEL")
         run("Any matching value in a table property will pass 1/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="1", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="1", dataType="IFCLENGTHMEASURE")
         run("Any matching value in a table property will pass 2/3", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Y", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="Y", dataType="IFCLABEL")
         run("Any matching value in a table property will pass 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         pset.HasProperties = [ifc.createIfcPropertyReferenceValue(Name="Foo")]
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL")
         run("Reference properties are treated as objects and not supported", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDoor")
         pset = ifc.create_entity(
             "IfcDoorPanelProperties",
             GlobalId=ifcopenshell.guid.new(),
@@ -1092,84 +1087,84 @@
         ifc.create_entity(
             "IfcRelDefinesByProperties",
             GlobalId=ifcopenshell.guid.new(),
             RelatedObjects=[element],
             RelatingPropertyDefinition=pset,
         )
         facet = Property(
-            propertySet="Foo_Bar", name="PanelOperation", value="SWINGING", datatype="IFCDOORPANELOPERATIONENUM"
+            propertySet="Foo_Bar", baseName="PanelOperation", value="SWINGING", dataType="IFCDOORPANELOPERATIONENUM"
         )
         run("Predefined properties are supported but discouraged 1/2", facet=facet, inst=element, expected=True)
         facet = Property(
-            propertySet="Foo_Bar", name="PanelOperation", value="SWONGING", datatype="IFCDOORPANELOPERATIONENUM"
+            propertySet="Foo_Bar", baseName="PanelOperation", value="SWONGING", dataType="IFCDOORPANELOPERATIONENUM"
         )
         run("Predefined properties are supported but discouraged 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLENGTHMEASURE")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         qto = ifcopenshell.api.run("pset.add_qto", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_qto", ifc, qto=qto, properties={"Foo": ifc.createIfcLengthMeasure(42)})
         run("A name check will match any quantity with any value", facet=facet, inst=element, expected=True)
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCAREAMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCAREAMEASURE")
         run("Quantities must also match the appropriate measure", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         complex_property = ifc.createIfcComplexProperty(Name="Foo", UsageName="RabbitAgilityTraining")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=complex_property, properties={"Rabbits": "Awesome"})
         pset.HasProperties = [complex_property]
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL")
         run("Complex properties are not supported 1/2", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo", name="Rabbits", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo", baseName="Rabbits", dataType="IFCLABEL")
         run("Complex properties are not supported 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         qto = ifcopenshell.api.run("pset.add_qto", ifc, product=element, name="Foo_Bar")
         complex_quantity = ifc.createIfcPhysicalComplexQuantity(Name="Foo", Discrimination="FurThickness")
         ifcopenshell.api.run(
             "pset.edit_qto", ifc, qto=complex_quantity, properties={"MyLength": ifc.createIfcLengthMeasure(42)}
         )
         qto.Quantities = [complex_quantity]
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLENGTHMEASURE")
         run("Complex properties are not supported 1/2", facet=facet, inst=element, expected=False)
-        facet = Property(propertySet="Foo", name="MyLength", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo", baseName="MyLength", dataType="IFCLENGTHMEASURE")
         run("Complex properties are not supported 2/2", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         restriction = Restriction(options={"pattern": "Foo_.*"})
-        facet = Property(propertySet=restriction, name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet=restriction, baseName="Foo", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("All matching property sets must satisfy requirements 1/3", facet=facet, inst=element, expected=True)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Baz")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"AnotherProperty": "AnotherValue"})
         run("All matching property sets must satisfy requirements 2/3", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
         run("All matching property sets must satisfy requirements 3/3", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
         restriction = Restriction(options={"pattern": "Foo.*"})
-        facet = Property(propertySet="Foo_Bar", name=restriction, value="x", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName=restriction, value="x", dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x"})
         run("All matching properties must satisfy requirements 1/3", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "x"})
         run("All matching properties must satisfy requirements 2/3", facet=facet, inst=element, expected=True)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "y"})
         run("All matching properties must satisfy requirements 3/3", facet=facet, inst=element, expected=False)
 
         ifc = self.setup_ifc()
         restriction1 = Restriction(options={"pattern": "Foo.*"})
         restriction2 = Restriction(options={"enumeration": ["x", "y"]})
-        facet = Property(propertySet="Foo_Bar", name=restriction1, value=restriction2, datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName=restriction1, value=restriction2, dataType="IFCLABEL")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foobar": "x", "Foobaz": "y"})
         run(
             "If multiple properties are matched, all values must satisfy requirements 1/2",
             facet=facet,
             inst=element,
@@ -1180,24 +1175,24 @@
             "If multiple properties are matched, all values must satisfy requirements 2/2",
             facet=facet,
             inst=element,
             expected=False,
         )
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IFCTIMEMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="2", dataType="IFCTIMEMEASURE")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcMassMeasure(2)})
         run("Measures are used to specify an IFC data type 1/2", facet=facet, inst=element, expected=False)
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcTimeMeasure(2)})
         run("Measures are used to specify an IFC data type 2/2", facet=facet, inst=element, expected=True)
 
         ifc = self.setup_ifc()
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="2", datatype="IFCLENGTHMEASURE")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="2", dataType="IFCLENGTHMEASURE")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=element, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": ifc.createIfcLengthMeasure(2)})
         run(
             "Unit conversions shall take place to IDS-nominated standard units 1/2",
             facet=facet,
             inst=element,
@@ -1210,30 +1205,30 @@
             inst=element,
             expected=True,
         )
 
         ifc = self.setup_ifc()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall_type, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
-        facet = Property(propertySet="Foo_Bar", name="Foo", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", dataType="IFCLABEL")
         run("Properties can be inherited from the type 1/2", facet=facet, inst=wall, expected=True)
         run("Properties can be inherited from the type 2/2", facet=facet, inst=wall_type, expected=True)
 
         ifc = self.setup_ifc()
         wall = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         wall_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=wall, relating_type=wall_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[wall], relating_type=wall_type)
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall_type, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Baz"})
         pset = ifcopenshell.api.run("pset.add_pset", ifc, product=wall, name="Foo_Bar")
         ifcopenshell.api.run("pset.edit_pset", ifc, pset=pset, properties={"Foo": "Bar"})
-        facet = Property(propertySet="Foo_Bar", name="Foo", value="Bar", datatype="IFCLABEL")
+        facet = Property(propertySet="Foo_Bar", baseName="Foo", value="Bar", dataType="IFCLABEL")
         run("Properties can be overriden by an occurrence 1/2", facet=facet, inst=wall, expected=True)
         run("Properties can be overriden by an occurrence 2/2", facet=facet, inst=wall_type, expected=False)
 
     def setup_ifc(self):
         ifc = ifcopenshell.file()
         ifc.createIfcProject()
         # Milli prefix used to check measurement conversions
@@ -1244,74 +1239,71 @@
         ifcopenshell.api.run("unit.assign_unit", ifc, units=[lengthunit, areaunit, volumeunit, timeunit])
         return ifc
 
 
 class TestMaterial:
     def test_creating_a_material_facet(self):
         facet = Material()
-        assert facet.asdict() == {"@maxOccurs": "unbounded"}
-        facet = Material(
-            value="value", uri="https://test.com", minOccurs="0", maxOccurs="unbounded", instructions="instructions"
-        )
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {"@cardinality": "required"}
+        facet = Material(value="value", uri="https://test.com", cardinality="required", instructions="instructions")
+        assert facet.asdict("requirement") == {
             "value": {"simpleValue": "value"},
             "@uri": "https://test.com",
-            "@minOccurs": "0",
-            "@maxOccurs": "unbounded",
+            "@cardinality": "required",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_material_facet(self):
         set_facet("material")
 
         facet = Material()
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         run("Elements without a material always fail", facet=facet, inst=element, expected=False)
         material = ifcopenshell.api.run("material.add_material", ifc)
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material)
         run("Elements with any material will pass an empty material facet", facet=facet, inst=element, expected=True)
 
         run("A required facet checks all parameters as normal", facet=facet, inst=element, expected=True)
-        facet = Material(minOccurs=0, maxOccurs=0)
+        facet = Material(cardinality="prohibited")
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=element, expected=False)
-        facet = Material(minOccurs=0)
+        facet = Material(cardinality="optional")
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        facet = Material(value="Foo", minOccurs=0)
+        facet = Material(value="Foo", cardinality="optional")
         run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Material(value="Foo")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         material = ifcopenshell.api.run("material.add_material", ifc)
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material)
         material.Name = "Foo"
         run("A material name may pass the value check", facet=facet, inst=element, expected=True)
         material.Name = "Bar"
         material.Category = "Foo"
         run("A material category may pass the value check", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Material(value="Foo")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         material_set = ifcopenshell.api.run("material.add_material_set", ifc, set_type="IfcMaterialList")
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material_set)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material_set)
         material = ifcopenshell.api.run("material.add_material", ifc)
         ifcopenshell.api.run("material.add_list_item", ifc, material_list=material_set, material=material)
         material.Name = "Foo"
         run("Any material Name in a list will pass a value check", facet=facet, inst=element, expected=True)
         material.Name = "Bar"
         material.Category = "Foo"
         run("Any material Category in a list will pass a value check", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Material(value="Foo")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         material_set = ifcopenshell.api.run("material.add_material_set", ifc, set_type="IfcMaterialLayerSet")
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material_set)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material_set)
         material = ifcopenshell.api.run("material.add_material", ifc)
         layer = ifcopenshell.api.run("material.add_layer", ifc, layer_set=material_set, material=material)
         layer.Name = "Foo"
         run("Any layer Name in a layer set will pass a value check", facet=facet, inst=element, expected=True)
         layer.Name = "Bar"
         layer.Category = "Foo"
         run("Any layer Category in a layer set will pass a value check", facet=facet, inst=element, expected=True)
@@ -1322,15 +1314,15 @@
         material.Category = "Foo"
         run("Any material Category in a layer set will pass a value check", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Material(value="Foo")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         material_set = ifcopenshell.api.run("material.add_material_set", ifc, set_type="IfcMaterialProfileSet")
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material_set)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material_set)
         material = ifcopenshell.api.run("material.add_material", ifc)
         profile = ifcopenshell.api.run("material.add_profile", ifc, profile_set=material_set, material=material)
         profile.Name = "Foo"
         profile.Profile = ifc.createIfcCircleProfileDef("AREA", None, None, 1)
         run("Any profile Name in a profile set will pass a value check", facet=facet, inst=element, expected=True)
         profile.Name = "Bar"
         profile.Category = "Foo"
@@ -1342,15 +1334,15 @@
         material.Category = "Foo"
         run("Any material category in a profile set will pass a value check", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         facet = Material(value="Foo")
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         material_set = ifcopenshell.api.run("material.add_material_set", ifc, set_type="IfcMaterialConstituentSet")
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material_set)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material_set)
         run("A constituent set with no data will fail a value check", facet=facet, inst=element, expected=False)
         material = ifcopenshell.api.run("material.add_material", ifc)
         constituent = ifcopenshell.api.run(
             "material.add_constituent", ifc, constituent_set=material_set, material=material
         )
         constituent.Name = "Foo"
         run(
@@ -1378,82 +1370,80 @@
             inst=element,
             expected=True,
         )
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         element_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=element, relating_type=element_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[element], relating_type=element_type)
         material = ifcopenshell.api.run("material.add_material", ifc)
-        ifcopenshell.api.run("material.assign_material", ifc, product=element_type, material=material)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element_type], material=material)
         material.Name = "Foo"
         facet = Material(value="Foo")
         run("Occurrences can inherit materials from their types", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         element_type = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWallType")
-        ifcopenshell.api.run("type.assign_type", ifc, related_object=element, relating_type=element_type)
+        ifcopenshell.api.run("type.assign_type", ifc, related_objects=[element], relating_type=element_type)
         material = ifcopenshell.api.run("material.add_material", ifc)
-        ifcopenshell.api.run("material.assign_material", ifc, product=element_type, material=material)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element_type], material=material)
         material.Name = "Bar"
         material = ifcopenshell.api.run("material.add_material", ifc)
-        ifcopenshell.api.run("material.assign_material", ifc, product=element, material=material)
+        ifcopenshell.api.run("material.assign_material", ifc, products=[element], material=material)
         material.Name = "Foo"
         facet = Material(value="Foo")
         run("Occurrences can override materials from their types", facet=facet, inst=element, expected=True)
 
 
 class TestPartOf:
     def test_creating_a_partof_facet(self):
         facet = PartOf()
-        assert facet.asdict() == {"entity": {"name": {"simpleValue": "IFCWALL"}}, "@maxOccurs": "unbounded" }
+        assert facet.asdict("requirement") == {
+            "entity": {"name": {"simpleValue": "IFCWALL"}},
+            "@cardinality": "required",
+        }
         facet = PartOf(
             name="IFCGROUP",
             predefinedType="predefinedType",
             relation="IFCRELASSIGNSTOGROUP",
-            minOccurs="0",
-            maxOccurs="unbounded",
+            cardinality="required",
             instructions="instructions",
         )
-        assert facet.asdict() == {
+        assert facet.asdict("requirement") == {
             "entity": {
                 "name": {"simpleValue": "IFCGROUP"},
                 "predefinedType": {"simpleValue": "predefinedType"},
             },
             "@relation": "IFCRELASSIGNSTOGROUP",
-            "@minOccurs": "0",
-            "@maxOccurs": "unbounded",
+            "@cardinality": "required",
             "@instructions": "instructions",
         }
 
     def test_filtering_using_a_partof_facet(self):
         set_facet("partof")
 
         ifc = ifcopenshell.file()
 
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcWall")
         facet = PartOf(name="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES")
         run("A non aggregated element fails an aggregate relationship", facet=facet, inst=subelement, expected=False)
-        ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
+        ifcopenshell.api.run("aggregate.assign_object", ifc, products=[subelement], relating_object=element)
         run("The aggregated whole fails an aggregate relationship", facet=facet, inst=element, expected=False)
         run("The aggregated part passes an aggregate relationship", facet=facet, inst=subelement, expected=True)
 
         run("A required facet checks all parameters as normal", facet=facet, inst=subelement, expected=True)
-        facet = PartOf(name="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES", minOccurs=0, maxOccurs=0)
+        facet = PartOf(name="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES", cardinality="prohibited")
         run("A prohibited facet returns the opposite of a required facet", facet=facet, inst=subelement, expected=False)
-        facet = PartOf(name="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES", minOccurs=0)
-        run("An optional facet always passes regardless of outcome 1/2", facet=facet, inst=element, expected=True)
-        run("An optional facet always passes regardless of outcome 2/2", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
-        ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
+        ifcopenshell.api.run("aggregate.assign_object", ifc, products=[subelement], relating_object=element)
         facet = PartOf(name="IFCSLAB", relation="IFCRELAGGREGATES")
         run("An aggregate may specify the entity of the whole 1/2", facet=facet, inst=subelement, expected=True)
         facet = PartOf(name="IFCWALL", relation="IFCRELAGGREGATES")
         run("An aggregate may specify the entity of the whole 2/2", facet=facet, inst=subelement, expected=False)
 
         element.PredefinedType = "BASESLAB"
         facet = PartOf(name="IFCSLAB", predefinedType="BASESLAB", relation="IFCRELAGGREGATES")
@@ -1468,16 +1458,16 @@
             expected=False,
         )
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subsubelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
-        ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
-        ifcopenshell.api.run("aggregate.assign_object", ifc, product=subsubelement, relating_object=subelement)
+        ifcopenshell.api.run("aggregate.assign_object", ifc, products=[subelement], relating_object=element)
+        ifcopenshell.api.run("aggregate.assign_object", ifc, products=[subsubelement], relating_object=subelement)
         facet = PartOf(name="IFCELEMENTASSEMBLY", relation="IFCRELAGGREGATES")
         run("An aggregate entity may pass any ancestral whole passes", facet=facet, inst=subsubelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         group = ifcopenshell.api.run("group.add_group", ifc)
         facet = PartOf(name="IFCGROUP", relation="IFCRELASSIGNSTOGROUP")
@@ -1501,54 +1491,54 @@
         run("A group predefined type must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
         facet = PartOf(name="IFCSPACE", relation="IFCRELCONTAINEDINSPATIALSTRUCTURE")
         run("Any contained element passes a containment relationship 1/2", facet=facet, inst=element, expected=False)
-        ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
+        ifcopenshell.api.run("spatial.assign_container", ifc, products=[element], relating_structure=container)
         run("Any contained element passes a containment relationship 2/2", facet=facet, inst=element, expected=True)
         run("The container itself always fails", facet=facet, inst=container, expected=False)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcElementAssembly")
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
-        ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
+        ifcopenshell.api.run("spatial.assign_container", ifc, products=[element], relating_structure=container)
         facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", name="IFCSITE")
         run("The container entity must match exactly 1/2", facet=facet, inst=element, expected=False)
         facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", name="IFCSPACE")
         run("The container entity must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         container.ObjectType = "BURROW"
         facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", name="IFCSPACE", predefinedType="WARREN")
         run("The container predefined type must match exactly 1/2", facet=facet, inst=element, expected=False)
         facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", name="IFCSPACE", predefinedType="BURROW")
         run("The container predefined type must match exactly 2/2", facet=facet, inst=element, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSlab")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcBeam")
-        ifcopenshell.api.run("aggregate.assign_object", ifc, product=subelement, relating_object=element)
+        ifcopenshell.api.run("aggregate.assign_object", ifc, products=[subelement], relating_object=element)
         container = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcSpace")
-        ifcopenshell.api.run("spatial.assign_container", ifc, product=element, relating_structure=container)
+        ifcopenshell.api.run("spatial.assign_container", ifc, products=[element], relating_structure=container)
         facet = PartOf(relation="IFCRELCONTAINEDINSPATIALSTRUCTURE", name="IFCSPACE")
         run("The container may be indirect", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
-        ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
+        ifcopenshell.api.run("nest.assign_object", ifc, related_objects=[subelement], relating_object=element)
         facet = PartOf(name="IFCFURNITURE", relation="IFCRELNESTS")
         run("Any nested part passes a nest relationship", facet=facet, inst=subelement, expected=True)
         run("Any nested whole fails a nest relationship", facet=facet, inst=element, expected=False)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
-        ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
+        ifcopenshell.api.run("nest.assign_object", ifc, related_objects=[subelement], relating_object=element)
         facet = PartOf(relation="IFCRELNESTS", name="IFCBEAM")
         run("The nest entity must match exactly 1/2", facet=facet, inst=subelement, expected=False)
         facet = PartOf(relation="IFCRELNESTS", name="IFCFURNITURE")
         run("The nest entity must match exactly 2/2", facet=facet, inst=subelement, expected=True)
 
         element.PredefinedType = "USERDEFINED"
         element.ObjectType = "WATERBOTTLE"
@@ -1557,16 +1547,16 @@
         facet = PartOf(relation="IFCRELNESTS", name="IFCFURNITURE", predefinedType="WATERBOTTLE")
         run("The nest predefined type must match exactly 2/2", facet=facet, inst=subelement, expected=True)
 
         ifc = ifcopenshell.file()
         element = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcFurniture")
         subelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcDiscreteAccessory")
         subsubelement = ifcopenshell.api.run("root.create_entity", ifc, ifc_class="IfcMechanicalFastener")
-        ifcopenshell.api.run("nest.assign_object", ifc, related_object=subelement, relating_object=element)
-        ifcopenshell.api.run("nest.assign_object", ifc, related_object=subsubelement, relating_object=subelement)
+        ifcopenshell.api.run("nest.assign_object", ifc, related_objects=[subelement], relating_object=element)
+        ifcopenshell.api.run("nest.assign_object", ifc, related_objects=[subsubelement], relating_object=subelement)
         facet = PartOf(relation="IFCRELNESTS", name="IFCFURNITURE")
         run("Nesting may be indirect", facet=facet, inst=subsubelement, expected=True)
 
 
 class TestRestriction:
     def test_creating_a_restriction(self):
         restriction = Restriction(options={"enumeration": ["foo", "bar"]})
```

### Comparing `ifctester-0.0.240318/test/test_ids.py` & `ifctester-0.0.240418/test/test_ids.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,47 +17,54 @@
 # along with IfcTester.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import pytest
 import xmlschema
 import ifcopenshell
 from ifctester import ids
+from typing import Optional
 
 
-def run(name, ids, ifc, expected, applicable_entities=None, failed_entities=None):
+def run(
+    name: str,
+    ids: ids.Ids,
+    ifc: ifcopenshell.file,
+    expected: bool,
+    applicable_entities: Optional[list[ifcopenshell.entity_instance]] = None,
+    failed_entities: Optional[list[ifcopenshell.entity_instance]] = None,
+):
     ids.validate(ifc)
     all_applicable = set()
     all_failures = set()
     if not applicable_entities:
         applicable_entities = []
     if not failed_entities:
         failed_entities = []
     for spec in ids.specifications:
         assert spec.status is expected
         all_applicable.update(spec.applicable_entities)
         for requirement in spec.requirements:
             if requirement.status is False:
-                all_failures.update(requirement.failed_entities)
+                all_failures.update([f["element"] for f in requirement.failures])
     assert set(all_applicable) == set(applicable_entities)
     assert set(all_failures) == set(failed_entities)
 
 
 class TestIds:
     def test_failing_on_opening_invalid_ids_data(self):
         with pytest.raises(xmlschema.validators.exceptions.XMLSchemaValidationError):
             ids.open("""<?xml version="1.0" encoding="UTF-8"?><clearly_not_an_ids/>""")
 
     def test_create_an_ids_with_minimal_information(self):
         specs = ids.Ids()
-        print('AAA', specs.asdict())
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.6/ids.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.7/ids.xsd",
             "info": {"title": "Untitled"},
             "specifications": {"specification": []},
         }
 
     def test_create_an_ids_with_all_possible_information(self):
         specs = ids.Ids(
             title="title",
@@ -69,15 +76,15 @@
             purpose="purpose",
             milestone="milestone",
         )
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.6/ids.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.7/ids.xsd",
             "info": {
                 "title": "title",
                 "copyright": "copyright",
                 "version": "version",
                 "description": "description",
                 "author": "author@test.com",
                 "date": "2020-01-01",
@@ -89,15 +96,15 @@
 
     def test_check_invalid_ids_information(self):
         specs = ids.Ids(title=None, author="author", date="9999-99-99")
         assert specs.asdict() == {
             "@xmlns": "http://standards.buildingsmart.org/IDS",
             "@xmlns:xs": "http://www.w3.org/2001/XMLSchema",
             "@xmlns:xsi": "http://www.w3.org/2001/XMLSchema-instance",
-            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.6/ids.xsd",
+            "@xsi:schemaLocation": "http://standards.buildingsmart.org/IDS http://standards.buildingsmart.org/IDS/0.9.7/ids.xsd",
             "info": {"title": "Untitled"},
             "specifications": {"specification": []},
         }
 
     def test_authoring_an_ids_with_no_specifications_is_invalid(self):
         specs = ids.Ids()
         with pytest.raises(xmlschema.validators.exceptions.XMLSchemaChildrenValidationError):
@@ -113,15 +120,15 @@
         result = specs.to_xml(fn)
         os.remove(fn)
 
     def test_creating_a_minimal_ids_and_validating(self):
         specs = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
-        spec.requirements.append(name_attr := ids.Attribute(name="Name", value="Waldo"))
+        spec.requirements.append(ids.Attribute(name="Name", value="Waldo"))
         specs.specifications.append(spec)
         assert "http://standards.buildingsmart.org/IDS" in specs.to_string()
         assert spec.status == None
 
         model = ifcopenshell.file()
         wall = model.createIfcWall()
         waldo = model.createIfcWall(Name="Waldo")
@@ -131,61 +138,72 @@
 
         spec.ifcVersion = ["IFC2X3"]
         run(
             "Specification version is purely metadata and does not impact pass or fail result",
             specs,
             model,
             True,
-            [wall, waldo]
+            [wall, waldo],
         )
 
         spec.ifcVersion = []
-        spec.minOccurs = 1
+        spec.set_usage("required")
         model = ifcopenshell.file()
         waldo = model.createIfcWall(Name="Waldo")
         run("Required specifications need at least one applicable entity 1/2", specs, model, True, [waldo])
         model = ifcopenshell.file()
         waldo = model.createIfcSlab(Name="Waldo")
         run("Required specifications need at least one applicable entity 2/2", specs, model, False)
 
-        spec.minOccurs = 0
+        spec.set_usage("optional")
         model = ifcopenshell.file()
         waldo = model.createIfcSlab(Name="Waldo")
         run("Optional specifications may still pass if nothing is applicable", specs, model, True)
 
-        spec.minOccurs = 0
-        spec.maxOccurs = 0
+        spec.set_usage("prohibited")
         model = ifcopenshell.file()
         wall = model.createIfcSlab(Name="Waldo")
         run("Prohibited specifications fail if at least one entity passes all requirements 1/3", specs, model, True)
         model = ifcopenshell.file()
         wall = model.createIfcWall(Name="Wally")
-        run("Prohibited specifications fail if at least one entity passes all requirements 2/3", specs, model, False, [wall], [wall])
+        run(
+            "Prohibited specifications fail if at least one entity passes all requirements 2/3",
+            specs,
+            model,
+            True,
+            [wall],
+            [],
+        )
         model = ifcopenshell.file()
         wall = model.createIfcWall(Name="Waldo")
-        run("Prohibited specifications fail if at least one entity passes all requirements 3/3", specs, model, False, [wall])
+        run(
+            "Prohibited specifications fail if at least one entity passes all requirements 3/3",
+            specs,
+            model,
+            False,
+            [wall],
+            [wall],
+        )
 
-        spec.minOccurs = 0
-        spec.maxOccurs = "unbounded"
+        spec.set_usage("optional")
         model = ifcopenshell.file()
         wall = model.createIfcWall(Name="Waldo")
         spec.requirements.append(description_attr := ids.Attribute(name="Description", value="Foobar"))
         run("A specification passes only if all requirements pass 1/2", specs, model, False, [wall], [wall])
         wall.Description = "Foobar"
         run("A specification passes only if all requirements pass 2/2", specs, model, True, [wall])
 
         # optional attribute
         # description_attr.minOccurs = 0
         # description_attr.maxOccurs = "unbounded"
         # wall.Description = None
         # run("Specification optionality and facet optionality can be combined", specs, model, True, [wall])
 
         # double negative / required attributes
-        # spec.minOccurs = 0
-        # spec.maxOccurs = 0
+        # spec.set_usage("prohibited")
         # name_attr.minOccurs = 0
         # name_attr.maxOccurs = 0
         # description_attr.minOccurs = 0
         # description_attr.maxOccurs = 0
         # wall.Name = "Waldo"
         # wall.Description = "Foobar"
         # run("A prohibited specification and a prohibited facet results in a double negative", specs, model, True, [wall])
@@ -222,27 +240,26 @@
         model = ifcopenshell.file()
         wall = model.createIfcWall()
         waldo = model.createIfcWall(Name="Waldo")
         specs.validate(model)
 
         assert spec.status == False
         assert set(spec.applicable_entities) == {wall, waldo}
-        assert spec.requirements[0].failed_entities == [wall]
-        assert spec2.requirements[0].failed_entities == [wall]
+        assert len(spec.requirements[0].failures) == 1
+        assert len(spec2.requirements[0].failures) == 1
+        assert spec.requirements[0].failures[0]["element"] == wall
+        assert spec2.requirements[0].failures[0]["element"] == wall
 
 
 class TestSpecification:
     def test_create_specification_with_minimal_information(self):
         spec = ids.Specification()
-        print(spec.asdict())
         assert spec.asdict() == {
             "@name": "Unnamed",
             "@ifcVersion": ["IFC2X3", "IFC4"],
-            "@minOccurs": 0,
-            "@maxOccurs": "unbounded",
             "applicability": {},
             "requirements": {},
         }
 
     def test_create_specification_with_all_possible_information(self):
         spec = ids.Specification(
             name="name",
@@ -251,56 +268,106 @@
             ifcVersion="IFC4",
             identifier="identifier",
             description="description",
             instructions="instructions",
         )
         assert spec.asdict() == {
             "@name": "name",
-            "@minOccurs": 1,
-            "@maxOccurs": 1,
             "@ifcVersion": "IFC4",
             "@identifier": "identifier",
             "@description": "description",
             "@instructions": "instructions",
             "applicability": {},
             "requirements": {},
         }
-    
+
     def test_specification_has_no_requirements(self):
         model = ifcopenshell.file()
         wall = model.createIfcWall()
         waldo = model.createIfcWall(Name="Waldo")
-        
+
         test_ids = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
         test_ids.specifications.append(spec)
-        spec.minOccurs = 1
-        run("A specification that is required and has at least one applicable entity but no requirements shall pass", test_ids, model, True, [wall, waldo], None)
-        
+        spec.set_usage("required")
+        run(
+            "A specification that is required and has at least one applicable entity but no requirements shall pass",
+            test_ids,
+            model,
+            True,
+            [wall, waldo],
+            None,
+        )
+
         test_ids = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         test_ids.specifications.append(spec)
-        spec.minOccurs = 1
-        run("A specification that is required but has no applicable entities or requirements shall fail", test_ids, model, False, None, None)
-        
+        spec.set_usage("required")
+        run(
+            "A specification that is required but has no applicable entities or requirements shall fail",
+            test_ids,
+            model,
+            False,
+            None,
+            None,
+        )
+
         test_ids = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
         test_ids.specifications.append(spec)
-        spec.minOccurs = 0
-        run("A specification that is optional and has at least one applicable entity but no requirements shall pass", test_ids, model, True, [wall, waldo], None)
-        
+        spec.set_usage("optional")
+        run(
+            "A specification that is optional and has at least one applicable entity but no requirements shall pass",
+            test_ids,
+            model,
+            True,
+            [wall, waldo],
+            None,
+        )
+
         test_ids = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         spec.applicability.append(ids.Entity(name="IFCWALL"))
         test_ids.specifications.append(spec)
-        spec.minOccurs = 0
-        spec.maxOccurs = 0
-        run("A specification that is prohibited and has at least one applicable entity but no requirements shall fail", test_ids, model, False, [wall, waldo], None)
-        
+        spec.set_usage("prohibited")
+        run(
+            "A specification that is prohibited and has at least one applicable entity but no requirements shall fail",
+            test_ids,
+            model,
+            False,
+            [wall, waldo],
+            None,
+        )
+
         test_ids = ids.Ids(title="Title")
         spec = ids.Specification(name="Name")
         test_ids.specifications.append(spec)
-        spec.minOccurs = 0
-        spec.maxOccurs = 0
-        run("A specification that is prohibited but has no applicable entities or requirements shall pass", test_ids, model, True, None, None)
+        spec.set_usage("prohibited")
+        run(
+            "A specification that is prohibited but has no applicable entities or requirements shall pass",
+            test_ids,
+            model,
+            True,
+            None,
+            None,
+        )
+
+    def test_prohibited_facet(self):
+        specs = ids.Ids(title="Title")
+        spec = ids.Specification(name="Name")
+        spec.applicability.append(ids.Entity(name="IFCWALL"))
+        spec.requirements.append(ids.Attribute(name="Name", value="Waldo", cardinality="prohibited"))
+        specs.specifications.append(spec)
+
+        spec.set_usage("required")
+        model = ifcopenshell.file()
+        wall = model.createIfcWall(Name="Wally")
+        run(
+            "Prohibited facet not to fail if no entity passes it",
+            specs,
+            model,
+            True,
+            [wall],
+            [],
+        )
```

