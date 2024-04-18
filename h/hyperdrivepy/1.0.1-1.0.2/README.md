# Comparing `tmp/hyperdrivepy-1.0.1.tar.gz` & `tmp/hyperdrivepy-1.0.2-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrivepy-1.0.1.tar", last modified: Mon Apr 15 23:25:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

