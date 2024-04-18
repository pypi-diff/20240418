# Comparing `tmp/mypy-boto3-workspaces-1.34.58.tar.gz` & `tmp/mypy_boto3_workspaces-1.34.87-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-1.34.58.tar", last modified: Thu Mar  7 20:22:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

