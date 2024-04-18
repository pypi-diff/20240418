# Comparing `tmp/Recherche Babac2-0.2.7.tar.gz` & `tmp/Recherche_Babac2-0.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Recherche Babac2-0.2.7.tar", last modified: Mon Jan 16 04:55:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

