# Comparing `tmp/socialmediaextractor-0.3.tar.gz` & `tmp/socialmediaextractor-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialmediaextractor-0.3.tar", last modified: Sun Apr  9 18:33:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

