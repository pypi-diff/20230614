# Comparing `tmp/descarteslabs-2.0.0.tar.gz` & `tmp/descarteslabs-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs-2.0.0.tar", last modified: Mon Jun 12 20:04:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

