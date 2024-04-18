# Comparing `tmp/jax_jynx-0.1.2.tar.gz` & `tmp/jax_jynx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_jynx-0.1.2.tar", max compression
+gzip compressed data, was "jax_jynx-0.1.3.tar", max compression
```

## Comparing `jax_jynx-0.1.2.tar` & `jax_jynx-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1078 2024-02-11 20:05:30.061426 jax_jynx-0.1.2/LICENSE
--rw-r--r--   0        0        0     4048 2024-02-11 20:36:38.703506 jax_jynx-0.1.2/README.md
--rw-r--r--   0        0        0      384 2024-03-06 15:31:30.498454 jax_jynx-0.1.2/jynx/__init__.py
--rw-r--r--   0        0        0     5425 2024-02-11 21:05:53.825702 jax_jynx-0.1.2/jynx/callbacks.py
--rw-r--r--   0        0        0     3603 2024-02-16 15:13:26.399756 jax_jynx-0.1.2/jynx/fit.py
--rw-r--r--   0        0        0     1755 2024-03-06 15:41:37.687121 jax_jynx-0.1.2/jynx/layers/__init__.py
--rw-r--r--   0        0        0    21128 2024-03-06 15:37:00.577514 jax_jynx-0.1.2/jynx/layers/containers.py
--rw-r--r--   0        0        0     2059 2024-02-11 21:10:42.794451 jax_jynx-0.1.2/jynx/layers/factory.py
--rw-r--r--   0        0        0    12781 2024-03-04 15:57:37.533217 jax_jynx-0.1.2/jynx/layers/linear.py
--rw-r--r--   0        0        0     6830 2024-03-04 16:54:52.401866 jax_jynx-0.1.2/jynx/layers/misc.py
--rw-r--r--   0        0        0     2785 2024-03-04 16:55:01.595117 jax_jynx-0.1.2/jynx/layers/module.py
--rw-r--r--   0        0        0     4614 2024-03-04 16:55:05.978236 jax_jynx-0.1.2/jynx/layers/nets.py
--rw-r--r--   0        0        0     8084 2024-03-04 16:55:17.121540 jax_jynx-0.1.2/jynx/layers/rnn.py
--rw-r--r--   0        0        0     3922 2024-03-04 16:55:26.559797 jax_jynx-0.1.2/jynx/layers/static.py
--rw-r--r--   0        0        0    22217 2024-03-06 15:49:47.954582 jax_jynx-0.1.2/jynx/layers/transformer.py
--rw-r--r--   0        0        0     4849 2024-03-06 15:36:05.966014 jax_jynx-0.1.2/jynx/pytree.py
--rw-r--r--   0        0        0     1138 2024-03-06 15:50:38.933982 jax_jynx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 jax_jynx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4048 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/README.md
+-rw-r--r--   0        0        0      384 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/__init__.py
+-rw-r--r--   0        0        0     5425 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/callbacks.py
+-rw-r--r--   0        0        0     3603 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/fit.py
+-rw-r--r--   0        0        0     1755 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/__init__.py
+-rw-r--r--   0        0        0    21152 2024-04-18 13:25:50.893671 jax_jynx-0.1.3/jynx/layers/containers.py
+-rw-r--r--   0        0        0     2059 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/factory.py
+-rw-r--r--   0        0        0    12781 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/linear.py
+-rw-r--r--   0        0        0     6896 2024-04-18 13:48:03.591997 jax_jynx-0.1.3/jynx/layers/misc.py
+-rw-r--r--   0        0        0     2785 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/module.py
+-rw-r--r--   0        0        0     4614 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/nets.py
+-rw-r--r--   0        0        0     8084 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/rnn.py
+-rw-r--r--   0        0        0     3922 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/layers/static.py
+-rw-r--r--   0        0        0    22219 2024-04-18 13:49:43.470562 jax_jynx-0.1.3/jynx/layers/transformer.py
+-rw-r--r--   0        0        0     4849 2024-04-18 13:22:10.769575 jax_jynx-0.1.3/jynx/pytree.py
+-rw-r--r--   0        0        0     1138 2024-04-18 13:58:08.443083 jax_jynx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4395 1970-01-01 00:00:00.000000 jax_jynx-0.1.3/PKG-INFO
```

### Comparing `jax_jynx-0.1.2/LICENSE` & `jax_jynx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/README.md` & `jax_jynx-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/callbacks.py` & `jax_jynx-0.1.3/jynx/callbacks.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/fit.py` & `jax_jynx-0.1.3/jynx/fit.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/__init__.py` & `jax_jynx-0.1.3/jynx/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/containers.py` & `jax_jynx-0.1.3/jynx/layers/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,17 @@
 
         Returns:
             tp.Sequence[dict[str, Key]]: A sequence of dictionaries,
                 each containing a split key for a module in the list.
                 Dicts may be empty if 'key' is not provided in kwargs.
 
         """
-        if "key" in kwargs:
-            return [{"key": k} for k in rnd.split(kwargs.pop("key"), len(self))]
+        key = kwargs.pop("key", None)
+        if key is not None:
+            return [{"key": k} for k in rnd.split(key, len(self))]
         else:
             return [{}] * len(self)
 
     def __repr__(self):
         return f"{self.__class__.__name__}{tuple(self)})"
 
     @tp.overload
```

### Comparing `jax_jynx-0.1.2/jynx/layers/factory.py` & `jax_jynx-0.1.3/jynx/layers/factory.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/linear.py` & `jax_jynx-0.1.3/jynx/layers/linear.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/misc.py` & `jax_jynx-0.1.3/jynx/layers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,17 @@
     subtract_mean: bool = static(default=True)
 
     def __call__(self, x: Array, *args, **kwargs) -> Array:
         del args, kwargs
         if self.subtract_mean:
             x = x - jnp.mean(x, axis=self.axis, keepdims=True)
 
-        x = x / jnp.square(x).sum(axis=self.axis, keepdims=True)
+        denom = jnp.square(x).sum(axis=self.axis, keepdims=True)
+        denom = jnp.clip(denom, 1e-6, None)
+        x = x / denom
 
         if self.weight is not None:
             x = x * self.weight
         if self.bias is not None:
             x = x + self.bias
         return x
```

### Comparing `jax_jynx-0.1.2/jynx/layers/module.py` & `jax_jynx-0.1.3/jynx/layers/module.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/nets.py` & `jax_jynx-0.1.3/jynx/layers/nets.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/rnn.py` & `jax_jynx-0.1.3/jynx/layers/rnn.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/static.py` & `jax_jynx-0.1.3/jynx/layers/static.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/jynx/layers/transformer.py` & `jax_jynx-0.1.3/jynx/layers/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         v: Array,
         mask: Array | None = None,
         **kwargs,
     ) -> Array:
         ...
 
 
-@jax.checkpoint  # pyright: ignore
+# @jax.checkpoint  # pyright: ignore
 def scaled_dot_product_attention(
     q: Array,
     k: Array,
     v: Array,
     mask: Array | None = None,
     **kwargs,
 ) -> Array:
```

### Comparing `jax_jynx-0.1.2/jynx/pytree.py` & `jax_jynx-0.1.3/jynx/pytree.py`

 * *Files identical despite different names*

### Comparing `jax_jynx-0.1.2/pyproject.toml` & `jax_jynx-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jax-jynx"
-version = "0.1.2"
+version = "0.1.3"
 description = "A neural network library using jax"
 authors = ["Scott Cameron"]
 readme = "README.md"
 packages = [
   { include = "jynx" }
 ]
```

### Comparing `jax_jynx-0.1.2/PKG-INFO` & `jax_jynx-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: jax-jynx
-Version: 0.1.2
+Version: 0.1.3
 Summary: A neural network library using jax
 Author: Scott Cameron
 Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jax (>=0.4.24,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.24,<0.5.0)
 Requires-Dist: optax (>=0.1.9,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Jynx
```

