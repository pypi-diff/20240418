# Comparing `tmp/beancount_black-1.0.0.tar.gz` & `tmp/beancount_black-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_black-1.0.0.tar", max compression
+gzip compressed data, was "beancount_black-1.0.1.tar", max compression
```

## Comparing `beancount_black-1.0.0.tar` & `beancount_black-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-03-17 02:18:42.683791 beancount_black-1.0.0/LICENSE
--rw-r--r--   0        0        0     4247 2024-03-17 02:18:42.683791 beancount_black-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-03-17 02:18:42.683791 beancount_black-1.0.0/beancount_black/__init__.py
--rw-r--r--   0        0        0    26728 2024-03-17 02:18:42.683791 beancount_black-1.0.0/beancount_black/formatter.py
--rw-r--r--   0        0        0     3208 2024-03-17 02:18:42.683791 beancount_black-1.0.0/beancount_black/main.py
--rw-r--r--   0        0        0      629 2024-03-17 02:18:42.683791 beancount_black-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 beancount_black-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 08:12:10.851392 beancount_black-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4247 2024-04-18 08:12:10.851392 beancount_black-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/__init__.py
+-rw-r--r--   0        0        0    27221 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/formatter.py
+-rw-r--r--   0        0        0     3208 2024-04-18 08:12:10.851392 beancount_black-1.0.1/beancount_black/main.py
+-rw-r--r--   0        0        0      629 2024-04-18 08:12:10.855392 beancount_black-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 beancount_black-1.0.1/PKG-INFO
```

### Comparing `beancount_black-1.0.0/LICENSE` & `beancount_black-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.0/README.md` & `beancount_black-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.0/beancount_black/formatter.py` & `beancount_black-1.0.1/beancount_black/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,25 @@
 
     def get_amount_columns(self, tree: Tree) -> typing.List[str]:
         if tree.data != "amount":
             raise ValueError("Expected a amount")
         number, currency = tree.children
         return [self.format_number_expr(number), currency.value]
 
+    def get_amount_tolerance_columns(self, tree: Tree) -> typing.List[str]:
+        if tree.data != "amount_tolerance":
+            raise ValueError("Expected a amount")
+        number, tolerance, currency = tree.children
+        return [
+            self.format_number_expr(number),
+            "~",
+            self.format_number_expr(tolerance),
+            currency.value,
+        ]
+
     def format_price(self, tree: Tree) -> str:
         if tree.data not in {"per_unit_price", "total_price"}:
             raise ValueError("Expected a per_unit_price or total_price")
         amount = tree.children[0]
         amount_value = " ".join(self.get_amount_columns(amount))
         if tree.data == "per_unit_price":
             prefix = "@"
@@ -350,14 +361,16 @@
             # TODO: some token may need reformat?
             return [child.value]
         tree: Tree = child
         if tree.data == "currencies":
             return [",".join(currency.value for currency in tree.children)]
         elif tree.data == "amount":
             return self.get_amount_columns(tree)
+        elif tree.data == "amount_tolerance":
+            return self.get_amount_tolerance_columns(tree)
         elif tree.data == "number_expr":
             return [self.format_number_expr(tree)]
         raise ValueError(f"Unknown tree type {tree.data}")
 
     def format_metadata_item_value(
         self, tree_or_token: typing.Union[Tree, Token]
     ) -> str:
```

### Comparing `beancount_black-1.0.0/beancount_black/main.py` & `beancount_black-1.0.1/beancount_black/main.py`

 * *Files identical despite different names*

### Comparing `beancount_black-1.0.0/pyproject.toml` & `beancount_black-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-black"
-version = "1.0.0"
+version = "1.0.1"
 description = "Opinioned code formatter, just like Python's black code formatter but for Beancount"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-black"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `beancount_black-1.0.0/PKG-INFO` & `beancount_black-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-black
-Version: 1.0.0
+Version: 1.0.1
 Summary: Opinioned code formatter, just like Python's black code formatter but for Beancount
 Home-page: https://github.com/LaunchPlatform/beancount-black
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beancount-black Version: 1.0.0 Summary: Opinioned
+Metadata-Version: 2.1 Name: beancount-black Version: 1.0.1 Summary: Opinioned
 code formatter, just like Python's black code formatter but for Beancount Home-
 page: https://github.com/LaunchPlatform/beancount-black License: MIT Author:
 Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beancount-parser
```

