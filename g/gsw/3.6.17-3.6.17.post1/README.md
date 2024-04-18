# Comparing `tmp/gsw-3.6.17.tar.gz` & `tmp/gsw-3.6.17.post1-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsw-3.6.17.tar", last modified: Thu Jun 22 17:18:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

