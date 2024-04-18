# Comparing `tmp/chaostoolkit-datadog-0.2.0.tar.gz` & `tmp/chaostoolkit_datadog-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-datadog-0.2.0.tar", last modified: Fri Jun  9 08:42:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

