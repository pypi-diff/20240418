# Comparing `tmp/OpenMEASURE-0.3.8.tar.gz` & `tmp/OpenMEASURE-0.3.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenMEASURE-0.3.8.tar", last modified: Mon Feb 26 16:10:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

