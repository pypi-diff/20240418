# Comparing `tmp/edurpa_google-1.0.3.tar.gz` & `tmp/edurpa_google-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edurpa_google-1.0.3.tar", last modified: Wed Apr 17 15:54:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

