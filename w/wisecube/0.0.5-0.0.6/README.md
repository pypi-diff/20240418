# Comparing `tmp/wisecube-0.0.5.tar.gz` & `tmp/wisecube-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisecube-0.0.5.tar", last modified: Wed Apr 17 08:53:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

