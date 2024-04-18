# Comparing `tmp/couchbase-4.2.0rc1.tar.gz` & `tmp/couchbase-4.2.1rc1-cp38-cp38-manylinux2014_aarch64.manylinux_2_17_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbase-4.2.0rc1.tar", last modified: Wed Mar 13 21:31:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

