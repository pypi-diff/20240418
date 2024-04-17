# Comparing `tmp/vts-0.1.1.tar.gz` & `tmp/vts-0.1.2.tar.gz`

## Comparing `vts-0.1.1.tar` & `vts-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-------   0     1000     1000      286 2024-04-12 22:37:11.000000 vts-0.1.1/vts_core/Cargo.toml
--rw-r--r--   0     1000     1000     6087 2024-04-15 22:49:36.000000 vts-0.1.1/vts_core/src/arch/checker.rs
--rw-r--r--   0     1000     1000     5479 2024-04-17 20:19:16.000000 vts-0.1.1/vts_core/src/arch/component.rs
--rw-r--r--   0     1000     1000     9479 2024-04-17 20:19:16.000000 vts-0.1.1/vts_core/src/arch/connection.rs
--rw-r--r--   0     1000     1000    25983 2024-04-17 01:23:21.000000 vts-0.1.1/vts_core/src/arch/de.rs
--rw-r--r--   0     1000     1000     7024 2024-04-15 22:50:06.000000 vts-0.1.1/vts_core/src/arch/linker.rs
--rw-r--r--   0     1000     1000     1629 2024-04-15 18:49:51.000000 vts-0.1.1/vts_core/src/arch/mod.rs
--rw-r--r--   0     1000     1000     3462 2024-04-12 22:23:16.000000 vts-0.1.1/vts_core/src/arch/module.rs
--rw-r--r--   0     1000     1000     8811 2024-04-17 01:29:30.000000 vts-0.1.1/vts_core/src/arch/port.rs
--rw-r--r--   0     1000     1000      402 2024-04-15 18:26:23.000000 vts-0.1.1/vts_core/src/arch/prelude.rs
--rw-r--r--   0     1000     1000     8477 2024-04-17 01:29:08.000000 vts-0.1.1/vts_core/src/arch/reference.rs
--rw-r--r--   0     1000     1000    10472 2024-04-17 01:35:05.000000 vts-0.1.1/vts_core/src/arch/ser.rs
--rw-r--r--   0     1000     1000       29 2024-04-12 20:42:36.000000 vts-0.1.1/vts_core/src/lib.rs
--rw-r--r--   0     1000     1000     9772 2024-03-14 10:37:36.000000 vts-0.1.1/vts_core/src/yosys.rs
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 vts-0.1.1/vts_api/Cargo.toml
--rw-r--r--   0     1000     1000    13976 2024-04-17 21:28:03.000000 vts-0.1.1/vts_api/src/arch/component.rs
--rw-r--r--   0     1000     1000     5162 2024-04-17 01:54:00.000000 vts-0.1.1/vts_api/src/arch/mod.rs
--rw-r--r--   0     1000     1000    10018 2024-04-16 00:05:33.000000 vts-0.1.1/vts_api/src/arch/module.rs
--rw-r--r--   0     1000     1000     4946 2024-04-17 20:19:16.000000 vts-0.1.1/vts_api/src/arch/port.rs
--rw-r--r--   0     1000     1000     6180 2024-04-17 20:19:16.000000 vts-0.1.1/vts_api/src/arch/reference.rs
--rw-r--r--   0     1000     1000     2475 2024-04-16 15:59:10.000000 vts-0.1.1/vts_api/src/lib.rs
--rw-r--r--   0     1000     1000    14744 2024-04-12 22:37:11.000000 vts-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      233 1970-01-01 00:00:00.000000 vts-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000      505 2024-04-17 21:37:57.000000 vts-0.1.1/pyproject.toml
--rw-r--r--   0     1000     1000        0 2024-04-08 03:15:36.000000 vts-0.1.1/python/vts/py.typed
--rw-r--r--   0     1000     1000        0 2024-04-10 23:37:43.000000 vts-0.1.1/python/vts/_vts/py.typed
--rw-r--r--   0     1000     1000     4668 2024-04-17 21:30:00.000000 vts-0.1.1/python/vts/_vts/arch.pyi
--rw-r--r--   0     1000     1000       39 2024-04-12 19:20:39.000000 vts-0.1.1/python/vts/__init__.py
--rw-r--r--   0     1000     1000      579 2024-04-16 22:18:13.000000 vts-0.1.1/python/vts/arch/__init__.py
--rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 vts-0.1.1/PKG-INFO
+-rw-------   0     1000     1000      286 2024-04-12 22:37:11.000000 vts-0.1.2/vts_core/Cargo.toml
+-rw-r--r--   0     1000     1000     6087 2024-04-15 22:49:36.000000 vts-0.1.2/vts_core/src/arch/checker.rs
+-rw-r--r--   0     1000     1000     5479 2024-04-17 20:19:16.000000 vts-0.1.2/vts_core/src/arch/component.rs
+-rw-r--r--   0     1000     1000     9479 2024-04-17 20:19:16.000000 vts-0.1.2/vts_core/src/arch/connection.rs
+-rw-r--r--   0     1000     1000    25983 2024-04-17 01:23:21.000000 vts-0.1.2/vts_core/src/arch/de.rs
+-rw-r--r--   0     1000     1000     7024 2024-04-15 22:50:06.000000 vts-0.1.2/vts_core/src/arch/linker.rs
+-rw-r--r--   0     1000     1000     1629 2024-04-15 18:49:51.000000 vts-0.1.2/vts_core/src/arch/mod.rs
+-rw-r--r--   0     1000     1000     3462 2024-04-12 22:23:16.000000 vts-0.1.2/vts_core/src/arch/module.rs
+-rw-r--r--   0     1000     1000     8811 2024-04-17 01:29:30.000000 vts-0.1.2/vts_core/src/arch/port.rs
+-rw-r--r--   0     1000     1000      402 2024-04-15 18:26:23.000000 vts-0.1.2/vts_core/src/arch/prelude.rs
+-rw-r--r--   0     1000     1000     8477 2024-04-17 01:29:08.000000 vts-0.1.2/vts_core/src/arch/reference.rs
+-rw-r--r--   0     1000     1000    10472 2024-04-17 01:35:05.000000 vts-0.1.2/vts_core/src/arch/ser.rs
+-rw-r--r--   0     1000     1000       29 2024-04-12 20:42:36.000000 vts-0.1.2/vts_core/src/lib.rs
+-rw-r--r--   0     1000     1000     9772 2024-03-14 10:37:36.000000 vts-0.1.2/vts_core/src/yosys.rs
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 vts-0.1.2/vts_api/Cargo.toml
+-rw-r--r--   0     1000     1000    13976 2024-04-17 21:28:03.000000 vts-0.1.2/vts_api/src/arch/component.rs
+-rw-r--r--   0     1000     1000     5162 2024-04-17 01:54:00.000000 vts-0.1.2/vts_api/src/arch/mod.rs
+-rw-r--r--   0     1000     1000    10018 2024-04-16 00:05:33.000000 vts-0.1.2/vts_api/src/arch/module.rs
+-rw-r--r--   0     1000     1000     4946 2024-04-17 20:19:16.000000 vts-0.1.2/vts_api/src/arch/port.rs
+-rw-r--r--   0     1000     1000     6180 2024-04-17 20:19:16.000000 vts-0.1.2/vts_api/src/arch/reference.rs
+-rw-r--r--   0     1000     1000     2475 2024-04-16 15:59:10.000000 vts-0.1.2/vts_api/src/lib.rs
+-rw-r--r--   0     1000     1000    14744 2024-04-12 22:37:11.000000 vts-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      233 1970-01-01 00:00:00.000000 vts-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000      916 2024-04-17 22:34:12.000000 vts-0.1.2/pyproject.toml
+-rw-r--r--   0     1000     1000        0 2024-04-08 03:15:36.000000 vts-0.1.2/python/vts/py.typed
+-rw-r--r--   0     1000     1000        0 2024-04-10 23:37:43.000000 vts-0.1.2/python/vts/_vts/py.typed
+-rw-r--r--   0     1000     1000     4668 2024-04-17 21:30:00.000000 vts-0.1.2/python/vts/_vts/arch.pyi
+-rw-r--r--   0     1000     1000       39 2024-04-12 19:20:39.000000 vts-0.1.2/python/vts/__init__.py
+-rw-r--r--   0     1000     1000      579 2024-04-16 22:18:13.000000 vts-0.1.2/python/vts/arch/__init__.py
+-rw-r--r--   0     1000     1000      449 2024-04-08 13:52:33.000000 vts-0.1.2/README.md
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 vts-0.1.2/PKG-INFO
```

### Comparing `vts-0.1.1/vts_core/src/arch/checker.rs` & `vts-0.1.2/vts_core/src/arch/checker.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/component.rs` & `vts-0.1.2/vts_core/src/arch/component.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/connection.rs` & `vts-0.1.2/vts_core/src/arch/connection.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/de.rs` & `vts-0.1.2/vts_core/src/arch/de.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/linker.rs` & `vts-0.1.2/vts_core/src/arch/linker.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/mod.rs` & `vts-0.1.2/vts_core/src/arch/mod.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/module.rs` & `vts-0.1.2/vts_core/src/arch/module.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/port.rs` & `vts-0.1.2/vts_core/src/arch/port.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/reference.rs` & `vts-0.1.2/vts_core/src/arch/reference.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/arch/ser.rs` & `vts-0.1.2/vts_core/src/arch/ser.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_core/src/yosys.rs` & `vts-0.1.2/vts_core/src/yosys.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/arch/component.rs` & `vts-0.1.2/vts_api/src/arch/component.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/arch/mod.rs` & `vts-0.1.2/vts_api/src/arch/mod.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/arch/module.rs` & `vts-0.1.2/vts_api/src/arch/module.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/arch/port.rs` & `vts-0.1.2/vts_api/src/arch/port.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/arch/reference.rs` & `vts-0.1.2/vts_api/src/arch/reference.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/vts_api/src/lib.rs` & `vts-0.1.2/vts_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/Cargo.lock` & `vts-0.1.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/python/vts/_vts/arch.pyi` & `vts-0.1.2/python/vts/_vts/arch.pyi`

 * *Files identical despite different names*

### Comparing `vts-0.1.1/python/vts/arch/__init__.py` & `vts-0.1.2/python/vts/arch/__init__.py`

 * *Files identical despite different names*

