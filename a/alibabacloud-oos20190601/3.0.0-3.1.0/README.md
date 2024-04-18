# Comparing `tmp/alibabacloud_oos20190601-3.0.0.tar.gz` & `tmp/alibabacloud_oos20190601-3.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oos20190601-3.0.0.tar", last modified: Wed Jan 10 07:43:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

