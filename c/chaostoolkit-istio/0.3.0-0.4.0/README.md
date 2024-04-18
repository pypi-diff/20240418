# Comparing `tmp/chaostoolkit-istio-0.3.0.tar.gz` & `tmp/chaostoolkit_istio-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chaostoolkit-istio/chaostoolkit-istio/dist/.tmp-u3ochlog/chaostoolkit-istio-0.3.0.tar", last modified: Mon Feb 27 10:09:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

