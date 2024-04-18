# Comparing `tmp/nuvla-api-3.0.9.tar.gz` & `tmp/nuvla_api-4.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla-api-3.0.9.tar", last modified: Tue Jul 18 09:44:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

