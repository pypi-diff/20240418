# Comparing `tmp/AdDownloader-0.2.4.1.tar.gz` & `tmp/AdDownloader-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdDownloader-0.2.4.1.tar", last modified: Wed Mar  6 13:34:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

