# Comparing `tmp/polars_ts-0.0.4.tar.gz` & `tmp/polars_ts-0.0.5.tar.gz`

## Comparing `polars_ts-0.0.4.tar` & `polars_ts-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,51 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.4/Cargo.toml
--rw-r--r--   0     1001      127     3402 2024-04-15 22:12:20.000000 polars_ts-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127     3107 2024-04-15 22:12:20.000000 polars_ts-0.0.4/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-15 22:12:20.000000 polars_ts-0.0.4/.python-version
--rw-r--r--   0     1001      127      147 2024-04-15 22:12:20.000000 polars_ts-0.0.4/.vscode/settings.json
--rw-r--r--   0     1001      127    11357 2024-04-15 22:12:20.000000 polars_ts-0.0.4/LICENSE
--rw-r--r--   0     1001      127      704 2024-04-15 22:12:20.000000 polars_ts-0.0.4/Makefile
--rw-r--r--   0     1001      127     1002 2024-04-15 22:12:20.000000 polars_ts-0.0.4/README.md
--rw-r--r--   0     1001      127      933 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/__init__.py
--rw-r--r--   0     1001      127     2918 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/calendar.py
--rw-r--r--   0     1001      127      638 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/display.py
--rw-r--r--   0     1001      127     3853 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/dummy.py
--rw-r--r--   0     1001      127     2089 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/dummymkt.py
--rw-r--r--   0     1001      127        0 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/expr/__init__.py
--rw-r--r--   0     1001      127     1580 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/expr/random.py
--rw-r--r--   0     1001      127     2852 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures.py
--rw-r--r--   0     1001      127        0 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures_helper/__init__.py
--rw-r--r--   0     1001      127      850 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures_helper/bbg_symbols.py
--rw-r--r--   0     1001      127     1135 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures_helper/generic_symbols.py
--rw-r--r--   0     1001      127     7757 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures_helper/roll_calendar.py
--rw-r--r--   0     1001      127      890 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/futures_helper/util.py
--rw-r--r--   0     1001      127      483 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/helpers.py
--rw-r--r--   0     1001      127      437 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/loader.py
--rw-r--r--   0     1001      127      930 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/resample.py
--rw-r--r--   0     1001      127     2168 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/sf.py
--rw-r--r--   0     1001      127     1211 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/time.py
--rw-r--r--   0     1001      127      324 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/tsf.py
--rw-r--r--   0     1001      127     1289 2024-04-15 22:12:20.000000 polars_ts-0.0.4/polars_ts/utils.py
--rw-r--r--   0     1001      127       32 2024-04-15 22:12:20.000000 polars_ts-0.0.4/requirements.txt
--rw-r--r--   0     1001      127      445 2024-04-15 22:12:20.000000 polars_ts-0.0.4/ruff.toml
--rw-r--r--   0     1001      127      212 2024-04-15 22:12:20.000000 polars_ts-0.0.4/run.py
--rw-r--r--   0     1001      127     2617 2024-04-15 22:12:20.000000 polars_ts-0.0.4/src/expressions.rs
--rw-r--r--   0     1001      127      382 2024-04-15 22:12:20.000000 polars_ts-0.0.4/src/lib.rs
--rw-r--r--   0     1001      127     1839 2024-04-15 22:12:20.000000 polars_ts-0.0.4/src/math/mod.rs
--rw-r--r--   0     1001      127     2712 2024-04-15 22:12:20.000000 polars_ts-0.0.4/src/utils.rs
--rw-r--r--   0     1001      127       27 2024-04-15 22:12:20.000000 polars_ts-0.0.4/tests/sf/test_sf.py
--rw-r--r--   0     1001      127      846 2024-04-15 22:12:20.000000 polars_ts-0.0.4/tests/test_rust_templates.py
--rw-r--r--   0     1001      127    36490 2024-04-15 22:12:20.000000 polars_ts-0.0.4/Cargo.lock
--rw-r--r--   0     1001      127      478 2024-04-15 22:12:20.000000 polars_ts-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      127     3402 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127     3107 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.python-version
+-rw-r--r--   0     1001      127      147 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.vscode/settings.json
+-rw-r--r--   0     1001      127    11357 2024-04-17 22:55:56.000000 polars_ts-0.0.5/LICENSE
+-rw-r--r--   0     1001      127      704 2024-04-17 22:55:56.000000 polars_ts-0.0.5/Makefile
+-rw-r--r--   0     1001      127     1002 2024-04-17 22:55:56.000000 polars_ts-0.0.5/README.md
+-rw-r--r--   0     1001      127      933 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/__init__.py
+-rw-r--r--   0     1001      127     1637 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/calendar.py
+-rw-r--r--   0     1001      127     2537 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/calendar_helper/__init__.py
+-rw-r--r--   0     1001      127      673 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/display.py
+-rw-r--r--   0     1001      127     2540 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummy.py
+-rw-r--r--   0     1001      127     2851 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummy_helper/__init__.py
+-rw-r--r--   0     1001      127     1178 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummymkt.py
+-rw-r--r--   0     1001      127     1633 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummymkt_helper/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/expr/__init__.py
+-rw-r--r--   0     1001      127     1580 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/expr/random.py
+-rw-r--r--   0     1001      127     1213 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures.py
+-rw-r--r--   0     1001      127     2307 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/__init__.py
+-rw-r--r--   0     1001      127      850 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/bbg_symbols.py
+-rw-r--r--   0     1001      127     1135 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/generic_symbols.py
+-rw-r--r--   0     1001      127     7751 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/roll_calendar.py
+-rw-r--r--   0     1001      127      890 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/util.py
+-rw-r--r--   0     1001      127     4810 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/grouper.py
+-rw-r--r--   0     1001      127      510 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/loader.py
+-rw-r--r--   0     1001      127     2317 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/resample.py
+-rw-r--r--   0     1001      127     3475 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/resample_helper/__init__.py
+-rw-r--r--   0     1001      127      876 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/sf.py
+-rw-r--r--   0     1001      127      539 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/sf_helper/__init__.py
+-rw-r--r--   0     1001      127      684 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/time.py
+-rw-r--r--   0     1001      127      937 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/time_helper/__init__.py
+-rw-r--r--   0     1001      127      397 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/tsf.py
+-rw-r--r--   0     1001      127      397 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/types.py
+-rw-r--r--   0     1001      127     1289 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/utils.py
+-rw-r--r--   0     1001      127       32 2024-04-17 22:55:56.000000 polars_ts-0.0.5/requirements.txt
+-rw-r--r--   0     1001      127      445 2024-04-17 22:55:56.000000 polars_ts-0.0.5/ruff.toml
+-rw-r--r--   0     1001      127      212 2024-04-17 22:55:56.000000 polars_ts-0.0.5/run.py
+-rw-r--r--   0     1001      127     2617 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/expressions.rs
+-rw-r--r--   0     1001      127      382 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      127     1839 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/math/mod.rs
+-rw-r--r--   0     1001      127     2712 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/utils.rs
+-rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/grouper/__init__.py
+-rw-r--r--   0     1001      127     2685 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/grouper/test_grouper.py
+-rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/resample/__init__.py
+-rw-r--r--   0     1001      127    10278 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/resample/test_resample.py
+-rw-r--r--   0     1001      127       27 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/sf/test_sf.py
+-rw-r--r--   0     1001      127      846 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/test_rust_templates.py
+-rw-r--r--   0     1001      127    36490 2024-04-17 22:55:56.000000 polars_ts-0.0.5/Cargo.lock
+-rw-r--r--   0     1001      127      478 2024-04-17 22:55:56.000000 polars_ts-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.5/PKG-INFO
```

### Comparing `polars_ts-0.0.4/Cargo.toml` & `polars_ts-0.0.5/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "polars-ts"
-version = "0.0.4"
+version = "0.0.5"
 edition = "2021"
 
 [lib]
 name = "polars_ts"
 crate-type= ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.21.1", features = ["extension-module", "abi3-py38"] }
+pyo3 = { version = "0.21.2", features = ["extension-module", "abi3-py38"] }
 pyo3-polars = { version = "0.13.0", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
-polars = { version = "0.39.1", default-features = false }
+polars = { version = "0.39.2", default-features = false }
 rand = "0.8.5"
 rand_distr = "0.4.3"
 wyhash = "0.5.0"
 
 [target.'cfg(target_os = "linux")'.dependencies]
 jemallocator = { version = "0.5", features = ["disable_initial_exec_tls"] }
```

### Comparing `polars_ts-0.0.4/.github/workflows/publish_to_pypi.yml` & `polars_ts-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/.gitignore` & `polars_ts-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/LICENSE` & `polars_ts-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/Makefile` & `polars_ts-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/README.md` & `polars_ts-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/__init__.py` & `polars_ts-0.0.5/polars_ts/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/calendar.py` & `polars_ts-0.0.5/polars_ts/calendar_helper/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,96 @@
-from typing import Optional
+from typing import Dict, Union
 
 import polars as pl
-from polars.type_aliases import IntoExpr
 
-from .sf import SeriesFrame
-from .futures_helper.util import month_to_imm_dict
-from .utils import parse_into_expr
-
-
-__NAMESPACE = "calendar"
-
-
-@pl.api.register_lazyframe_namespace(__NAMESPACE)
-class CalendarFrame(SeriesFrame):
-    def __init__(self, df: pl.LazyFrame):
-        super().__init__(df)
-
-    def date_to_imm_contract(
-        self,
-        col_name: IntoExpr,
-        prefix: IntoExpr = pl.lit(""),
-        suffix: IntoExpr = pl.lit(""),
-        out: Optional[str] = None,
-    ) -> pl.LazyFrame:
-        col_expr = parse_into_expr(col_name)
-        prefix = parse_into_expr(prefix)
-        suffix = parse_into_expr(suffix)
-        out = col_expr.meta.output_name() if out is None else out
-
-        imm_dict = month_to_imm_dict()
-        self._df = self._df.with_columns(
-            pl.when(col_expr.is_null())
-            .then(pl.lit(None).cast(pl.String))
-            .otherwise(
-                pl.concat_str(
-                    [
-                        prefix,
-                        pl.struct(
-                            col_expr.dt.month().alias("month"),
-                            col_expr.dt.strftime("%y").alias("year"),
-                        ).map_elements(
-                            lambda se: f"""{imm_dict.get(se['month'], "@@")}{se['year']}""",
-                            return_dtype=pl.String,
-                        ),
-                        suffix,
-                    ]
-                )
-            )
-            .cast(pl.Categorical)
-            .alias(out)
-        )
+from ..types import FrameType
 
-        return self.result_df
 
-    def imm_contract_to_date(self, col_name: str, default_day: int = 1) -> pl.LazyFrame:
-        imm_dict = month_to_imm_dict(invert=True)
-        self._df = self._df.with_columns(
-            pl.col(col_name)
-            .str.extract_groups(".*(?<imm>[F-Z])(?<year>[0-9]{2})")
-            .map_elements(
-                lambda se: (
-                    f"{str(default_day).rjust(2, '0')}-{str(imm_dict[se['imm']]).rjust(2, '0')}-{se['year']}"
-                ),
-                return_dtype=pl.String,
+def impl_date_to_imm_contract(
+    df: FrameType,
+    col_name: pl.Expr,
+    prefix: pl.Expr,
+    suffix: pl.Expr,
+    out: str,
+) -> FrameType:
+    imm_dict = impl_month_to_imm_dict()
+
+    result = df.with_columns(
+        pl.when(col_name.is_null())
+        .then(pl.lit(None).cast(pl.String))
+        .otherwise(
+            pl.concat_str(
+                [
+                    prefix,
+                    pl.struct(
+                        col_name.dt.month().alias("month"),
+                        col_name.dt.strftime("%y").alias("year"),
+                    ).map_elements(
+                        lambda se: f"""{imm_dict.get(se['month'], "@@")}{se['year']}""",
+                        return_dtype=pl.String,
+                    ),
+                    suffix,
+                ]
             )
-            .str.to_date("%d-%m-%y")
         )
+        .cast(pl.Categorical)
+        .alias(out)
+    )
+
+    return result
+
+
+def impl_imm_contract_to_date(
+    df: FrameType, col_name: str, default_day: int
+) -> FrameType:
+    imm_dict = impl_month_to_imm_dict(invert=True)
+    result = df.with_columns(
+        pl.col(col_name)
+        .str.extract_groups(".*(?<imm>[F-Z])(?<year>[0-9]{2})")
+        .map_elements(
+            lambda se: (
+                f"{str(default_day).rjust(2, '0')}-{str(imm_dict[se['imm']]).rjust(2, '0')}-{se['year']}"
+            ),
+            return_dtype=pl.String,
+        )
+        .str.to_date("%d-%m-%y")
+    )
 
-        return self.result_df
+    return result
 
-    def int_to_date(self, col_name: str) -> pl.LazyFrame:
-        self._df = self._df.with_columns(
-            pl.col(col_name).cast(pl.String).str.strptime(pl.Date, "%Y%m%d")
-        )
 
-        return self.result_df
+def impl_int_to_date(df: FrameType, col_name: str) -> FrameType:
+    result = df.with_columns(
+        pl.col(col_name).cast(pl.String).str.strptime(pl.Date, "%Y%m%d")
+    )
 
-    def date_to_int(self, col_name: str, out: Optional[str] = None) -> pl.LazyFrame:
-        out = col_name if out is None else out
+    return result
 
-        self._df = self._df.with_columns(
-            (
-                (pl.col(col_name).dt.year() * 10000)
-                + (pl.col(col_name).dt.month().cast(pl.UInt16) * 100)
-                + (pl.col(col_name).dt.day())
-            )
-            .alias(out)
-            .cast(pl.UInt64)
+
+def impl_date_to_int(df: FrameType, col_name: str, out: str) -> FrameType:
+    result = df.with_columns(
+        (
+            (pl.col(col_name).dt.year() * 10000)
+            + (pl.col(col_name).dt.month().cast(pl.UInt16) * 100)
+            + (pl.col(col_name).dt.day())
+        )
+        .alias(out)
+        .cast(pl.UInt64)
+    )
+
+    return result
+
+
+def impl_month_to_imm_dict(
+    invert: bool = False,
+) -> Dict[Union[str, int], Union[str, int]]:
+    result_cols = ["month_idx", "imm_code"]
+    df = (
+        pl.DataFrame({"imm_code": "FGHJKMNQUVXZ"})
+        .select(
+            pl.col("imm_code").str.extract_all("[F-Z]").explode().cast(pl.Categorical)
         )
+        .with_row_index("month_idx", offset=1)
+        .select(reversed(result_cols) if invert else result_cols)
+    )
 
-        return self.result_df
+    return dict(df.iter_rows())
```

### Comparing `polars_ts-0.0.4/polars_ts/display.py` & `polars_ts-0.0.5/polars_ts/display.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 if len(repr_overloaded) == 0:
     oldrepr = pl.DataFrame._repr_html_
 
     def newrepr(self, **kwargs: Any) -> str:
         time_col = ["time"] if "time" in self.columns else []
         category_cols = [
-            c for c, dtype in zip(self.columns, self.dtypes) if dtype == pl.Categorical
+            c
+            for c, dtype in zip(self.columns, self.dtypes)
+            if dtype in [pl.Categorical, pl.Enum]
         ]
 
         cols = time_col + category_cols
 
         return oldrepr(
             self.select(*[pl.col(c) for c in cols], pl.exclude(cols)), **kwargs
         )
```

### Comparing `polars_ts-0.0.4/polars_ts/dummymkt.py` & `polars_ts-0.0.5/polars_ts/dummymkt_helper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 import polars as pl
-from polars.type_aliases import IntoExpr
 
-from .sf import SeriesFrame
-from .utils import parse_into_expr
+from ..types import FrameType
+from ..dummy_helper import impl_random_normal
+from ..grouper import Grouper
 
-__NAMESPACE = "dummymkt"
 
-
-@pl.api.register_lazyframe_namespace(__NAMESPACE)
-class DummyMktFrame(SeriesFrame):
-    def __init__(self, df: pl.LazyFrame):
-        super().__init__(df)
-
-    def fetch_instrument_prices(
-        self, start_dt: IntoExpr, end_dt: IntoExpr, remove_weekends: bool = True
-    ) -> pl.LazyFrame:
-        start_dt_expr = parse_into_expr(start_dt, dtype=pl.Date)
-        end_dt_expr = parse_into_expr(end_dt, dtype=pl.Date)
-        hols = [6, 7] if remove_weekends else []
-
-        df = (
-            self._df.select(
-                time=pl.date_ranges(start_dt_expr, end_dt_expr),
-                asset=pl.col("asset"),
-                instrument_id=pl.col("instrument_id"),
-            )
-            .explode(pl.col("time"))
-            .dummy.random_normal()  # type: ignore[attr-defined]
-            .filter(pl.col("time").dt.weekday().is_in(hols).not_())
-            .with_columns(pl.col("value").cum_sum().over("asset", "instrument_id"))
+def impl_fetch_instrument_prices(
+    df: FrameType, start_dt: pl.Expr, end_dt: pl.Expr, remove_weekends: bool
+) -> FrameType:
+    hols = [6, 7] if remove_weekends else []
+
+    result = (
+        df.select(
+            time=pl.date_ranges(start_dt, end_dt),
+            asset=pl.col("asset"),
+            instrument_id=pl.col("instrument_id"),
         )
-
-        return df
-
-    def fetch_roll_calendar_prices(
-        self, roll_calendar: pl.LazyFrame, instrument_prices: pl.LazyFrame
-    ) -> pl.LazyFrame:
-        prices = instrument_prices.rename({"time": "roll_date"})
-
-        df = (
-            roll_calendar.join(
-                prices.rename(
-                    {"instrument_id": "near_contract", "value": "near_price"}
-                ),
-                on=["roll_date", "asset", "near_contract"],
-                how="left",
-            )
-            .join(
-                prices.rename({"instrument_id": "far_contract", "value": "far_price"}),
-                on=["roll_date", "asset", "far_contract"],
-                how="left",
-            )
-            .join(
-                prices.rename(
-                    {"instrument_id": "carry_contract", "value": "carry_price"}
-                ),
-                on=["roll_date", "asset", "carry_contract"],
-                how="left",
+        .explode(pl.col("time"))
+        .pipe(
+            lambda df: impl_random_normal(
+                df, partition=Grouper(), out="value", mu=0.0, sigma=1.0
             )
         )
+        .filter(pl.col("time").dt.weekday().is_in(hols).not_())
+        .with_columns(pl.col("value").cum_sum().over("asset", "instrument_id"))
+    )
+
+    return result
+
+
+def impl_fetch_roll_calendar_prices(
+    roll_calendar: FrameType, instrument_prices: FrameType
+) -> FrameType:
+    prices = instrument_prices.rename({"time": "roll_date"})
+
+    df = (
+        roll_calendar.join(
+            prices.rename({"instrument_id": "near_contract", "value": "near_price"}),
+            on=["roll_date", "asset", "near_contract"],
+            how="left",
+        )
+        .join(
+            prices.rename({"instrument_id": "far_contract", "value": "far_price"}),
+            on=["roll_date", "asset", "far_contract"],
+            how="left",
+        )
+        .join(
+            prices.rename({"instrument_id": "carry_contract", "value": "carry_price"}),
+            on=["roll_date", "asset", "carry_contract"],
+            how="left",
+        )
+    )
 
-        return df
+    return df
```

### Comparing `polars_ts-0.0.4/polars_ts/expr/random.py` & `polars_ts-0.0.5/polars_ts/expr/random.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/futures.py` & `polars_ts-0.0.5/polars_ts/futures_helper/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 import polars as pl
 
-from .sf import SeriesFrame
-from .futures_helper.roll_calendar import create_roll_calendar_helper
+from ..types import FrameType
+from .roll_calendar import create_roll_calendar_helper
 
-__NAMESPACE = "future"
 
-
-@pl.api.register_lazyframe_namespace(__NAMESPACE)
-class FuturesFrame(SeriesFrame):
-    def __init__(self, df: pl.LazyFrame) -> None:
-        super().__init__(df)
-
-    def create_roll_calendar(
-        self,
-        roll_config: pl.LazyFrame,
-        security_expiries: pl.LazyFrame,
-        include_debug: bool = False,
-    ) -> pl.LazyFrame:
-        self._df = create_roll_calendar_helper(
-            roll_config, security_expiries, include_debug
-        )
-
-        return self.result_df
-
-    def prepare_unadjusted_for_stitching(
-        self,
-        roll_calendar: pl.LazyFrame,
-        price_universe: pl.LazyFrame,
-    ) -> pl.LazyFrame:
-        far_contract_prices = (
-            pl.LazyFrame()
-            .dummymkt.fetch_roll_calendar_prices(roll_calendar, price_universe)  # type: ignore[attr-defined]
-            .select(
-                "asset",
-                time="roll_date",
-                instrument_id="near_contract",
-                next_instrument_id="far_contract",
-                next_value="far_price",
-            )
+def impl_create_roll_calendar(
+    roll_config: FrameType,
+    security_expiries: FrameType,
+    include_debug: bool = False,
+) -> FrameType:
+    result = create_roll_calendar_helper(roll_config, security_expiries, include_debug)
+
+    return result
+
+
+def impl_prepare_unadjusted_for_stitching(
+    df: FrameType,
+    roll_calendar: FrameType,
+    price_universe: FrameType,
+) -> FrameType:
+    far_contract_prices = (
+        df.select()
+        .dummymkt.fetch_roll_calendar_prices(roll_calendar, price_universe)  # type: ignore[attr-defined]
+        .select(
+            "asset",
+            time="roll_date",
+            instrument_id="near_contract",
+            next_instrument_id="far_contract",
+            next_value="far_price",
         )
+    )
 
-        self._df = (
-            roll_calendar.select(
-                "asset",
-                instrument_id="near_contract",
-                instrument_start_date=pl.col("roll_date")
-                .shift(1, fill_value=pl.min("roll_date").dt.offset_by("-5y"))
-                .over("asset"),
-                instrument_end_date="roll_date",
-            )
-            .join(price_universe, on=["asset", "instrument_id"], how="left")
-            .join(
-                far_contract_prices, on=["time", "asset", "instrument_id"], how="left"
-            )
-            .filter(
-                pl.col("time")
-                .is_between("instrument_start_date", "instrument_end_date", "right")
-                .over("instrument_id")
-            )
-            .select(pl.exclude("instrument_start_date", "instrument_end_date"))
+    result = (
+        roll_calendar.select(
+            "asset",
+            instrument_id="near_contract",
+            instrument_start_date=pl.col("roll_date")
+            .shift(1, fill_value=pl.min("roll_date").dt.offset_by("-5y"))
+            .over("asset"),
+            instrument_end_date="roll_date",
+        )
+        .join(price_universe, on=["asset", "instrument_id"], how="left")
+        .join(far_contract_prices, on=["time", "asset", "instrument_id"], how="left")
+        .filter(
+            pl.col("time")
+            .is_between("instrument_start_date", "instrument_end_date", "right")
+            .over("instrument_id")
         )
+        .select(pl.exclude("instrument_start_date", "instrument_end_date"))
+    )
 
-        return self._df
+    return result
 
-    def stitch_panama_backwards(self) -> pl.LazyFrame:
-        self._df = (
-            self._df.with_columns(
-                roll_adj=(
-                    pl.when(pl.col("next_value").is_not_null())
-                    .then(pl.col("next_value") - pl.col("value"))
-                    .otherwise(0.0)
-                )
-            )
-            .with_columns(
-                cum_adj=(pl.col("roll_adj").reverse().cum_sum().reverse().over("asset"))
-            )
-            .with_columns(adj=pl.col("value") + pl.col("cum_adj"))
-            # cleanup
-            .select(
-                "time",
-                "asset",
-                "instrument_id",
-                unadjusted="value",
-                panama_backwards="adj",
+
+def impl_stitch_panama_backwards(df: FrameType) -> FrameType:
+    result = (
+        df.with_columns(
+            roll_adj=(
+                pl.when(pl.col("next_value").is_not_null())
+                .then(pl.col("next_value") - pl.col("value"))
+                .otherwise(0.0)
             )
         )
+        .with_columns(
+            cum_adj=(pl.col("roll_adj").reverse().cum_sum().reverse().over("asset"))
+        )
+        .with_columns(adj=pl.col("value") + pl.col("cum_adj"))
+        # cleanup
+        .select(
+            "time",
+            "asset",
+            "instrument_id",
+            unadjusted="value",
+            panama_backwards="adj",
+        )
+    )
 
-        return self.result_df
+    return result
```

### Comparing `polars_ts-0.0.4/polars_ts/futures_helper/bbg_symbols.py` & `polars_ts-0.0.5/polars_ts/futures_helper/bbg_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/futures_helper/generic_symbols.py` & `polars_ts-0.0.5/polars_ts/futures_helper/generic_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/futures_helper/roll_calendar.py` & `polars_ts-0.0.5/polars_ts/futures_helper/roll_calendar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import polars as pl
 
 from .util import month_to_imm_dict, make_generic_contract
+from ..types import FrameType
 
 
 def guess_security_meta(
-    generic_contracts: pl.LazyFrame, roll_config: pl.LazyFrame
-) -> pl.LazyFrame:
+    generic_contracts: FrameType, roll_config: FrameType
+) -> FrameType:
     df = (
         roll_config.join(generic_contracts, on="asset")
         .filter(
             pl.col("priced_roll_cycle").str.contains(
                 pl.col("instrument_id").struct.field("tenor").cast(pl.String)
             )
         )
@@ -46,15 +47,15 @@
         ),
         (expiry_date.dt.offset_by(min_trade_days)),
     )
 
     return first_trade_dt
 
 
-def asset_carry_contracts(roll_config: pl.LazyFrame) -> pl.LazyFrame:
+def asset_carry_contracts(roll_config: FrameType) -> FrameType:
     def _find_carry_month(hc: dict):
         allowed_contracts = hc["priced_roll_cycle"]
         current_contract = hc["hold_roll_cycle"]
         carry_offset = hc["carry_contract_offset"]
 
         idx = allowed_contracts.find(current_contract)
         carry_idx = (idx + carry_offset) % len(allowed_contracts)
@@ -104,15 +105,15 @@
                 )
             )
         )
         .select("asset", "hold_month", "carry_month_offset")
     )
 
 
-def asset_near_far_contracts(roll_config: pl.LazyFrame) -> pl.LazyFrame:
+def asset_near_far_contracts(roll_config: FrameType) -> FrameType:
     return (
         roll_config.select(
             "asset",
             hold_near=pl.col("hold_roll_cycle")
             .cast(pl.String)
             .str.extract_all("[F-Z]"),
             hold_far=pl.concat_str(
@@ -141,15 +142,15 @@
                     pl.lit("mo"),
                 ]
             )
         )
     )
 
 
-def asset_contracts(roll_config: pl.LazyFrame) -> pl.LazyFrame:
+def asset_contracts(roll_config: FrameType) -> FrameType:
     return (
         asset_near_far_contracts(roll_config)
         .join(
             asset_carry_contracts(roll_config),
             left_on=[pl.col("asset"), pl.col("hold_near_month")],
             right_on=[pl.col("asset"), pl.col("hold_month")],
             how="left",
@@ -157,16 +158,16 @@
         .select(
             "asset", "hold_near_month", "hold_far_month_offset", "carry_month_offset"
         )
     )
 
 
 def create_roll_calendar_helper(
-    roll_config: pl.LazyFrame, security_dates: pl.LazyFrame, include_debug: bool
-) -> pl.LazyFrame:
+    roll_config: FrameType, security_dates: FrameType, include_debug: bool
+) -> FrameType:
     result_schema = [
         "roll_date",
         "asset",
         "near_contract",
         "far_contract",
         "carry_contract",
     ]
```

### Comparing `polars_ts-0.0.4/polars_ts/futures_helper/util.py` & `polars_ts-0.0.5/polars_ts/futures_helper/util.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/polars_ts/utils.py` & `polars_ts-0.0.5/polars_ts/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/src/expressions.rs` & `polars_ts-0.0.5/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/src/math/mod.rs` & `polars_ts-0.0.5/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/src/utils.rs` & `polars_ts-0.0.5/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/tests/test_rust_templates.py` & `polars_ts-0.0.5/tests/test_rust_templates.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.4/Cargo.lock` & `polars_ts-0.0.5/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -449,32 +449,32 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c352aaa0399c0863eecd879f2cbe585c9026c5cafe432f029025e4bec3adf43"
+checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-parquet",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f88d3cfc6b500f106f03a5f4d37f700deef38c5b58a2e843edb3ec31f5a0ec19"
+checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
 dependencies = [
  "ahash",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
@@ -504,33 +504,33 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf264bfb632aaeba859fe19a87fa051d850e72542c36177ccea71fd9cae84079"
+checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
 dependencies = [
  "bytemuck",
  "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85cb72917958e82f29d604429ab55851f561c7cd336f7744a7360f9e50b9ac88"
+checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
  "bitflags 2.5.0",
  "bytemuck",
  "either",
  "hashbrown",
  "indexmap",
@@ -548,17 +548,17 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c18ef81979a6d9e9fdbd25ad3bf1591cbd5c474489f785af44604cf591cd636d"
+checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
  "polars-arrow-format",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
@@ -617,17 +617,17 @@
  "regex",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cd1f445fea8377350dfa2bd216785839ce97c826299c7e0e9557c1dbe887f"
+checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
 dependencies = [
  "ahash",
  "base64",
  "ethnum",
  "num-traits",
  "parquet-format-safe",
  "polars-arrow",
@@ -659,43 +659,43 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "695a9954f5aa273e44c497c19f806177f787ccf87cd4b3044c96a5057266a861"
+checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
 dependencies = [
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-ts"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
  "jemallocator",
  "polars",
  "pyo3",
  "pyo3-polars",
  "rand",
  "rand_distr",
  "serde",
  "wyhash",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.39.1"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "355b126757b4a87da5248ae6eb644e99b5583a11ffc2d42e13b2b856d43e84be"
+checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
@@ -735,17 +735,17 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -753,49 +753,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.53",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.53",
 ]
```

### Comparing `polars_ts-0.0.4/PKG-INFO` & `polars_ts-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ts
-Version: 0.0.4
+Version: 0.0.5
 Requires-Dist: polars >=0.20.21
 Requires-Dist: polars-xdt
 Requires-Dist: hvplot
 Requires-Dist: pyarrow
 Requires-Dist: hvplot ; extra == 'dev'
 Requires-Dist: pyarrow ; extra == 'dev'
 Provides-Extra: dev
```

