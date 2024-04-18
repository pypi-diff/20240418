# Comparing `tmp/edc_consent-0.3.83.tar.gz` & `tmp/edc_consent-0.3.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc_consent-0.3.83.tar", last modified: Thu Apr 18 02:19:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

