# Comparing `tmp/polars_qt-0.1.6.tar.gz` & `tmp/polars_qt-0.1.7.tar.gz`

## Comparing `polars_qt-0.1.6.tar` & `polars_qt-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 polars_qt-0.1.6/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      111 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-16 06:29:43.000000 polars_qt-0.1.6/.python-version
--rw-r--r--   0     1001      127      645 2024-04-16 06:29:43.000000 polars_qt-0.1.6/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-16 06:29:43.000000 polars_qt-0.1.6/README.md
--rw-r--r--   0     1001      127       38 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/__init__.py
--rw-r--r--   0     1001      127     2898 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/funcs.py
--rw-r--r--   0     1001      127     3357 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/qt.py
--rw-r--r--   0     1001      127     3210 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/strategy.py
--rw-r--r--   0     1001      127     2567 2024-04-16 06:29:43.000000 polars_qt-0.1.6/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-16 06:29:43.000000 polars_qt-0.1.6/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-16 06:29:43.000000 polars_qt-0.1.6/rust-toolchain.toml
--rw-r--r--   0     1001      127     2054 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/if_then.rs
--rw-r--r--   0     1001      127      319 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/rolling_rank.rs
--rw-r--r--   0     1001      127      648 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/boll.rs
--rw-r--r--   0     1001      127      580 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/from_input.rs
--rw-r--r--   0     1001      127       26 2024-04-16 06:29:43.000000 polars_qt-0.1.6/src/strategy/mod.rs
--rw-r--r--   0     1001      127     1375 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127     1919 2024-04-16 06:29:43.000000 polars_qt-0.1.6/tests/test_strategy.py
--rw-r--r--   0     1001      127    44016 2024-04-16 06:30:03.000000 polars_qt-0.1.6/Cargo.lock
--rw-r--r--   0     1001      127     1773 2024-04-16 06:29:43.000000 polars_qt-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      808 1970-01-01 00:00:00.000000 polars_qt-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-18 01:26:04.000000 polars_qt-0.1.7/.python-version
+-rw-r--r--   0     1001      127      665 2024-04-18 01:26:04.000000 polars_qt-0.1.7/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-18 01:26:04.000000 polars_qt-0.1.7/README.md
+-rw-r--r--   0     1001      127       62 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     2898 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     3357 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/qt.py
+-rw-r--r--   0     1001      127     6413 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-18 01:26:04.000000 polars_qt-0.1.7/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-18 01:26:04.000000 polars_qt-0.1.7/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-18 01:26:04.000000 polars_qt-0.1.7/rust-toolchain.toml
+-rw-r--r--   0     1001      127     2054 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/if_then.rs
+-rw-r--r--   0     1001      127      319 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      127     3250 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     1151 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/boll.rs
+-rw-r--r--   0     1001      127      580 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/from_input.rs
+-rw-r--r--   0     1001      127      672 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/martingale.rs
+-rw-r--r--   0     1001      127       42 2024-04-18 01:26:04.000000 polars_qt-0.1.7/src/strategy/mod.rs
+-rw-r--r--   0     1001      127     1375 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1919 2024-04-18 01:26:04.000000 polars_qt-0.1.7/tests/test_strategy.py
+-rw-r--r--   0     1001      127    43211 2024-04-18 01:26:19.000000 polars_qt-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-18 01:26:04.000000 polars_qt-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.7/PKG-INFO
```

### Comparing `polars_qt-0.1.6/Cargo.toml` & `polars_qt-0.1.7/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-qt"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 
 [lib]
 name = "polars_qt"
 crate-type= ["cdylib"]
 
 [features]
@@ -15,19 +15,20 @@
 [dependencies]
 itertools = "0.12.1"
 pyo3 = { version = "0.20.0", features = ["extension-module", "abi3-py38"] }
 pyo3-polars = { version = "0.12.0", features = ["derive"] }
 serde = { version = "1", features = ["derive"] }
 polars = { version = "0.38", default-features = false, features=["rolling_window", "temporal"] }
 
-[dependencies.tea-core]
-git = "https://github.com/Teamon9161/tevec.git"
-rev = "4e89266"
-default-features = false
-features = ["pl"]
+# [dependencies.tevec]
+# git = "https://github.com/Teamon9161/tevec.git"
+# # rev = "4e89266"
+# branch = "master"
+# default-features = false
+# features = ["pl"]
 
 
 [dependencies.tea_strategy]
 git = "https://github.com/Teamon9161/tea_strategy.git"
-rev = "1d5db93"
+rev = "0c1e2fe"
 default-features = false
 features = ['pl']
```

### Comparing `polars_qt-0.1.6/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/Makefile` & `polars_qt-0.1.7/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 	ruff check . --fix --exit-non-zero-on-fix
 	ruff format polars_qt tests
 	# .venv/bin/mypy polars_qt tests
 
 format:
 	cargo fmt --all
 	cargo clippy --all-features
-	ruff check
+	ruff check --fix
+	# ruff check
 
 test: .venv
 	pytest tests
 
 debug: 
 	maturin develop
```

### Comparing `polars_qt-0.1.6/README.md` & `polars_qt-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/polars_qt/funcs.py` & `polars_qt-0.1.7/polars_qt/funcs.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/polars_qt/qt.py` & `polars_qt-0.1.7/polars_qt/qt.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/polars_qt/strategy.py` & `polars_qt-0.1.7/polars_qt/strategy.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     short_signal: float=-1,
     close_signal: float=0,
 ) -> pl.Expr:
     """
     Bollinger Bands
     fac: factor to calculate bollinger bands
     params:
-        if fac_vol is None
-            params: window, open_width, close_width(default: 0.0), stop_width(default: None)
-        if we use fac_vol stop
-            params: window, open_width, close_width(default: 0.0), fac_vol_width
-            the last of the params will be parsed as fac_vol_width
+        # if fac_vol is None
+        params: window, open_width, close_width(default: 0.0), stop_width(default: None)
+        # if we use fac_vol stop
+        #     params: window, open_width, close_width(default: 0.0), fac_vol_width
+        #     the last of the params will be parsed as fac_vol_width
     min_periods: minimum periods to calculate bollinger bands
     filters: long_open, long_stop, short_open, short_stop
         for open condition, if filter is False, open behavior is disabled
         for stop condition, if filter is True, return signal will be close_signal
     # fac_vol:
     #     a expression to calculate fac_vol, if None, we will use the default bollinger bands
     rev: reverse the long and short signal, filters will also be reversed automatically
@@ -51,41 +51,138 @@
     elif len(params) == 2:
         params = (*params, 0., last_param)
     elif len(params) == 3:
         params = (*params, last_param)
     # process min_periods
     if min_periods is None:
         min_periods = params[0] // 2
-    # calculate bollinger bands
-    # middle = fac.rolling_mean(params[0], min_periods=min_periods)
-    # std = fac.rolling_std(params[0], min_periods=min_periods)
 
     # process args and filters
     args = [fac]
     if filters is not None:
         assert len(filters) == 4, "filters must be a list of 4 elements"
-        # filter_flag = True
         filters = [parse_into_expr(f).cast(pl.Boolean) if not isinstance(f, bool) else pl.repeat(f, fac.len()) for f in filters]
         filters = [*filters[2:], *filters[:2]] if rev else filters
         args.extend(filters)
     else:
         pass
-        # filter_flag = False
-        # args.extend([pl.lit(None)*4])
     if rev:
         long_signal, short_signal = short_signal, long_signal
     kwargs = {
         "params": params,
-        # "filter_flag": filter_flag,
         "min_periods": min_periods,
         "delay_open": delay_open,
         "long_signal": float(long_signal),
         "short_signal": float(short_signal),
         "close_signal": float(close_signal),
     }
     return register_plugin(
         args=args,
         kwargs=kwargs,
         symbol="boll",
         is_elementwise=False,
     )
 
+def auto_boll(
+    fac: IntoExpr,
+    params: tuple[int, float, float] | tuple[int, float] | int,
+    min_periods: int | None=None,
+    filters: tuple[IntoExpr, IntoExpr, IntoExpr, IntoExpr] | None=None,
+    *,
+    # fac_vol: IntoExpr | None=None,
+    rev=False,
+    delay_open: bool=True,
+    long_signal: float=1,
+    short_signal: float=-1,
+    close_signal: float=0,
+) -> pl.Expr:
+    """
+    Bollinger Bands
+    fac: factor to calculate bollinger bands
+    params:
+        params: window, open_width, close_width(default: 0.0), win_trade_num
+        the last of the params will be parsed as number of trades profit to record
+    min_periods: minimum periods to calculate bollinger bands
+    filters: long_open, long_stop, short_open, short_stop
+        for open condition, if filter is False, open behavior is disabled
+        for stop condition, if filter is True, return signal will be close_signal
+    # fac_vol:
+    #     a expression to calculate fac_vol, if None, we will use the default bollinger bands
+    rev: reverse the long and short signal, filters will also be reversed automatically
+    delay_open: if open signal is blocked by filters, whether to delay the open signal when filters are True
+    """
+    fac = parse_into_expr(fac)
+    # process params
+    params, last_param = (params[:-1], params[-1])
+    if not isinstance(params, (tuple, list)):
+        params = (params, 0., 0., last_param)
+    elif len(params) == 1:
+        params = (*params, 0., 0., last_param)
+    elif len(params) == 2:
+        params = (*params, 0., last_param)
+    elif len(params) == 3:
+        params = (*params, last_param)
+    # process min_periods
+    if min_periods is None:
+        min_periods = params[0] // 2
+
+    # process args and filters
+    args = [fac]
+    if filters is not None:
+        assert len(filters) == 4, "filters must be a list of 4 elements"
+        filters = [parse_into_expr(f).cast(pl.Boolean) if not isinstance(f, bool) else pl.repeat(f, fac.len()) for f in filters]
+        filters = [*filters[2:], *filters[:2]] if rev else filters
+        args.extend(filters)
+    else:
+        pass
+    if rev:
+        long_signal, short_signal = short_signal, long_signal
+
+    kwargs = {
+        "params": params,
+        "min_periods": min_periods,
+        "delay_open": delay_open,
+        "long_signal": float(long_signal),
+        "short_signal": float(short_signal),
+        "close_signal": float(close_signal),
+    }
+    return register_plugin(
+        args=args,
+        kwargs=kwargs,
+        symbol="auto_boll",
+        is_elementwise=False,
+    )
+
+def martingale(
+    close: IntoExpr,
+    n: int,
+    step: int | None,
+    init_pos: float,
+    take_profit: float,
+    filters: IntoExpr | None=None,
+    win_p_addup: float | None = None,
+    pos_mul: float | None = 2,
+    b: float=1,
+    stop_loss_m: float | None = None,
+) -> pl.Expr:
+    close = parse_into_expr(close)
+    args = [close]
+    if filters is not None:
+        args.extend([parse_into_expr(filters).cast(pl.Boolean), pl.repeat(True, close.len()), pl.repeat(False, close.len()), pl.repeat(False, close.len())])
+    else:
+        pass
+    kwargs = {
+        'n': n,
+        'step': step,
+        'init_pos': init_pos,
+        'win_p_addup': win_p_addup,
+        'pos_mul': pos_mul,
+        'take_profit': take_profit,
+        'b': b,
+        'stop_loss_m': stop_loss_m,
+    }
+    return register_plugin(
+        args=args,
+        kwargs=kwargs,
+        symbol='martingale',
+        is_elementwise=False,
+    )
```

### Comparing `polars_qt-0.1.6/polars_qt/utils.py` & `polars_qt-0.1.7/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/src/equity.rs` & `polars_qt-0.1.7/src/equity.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/src/if_then.rs` & `polars_qt-0.1.7/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/src/rolling_rank.rs` & `polars_qt-0.1.7/src/rolling_rank.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/src/strategy/boll.rs` & `polars_qt-0.1.7/src/strategy/martingale.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #![allow(clippy::unused_unit)]
 use super::from_input::FromInput;
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
-use tea_strategy::{BollKwargs, StrategyFilter};
+use tea_strategy::{MartingaleKwargs, StrategyFilter};
 
 #[polars_expr(output_type=Float64)]
-fn boll(inputs: &[Series], kwargs: BollKwargs) -> PolarsResult<Series> {
+fn martingale(inputs: &[Series], kwargs: MartingaleKwargs) -> PolarsResult<Series> {
     let fac = inputs[0].f64()?;
     let filter = if inputs.len() == 5 {
         Some(StrategyFilter::from_inputs(inputs, &[1, 2, 3, 4])?)
     } else if inputs.len() == 1 {
         None
     } else {
         panic!("wrong lenght of inputs in function boll")
     };
-    let out: Float64Chunked = tea_strategy::boll(fac, filter, &kwargs);
+    let out: Float64Chunked = tea_strategy::martingale(fac, filter, &kwargs);
     Ok(out.into_series())
 }
```

### Comparing `polars_qt-0.1.6/src/strategy/from_input.rs` & `polars_qt-0.1.7/src/strategy/from_input.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/tests/test_equity.py` & `polars_qt-0.1.7/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/tests/test_if_then.py` & `polars_qt-0.1.7/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/tests/test_rolling_rank.py` & `polars_qt-0.1.7/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/tests/test_strategy.py` & `polars_qt-0.1.7/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/Cargo.lock` & `polars_qt-0.1.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -157,17 +157,15 @@
 name = "chrono"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
- "js-sys",
  "num-traits",
- "wasm-bindgen",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -233,15 +231,15 @@
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -856,22 +854,21 @@
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
- "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?rev=4e89266)",
  "tea_strategy",
 ]
 
 [[package]]
 name = "polars-row"
 version = "0.38.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -932,17 +929,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -986,28 +983,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-polars"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
@@ -1030,15 +1027,15 @@
 checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -1175,17 +1172,17 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-pickle"
 version = "1.1.1"
@@ -1197,21 +1194,21 @@
  "num-bigint",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
@@ -1266,15 +1263,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1282,17 +1279,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1320,77 +1317,57 @@
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
 version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
-dependencies = [
- "num-traits",
- "polars",
- "polars-arrow",
- "serde",
- "tea-dtype 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
-]
-
-[[package]]
-name = "tea-core"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?rev=4e89266#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
 dependencies = [
  "num-traits",
  "polars",
  "polars-arrow",
  "serde",
- "tea-dtype 0.1.1 (git+https://github.com/Teamon9161/tevec.git?rev=4e89266)",
+ "tea-dtype",
 ]
 
 [[package]]
 name = "tea-dtype"
 version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
-dependencies = [
- "num-traits",
- "tea-time",
-]
-
-[[package]]
-name = "tea-dtype"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?rev=4e89266#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "tea-rolling"
 version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
 dependencies = [
  "num-traits",
- "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
-]
-
-[[package]]
-name = "tea-time"
-version = "0.1.1"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#4e89266ddddf077ded7e9804d5b04a0c1c872bd0"
-dependencies = [
- "chrono",
+ "tea-core",
 ]
 
 [[package]]
 name = "tea_strategy"
 version = "0.1.0"
-source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=1d5db93#1d5db934079015e1329217603b374608aa993b41"
+source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=0c1e2fe#0c1e2fe8f66bc887f9a172645635158223aa0249"
 dependencies = [
  "itertools",
  "serde",
- "tea-core 0.1.1 (git+https://github.com/Teamon9161/tevec.git?branch=master)",
+ "tevec",
+]
+
+[[package]]
+name = "tevec"
+version = "0.1.1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#3abf4cd9a3e775d724585be4c503a205b99113a2"
+dependencies = [
+ "tea-core",
+ "tea-dtype",
  "tea-rolling",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1403,15 +1380,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -1460,15 +1437,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1482,15 +1459,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1687,15 +1664,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `polars_qt-0.1.6/pyproject.toml` & `polars_qt-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.6/PKG-INFO` & `polars_qt-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

