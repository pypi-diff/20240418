# Comparing `tmp/pytrip98-3.9.0.tar.gz` & `tmp/pytrip98-3.9.1-cp36-cp36m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrip98-3.9.0.tar", last modified: Sat Sep 23 19:43:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

