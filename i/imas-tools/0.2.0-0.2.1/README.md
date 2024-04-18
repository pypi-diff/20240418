# Comparing `tmp/imas_tools-0.2.0.tar.gz` & `tmp/imas_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.2.0.tar", max compression
+gzip compressed data, was "imas_tools-0.2.1.tar", max compression
```

## Comparing `imas_tools-0.2.0.tar` & `imas_tools-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.2.0/imas_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.2.0/imas_tools/portal/__init__.py
--rw-r--r--   0        0        0     4499 2024-04-16 16:33:35.339011 imas_tools-0.2.0/imas_tools/portal/calendar.py
--rw-r--r--   0        0        0     1787 2024-04-16 16:32:38.339304 imas_tools-0.2.0/imas_tools/portal/interfaces.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.2.0/imas_tools/recochoku.py
--rw-r--r--   0        0        0      465 2024-04-16 16:46:12.955123 imas_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.2.0/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.2.1/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.2.1/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4808 2024-04-18 15:59:32.758162 imas_tools-0.2.1/imas_tools/portal/calendar.py
+-rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.2.1/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.2.1/imas_tools/recochoku.py
+-rw-r--r--   0        0        0      465 2024-04-18 16:00:34.600457 imas_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.2.1/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.2.1/PKG-INFO
```

### Comparing `imas_tools-0.2.0/imas_tools/portal/calendar.py` & `imas_tools-0.2.1/imas_tools/portal/calendar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 from typing_extensions import Never
 import requests, json, time, pytz
 from calendar import monthrange
 from datetime import datetime, timedelta
-from .interfaces import BRAND_CODE, SUBCATEGORY_CODE, CalendarResponse
+from .interfaces import (
+    BRAND_CODE,
+    SUBCATEGORY_CODE,
+    CalendarResponse,
+    validate_subcategory_code,
+    validate_brand_code,
+)
+
+
+def validate_brands_and_catogories(
+    brands: list[BRAND_CODE], subcategories: list[SUBCATEGORY_CODE]
+):
+    for brand in brands:
+        validate_brand_code(brand)
+    for subcategory in subcategories:
+        validate_subcategory_code(subcategory)
+
 
 def fetch_news_for_today():
     return NotImplemented
 
 
 def fetch_articles_for_today(
     brands: list[BRAND_CODE] = [],
     subcategories: list[SUBCATEGORY_CODE] = [],
 ):
+    validate_brands_and_catogories(brands, subcategories)
     japan_timezone = pytz.timezone("Asia/Tokyo")
     now_in_japan = datetime.now(japan_timezone)
 
     midnight_today = japan_timezone.localize(
         datetime(now_in_japan.year, now_in_japan.month, now_in_japan.day, 0, 0, 0)
     )
     midnight_tomorrow = midnight_today + timedelta(days=1)
@@ -29,33 +46,29 @@
 
 def fetch_articles_for_month(
     year: int = 0,
     month: int = 0,
     brands: list[BRAND_CODE] = [],
     subcategories: list[SUBCATEGORY_CODE] = [],
 ):
-    # 设置日本时区
+    validate_brands_and_catogories(brands, subcategories)
     japan_timezone = pytz.timezone("Asia/Tokyo")
 
     if year == 0:
         year = datetime.now(japan_timezone).year
 
     if month == 0:
         month = datetime.now(japan_timezone).month
 
-    # 计算本月第一天和最后一天
-    first_day_this_month = japan_timezone.localize(
-        datetime(year, month, 1, 0, 0, 0)
-    )
+    first_day_this_month = japan_timezone.localize(datetime(year, month, 1, 0, 0, 0))
     last_day = monthrange(year, month)[1]
     last_day_this_month = japan_timezone.localize(
         datetime(year, month, last_day, 0, 0, 0)
     )
 
-    # 计算下月的第一天（即本月最后一天的24点）
     first_day_next_month = last_day_this_month + timedelta(days=1)
 
     return _fetch_articles(
         first_day_this_month,
         first_day_next_month,
         brands,
         subcategories,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `imas_tools-0.2.0/imas_tools/portal/interfaces.py` & `imas_tools-0.2.1/imas_tools/portal/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Any, Literal
+from typing import List, Optional, Any, Literal, get_args, Type
 from typing_extensions import TypedDict
 
 BRAND_CODE = Literal[
     "IDOLMASTER", "CINDERELLAGIRLS", "MILLIONLIVE", "SIDEM", "SHINYCOLORS", "GAKUEN", "OTHER"
 ]
 
 SUBCATEGORY_CODE = Literal[
@@ -15,14 +15,35 @@
     "OTHER",
     "DVD-BD",
     "BOOK",
     "CD",
     "COLLABO-CAMP",
 ]
 
+class InvalidBrandCode(ValueError):
+    pass
+
+
+class InvalidSubcategoryCode(ValueError):
+    pass
+
+
+def validate_brand_code(value: str):
+    if is_literal_str(value, BRAND_CODE):
+        return
+    raise InvalidBrandCode(f"Invalid brand code: {value}")
+
+def validate_subcategory_code(value: str):
+    if is_literal_str(value, SUBCATEGORY_CODE):
+        return
+    raise InvalidSubcategoryCode(f"Invalid subcategory code: {value}")
+
+def is_literal_str(value: str, typ) -> bool:
+    return isinstance(value, str) and value in get_args(typ)
+
 
 class Brand(TypedDict):
     name: str
     code: BRAND_CODE
 
 
 class Subcategory(TypedDict):
```

### Comparing `imas_tools-0.2.0/imas_tools/recochoku.py` & `imas_tools-0.2.1/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.2.0/PKG-INFO` & `imas_tools-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

