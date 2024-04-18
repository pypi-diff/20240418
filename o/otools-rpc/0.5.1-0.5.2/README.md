# Comparing `tmp/otools-rpc-0.5.1.tar.gz` & `tmp/otools_rpc-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.5.1.tar", last modified: Tue Jan 23 11:26:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

