# Comparing `tmp/vjepa_encoder-0.0.4.tar.gz` & `tmp/vjepa_encoder-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vjepa_encoder-0.0.4.tar", last modified: Wed Apr 17 01:37:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

