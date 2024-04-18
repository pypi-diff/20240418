# Comparing `tmp/tllab_common-2024.4.1.tar.gz` & `tmp/tllab_common-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2024.4.1.tar", max compression
+gzip compressed data, was "tllab_common-2024.4.2.tar", max compression
```

## Comparing `tllab_common-2024.4.1.tar` & `tllab_common-2024.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.1/LICENSE
--rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.1/README.md
--rw-r--r--   0        0        0      963 2024-04-10 14:31:27.762533 tllab_common-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.1/tllab_common/__init__.py
--rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.1/tllab_common/findcells.py
--rw-r--r--   0        0        0    11610 2024-04-10 11:07:13.403168 tllab_common-2024.4.1/tllab_common/fit.py
--rw-r--r--   0        0        0     7924 2024-04-09 12:21:00.201925 tllab_common-2024.4.1/tllab_common/io.py
--rw-r--r--   0        0        0    19679 2024-04-10 12:13:00.480242 tllab_common-2024.4.1/tllab_common/misc.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 tllab_common-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2024.4.2/LICENSE
+-rw-r--r--   0        0        0      706 2023-08-24 13:53:49.878008 tllab_common-2024.4.2/README.md
+-rw-r--r--   0        0        0      963 2024-04-18 08:20:21.063902 tllab_common-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-02-27 12:16:59.090201 tllab_common-2024.4.2/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0     9595 2024-03-26 10:33:49.874564 tllab_common-2024.4.2/tllab_common/findcells.py
+-rw-r--r--   0        0        0    11777 2024-04-18 08:03:45.704570 tllab_common-2024.4.2/tllab_common/fit.py
+-rw-r--r--   0        0        0     7944 2024-04-11 14:21:45.280730 tllab_common-2024.4.2/tllab_common/io.py
+-rw-r--r--   0        0        0    19679 2024-04-10 12:13:00.480242 tllab_common-2024.4.2/tllab_common/misc.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 tllab_common-2024.4.2/PKG-INFO
```

### Comparing `tllab_common-2024.4.1/LICENSE` & `tllab_common-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.1/README.md` & `tllab_common-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.1/pyproject.toml` & `tllab_common-2024.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2024.4.1"
+version = "2024.4.2"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2024.4.1/tllab_common/findcells.py` & `tllab_common-2024.4.2/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.1/tllab_common/fit.py` & `tllab_common-2024.4.2/tllab_common/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 
 class Fit(metaclass=ABCMeta):
     bounds = None
 
     def __init__(self, x: ArrayLike, y: ArrayLike,
                  w: [ArrayLike, None] = None, s: [ArrayLike, None] = None,
-                 fit_window: Sequence[float] = None, log_scale: bool = False) -> None:
+                 fit_window: Sequence[float] = None, log_scale: bool = False, fit_s: bool = True) -> None:
         x = np.asarray(x)
         y = np.asarray(y)
         w = np.ones_like(x) if w is None else np.asarray(w)
         if log_scale:
             s = np.ones_like(x) if s is None else np.asarray(s) / np.abs(y)
         else:
             s = np.ones_like(x) if s is None else np.asarray(s)
 
         if fit_window:
             idx = (fit_window[0] <= x) & (x < fit_window[1])
             x, y, w, s = x[idx], y[idx], w[idx], s[idx]
 
         self.x, self.y, self.w, self.s = nonnan(x, y, w, s)
         self.log_scale = log_scale
+        self.fit_s = fit_s
         self.n = np.sum(self.w)
         self.p_ci95 = None
         self.r_squared = None
         self.chi_squared = None
         self.r_squared_adjusted = None
 
     @property
@@ -79,20 +80,21 @@
         else:
             x = np.asarray(x)
         f = self.fun(self.p, x)
         df = np.sqrt(np.sum((self.dfun(self.p, x).T * self.p_ci95).T ** 2, 0))
         return x.real, f - df, f + df
 
     def get_cost_fun(self) -> Callable[[ArrayLike], float]:
+        s = self.s if self.fit_s else 1
         if self.log_scale:
             def cost(p: ArrayLike) -> float:
-                return np.nansum(np.abs(self.w / self.s * np.log(self.y / self.fun(p, self.x)) ** 2))
+                return np.nansum(np.abs(self.w / s * np.log(self.y / self.fun(p, self.x)) ** 2))
         else:
             def cost(p: ArrayLike) -> float:
-                return np.nansum(np.abs(self.w / self.s * (self.y - self.fun(p, self.x)) ** 2))
+                return np.nansum(np.abs(self.w / s * (self.y - self.fun(p, self.x)) ** 2))
         return cost
 
     def fit(self) -> Fit:
         _ = self.r
         return self
 
     @cached_property
@@ -108,17 +110,21 @@
                                                                     self.w, np.log(self.s))
         else:
             self.chi_squared, self.p_ci95, self.r_squared = fminerr(self.fun, r.x,
                                                                     self.y, (self.x,), self.w, self.s)
         self.r_squared_adjusted = 1 - (1 - self.r_squared) * (self.n - 1) / (len(r.x) - 1)
         return r
 
+    @staticmethod
+    def sort(p: np.ndarray) -> np.ndarray:
+        return p
+
     @property
     def p(self) -> np.ndarray:
-        return np.full(self.n_p, np.nan) if self.r is None else self.r.x
+        return np.full(self.n_p, np.nan) if self.r is None else self.sort(self.r.x)
 
     @property
     def log_likelihood(self) -> float:
         return -self.n * np.log(2 * np.pi * self.r.fun / (self.n - 1)) / 2 - (self.n - 1) / 2
 
     @property
     def bic(self) -> float:
```

### Comparing `tllab_common-2024.4.1/tllab_common/io.py` & `tllab_common-2024.4.2/tllab_common/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         y.Representer = RoundTripRepresenter
         if isinstance(stream, (str, bytes, Path)):
             stream = stack.enter_context(open(stream, 'w'))
         return y.dump(data, stream)
 
 
 def get_params(parameter_file: [str, Path], template_file: [str, Path] = None,
-               required: dict = None) -> CommentedDefaultMap:
+               required: Sequence[dict] = None) -> CommentedDefaultMap:
     """ Load parameters from a parameterfile and parameters missing from that from the templatefile. Raise an error when
         parameters in required are missing. Return a dictionary with the parameters.
     """
 
     from .misc import cprint
 
     def more_params(parameters: dict, file: [str, Path]) -> None:
@@ -165,15 +165,15 @@
         for key, value in template.items():
             if key not in parameters and value is not None:
                 cprint(f'<Parameter <{path}{key}:.b> missing in parameter file, adding with default value: {value}.:r>')
                 parameters[key] = value
             elif isinstance(value, dict):
                 check_params(parameters[key], value, f'{path}{key}.')
 
-    def check_required(parameters: dict, required: dict) -> None:  # noqa
+    def check_required(parameters: dict, required: Sequence[dict]) -> None:  # noqa
         if required is not None:
             for p in required:
                 if isinstance(p, dict):
                     for key, value in p.items():
                         check_required(parameters[key], value)
                 else:
                     if p not in parameters:
```

### Comparing `tllab_common-2024.4.1/tllab_common/misc.py` & `tllab_common-2024.4.2/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2024.4.1/PKG-INFO` & `tllab_common-2024.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab_common
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.10,<4.0
```

