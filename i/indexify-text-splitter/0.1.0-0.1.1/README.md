# Comparing `tmp/indexify_text_splitter-0.1.0.tar.gz` & `tmp/indexify_text_splitter-0.1.1.tar.gz`

## Comparing `indexify_text_splitter-0.1.0.tar` & `indexify_text_splitter-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 indexify_text_splitter-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     1680 2024-04-17 09:03:31.000000 indexify_text_splitter-0.1.0/src/lib.rs
--rw-r--r--   0      501       20    68328 2024-04-17 09:03:31.000000 indexify_text_splitter-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      146 2024-04-17 09:03:31.000000 indexify_text_splitter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      142 1970-01-01 00:00:00.000000 indexify_text_splitter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 indexify_text_splitter-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20     2338 2024-04-18 10:20:14.000000 indexify_text_splitter-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20    68328 2024-04-18 10:23:11.000000 indexify_text_splitter-0.1.1/Cargo.lock
+-rw-r--r--   0      501       20      146 2024-04-18 09:26:03.000000 indexify_text_splitter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      142 1970-01-01 00:00:00.000000 indexify_text_splitter-0.1.1/PKG-INFO
```

### Comparing `indexify_text_splitter-0.1.0/Cargo.lock` & `indexify_text_splitter-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -901,15 +901,15 @@
  "same-file",
  "walkdir",
  "winapi-util",
 ]
 
 [[package]]
 name = "indexify_text_splitter"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "maturin",
  "pyo3",
  "regex",
 ]
 
 [[package]]
```

